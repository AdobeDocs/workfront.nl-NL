---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Verzend  [!DNL Adobe Workfront]  uitgaven aan een  [!DNL Anaplan]  lijstitem
description: Dit integratiescenario deelt op kosten betrekking hebbende details van een  [!DNL Adobe Workfront]  project met een  [!DNL Anaplan]  punt van de begrotingslijst. Het delen van deze informatie staat u toe om beter voordeel te halen uit de uitgavenoptimalisering en financiële analyse die  [!DNL Anaplan]  verstrekt.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: cb38223c4dd8048fd2ab105abce2c9a79b84c43f
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 0%

---

# Verstuur [!DNL Adobe Workfront] kosten naar een [!DNL Anaplan] lijstitem

Dit integratiescenario deelt kosten-gerelateerde details van een [!DNL Adobe Workfront] -project met een [!DNL Anaplan] budgetlijstitem. Door deze informatie te delen, kunt u beter profiteren van de optimalisatie van uitgaven en de financiële analyse die [!DNL Anaplan] biedt.

>[!IMPORTANT]
>
>‘Campagne’ in dit artikel verwijst naar het gebruik van de marketingcampagne dat dit scenario vertegenwoordigt en dat op geen enkele manier is verbonden met de [!DNL Workfront Fusion] Adobe Campaign-connector of het onlangs vervangen [!UICONTROL Campaign] -object in [!DNL Workfront] .

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

&#42;&#42; voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration)

## Triginggebeurtenis

Dit scenario wordt gepland om de 15 minuten uit te voeren.

## [!DNL Workfront] Configuratie verwacht

U moet het volgende in [!DNL Workfront] hebben om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Workfront] genoemd * [!UICONTROL *[!DNL Anaplan] Integration] ***, dat systeembeheerderrechten heeft.

  Voor informatie bij het creëren van een gebruiker in [!DNL Workfront], zie [ gebruikers ](../../administration-and-setup/add-users/create-and-manage-users/add-users.md) toevoegen.

* Een **[!UICONTROL Campaign Brief]** aangepast formulier dat aan het projectobject is gekoppeld, waarin aangepaste gegevenswaarden worden opgeslagen die u naar [!DNL Anaplan] wilt verzenden.

  Het formulier moet de volgende velden bevatten:

  | Veldnaam | Veldtype |
  |---|---|
  | [!UICONTROL Last Transmission Date] | Datum |
  | [!UICONTROL Integration Notes] | Alineatekstveld |

  Voor informatie bij het creëren van douaneformulieren, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

## [!DNL Anaplan] Configuratie verwacht

U moet het volgende in [!DNL Anaplan] hebben om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Anaplan] genaamd **[!UICONTROL [!DNL Workfront] Integration]** dat systeembeheerdersrechten heeft.
* Het [!DNL Anaplan] -model dat u voor dit scenario wilt gebruiken.
* De lijst in het [!DNL Anaplan] model dat u wilt vangen campagnebegrotingen.
* Een **[!UICONTROL Anaplan Actual Expense Import]** -bestand dat de volgende kolommen in deze volgorde bevat:

   1. [!UICONTROL [!DNL Workfront] Expense GUID]

   2. [!UICONTROL [!DNL Workfront] Project GUID]

   3. [!UICONTROL Actual Amount]

   4. [!UICONTROL Description]

   5. [!UICONTROL Expense Type]

   6. [!UICONTROL Effective Date]

   7. [!UICONTROL Campaign Name]

   8. [!UICONTROL [!DNL Anaplan] List Item ID]

  Het [!UICONTROL [!DNL Anaplan] Actual Expense Import] -bestand voorbereiden:

   1. Kopieer en plak het volgende in een teksteditor of [!DNL Excel] .
   1. Sla het bestand op in een CSV-indeling.
   1. Upload het bestand naar [!DNL Anaplan] .

      Zie de documentatie van [!DNL Anaplan] over het importeren van gegevens uit een bestand in modules voor instructies.

   1. Noteer de naam die u aan het bestand hebt gegeven; deze wordt gebruikt tijdens de implementatie van de [!UICONTROL Fusion] -scenario-sjabloon.

  Voorbeeld-CSV-inhoud

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Actual Amount","Description","Expense Type","Effective Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","2345","Expense 1","","2022-03-09","New Project 6","202000001030"</code></pre>

* Een **[!UICONTROL [!DNL Anaplan] Planned Expense Import]** -bestand dat de volgende kolommen in deze volgorde bevat:

   1. [!UICONTROL [!DNL Workfront] Expense GUID]

   2. [!UICONTROL [!DNL Workfront] Project GUID]

   3. [!UICONTROL Actual Amount]

   4. [!UICONTROL Description]

   5. [!UICONTROL Expense Type]

   6. [!UICONTROL Effective Date]

   7. [!UICONTROL Campaign Name]

   8. [!UICONTROL [!DNL Anaplan] List Item ID]

  Het [!UICONTROL [!DNL Anaplan] Planned Expense Import] -bestand voorbereiden:

   1. Kopieer en plak het volgende in een teksteditor of [!DNL Excel]
   1. Het bestand opslaan in een CSV-indeling
   1. Upload het bestand naar Anaplan.

      Zie de documentatie van [!DNL Anaplan] over het importeren van gegevens uit een bestand in modules voor instructies.

   1. Noteer de naam die u aan het bestand hebt gegeven; deze wordt gebruikt tijdens de implementatie van de [!UICONTROL Fusion] -scenario-sjabloon.

  Voorbeeld-CSV-inhoud

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Planned Amount","Description","Expense Type","Planned Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","1234","Expense 1","Entertainment","2022-03-08","New Project 6","202000001030"</code></pre>


