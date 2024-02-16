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
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 0%

---

# Documentintegratie configureren

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Als [!DNL Adobe Workfront] beheerder, kunt u documentintegratie vormen om documenten te beheren in [!UICONTROL Workfront]. U kunt ook [!UICONTROL Workfront] zodat documenten alleen worden opgeslagen in documentservices en niet in [!UICONTROL Workfront] zelf. Zie voor meer informatie [Een document bijwerken en koppelen vanuit [!UICONTROL Workfront] naar een externe cloud provider](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) in [Documenten van externe toepassingen koppelen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Openbare communicatie tussen [!DNL Workfront Proof] en de [!DNL Workfront] servers, zou u bepaalde IP adressen aan uw lijst van gewenste personen kunnen moeten toevoegen. Zie voor meer informatie [De lijst van gewenste personen van uw firewall configureren](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Toegangsvereisten

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
   <td> <p>U moet een [!DNL Workfront] beheerder.</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Ondersteunde integratie

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

U kunt de volgende integraties configureren voor het beheer van documenten:

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  Proefdrukken koppelen van [!DNL Workfront Proof] kunt u proefdrukken maken die oorspronkelijk zijn gemaakt in [!DNL Workfront Proof] beschikbaar binnen [!DNL Workfront]. Voor de huidige plannen [!UICONTROL Pro] [!DNL Workfront] Een abonnement of hoger is vereist om deze functie te kunnen gebruiken. Voor de nieuwe plannen, is deze eigenschap beschikbaar met alle plannen. Zie voor meer informatie over de verschillende beschikbare plannen [Workfront-plannen](https://www.workfront.com/plans).

* [!DNL Microsoft SharePoint]

  Voor informatie over integratie met [!DNL SharePoint], zie [Vorm [!DNL SharePoint] integratie](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Leveranciers van clouddocumenten van derden:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google Drive]

     <!--Quip-->
  >[!TIP]
  >
  >U kunt documenten die zijn gekoppeld van een externe cloud provider op dezelfde manier controleren en goedkeuren als documenten die rechtstreeks zijn geüpload naar [!DNL Workfront].

* Andere documentproviders (via aangepaste documentintegratie).

  Voor de huidige plannen [!UICONTROL Pro] [!DNL Workfront] Een abonnement of hoger is vereist om deze functie te kunnen gebruiken. Voor de nieuwe plannen, is deze eigenschap beschikbaar met alle plannen. Zie voor meer informatie over de verschillende beschikbare plannen [Workfront-plannen](https://www.workfront.com/plans).

Bovendien kunt u uw [!DNL Workfront] documentervaring met een native Digital Asset Management (DAM)-systeem of met DAM-integratie van derden. De beheerders moeten deze eigenschappen toelaten opdat de gebruikers de dienst aan hun verbinden [!DNL Workfront] account. Zie voor meer informatie over Workfront DAM [Documenten beheren met [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## Integraties configureren om documenten te beheren

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **[!UICONTROL Documents]** > **[!UICONTROL Cloud Providers].**

1. (Optioneel) Naar opgeslagen documenten in een toepassing voor documentservices en niet in [!DNL Workfront], selecteert u **[!UICONTROL Prevent Users From Storing Documents in [!DNL Workfront]].**

1. Selecteer de integraties die u wilt inschakelen.
1. Klik op **[!UICONTROL Save]**.

Als u integratie instelt met [!DNL Workfront DAM]kunt u [!DNL Workfront] om metagegevens in documenten op te nemen. Voor informatie over toewijzingsmetagegevens raadpleegt u [Metagegevenstoewijzing instellen](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Aangepaste documentintegratie configureren

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Een aangepaste documentintegratie maakt [!DNL Workfront] gebruikers om bestanden te koppelen naar [!DNL Workfront] van vrijwel elk systeem, op voorwaarde dat het systeem wordt gebruikt [!DNL Workfront].

Als u de aangepaste integratie beschikbaar wilt maken voor gebruikers, moet u eerst de integratie maken. Voor informatie over hoe te om integratie te bouwen die met moet worden gebruikt [!DNL Workfront], zie [Document Webhooks-API](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Nadat de integratie van aangepaste documenten is voltooid, kunt u deze beschikbaar maken voor gebruikers op uw site.

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **[!UICONTROL Documents]** > **[!UICONTROL Custom Integration]**.

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
      <td>De basis HTTP of veilige HTTP URL voor API vraag. Bijvoorbeeld: <code>https://documentprovider.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication Type]</td> 
      <td> <p>De verificatiemethode die moet worden gebruikt wanneer geautoriseerde API-aanroepen naar de aangepaste integratie worden uitgevoerd.</p> 
       <ul> 
        <li>Als u <strong>[!UICONTROL OAuth]</strong>, gaat u verder met stap 5.</li> 
        <li>Als u <strong>[!UICONTROL ApiKey]</strong>, gaat u verder met stap 6.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Voorwaardelijk) Als u **[!UICONTROL OAuth]** verificatie voor de **[!UICONTROL Authentication Type]** Voer de volgende gegevens in:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authentication URL]</td> 
      <td>De volledige URL die wordt gebruikt voor gebruikersverificatie. [!DNL Workfront] navigeert gebruikers aan dit adres als deel van het Leveringsproces OAuth.</td> 
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
      <td> <p>Voer optionele waarden in die aan de queryreeks van elke API-aanroep moeten worden toegevoegd. Bijvoorbeeld access_type=offline.</p> <p>Om veelvoudige verzoekparameters toe te voegen, klik <strong>+Aanvraagparameter toevoegen</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >De [!DNL Workfront] URI omleiden die onder aan het dialoogvenster wordt weergegeven [!UICONTROL Custom Integration] Deze pagina bevat de URI waarmee deze integratie met de externe documentprovider wordt geregistreerd.

1. (Voorwaardelijk) Als u **[!UICONTROL ApiKey]** verificatie voor de **[!UICONTROL Authentication Type]**, voert u de API-sleutel in die door de aangepaste documentprovider is uitgegeven.

   [!DNL Workfront] gebruikt deze API-sleutel om geoorloofde API-aanroepen naar de documentprovider te maken.

1. Klikken **[!UICONTROL Save]** de integratie tot stand te brengen.

## Documentintegratie gebruiken

Voor informatie over hoe gebruikers kunnen gebruiken [!DNL Workfront DAM], zie [Documenten beheren met [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

Voor informatie over hoe de gebruikers het proef kunnen gebruiken, zie [Proefdrukken maken](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md).

Voor informatie over hoe de gebruikers de integratie van het derdedocument kunnen gebruiken nadat u hen hebt gevormd, zie [Documenten van externe toepassingen koppelen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configureren [!DNL Workfront] metagegevens verzenden naar [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Bij het verzenden van een document vanuit [!DNL Workfront] tot [!DNL Workfront DAM], kunt u ook informatie verzenden die aan dat document is gekoppeld. Informatie over het document is toegewezen aan [!DNL Workfront DAM] als metagegevens.

Informatie wordt slechts in één richting toegewezen, van [!DNL Workfront] tot [!DNL Workfront DAM] en wordt alleen overgedragen wanneer het document wordt geüpload naar [!DNL Workfront DAM]. In de toekomst worden metagegevensvelden in de Workfront-velden niet bijgewerkt in [!DNL Workfront DAM] nadat het document al is geüpload.\
U kunt hetzelfde toewijzen [!DNL Workfront] veld naar diverse [!DNL Workfront DAM] velden, maar u kunt niet hetzelfde gebruiken [!DNL Workfront DAM] veld voor meerdere [!DNL Workfront] velden.

Als u veelvoudige moet vormen [!DNL Workfront] velden die u naar één wilt exporteren [!DNL Workfront DAM] veld, maakt u eerst een berekend aangepast veld in [!DNL Workfront] alle afzonderlijke aangepaste velden van een object weergeven. Wijs vervolgens de berekende waarden toe [!DNL Workfront] veld naar één [!DNL Workfront DAM] veld.\
Zie voor meer informatie over berekende aangepaste velden [Berekende gegevens toevoegen aan een aangepast formulier](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

De toewijzing beïnvloedt alle documenten die door om het even welke gebruiker van worden geupload [!DNL Workfront] tot [!UICONTROL Workfront] DAM.

Als [!DNL Workfront] beheerder, moet u toelaten [!DNL Workfront DAM] in Workfront voordat u de velden voor het proces voor het toewijzen van metagegevens kunt toewijzen.

Om te vormen [!DNL Workfront] metagegevens verzenden naar [!DNL Workfront DAM]:

{{step-1-to-setup}}

1. Klikken **[!UICONTROL Documents]** > **[!UICONTROL Metadata Mapping]**.

1. In de **[!UICONTROL Select Source Field for Mapping]** veld, typ de naam van het Workfront-veld waarnaar u wilt toewijzen [!DNL Workfront DAM]en selecteert u de optie wanneer deze in de lijst wordt weergegeven.
1. In de **[!UICONTROL Select Target Field for Mapping]**, selecteert u de [!DNL Workfront DAM] veld dat u wilt vullen met de informatie in het geselecteerde veld [!DNL Workfront] veld.

   >[!NOTE]
   >
   > Alle documenten verzonden naar [!DNL Workfront DAM] door gebruikers die daartoe gemachtigd zijn, hun metagegevens laten bijwerken met de [!DNL Workfront] hier toegewezen velden, wanneer ze worden geüpload naar [!DNL Workfront DAM].

1. Klik op **[!UICONTROL Add Mapping]**.

1. Doorgaan met meer toevoegen [!UICONTROL Workfront] velden en bijbehorende [!DNL Workfront DAM] velden.

### Toegewezen velden verwijderen

{{step-1-to-setup}}

1. Uitbreiden **[!UICONTROL Documents]** en klik vervolgens op **[!UICONTROL Metadata Mapping]**.

1. Selecteer in de lijst met velden de velden die u uit de metagegevenstoewijzing wilt verwijderen.
1. Klik op **[!UICONTROL Delete]**.

   De velden worden verwijderd uit de metagegevenstoewijzing en de informatie daarin wordt niet overgedragen naar [!DNL Workfront DAM] met de geüploade documenten.
