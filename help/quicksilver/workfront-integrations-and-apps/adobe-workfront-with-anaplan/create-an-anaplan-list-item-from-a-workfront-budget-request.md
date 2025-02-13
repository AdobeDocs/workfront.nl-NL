---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Creeer een  [!DNL Anaplan]  lijstitem van een  [!DNL Adobe Workfront]  begrotingsverzoek
description: Dit integratiescenario verbindt een  [!DNL Adobe Workfront]  project (campagne) met een  [!DNL Anaplan]  punt van de begrotingslijst. Dit wordt verwezenlijkt door een begrotingsverzoek aan het  [!DNL Workfront]  project toe te voegen dat financiering moet ontvangen. Dit scenario controleert voor onverwerkte begrotingsverzoeken, dan voert een proces uit om een leeg punt van de begrotingslijst in  [!DNL Anaplan]  tot stand te brengen om de processen van de begrotingstoewijzing in Anaplan af te schoppen.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: d6fd224fb8a7b8094946814ae905bc0ff6e8223c
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# Een [!DNL Anaplan] lijstitem maken op basis van een [!DNL Adobe Workfront] budget request

In dit integratiescenario wordt een [!DNL Adobe Workfront] -project (campagne) gekoppeld aan een [!DNL Anaplan] -item in de begrotingslijst. Dit wordt verwezenlijkt door een begrotingsverzoek aan het [!DNL Workfront] project toe te voegen dat financiering moet ontvangen. In dit scenario wordt gezocht naar onverwerkte begrotingsaanvragen en wordt vervolgens een proces uitgevoerd om een leeg item in de begrotingslijst in [!DNL Anaplan] te maken en de procedures voor begrotingstoewijzing in [!DNL Anaplan] af te starten.

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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</td> 
  </tr>
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

&#42;&#42; voor informatie over [!DNL  Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration)

## Triginggebeurtenis

Dit scenario wordt gepland om de 15 minuten uit te voeren.

## [!DNL Workfront] Configuratie verwacht

U moet het volgende in [!DNL Workfront] hebben om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Workfront] genoemd **[!DNL Anaplan]Integratie**, dat systeembeheerderrechten heeft.

  Voor informatie bij het creëren van een gebruiker in [!DNL Workfront], zie [ gebruikers ](../../administration-and-setup/add-users/create-and-manage-users/add-users.md) toevoegen.

* Een **[!UICONTROL Budget Request]** aangepast formulier dat is gekoppeld aan het [!UICONTROL Request] -object.

  De volgende vereiste velden moeten in het aangepaste formulier worden opgenomen als hulpmiddel bij het toewijzen van gegevens aan [!DNL Anaplan] :

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <thead> 
    <tr> 
     <th>Veldnaam</th> 
     <th>Veldtype</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL Budget Request Type]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Opties:</p> 
      <ul> 
       <li> <p>[!UICONTROL Adjustment to Funding]</p> </li> 
       <li> <p>[!UICONTROL Initial Funding]</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Requested Labor Funds]</td> 
     <td> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Requested Expense Funds]</td> 
     <td> </td> 
    </tr> 
   </tbody> 
  </table>

  Voor informatie bij het creëren van douaneformulieren, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

* Projectsjablonen die campagnes en andere projecten vertegenwoordigen waarvoor financiering is vereist, geconfigureerd met een [!UICONTROL Budget Request] -rijonderwerp. Het onderwerp in de wachtrij van [!UICONTROL Budget Request] wordt toegewezen aan het aangepaste formulier van [!UICONTROL Budget Request] .
* Een **[!UICONTROL Campaign Brief]** -formulier voor het projectobject.

  Dit formulier moet de volgende velden bevatten:

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
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
     <td>[!UICONTROL Rich Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>[!UICONTROL Rich Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Neem opties op die geschikt zijn voor uw processen.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Voor informatie bij het creëren van douaneformulieren, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

## [!DNL Anaplan] Configuratie verwacht

U moet het volgende in [!DNL Anaplan] hebben om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Anaplan] genaamd **[!UICONTROL [!DNL Workfront] Integration]** dat systeembeheerdersrechten heeft.
* Het [!DNL Anaplan] -model dat u voor dit scenario wilt gebruiken.
* De lijst binnen het [!DNL Anaplan] model dat campagnebegrotingen vangt.

  De module van de lijst moet het ontvangen van de volgende attributen steunen:

   * [!UICONTROL Workfront Project GUID]
   * [!UICONTROL Campaign Name]
   * [!UICONTROL Requested Labor Funds]
   * [!UICONTROL Requested Expense Funds]
   * [!UICONTROL Budget Request Type]
   * [!UICONTROL Reason for Funding Adjustment]

  In deze lijst en module moeten aanvullende gegevens worden opgeslagen die nodig zijn voor de normale functionaliteit van [!DNL Anaplan] , waaronder de mogelijkheid om een budget in te stellen en te communiceren dat het item in de begrotingslijst gereed is om te worden gesynchroniseerd naar [!DNL Workfront] .

Zie de documentatie van [!DNL Anaplan] voor instructies over deze handelingen.

## Distribueren naar [!DNL Workfront Fusion]

Voer de volgende stappen uit om dit integratiescenario te implementeren voor uw [!DNL Fusion] -account. Dit mag alleen gebeuren nadat de vereiste [!DNL Workfront] - en [!DNL Anaplan] -configuratie is voltooid.

1. Navigeer naar het [!UICONTROL Templates] -menu in [!DNL Workfront Fusion] en klik op de sjabloon van het **[!UICONTROL Create an [!DNL Anaplan] list item from a Workfront budget request]** -scenario.
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

* [[!UICONTROL Apply an [!DNL Anaplan] begrotingstoewijzing aan een  [!DNL Adobe Workfront]  project]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Aanvullende scenario&#39;s voor optimalisatie van uitgaven zijn:

* [[!UICONTROL Send [!DNL Adobe Workfront] projectupdates aan een  [!DNL Anaplan]  lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] daadwerkelijke uren updates aan een  [!DNL Anaplan]  lijstpunt]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] uitgaven aan een  [!DNL Anaplan]  lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
