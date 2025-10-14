---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Verzend  [!DNL Adobe Workfront]  projectupdates aan een  [!DNL Anaplan]  lijstitem
description: Dit integratiescenario deelt vooruitgang, status, en zeer belangrijke planningsdetails van een  [!DNL Adobe Workfront]  project met een  [!DNL Anaplan]  punt van de begrotingslijst. Het delen van deze informatie staat u toe om beter voordeel te halen uit de uitgavenoptimalisering en financiële analyse die  [!DNL Anaplan]  verstrekt.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: cb38223c4dd8048fd2ab105abce2c9a79b84c43f
workflow-type: tm+mt
source-wordcount: '774'
ht-degree: 0%

---

# [!DNL Adobe Workfront] projectupdates verzenden naar een [!DNL Anaplan] lijstitem

Dit integratiescenario deelt vooruitgang, status, en belangrijkste programmadetails van een [!DNL Adobe Workfront] project met een [!DNL Anaplan] begrotingspost. Door deze informatie te delen, kunt u beter profiteren van de optimalisatie van uitgaven en de financiële analyse die [!DNL Anaplan] biedt.

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

&#42;&#42; voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

## Triginggebeurtenis

Dit scenario wordt gepland om de 15 minuten uit te voeren.

## [!DNL Workfront] Configuratie verwacht

U moet het volgende in [!DNL Workfront] hebben om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Workfront] genaamd **[!UICONTROL [!DNL Anaplan] Integration]** dat systeembeheerdersrechten heeft.

  Voor informatie bij het creëren van een gebruiker in [!DNL Workfront], zie [&#x200B; gebruikers &#x200B;](../../administration-and-setup/add-users/create-and-manage-users/add-users.md) toevoegen.

* Een **[!UICONTROL Campaign Brief]** aangepast formulier dat aan het projectobject is gekoppeld, waarin aangepaste gegevenswaarden worden opgeslagen die u naar Anaplan wilt verzenden.

  De volgende velden bevatten voorbeelden van velden die in het aangepaste formulier kunnen worden opgenomen om te helpen bij het in kaart brengen van gegevens naar Anaplan, maar zijn niet vereist voor dit integratiescenario:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Veldnaam</th> 
     <th>Veldtype</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market Start Date]</td> 
     <td>[!UICONTROL Date] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market End Date]</td> 
     <td>[!UICONTROL Date]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Campaign Overview]</td> 
     <td>[!UICONTROL Paragraph Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>[!UICONTROL Paragraph Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Neem opties op die geschikt zijn voor uw processen.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Voor informatie bij het creëren van douaneformulieren, zie [&#x200B; een douaneformulier &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## [!DNL Anaplan] Configuratie verwacht

U moet het volgende in [!DNL Anaplan] hebben om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Anaplan] genaamd **[!UICONTROL [!DNL Workfront] Integration]** dat systeembeheerdersrechten heeft.
* Het [!DNL Anaplan] -model dat u voor dit scenario wilt gebruiken.
* De lijst binnen het [!DNL Anaplan] Model dat u voor dit scenario wilt gebruiken.
* Een **[!UICONTROL Project Update Import]** -bestand dat de volgende kolommen in deze volgorde bevat:

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront] Project GUID]

3. [!UICONTROL Campaign Name]

4. [!UICONTROL Percent Complete]

5. [!UICONTROL Planned Start Date]

6. [!UICONTROL Planned Completion Date]

7. [!UICONTROL Planned Hours]

8. [!UICONTROL Planned Cost]

9. [!UICONTROL Planned Expense Cost]

10. [!UICONTROL Actual Labor Cost]

11. [!UICONTROL Planned Labor Cost]

12. [!UICONTROL Status]

Het [!UICONTROL [!DNL Anaplan] Planned Expense Import] -bestand voorbereiden:

1. Kopieer en plak het volgende in een teksteditor of [!DNL Excel]
1. Het bestand opslaan in een CSV-indeling
1. Upload het bestand naar Anaplan.

   Zie de documentatie van [!DNL Anaplan] over het importeren van gegevens uit een bestand in modules voor instructies.

1. Noteer de naam die u aan het bestand hebt gegeven; deze wordt gebruikt tijdens de implementatie van de [!UICONTROL Fusion] -scenario-sjabloon.

Voorbeeld-CSV-inhoud

<!-- [Copy](javascript:void(0);) -->
<pre><code>"itemID","Workfront Project GUID","Campaign Name","Percent Complete","Planned Start Date","Planned Completion Date","Planned Hours","Planned Cost","Planned Expense Cost","Actual Labor Cost","Planned Labor Cost","Status","Campaign Overview","Key Message","In Market Start Date","In Market End Date","Target Audience"<br>"202000001019","6182bc1f0025e184b2c00d9205e22c49","Launch Be U APAC Styles Catalog","0","2022-03-31","2022-05-31","88.25","0","0","0","0","Planning","","","","",""</code></pre>Facultatieve kolommen kunnen omvatten:

