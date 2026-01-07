---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Verzend  [!DNL Adobe Workfront]  daadwerkelijke uren updates aan een  [!DNL Anaplan]  lijstitem
description: Dit integratiescenario deelt daadwerkelijke uren details die op een  [!DNL Adobe Workfront]  project met een  [!DNL Anaplan]  punt van de begrotingslijst worden gevangen. Het delen van deze informatie staat u toe om beter voordeel te halen uit de uitgavenoptimalisering en financiële analyse die  [!DNL Anaplan]  verstrekt.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# [!DNL Adobe Workfront] werkelijke uren updates verzenden naar een [!DNL Anaplan] lijstitem

In dit integratiescenario worden de werkelijke uren die zijn vastgelegd voor een [!DNL Adobe Workfront] -project gedeeld met een [!DNL Anaplan] -begrotingspost. Door deze informatie te delen, kunt u beter profiteren van de optimalisatie van uitgaven en de financiële analyse die [!DNL Anaplan] biedt.

Dit scenario malplaatje levert een lijst van uren die door project, dag, en rol worden samengevat op actieve projecten in toen afgelopen drie maanden wordt geregistreerd.

>[!IMPORTANT]
>
>‘Campagne’ in dit artikel verwijst naar het gebruik van de marketingcampagne dat dit scenario vertegenwoordigt en dat op geen enkele manier is verbonden met de [!DNL Workfront Fusion] Adobe Campaign-connector of het onlangs vervangen [!UICONTROL Campaign] -object in [!DNL Workfront] .

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Elk Adobe Workfront Workflow-pakket en elk Adobe Workfront Automation and Integration-pakket</p><p>Workfront Ultimate</p><p>Workfront Prime en Select packages, met extra aanschaf van Workfront Fusion.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront-licenties</td> 
   <td> <p>Standard</p><p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion-licentie</td> 
   <td>
   <p>Exploitatie gebaseerd: geen Workfront Fusion-licentievereisten</p>
   <p>Connectorgebaseerde (verouderde): Workfront Fusion for Work Automation and Integration </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Als uw organisatie een Select- of Prime Workfront-pakket heeft dat geen Workfront Automation and Integration bevat, moet uw organisatie Adobe Workfront Fusion aanschaffen.</li></ul>
   </td> 
  </tr>
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in documentatie &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Voor informatie over de vergunningen van de Fusie van Adobe Workfront, zie [&#x200B; de Fusie van Adobe Workfront vergunningen &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

+++

## Triginggebeurtenis

Dit scenario wordt gepland om de 15 minuten uit te voeren.

## [!DNL Workfront] Configuratie verwacht

U moet het volgende in [!DNL Workfront] hebben om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Workfront] genaamd **[!UICONTROL Anaplan Integration]** dat systeembeheerdersrechten heeft.

  Voor informatie bij het creëren van een gebruiker in [!DNL Workfront], zie [&#x200B; gebruikers &#x200B;](../../administration-and-setup/add-users/create-and-manage-users/add-users.md) toevoegen.

## [!DNL Anaplan] Configuratie verwacht

U moet het volgende in [!DNL Anaplan] hebben om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Anaplan] genaamd **[!UICONTROL [!DNL Workfront] Integration]** dat systeembeheerdersrechten heeft.
* Het [!DNL Anaplan] -model dat u voor dit scenario wilt gebruiken.
* De lijst binnen het [!DNL Anaplan] Model dat u voor dit scenario wilt gebruiken.
* Een bestand in [!DNL Anaplan] named **[!UICONTROL Anaplan Actual Hours Import]** dat de volgende kolommen bevat, in deze volgorde:

   1. [!UICONTROL Workfront Project GUID]

   2. [!UICONTROL Hours]

   3. [!UICONTROL Hours Estimated Cost]

   4. [!UICONTROL Entry Date]

   5. [!UICONTROL Role Name]

   6. [!UICONTROL Campaign Name]

   7. [!UICONTROL [!DNL Anaplan] List Item ID]

  Het [!DNL Anaplan] bestand met het rapport Werkelijke uitgaven voorbereiden:

   1. Kopieer en plak het volgende in een teksteditor of [!DNL Excel]
   1. Het bestand opslaan in een CSV-indeling
   1. Upload het bestand naar [!DNL Anaplan] .

      Zie de documentatie van [!DNL Anaplan] over het importeren van gegevens uit een bestand in modules voor instructies.

   1. Noteer de naam die u aan het bestand hebt gegeven; deze wordt gebruikt tijdens de implementatie van de [!UICONTROL Fusion] -scenario-sjabloon.

  Voorbeeld-CSV-inhoud

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>[!DNL Workfront] Project GUID,Hours,Hours Estimated Cost,Entry Date,Role Name,Workfront Project Name,Item ID<br>6218062a000d0442903fcfa21e11f556,2,0,3/7/22,Designer,New Project 6,202000001030</code></pre>

* Een **[!UICONTROL Project Actual Hours Import]** -proces dat is voorbereid om de import uit te voeren van gegevens die zijn geleverd tijdens een bestandsupload.

Zie de documentatie van [!DNL Anaplan] voor instructies over deze handelingen.

## Distribueren naar [!DNL Workfront Fusion]

Voer de volgende stappen uit om dit integratiescenario te implementeren voor uw [!DNL Fusion] -account. Dit mag alleen gebeuren nadat de vereiste [!DNL Workfront] - en [!DNL Anaplan] -configuratie is voltooid.

1. Navigeer naar het [!UICONTROL Templates] -menu in [!DNL Workfront Fusion] en klik op de sjabloon van het **[!UICONTROL Send Workfront actual hours updates to [!DNL Anaplan] list item]** -scenario.
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
      <td role="rowheader">[!UICONTROL File Name: Actual Hours Import]</td> 
      <td> <p>De naam van het bestand dat de werkelijke gegevens over de projecturen ontvangt.</p> <p> (Voorbeeld: WorkfrontUpdateLinkedprojects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Actual Hours Import]</td> 
      <td> <p>De naam van het proces dat de invoer van de gegevens van projecturen zal uitvoeren.</p> <p>(Voorbeeld: WF Int - Projecturen laden op rol)</p> </td> 
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
1. Werk alle resterende [!DNL Workfront] -modules bij met een [!DNL Workfront] -verbinding wanneer hierom wordt gevraagd.

## Andere aanbevolen scènemasjablonen

Dit scenario malplaatje wordt gecomplimenteerd door het volgende speer malplaatjes van het optimalisatiescenario die ook kunnen worden opgesteld:

* [[!UICONTROL Send [!DNL Adobe Workfront] projectupdates aan een  [!DNL Anaplan]  lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] uitgaven aan een  [!DNL Anaplan]  lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Aanvullende scenario&#39;s voor het koppelen van begrotingsaanvragen:

* [[!UICONTROL Create an [!DNL Anaplan] lijstitem van een  [!DNL Adobe Workfront]  begrotingsverzoek]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] begrotingstoewijzing aan een  [!DNL Adobe Workfront]  project]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Aanvullende scenario&#39;s voor het koppelen van campagneverzoeken:

* [[!UICONTROL Create an [!DNL Anaplan] lijstitem van een  [!DNL Adobe Workfront]  campagneverzoek]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] begrotingstoewijzing aan een  [!DNL Adobe Workfront]  campagneverzoek of campagneproject]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
