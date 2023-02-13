---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Pas een [!DNL Anaplan] begrotingstoewijzing aan een [!DNL Adobe Workfront] project
description: In dit integratiescenario worden alle begrotingstoewijzingen gesynchroniseerd die in [!DNL Anaplan] terug naar [!DNL Workfront]. Het scenario trekt alle gekoppelde begrotingsposten van de campagnebegroting, dan gaat de begrote waarde aan het verbonden project van Workfront over als de begrotingswaarde is veranderd.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 9b8add8f-1978-4ab4-87ac-f1159e7d6cbb
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# Pas een [!DNL Anaplan] begrotingstoewijzing aan een [!DNL Adobe Workfront] project

In dit integratiescenario worden alle begrotingstoewijzingen gesynchroniseerd die in [!DNL Anaplan] terug naar [!DNL Workfront]. Het scenario trekt alle verbonden begrotingsposten van de campagnebegroting, dan gaat de begrote waarde tot verbonden over [!DNL Workfront] , indien de begrotingswaarde is gewijzigd.

>[!IMPORTANT]
>
>&quot;Campagne&quot;in dit artikel verwijst naar de het gebruikscase van de marketing campagne die dit scenario vertegenwoordigt en op geen enkele wijze verbonden met [!DNL Workfront Fusion] Adobe Campaign-aansluiting of de onlangs vervangen [!UICONTROL Campaign] object in [!DNL Workfront].

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
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

&#42;&#42;Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Triginggebeurtenis

Dit scenario wordt gepland om de 15 minuten uit te voeren.

## Verwacht [!DNL Workfront] Configuratie

U moet het volgende opgeven in [!DNL Workfront] om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Workfront] benoemd **Anaplan-integratie**, die beheerdersrechten voor het systeem heeft.

   Voor informatie over het maken van een gebruiker in [!DNL Workfront], zie [Gebruikers toevoegen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Verwacht [!DNL Anaplan] Configuratie

U moet het volgende opgeven in [!DNL Anaplan] om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Anaplan] benoemd **[!DNL Workfront]Integratie**, die beheerdersrechten voor het systeem heeft.
* De [!DNL Anaplan] Model dat u voor dit scenario wilt gebruiken.
* De lijst in de [!DNL Anaplan] Model dat campagnebudgetten vastlegt.

   De module van de lijst moet het ontvangen van de volgende attributen steunen:

   * [!UICONTROL Workfront Project GUID]
   * [!UICONTROL Campaign Name]
   * [!UICONTROL Requested Labor Funds]
   * [!UICONTROL Estimated Revenue]
   * [!UICONTROL Brand]

   In deze lijst en module moeten aanvullende gegevens worden opgeslagen die nodig zijn voor de normale functionaliteit van [!DNL Anaplan], met inbegrip van de mogelijkheid om een begroting vast te stellen en te melden dat de begrotingspost gereed is om te worden gesynchroniseerd naar [!DNL Workfront].

* Een weergave in [!DNL Anaplan] benoemd **[!UICONTROL Campaigns.Update Campaigns in Adobe Workfront]**.

   Deze weergave moet de volgende kolommen in deze volgorde bevatten:

   1. [!UICONTROL Item Name]

   2. [!UICONTROL [!DNL Workfront] Project GUID]

   3. [!UICONTROL Campaign Name]

   4. [!UICONTROL Budget]

   5. [!UICONTROL Estimated Revenue]

   6. [!UICONTROL Brand]
   De weergave moet worden gefilterd om items met een [!UICONTROL [!DNL Workfront] Project GUID] en enige aanwijzing dat de begrotingstoewijzingen moeten worden doorgegeven aan [!DNL Workfront].

Voor instructies over een van deze handelingen raadpleegt u de [!DNL Anaplan] documentatie.

## Distribueren naar [!DNL Workfront Fusion]

Voltooi de volgende stappen om dit integratiescenario aan uw op te stellen [!DNL Fusion] account. Dit mag alleen gebeuren nadat de vereiste [!DNL Workfront] en [!DNL Anaplan] configuratie.

1. Ga naar de [!UICONTROL Templates] menu in [!DNL Workfront Fusion] en klik op de knop **[!UICONTROL Apply [!DNL Anaplan] budget allocations to Workfront projects]** scenario-sjabloon.
1. De waarden van variabelen vervangen voor het volgende [!DNL Anaplan] variabelen:

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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Werkruimte-id]</td> 
      <td>De id van een werkruimte van uw [!DNL Anaplan] account.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Model-id] </td> 
      <td>De id van een model van uw [!DNL Anaplan] en de geselecteerde werkruimte.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Modulenaam]</td> 
      <td>De naam van de module die de campagnekenmerken in de geselecteerde [!DNL Anaplan] Lijst.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>De naam van de lijst in uw [!DNL Anaplan] en de geselecteerde werkruimte en het geselecteerde model.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Naam weergeven]</td> 
      <td> <p>De naam van de weergave die kant-en-klare campagnebudgetten bevat voor [!DNL Workfront].</p> <p>(Voorbeeld: [!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   In het dialoogvenster [!DNL Anaplan] installatiedocumentatie.

1. Een [!DNL Anaplan] verbindingsprofiel.
1. Alle resterende bijwerken [!DNL Anaplan] modules met een [!DNL Anaplan] verbinding, wanneer hierom wordt gevraagd.
1. Op de **[!UICONTROL Convert CSV to JSON Object module]** voegt u een nieuwe gegevensstructuur toe om de CSV-kolommen toe te wijzen aan een bruikbaar JSON-object.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Wanneer ertoe aangezet, selecteer deze gegevensstructuur voor andere modules in dit scenario plaatsing.
1. Op de **[!UICONTROL Check Linked Project]** of een [!DNL Workfront] verbindingsprofiel.
1. Alle resterende bijwerken [!DNL Workfront] modules met een [!DNL Workfront] verbinding, wanneer hierom wordt gevraagd.

## Andere aanbevolen scènemasjablonen

Om het werkschema te voltooien door dit malplaatje wordt vertegenwoordigd, moet u het volgende extra malplaatje ook opstellen dat:

* [[!UICONTROL Create an [!DNL Anaplan] lijstitem uit een [!DNL Adobe Workfront] begrotingsverzoek]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)

Aanvullende scenario&#39;s voor optimalisatie van uitgaven zijn:

* [[!UICONTROL Send [!DNL Adobe Workfront] projectupdates voor een [!DNL Anaplan] lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Send [!DNL Adobe Workfront] de daadwerkelijke uren updates aan een [!DNL Anaplan] lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Send [!DNL Adobe Workfront] uitgaven voor een [!DNL Anaplan] lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
