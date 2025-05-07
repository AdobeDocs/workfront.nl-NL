---
title: Documentintegratie configureren
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Als Adobe Workfront-beheerder kunt u documentintegratie configureren om documenten in Workfront te beheren.
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: ec0e2be036ce1298e285ce85cdeddae97cd1f144
workflow-type: tm+mt
source-wordcount: '1111'
ht-degree: 0%

---

# Documentintegratie configureren

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Als [!DNL Adobe Workfront] -beheerder kunt u documentintegratie configureren om documenten te beheren in [!UICONTROL Workfront] . U kunt [!UICONTROL Workfront] ook zo configureren dat documenten alleen worden opgeslagen in documentservices en niet in [!UICONTROL Workfront] zelf. Voor meer informatie, zie [ Update en verbind een document van [!UICONTROL Workfront] met een externe wolkenleverancier ](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) in [ documenten van de Verbinding van externe toepassingen ](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Om open communicatie tussen [!DNL Workfront Proof] en de [!DNL Workfront] servers toe te staan, zou u bepaalde IP adressen aan uw lijst van gewenste personen kunnen moeten toevoegen. Voor meer informatie, zie [ de lijst van gewenste personen van uw firewall ](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) vormen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td><p>Nieuw: [!UICONTROL Standard]</p>
       <p>of</p>
       <p>Huidige: [!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ondersteunde integratie

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

U kunt de volgende integraties configureren voor het beheer van documenten:

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  Door proefdrukken van [!DNL Workfront Proof] te koppelen, kunt u proefdrukken maken die oorspronkelijk zijn gemaakt in [!DNL Workfront Proof] , beschikbaar zijn in [!DNL Workfront] . Voor de huidige plannen is een [!UICONTROL Pro] [!DNL Workfront] -abonnement of hoger vereist als u deze functie wilt gebruiken. Voor de nieuwe plannen, is deze eigenschap beschikbaar met alle plannen. Voor meer informatie over de diverse beschikbare plannen, zie [ Abonnementen van Workfront ](https://business.adobe.com/products/workfront/pricing.html).

* [!DNL Microsoft SharePoint]

  Voor informatie over het integreren met [!DNL SharePoint], zie [ de  [!DNL SharePoint]  integratie ](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md) vormen.

* Leveranciers van clouddocumenten van derden:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google Drive]
   * Quip

  >[!TIP]
  >
  >Documenten die zijn gekoppeld via een externe cloud provider, kunt u controleren en goedkeuren op dezelfde manier als documenten die rechtstreeks naar [!DNL Workfront] zijn geüpload.

* Andere documentproviders (via aangepaste documentintegratie).

  Voor de huidige plannen is een [!UICONTROL Pro] [!DNL Workfront] -abonnement of hoger vereist als u deze functie wilt gebruiken. Voor de nieuwe plannen, is deze eigenschap beschikbaar met alle plannen. Voor meer informatie over de diverse beschikbare plannen, zie [ Abonnementen van Workfront ](https://business.adobe.com/products/workfront/pricing.html).

Bovendien kunt u uw [!DNL Workfront] -documentervaring verbeteren met DAM-integratie van derden. Beheerders moeten deze functies inschakelen om gebruikers de service te laten koppelen aan hun [!DNL Workfront] -account.

## Integraties configureren om documenten te beheren

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **[!UICONTROL Documents]** > **[!UICONTROL Cloud Providers].**

1. (Optioneel) Selecteer **[!UICONTROL Prevent Users From Storing Documents in [!DNL Workfront]]** als u documenten wilt opslaan in een toepassing voor documentservices en niet in [!DNL Workfront] .

1. Selecteer de integraties die u wilt inschakelen.
1. Klik op **[!UICONTROL Save]**.

Als u integraties instelt met [!DNL Workfront DAM] , kunt u [!DNL Workfront] inschakelen om metagegevens op te nemen in documenten. Voor informatie over kaartmeta-gegevens, zie [ de meta-gegevensafbeelding van de Opstelling ](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Aangepaste documentintegratie configureren

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Dankzij de integratie van aangepaste documenten kunnen [!DNL Workfront] -gebruikers vanuit vrijwel elk systeem bestanden koppelen naar [!DNL Workfront] , op voorwaarde dat het systeem is ontworpen voor samenwerking met [!DNL Workfront] .

Als u de aangepaste integratie beschikbaar wilt maken voor gebruikers, moet u eerst de integratie maken. Voor informatie over hoe te om integratie te bouwen die met [!DNL Workfront] moet worden gebruikt, zie [ Webhooks API van het Document ](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Nadat de integratie van aangepaste documenten is voltooid, kunt u deze beschikbaar maken voor gebruikers op uw site.

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **[!UICONTROL Documents]** > **[!UICONTROL Custom Integration]** .

1. Klik op **[!UICONTROL Add Custom integration]**.
1. Voer de volgende informatie in om de integratie te configureren:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>De naam van de aangepaste integratie. Dit is de naam die gebruikers zien wanneer ze de integratie in Workfront gebruiken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Base API URL] </td> 
      <td>De basis HTTP of veilige HTTP URL voor API vraag. Bijvoorbeeld: <code>https://&lt;documentprovider&gt;.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication Type]</td> 
      <td> <p>De verificatiemethode die moet worden gebruikt wanneer geautoriseerde API-aanroepen naar de aangepaste integratie worden uitgevoerd.</p> 
       <ul> 
        <li>Als u <strong>[!UICONTROL OAuth]</strong> kiest, gaat u verder met Stap 5.</li> 
        <li>Als u <strong>[!UICONTROL ApiKey]</strong> kiest, gaat u verder met Stap 6.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Voorwaardelijk) Als u **[!UICONTROL OAuth]** -verificatie hebt geselecteerd voor de **[!UICONTROL Authentication Type]** , voert u de volgende informatie in:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication URL]</td> 
      <td>De volledige URL die wordt gebruikt voor gebruikersverificatie. [!DNL Workfront] navigeert gebruikers naar dit adres als onderdeel van het OAuth-inrichtingsproces.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Endpoint URL]</td> 
      <td>De volledige API-URL waarmee OAuth-tokens worden opgehaald.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>De OAut Client ID voor deze integratie.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>Het geheim van de Cliënt OAut voor deze integratie.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Parameters]</td> 
      <td> <p>Voer optionele waarden in die aan de queryreeks van elke API-aanroep moeten worden toegevoegd. Bijvoorbeeld access_type=offline.</p> <p>Om veelvoudige verzoekparameters toe te voegen, klik <strong> + voeg de Parameter van het Verzoek toe </strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >De [!DNL Workfront] Redirect URI die onder aan de [!UICONTROL Custom Integration] -pagina wordt weergegeven, geeft de URI weer die wordt gebruikt om deze integratie te registreren bij de externe documentprovider.

