---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Pas een  [!DNL Anaplan]  begrotingstoewijzing op een  [!DNL Adobe Workfront]  campagneverzoek of campagneproject toe
description: Dit integratiescenario synchroniseert om het even welke begrotingstoewijzingen die in  [!DNL Anaplan]  terug naar  [!DNL Workfront] zijn gemaakt. Het scenario trekt alle gekoppelde begrotingsposten van de campagnebegroting, dan gaat de begrote waarde aan het verbonden project van Workfront over als de begrotingswaarde is veranderd.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 8ae28911-fa18-459a-aa50-cfb347e70e61
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 0%

---

# Een [!DNL Anaplan] budget toewijzen aan een [!DNL Adobe Workfront] campagneverzoek- of campagneproject

In dit integratiescenario worden alle begrotingstoewijzingen gesynchroniseerd die zijn gemaakt in [!DNL Anaplan] terug naar [!DNL Workfront] . Het scenario trekt alle verbonden begrotingsposten van de campagnebegroting, dan gaat de begrotingswaarde aan het verbonden [!DNL Workfront] project over als de begrotingswaarde is veranderd.

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

* Een gebruikersprofiel in [!DNL Workfront] genaamd **[!DNL Anaplan Integration]** dat systeembeheerdersrechten heeft.

  Voor informatie bij het creëren van een gebruiker in [!DNL Workfront], zie [&#x200B; gebruikers &#x200B;](../../administration-and-setup/add-users/create-and-manage-users/add-users.md) toevoegen.

## [!DNL Anaplan] Configuratie verwacht

U moet het volgende in [!DNL Anaplan] hebben om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Anaplan] genaamd **[!UICONTROL [!DNL Workfront] Integration]** dat systeembeheerdersrechten heeft.
* Het [!DNL Anaplan] -model dat u voor dit scenario wilt gebruiken.
* De lijst binnen het [!DNL Anaplan] model dat campagnebegrotingen vangt.

  De module van de lijst moet het ontvangen van de volgende attributen steunen:

   * [!UICONTROL [!DNL Workfront] Request GUID]
   * [!UICONTROL [!DNL Workfront] Project GUID]
   * [!UICONTROL Campaign Name]
   * [!UICONTROL Requested Labor Funds]
   * [!UICONTROL Estimated Revenue]
   * [!UICONTROL Brand]

  In deze lijst en module moeten aanvullende gegevens worden opgeslagen die nodig zijn voor de normale functionaliteit van [!DNL Anaplan] , waaronder de mogelijkheid om een budget in te stellen en te communiceren dat het item in de begrotingslijst gereed is om te worden gesynchroniseerd naar [!DNL Workfront] .

* Een weergave in [!DNL Anaplan] met de naam **[!UICONTROL Campaigns.Update Campaigns in Adobe Workfront]** .

  Deze weergave moet de volgende kolommen in deze volgorde bevatten:

   1. [!UICONTROL Item Name]

   2. [!UICONTROL [!DNL Workfront] Request GUID]

   3. [!UICONTROL [!DNL Workfront] Project GUID]

   4. [!UICONTROL Campaign Name]

   5. [!UICONTROL Budget]

   6. [!UICONTROL Estimated Revenue]

   7. [!UICONTROL Brand]

  De weergave moet worden gefilterd om items weer te geven met een [!UICONTROL [!DNL Workfront] Project GUID] -teken en een indicatie dat de begrotingstoewijzingen naar Workfront moeten worden verzonden.

Zie de documentatie van [!DNL Anaplan] voor instructies over deze handelingen.

## Distribueren naar Workfront Fusion

Voer de volgende stappen uit om dit integratiescenario in te zetten op uw Fusion-account. Dit mag alleen gebeuren nadat de vereiste [!DNL Workfront] - en [!DNL Anaplan] -configuratie is voltooid.

1. Navigeer naar het [!UICONTROL Templates] -menu in [!DNL Workfront Fusion] en klik op de sjabloon van het **[!UICONTROL Apply [!DNL Anaplan] budget allocations to Workfront campaign requests & projects]** -scenario.
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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Weergavenaam]</td> 
      <td> <p>De naam van de weergave die kant-en-klare campagnebudgetten naar [!DNL Workfront] bevat.</p> <p>(Voorbeeld: [!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   In de installatiedocumentatie van [!DNL Anaplan] vindt u meer informatie over het instellen van de bestanden en processen.

1. Selecteer of voeg een [!DNL Anaplan] verbindingsprofiel toe.
1. Werk alle resterende [!DNL Anaplan] -modules bij met een [!DNL Anaplan] -verbinding wanneer hierom wordt gevraagd.
1. Voeg in de module **[!UICONTROL Convert CSV to JSON Object]** een nieuwe gegevensstructuur toe om de CSV-kolommen toe te wijzen aan een bruikbaar JSON-object.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Request GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. Wanneer ertoe aangezet, selecteer deze gegevensstructuur voor andere modules in dit scenario plaatsing.
1. Selecteer of voeg een **[!UICONTROL Check Linked Project]** -verbindingsprofiel toe in de module [!DNL Workfront] .
1. Werk alle resterende [!DNL Workfront] -modules bij met een [!DNL Workfront] -verbinding wanneer hierom wordt gevraagd.

## Andere aanbevolen scènemasjablonen

Om het werkschema te voltooien door dit malplaatje wordt vertegenwoordigd, moet u het volgende extra malplaatje ook opstellen dat:

* [[!UICONTROL Create an [!DNL Anaplan] lijstitem van een  [!DNL Adobe Workfront]  campagneverzoek]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)

Aanvullende scenario&#39;s voor optimalisatie van uitgaven zijn:

* [[!UICONTROL Send [!DNL Adobe Workfront] projectupdates aan een  [!DNL Anaplan]  lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Send [!DNL Adobe Workfront] daadwerkelijke uren updates aan een  [!DNL Anaplan]  lijstpunt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Send [!DNL Adobe Workfront] uitgaven aan een  [!DNL Anaplan]  lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
