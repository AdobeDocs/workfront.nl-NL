---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Een document verzenden naar Experience Manager Assets of Assets Essentials
description: U kunt documenten van Workfront naar Experience Manager Assets of Assets Essentials verzenden. Documenten die vanuit Workfront zijn geüpload en naar Assets Essentials zijn verzonden, worden nog steeds in mindering gebracht op de totale opslag van het document. Assets gekoppeld van Assets Essentials telt niet mee voor algemene opslag.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 7fa4493d269862c9cdece75f0bf216931c671ea6
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# Een document verzenden naar Experience Manager Assets of Assets Essentials

<span class="preview">De gemarkeerde informatie op deze pagina verwijst naar functionaliteit die nog niet algemeen beschikbaar is. Deze optie is alleen beschikbaar in de omgeving van de voorvertoningssandbox.</span>

U kunt documenten van Workfront naar Experience Manager Assets of Assets Essentials verzenden. Documenten die vanuit Workfront zijn geüpload en naar Assets Essentials zijn verzonden, worden nog steeds in mindering gebracht op de totale opslag van het document. Assets gekoppeld van Assets Essentials telt niet mee voor algemene opslag.

Assets dat via deze integratie naar Experience Manager wordt gestuurd, heeft een formaatlimiet **5 GB**.

<span class="preview">In de voorvertoningsomgeving geldt dat Assets die via deze integratie naar de Experience Manager wordt verzonden, een formaatlimiet heeft van **30 GB**.</span>

Metagegevensvelden worden eerst toegewezen wanneer u een element verzendt van Workfront naar Experience Manager Assets of Assets Essentials. Eventuele metagegevens die zijn geconfigureerd om toe te wijzen voor bovenliggende objecten, worden ook verzonden. Zie voor meer informatie over het configureren van metagegevenstoewijzing [De as a Cloud Service integratie van Experience Manager Assets configureren](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) of [De integratie met Experience Manager Assets Essentials configureren](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Voorbeeld** Wanneer u voor het eerst een element verzendt dat aan een taak is gekoppeld, worden de metagegevens van de taak toegewezen aan Experience Manager Assets of Assets Essentials en aan alle toegewezen metagegevens van bovenliggende objecten, zoals een project, portfolio en programma.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront-plan</a>*</td> 
   <td> <p> Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Overzicht van verouderde licenties</a>*</td> 
   <td> <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>U moet Experience Manager as a Cloud Service Assets Essentials hebben, en u moet aan het product als gebruiker in de Admin Console worden toegevoegd.
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang of hoger weergeven op documenten</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

Voordat u begint,

* Uw Workfront-beheerder moet een Experience Manager-integratie configureren. Zie voor meer informatie [De as a Cloud Service integratie van Experience Manager Assets configureren](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) of [De integratie met Experience Manager Assets Essentials configureren](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Een document verzenden vanuit Workfront

Wanneer een gebruiker een document van Workfront naar Experience Manager Assets of Assets Essentials verzendt, worden toegewezen metagegevens over het document overgedragen. Nadat het document is verzonden, worden wijzigingen die in de metagegevens van het document in Workfront zijn aangebracht, niet doorgevoerd in Assets of Assets Essentials. Als een toegewezen veld in Workfront wordt gewijzigd, moet u een nieuwe versie van het document met de bijgewerkte metagegevens naar Assets of Assets Essentials sturen. Als u metagegevens wilt instellen of bewerken, raadpleegt u [De as a Cloud Service integratie van Experience Manager Assets configureren](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) of [De integratie met Experience Manager Assets Essentials configureren](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

Een document verzenden:

1. Ga naar de **Documenten** in Workfront en selecteer het document dat u wilt verzenden.
1. Klikken **Verzenden naar** kiest u vervolgens de Experience Manager-integratie die uw beheerdersinstelling heeft ingesteld.

   >[!NOTE]
   >
   >De Workfront-beheerder kan elke naam voor deze integratie kiezen. Assets of Assets Essentials worden dus niet specifiek vermeld.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Kies waar u het element wilt plaatsen en klik op **Map selecteren**.
1. Wanneer u het gewenste doel hebt gevonden, klikt u op **Opslaan**.

## Nieuwe versie verzenden

U kunt een nieuwe versie toevoegen aan een document dat u eerder naar Workfront hebt geüpload. Zie voor meer informatie [Een nieuwe versie van een document uploaden](../../documents/managing-documents/upload-new-document-version.md). Nadat de meest recente versie is geüpload, kunt u deze naar de Assets Essentials verzenden. Als een toegewezen veld in Workfront is gewijzigd, werkt de nieuwe versie de metagegevens in Assets Essentials bij wanneer het wordt verzonden.

>[!IMPORTANT]
>
>Voordat u een nieuwe versie naar Workfront uploadt, raden we u aan de naam van het bestand te wijzigen. Als u een nieuwe versie uploadt met precies dezelfde bestandsnaam als een vorige versie, kan alleen de meest recente versie worden gedownload van Workfront. Alle versies kunnen worden gedownload van Experience Manager Assets of Assets Essentials, ongeacht de bestandsnaam.

De meest recente versie verzenden:

1. Ga naar de **Documenten** in Workfront en zoek het document.
1. Selecteren **Verzenden naar** kiest u vervolgens de Experience Manager-integratie die uw beheerdersinstelling heeft ingesteld.

   >[!NOTE]
   >
   >De Workfront-beheerder kan een willekeurige naam voor deze integratie kiezen, dus Assets of Assets Essentials worden niet specifiek genoemd.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Klikken **Opslaan**. De nieuwe versie slaat op dezelfde locatie op als de vorige versie.

## Een document naar een gekoppelde map in Experience Manager Assets verplaatsen

>[!NOTE]
>
>Deze functionaliteit is alleen beschikbaar voor Experience Manager Assets as a Cloud Service. Deze is niet beschikbaar voor Experience Manager Assets Essentials.

U kunt een document naar een gekoppelde map in Experience Manager Assets verplaatsen als zowel het document als de gekoppelde map zich in dezelfde documentlijst bevinden (zoals het documentgebied van een project).

1. Zoek het document dat u wilt verplaatsen.
1. Sleep het document naar de gekoppelde Experience Manager Assets-map waarnaar u het wilt verplaatsen.

De documentopties zijn niet beschikbaar wanneer het document wordt verplaatst. Nadat het document naar Experience Manager Assets is verplaatst, is het niet meer zichtbaar in de documentlijst in Workfront.

>[!NOTE]
>
> Handelingen of bewerkingen die u tijdens het verplaatsen in het document aanbrengt, worden niet in het document in Experience Manager Assets weergegeven en gaan daarom verloren.