1. (Voorwaardelijk) Als u **[!UICONTROL ApiKey]** -verificatie hebt geselecteerd voor de **[!UICONTROL Authentication Type]** , voert u de API-sleutel in die is uitgegeven door de aangepaste documentprovider.

   [!DNL Workfront] gebruikt deze API-sleutel om geoorloofde API-aanroepen naar de documentprovider te maken.

1. Klik op **[!UICONTROL Save]** om de integratie te maken.

## Documentintegratie gebruiken

Voor informatie over hoe de gebruikers het proef kunnen gebruiken, zie [ tot proeven ](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md) leiden.

Voor informatie over hoe de gebruikers de integratie van het derdedocument kunnen gebruiken nadat u hen hebt gevormd, zie [ documenten van de Verbinding van externe toepassingen ](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### [!DNL Workfront] configureren voor het verzenden van metagegevens naar [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Wanneer u een document verzendt van [!DNL Workfront] naar [!DNL Workfront DAM] , kunt u ook de informatie verzenden die aan dat document is gekoppeld. Informatie over het document wordt toegewezen aan [!DNL Workfront DAM] als metagegevens.

Informatie wordt slechts in één richting toegewezen, van [!DNL Workfront] naar [!DNL Workfront DAM] en wordt alleen overgedragen wanneer het document wordt geüpload naar [!DNL Workfront DAM] . Eventuele toekomstige wijzigingen in de Workfront-velden werken geen metagegevensvelden bij in [!DNL Workfront DAM] nadat het document al is geüpload.\
U kunt hetzelfde [!DNL Workfront] -veld toewijzen aan verschillende [!DNL Workfront DAM] -velden, maar u kunt niet hetzelfde [!DNL Workfront DAM] -veld gebruiken voor meerdere [!DNL Workfront] -velden.

Als u meerdere [!DNL Workfront] -velden moet configureren om te exporteren naar één [!DNL Workfront DAM] -veld, maakt u eerst een berekend aangepast veld in [!DNL Workfront] om alle afzonderlijke aangepaste velden van een object weer te geven. Wijs vervolgens het berekende [!DNL Workfront] veld toe aan één [!DNL Workfront DAM] veld.\
Voor meer informatie over berekende douanevelden, zie [ berekende gebieden aan een vorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) toevoegen.

De toewijzing is van invloed op alle documenten die door een gebruiker zijn geüpload van [!DNL Workfront] naar [!UICONTROL Workfront] DAM.

Als [!DNL Workfront] -beheerder moet u [!DNL Workfront DAM] inschakelen in Workfront voordat u de velden kunt toewijzen voor het proces voor het toewijzen van metagegevens.

U configureert als volgt [!DNL Workfront] om metagegevens naar [!DNL Workfront DAM] te verzenden:

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Documents]** > **[!UICONTROL Metadata Mapping]** .

