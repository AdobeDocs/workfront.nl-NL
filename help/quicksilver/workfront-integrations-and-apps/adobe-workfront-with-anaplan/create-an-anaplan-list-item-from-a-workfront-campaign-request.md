---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Creeer een  [!DNL Anaplan]  lijstitem van een  [!DNL Adobe Workfront]  campagneverzoek
description: Dit integratiescenario verbindt een  [!DNL Adobe Workfront]  project met een  [!DNL Anaplan]  punt van de begrotingslijst.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: daf6a18d-a3df-497d-a612-8a4645b1a8c9
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---

# Een [!DNL Anaplan] lijstitem maken op basis van een [!DNL Adobe Workfront] campagneverzoek

In dit integratiescenario wordt een [!DNL Adobe Workfront] -project gekoppeld aan een [!DNL Anaplan] -begrotingstitem.

Dit scenario kijkt voor nieuwe campagneverzoeken die aan een verzoekrij worden toegevoegd. Zodra een campagneverzoek wordt geregistreerd, wordt een begrotingspost toegevoegd in [!DNL Anaplan] om het financieringsproces te beginnen.

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

Voor informatie over de vergunningen van de Fusie van Adobe Workfront, zie [&#x200B; de Fusie van Adobe Workfront vergunningen &#x200B;](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

+++

## Triginggebeurtenis

Dit scenario wordt gepland om de 15 minuten uit te voeren.

## [!DNL Workfront] Configuratie verwacht

U moet het volgende in [!DNL Workfront] hebben om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Workfront] genaamd **[!UICONTROL [!DNL Anaplan] Integration]** dat systeembeheerdersrechten heeft.

  Voor informatie bij het creëren van een gebruiker in [!DNL Workfront], zie [&#x200B; gebruikers &#x200B;](../../administration-and-setup/add-users/create-and-manage-users/add-users.md) toevoegen.

* Een **[!UICONTROL Campaign Brief]** aangepast formulier dat is gekoppeld aan het [!UICONTROL Request] -object.

  De volgende vereiste velden moeten in het aangepaste formulier worden opgenomen om te helpen bij het in kaart brengen van gegevens naar Anaplan:

  | Veldnaam | Veldtype |
  |---|---|
  | [!UICONTROL Total Requested Funds] |   |
  | [!UICONTROL Requested Labor Funds] |   |
  | [!UICONTROL Requested Expense Funds] |   |
  | [!UICONTROL Sent to [!DNL Anaplan]] | Selectievakje |

  De volgende optionele velden kunnen voorkomen op het formulier. In dit scenario worden alleen de bovenstaande velden toegewezen, maar eventuele extra velden in het campagneremorandum kunnen worden toegewezen.

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
     <td>Datum </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market End Date]</td> 
     <td>Datum</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Campaign Overview]</td> 
     <td>Alineatekstveld</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>Alineatekstveld</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>Vervolgkeuzelijst</p> <p>Neem opties op die geschikt zijn voor uw processen.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Voor informatie bij het creëren van douaneformulieren, zie [&#x200B; een douaneformulier &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

* Een project opstelling als verzoekrij om nieuwe campagneverzoeken te vangen. Het [!UICONTROL Campaign Brief] -formulier moet bij deze aanvragen worden gevoegd.

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
   * [!UICONTROL Requested Expense Funds]
   * [!UICONTROL Budget Request Type]

  In deze lijst en module moeten aanvullende gegevens worden opgeslagen die nodig zijn voor de normale functionaliteit van [!DNL Anaplan] , waaronder de mogelijkheid om een budget in te stellen en te communiceren dat het item in de begrotingslijst gereed is om te worden gesynchroniseerd naar [!DNL Workfront] .

Zie de documentatie van [!DNL Anaplan] voor instructies over deze handelingen.

## Distribueren naar [!DNL Workfront Fusion]

Voer de volgende stappen uit om dit integratiescenario te implementeren voor uw [!DNL Fusion] -account. Dit mag alleen gebeuren nadat de vereiste [!DNL Workfront] - en [!DNL Anaplan] -configuratie is voltooid.

1. Navigeer naar het [!UICONTROL Templates] -menu in [!DNL Workfront Fusion] en klik op de sjabloon van het **[!UICONTROL Create an [!DNL Anaplan] list item from a Workfront campaign request]** -scenario.
1. Vervang de variabelewaarden voor de volgende [!DNL Anaplan] -variabelen:

   | Naam variabele | Waarde vervangen door |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] Workspace ID] | De id van een werkruimte vanuit uw [!DNL Anaplan] -account. |
   | [!UICONTROL [!DNL Anaplan] Model ID] | De id van een model uit uw [!DNL Anaplan] -account en de geselecteerde werkruimte. |
   | [!UICONTROL [!DNL Anaplan] Module Name] | De naam van de module die de campagnerekenmerken in de geselecteerde [!DNL Anaplan] lijst beschrijft. |
   | [!UICONTROL Campaign List Name] | De naam van de lijst in uw [!DNL Anaplan] -account en de geselecteerde werkruimte en het geselecteerde model. |

   {style="table-layout:auto"}

   In de installatiedocumentatie van [!DNL Anaplan] vindt u meer informatie over het instellen van de bestanden en processen.

1. Selecteer of voeg een [!DNL Anaplan] verbindingsprofiel toe.
1. Werk alle resterende [!DNL Anaplan] -modules bij met een [!DNL Anaplan] -verbinding wanneer hierom wordt gevraagd.
1. Selecteer of voeg een [!DNL Workfront] verbindingsprofiel toe.

   Na het opstellen van het malplaatje, is dit de module u zult bijwerken om douanegebiedsverwijzingen aan de waarde van het gebiedsbezit toe te voegen of te verwijderen als u de standaard in kaart gebrachte gebieden aan [!DNL Anaplan] wilt veranderen.

1. Werk alle resterende [!DNL Workfront] -modules bij met een [!DNL Workfront] -verbinding wanneer hierom wordt gevraagd.

## Andere aanbevolen scènemasjablonen

Om het werkschema te voltooien door dit malplaatje wordt vertegenwoordigd, moet u het volgende extra malplaatje ook opstellen dat:

* [[!UICONTROL Apply an [!DNL Anaplan] begrotingstoewijzing aan een  [!DNL Adobe Workfront]  campagneverzoek of campagneproject]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)

Aanvullende scenario&#39;s voor optimalisatie van uitgaven zijn:

* [[!UICONTROL Send [!DNL Adobe Workfront] projectupdates aan een  [!DNL Anaplan]  lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Send [!DNL Adobe Workfront] daadwerkelijke uren updates aan een  [!DNL Anaplan]  lijstpunt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Send [!DNL Adobe Workfront] uitgaven aan een  [!DNL Anaplan]  lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