1. [!UICONTROL Campaign Overview]

2. [!UICONTROL Key Message]

3. [!UICONTROL In Market Start Date]

4. [!UICONTROL In Market End Date]

5. [!UICONTROL Target Audience]

Neem ook alle andere velden op die u in de toewijzing wilt instellen.

* Een **[!UICONTROL Project Update Import]** -proces dat is voorbereid om de import uit te voeren van gegevens die zijn geleverd tijdens een bestandsupload.

Zie de documentatie van [!DNL Anaplan] voor instructies over deze handelingen.

## Distribueren naar [!DNL Workfront Fusion]

Voer de volgende stappen uit om dit integratiescenario in te zetten op uw Fusion-account. Dit mag alleen gebeuren nadat de vereiste [!DNL Workfront] - en [!DNL Anaplan] -configuratie is voltooid.

1. Navigeer naar het [!UICONTROL Templates] -menu in [!DNL Workfront Fusion] en klik op de sjabloon van het **[!UICONTROL Send Workfront project updates to [!DNL Anaplan] list item]** -scenario.
1. Vervang de variabelewaarden voor de volgende [!DNL Anaplan] -variabelen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Naam variabele</th> 
      <th>Waarde vervangen door</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace-id]</td> 
      <td>De id van een werkruimte vanuit uw [!DNL Anaplan] -account.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Model-id] </td> 
      <td>De id van een model uit uw [!DNL Anaplan] -account en de geselecteerde werkruimte.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>De naam van de lijst in uw [!DNL Anaplan] -account en de geselecteerde werkruimte en het geselecteerde model.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL File Name: Project Update Import]</td> 
      <td>De naam van het bestand dat de projectupdategegevens ontvangt.<p>(Voorbeeld: WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Project Update Import]</td> 
      <td> <p>De naam van het proces dat de invoer van projectgegevens zal uitvoeren.</p> <p>(Voorbeeld: WF Int - Campagnegegevens bijwerken)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Subdomein]</td> 
      <td>Het subdomein van uw [!DNL Workfront] account. Hiermee maakt u een koppeling naar uw [!DNL Workfront] -project in een notitie die kan worden gegenereerd.</td> 
     </tr> 
    </tbody> 
   </table>

   In de installatiedocumentatie van [!DNL Anaplan] vindt u meer informatie over het instellen van de bestanden en processen.

1. Selecteer of voeg een [!DNL Anaplan] verbindingsprofiel toe.
1. Werk alle resterende [!DNL Anaplan] -modules bij met een [!DNL Anaplan] -verbinding wanneer hierom wordt gevraagd.
1. Selecteer of voeg een [!DNL Workfront] verbindingsprofiel toe.

   Het filter wordt gevormd om in al onvolledig verbonden project en die projecten te trekken die in de laatste 29 minuten werden voltooid. Als u de frequentie van het [!DNL Fusion] scenario verandert zult u deze waarde willen bijwerken zodra het scenario malplaatje is opgesteld.

1. Voeg in de module **[!UICONTROL Build Projects Update CSV]** een nieuwe gegevensstructuur toe om de projectkenmerken toe te wijzen aan CSV-kolommen.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "itemID": 1000001,<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Percent Complete": 10.01,<br>        "Planned Start Date":"2022-02-22",<br>        "Planned Completion Date":"2022-02-22",<br>        "Planned Hours": 12.5,<br>        "Planned Cost": 123.45,<br>        "Planned Expense Cost": 123.45,<br>        "Planned Labor Cost": 123.45,<br>        "Status": "CUR",<br>        "Campaign Overview":"text",<br>        "Key Message":"text",<br>        "In Market Start Date":"2022-02-22",<br>        "In Market End Date":"2022-02-22",<br>        "Target Audience":"text"<br>    }<br>]<br></code></pre>

1. Werk alle resterende [!DNL Workfront] -modules bij met een [!DNL Workfront] -verbinding wanneer hierom wordt gevraagd.

## Andere aanbevolen scènemasjablonen

Dit scenario malplaatje wordt gecomplimenteerd door het volgende speer malplaatjes van het optimalisatiescenario die ook kunnen worden opgesteld:

* [[!UICONTROL Send [!DNL Adobe Workfront] daadwerkelijke uren updates aan een  [!DNL Anaplan]  lijstpunt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] uitgaven aan een  [!DNL Anaplan]  lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Aanvullende scenario&#39;s voor het koppelen van begrotingsaanvragen:

* [[!UICONTROL Create an [!DNL Anaplan] lijstitem van een  [!DNL Adobe Workfront]  begrotingsverzoek]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] begrotingstoewijzing aan een  [!DNL Adobe Workfront]  project]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Aanvullende scenario&#39;s voor het koppelen van campagneverzoeken:

* [[!UICONTROL Create an [!DNL Anaplan] lijstitem van een  [!DNL Adobe Workfront]  campagneverzoek]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] begrotingstoewijzing aan een  [!DNL Adobe Workfront]  campagneverzoek of campagneproject]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