* Een **[!UICONTROL Project Update Import]** -proces dat is voorbereid om de import uit te voeren van gegevens die zijn geleverd tijdens een bestandsupload.

>[!NOTE]
>
>Er zijn afzonderlijke invoerbestanden voor geplande en werkelijke uitgaven, zodat deze onafhankelijk kunnen worden gerapporteerd over de geplande en effectieve data.

Zie de documentatie van [!DNL Anaplan] voor instructies over deze handelingen.

## Distribueren naar [!DNL Fusion]

Voer de volgende stappen uit om dit integratiescenario te implementeren voor uw [!DNL Fusion] -account. Dit mag alleen gebeuren nadat de vereiste [!DNL Workfront] - en [!DNL Anaplan] -configuratie is voltooid.

1. Navigeer naar het [!UICONTROL Templates] -menu in [!DNL Workfront Fusion] en klik op de sjabloon van het **[!UICONTROL Send Workfront expenses updates to [!DNL Anaplan] list item]** -scenario.
1. Vervang de variabelewaarden voor de volgende [!DNL Anaplan] -variabelen:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>Naam variabele</th> 
      <th>Waarde vervangen door</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace-id]</td> 
      <td>De id van de werkruimte van uw [!DNL Anaplan] -account die u voor dit scenario wilt gebruiken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Model-id] </td> 
      <td>De id van het model van uw [!DNL Anaplan] -account en de geselecteerde werkruimte die u voor dit scenario wilt gebruiken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>De naam van de lijst van uw [!DNL Anaplan] rekening en de geselecteerde werkruimte en het model dat u voor dit scenario wilt gebruiken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL File Name: Actual Expense Import]</td> 
      <td> <p>De naam van het bestand dat de werkelijke projectuitgavengegevens ontvangt.</p> <p> (Voorbeeld: WorkfrontUpdateLinkedprojects_ActExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL File Name: Planned Expense Import]</td> 
      <td> <p>De naam van het dossier dat project geplande uitgavengegevens zal ontvangen.</p> <p> (Voorbeeld: WorkfrontUpdateLinkedprojects_PlannedExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Project Update Import]</td> 
      <td> <p>De naam van het proces dat de invoer van de gegevens van de projectuitgave zal uitvoeren.</p> <p>(Voorbeeld: WF Int - projectkosten laden)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   In de installatiedocumentatie van [!DNL Anaplan] vindt u meer informatie over het instellen van de bestanden en processen.

1. Selecteer of voeg een [!DNL Anaplan] verbindingsprofiel toe.
1. Werk alle resterende [!DNL Anaplan] -modules bij met een [!DNL Anaplan] -verbinding wanneer hierom wordt gevraagd.
1. Selecteer of voeg een [!DNL Workfront] verbindingsprofiel toe.
1. Werk alle resterende [!DNL Workfront] -modules bij met een [!DNL Workfront] -verbinding wanneer hierom wordt gevraagd.
1. Voeg in de module **[!UICONTROL Build Actual Expense CSV]** een nieuwe gegevensstructuur toe om de projectkenmerken toe te wijzen aan CSV-kolommen.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Actual Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Effective Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

1. Voeg in de module **[!UICONTROL Build Planned Expense CSV]** een nieuwe gegevensstructuur toe om de projectkenmerken toe te wijzen aan CSV-kolommen.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Planned Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Planned Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

## Andere aanbevolen scènemasjablonen

Dit scenario malplaatje wordt gecomplimenteerd door het volgende speer malplaatjes van het optimalisatiescenario die ook kunnen worden opgesteld:

* [[!UICONTROL Send [!DNL Adobe Workfront] projectupdates aan een  [!DNL Anaplan]  lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] daadwerkelijke uren updates aan een  [!DNL Anaplan]  lijstpunt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

Aanvullende scenario&#39;s voor het koppelen van begrotingsaanvragen:

* [[!UICONTROL Create an [!DNL Anaplan] lijstitem van een  [!DNL Adobe Workfront]  begrotingsverzoek]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] begrotingstoewijzing aan een  [!DNL Adobe Workfront]  project]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Aanvullende scenario&#39;s voor het koppelen van campagneverzoeken:

* [[!UICONTROL Create an [!DNL Anaplan] lijstitem van een  [!DNL Adobe Workfront]  campagneverzoek]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] begrotingstoewijzing aan een  [!DNL Adobe Workfront]  campagneverzoek of campagneproject]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