1. Typ in het veld **[!UICONTROL Select Source Field for Mapping]** de naam van het Workfront-veld dat u wilt toewijzen aan [!DNL Workfront DAM] en selecteer het veld wanneer het in de lijst wordt weergegeven.
1. Selecteer in **[!UICONTROL Select Target Field for Mapping]** het veld [!DNL Workfront DAM] dat u wilt vullen met de gegevens in het geselecteerde veld [!DNL Workfront] .

   >[!NOTE]
   >
   > In alle documenten die gebruikers met de juiste machtigingen naar [!DNL Workfront DAM] hebben verzonden, worden de metagegevens bijgewerkt met de [!DNL Workfront] -velden die hier zijn toegewezen, wanneer ze worden geüpload naar [!DNL Workfront DAM] .

1. Klik op **[!UICONTROL Add Mapping]**.

1. Voeg meer [!UICONTROL Workfront] velden en bijbehorende [!DNL Workfront DAM] velden toe.

### Toegewezen velden verwijderen

{{step-1-to-setup}}

1. Vouw **[!UICONTROL Documents]** uit en klik op **[!UICONTROL Metadata Mapping]** .

1. Selecteer in de lijst met velden de velden die u uit de metagegevenstoewijzing wilt verwijderen.
1. Klik op **[!UICONTROL Delete]**.

   De velden worden verwijderd uit de metagegevenstoewijzing en de informatie in deze velden wordt niet samen met de geüploade documenten overgebracht naar [!DNL Workfront DAM] .


## Beperkingen

### Integratie met Google Drive

* Wanneer een gekoppelde map aan Workfront wordt toegevoegd, worden de bestanden in de map niet meer automatisch toegevoegd.
   * U kunt de Google-map zonder de bestanden aan Workfront toevoegen en vervolgens de afzonderlijke bestanden aan Workfront toevoegen. De bestanden worden automatisch toegevoegd aan de Google-map in Workfront.
of
   * U kunt een documentmap maken in Workfront, vervolgens alle bestanden in de Google-map selecteren en deze toevoegen aan de Workfront-map.


* De integratie van Google Drive-documenten ondersteunt het toevoegen van bestanden van de sectie Mijn schijf van uw Google Drive. U kunt geen mappen of afbeeldingen toevoegen vanaf een gedeeld station. Leer meer over [ Google Gedeelde aandrijving ](https://support.google.com/a/users/answer/7212025?hl=en).
