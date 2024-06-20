---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Gekoppelde mappen en documenten migreren
description: U kunt de API gebruiken om gekoppelde mappen en documenten te migreren naar Adobe Experience Manager Assets.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: aad8f4648a57c93047a1a691d5e608c327d78c1b
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# Gekoppelde mappen en documenten migreren

U kunt de API gebruiken om gekoppelde mappen en documenten te migreren naar Adobe Experience Manager Assets.

## Procedure

1. Identificeer alle documenten en mappen die aan het vorige externe documentopslagbureau zijn gekoppeld. Hierbij worden de interne document- of mapid&#39;s van de Workfront en alle mappen met deze map vermeld.

   >[!NOTE]
   >
   > Controleer alle ontdekte mappen of documenten om te controleren of ze nog geen koppeling voor deze mappen of documenten hebben gemaakt met de nieuwe provider.

1. Zoek de documenten en mappen in de nieuwe opslagplaats op pad en zoek vervolgens hun identiteit op in het externe systeem.

1. Maak een toewijzing van de interne Workfront-id aan de id in de nieuwe externe opslag. U hebt dit nodig om in de volgende stap een nieuwe koppeling te maken.

1. Maak een koppeling naar een nieuw document of een nieuwe documentmap in Workfront en wijs de bron via de nieuwe externe id naar de nieuwe locatie.

   1. **Documenten**: Voeg een nieuwe versie van het bestaande document toe met de nieuwe externe documentprovider.
   1. **Mappen**: Maak een nieuwe map op dezelfde plaats met dezelfde naam.

>[!CAUTION]
>
>   Verwijder de bestaande gekoppelde mappen niet. Dit kan leiden tot gegevensverlies. Als u oude mapkoppelingen uit de Workfront-toepassing wilt verwijderen, schakelt u de integratie van aangepaste documenten in het gedeelte Instellen uit.


## Voorbeeld van migreren van koppelingen

![Simplilink-flow](assets/links-flow-simplified.png)

## API-informatie

Zie voor meer informatie over de Workfront API&#39;s in deze sectie [documentatie voor ontwikkelaars:documenten](https://developer.workfront.com/documents.html).

### Alle documenten zoeken

Alles zoeken **Documenten (DOCU)** Gekoppeld aan **Documentprovider** van **providerType** with **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[API DOCS-verwijzing](https://developer.workfront.com/documents.html#get-/docu/search)

### Alle mappen zoeken

Alles zoeken **Documentmappen (DOCFDR)** Gekoppeld aan documentprovider van **providerType** with **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

API DOCS: (Eindpunten van documentmap worden momenteel niet gedekt door developer.workfront.com)

### Documenten koppelen

Koppeling **Documenten (DOCU)** van **Externe documentprovider** van **providerType** with **documentProviderID**.

>[!IMPORTANT]
>
>Documenten worden tijdelijk opgeslagen. Dit betekent dat u toegang hebt tot alle versies van het document. Wanneer u de koppeling maakt, kunt u de bestaande document-id opgeven. U schrijft dus gewoon een nieuwe versie naar dat document, waarbij de gegevens extern in de nieuwe provider worden gehost. Dit document-id is dezelfde als de document-id die u vindt op de documentkoppeling die u vervangt. Het is hetzelfde conceptuele document. U geeft gewoon aan dat de bytes voor deze nieuwe versie worden opgeslagen met een andere provider.

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

API DOCS: (Internal Link Endpoints zijn momenteel niet opgenomen in developer.workfront.com)

### Mappen koppelen

Koppeling **Documentmappen (DOCFDR)** van **Externe documentprovider** van **providerType** with **documentProviderID**.

>[!IMPORTANT]
>
>Voor mapkoppelingen hebt u, in tegenstelling tot documentkoppelingen, de &#39;documentFolderId&#39; nodig van de map in Workfront waarin u de nieuwe koppeling wilt plaatsen. Dit is waarschijnlijk dezelfde bovenliggende map als de gekoppelde map die we kopiëren.

>[!CAUTION]
>
>Mappen worden niet tijdelijk opgeslagen. Verwijder de oude mappen niet. Schakel de integratie van aangepaste documenten in het installatiegebied uit om oude mappen te verwijderen.


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

API DOCS: (Internal Link Endpoints zijn momenteel niet opgenomen in developer.workfront.com)

## Belangrijke termen

* **Document**: Een digitaal middel in Workfront

* **Documentmap**: Een container voor digitale middelen in Workfront

* **Document-id**: Workfront interne id voor een digitaal middel

* **Documentmap-id**: Workfront interne id voor een map met digitale middelen

* **Documentprovider-id**: ID gekoppeld aan specifieke documentproviders

>[!IMPORTANT]
>
> Voor een bepaald type documentprovider kunnen er meerdere gekoppelde instanties zijn. Ze kunnen bijvoorbeeld meerdere AEM opslagplaatsen hebben gekoppeld. Of meerdere Google Drive-instanties gekoppeld. De Document Provider ID wijst op de specifieke instantie van het verbindingstype wij of willen vervangen.

* **Documentopslagprovider (ook &quot;type externe integratie&quot;)**: Het type integratie van de documentopslagprovider dat Workfront ondersteunt. Of via een specifieke integratie of een &quot;aangepaste integratie&quot;.

* **Huidige typen opslagproviders van documenten ( providerType)**:

  ```
  ATTASK
  BOX
  GOOGLE
  SHAREPOINT
  WEBDAM
  WORKFRONTDAM
  INFERNO
  WIDEN
  DROPBOX
  DROPBOX_BUSINESS
  ONEDRIVE
  QUIP
  WEBHOOKS
  AEM
  MOCK
  ```

* **Gekoppeld document**: Een digitaal element dat wordt gehost in een externe documentopslagprovider. Workfront heeft een eigen interne Document ID voor het element, maar de bytes worden extern opgeslagen. Om dit mogelijk te maken, slaat Workfront ook een &quot;externe document-id&quot; op die u helpt bij het zoeken naar de bron waarnaar extern wordt verwezen in de externe opslagplaats of opslagplaats.

* **Map voor gekoppeld document**: Een container voor digitale elementen die wordt gehost in een externe documentopslagprovider. Workfront heeft een eigen interne Document Folder ID voor het element, maar de bytes worden extern opgeslagen. Om dit mogelijk te maken, slaat Workfront ook een &quot;externe document-id&quot; op die u helpt bij het zoeken naar de bron waarnaar extern wordt verwezen in de externe opslagplaats of opslagplaats.

* **Externe document-id**: ID toegewezen wanneer elementen buiten Workfront zijn opgeslagen. Workfront wijst zijn interne id toe aan de id die wordt gebruikt om het element in het externe systeem te vinden, via dit veld voor de id van het externe document. Daarom moet bij het koppelen van het document of de map vanuit een nieuwe externe opslag een nieuwe externe document-id worden samengesteld in de juiste indeling voor de externe documentprovider om het document in de nieuwe opslagplaats of opslagplaats te identificeren.

  >[!NOTE]
  >
  > Workfront heeft nog geen standaard voor externe document-id&#39;s. Er wordt een nieuwe specificatie gebruikt voor AEM-id&#39;s, maar voor andere id&#39;s kan de externe document-id verschillende vormen aannemen, afhankelijk van het providertype.


* **Objecttype**: Dit is alleen een API-term voor de doeleinden van dit document. Het is een soort algemeen object in Workfront waarmee je wilt communiceren. In deze gevallen zult u werken met documenten en mappen die respectievelijk de typen &quot;DOCU&quot; en &quot;DOCFDR&quot; hebben.

* **Object-id**: De interne Workfront-id voor het algemene object waarmee u wilt communiceren. U gaat werken met documenten en mappen, dus dit is respectievelijk de document-id of de documentmap-id.
