---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Verzenden [!DNL Adobe Workfront] de daadwerkelijke uren updates aan een [!DNL Anaplan] lijstitem
description: Dit integratiescenario deelt de werkelijke uren die zijn vastgelegd op een [!DNL Adobe Workfront] met een [!DNL Anaplan] begrotingspost. Door deze informatie te delen kunt u beter profiteren van de optimalisatie van uitgaven en de financiële analyse die [!DNL Anaplan] verstrekt.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# Verzenden [!DNL Adobe Workfront] de daadwerkelijke uren updates aan een [!DNL Anaplan] lijstitem

Dit integratiescenario deelt de werkelijke uren die zijn vastgelegd op een [!DNL Adobe Workfront] met een [!DNL Anaplan] begrotingspost. Door deze informatie te delen kunt u beter profiteren van de optimalisatie van uitgaven en de financiële analyse die [!DNL Anaplan] verstrekt.

Dit scenario malplaatje levert een lijst van uren die door project, dag, en rol worden samengevat op actieve projecten in toen afgelopen drie maanden wordt geregistreerd.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p> </td> 
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

* Een gebruikersprofiel in [!DNL Workfront] benoemd **[!UICONTROL Anaplan Integration]**, die beheerdersrechten voor het systeem heeft.

   Voor informatie over het maken van een gebruiker in [!DNL Workfront], zie [Gebruikers toevoegen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Verwacht [!DNL Anaplan] Configuratie

U moet het volgende opgeven in [!DNL Anaplan] om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Anaplan] benoemd **[!UICONTROL [!DNL Workfront ] Integration]**, die beheerdersrechten voor het systeem heeft.
* De [!DNL Anaplan] Model dat u voor dit scenario wilt gebruiken.
* De lijst in de [!DNL Anaplan] Model dat u voor dit scenario wilt gebruiken.
* Een bestand in [!DNL Anaplan] benoemd **[!UICONTROL Anaplan Actual Hours Import]** die de volgende kolommen in deze volgorde bevat:

   1. [!UICONTROL Workfront Project GUID]

   2. [!UICONTROL Hours]

   3. [!UICONTROL Hours Estimated Cost]

   4. [!UICONTROL Entry Date]

   5. [!UICONTROL Role Name]

   6. [!UICONTROL Campaign Name]

   7. [!UICONTROL [!DNL Anaplan] List Item ID]
   Om het [!DNL Anaplan] Rapport van werkelijke kosten:

   1. Kopieer en plak het volgende in een teksteditor of [!DNL Excel]
   1. Het bestand opslaan in een CSV-indeling
   1. Het bestand uploaden naar [!DNL Anaplan].

      Zie voor instructies de [!DNL Anaplan] documentatie over het invoeren van gegevens in modules van een dossier.

   1. Noteer de naam die u aan het bestand hebt gegeven; het zal worden gebruikt tijdens de inzet van [!UICONTROL Fusion] scenario-sjabloon.

   Voorbeeld-CSV-inhoud

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

* A **[!UICONTROL Project Actual Hours Import]** proces voorbereid om de invoer van gegevens uit te voeren die in een dossier worden geleverd uploadt.

Voor instructies over een van deze handelingen raadpleegt u de [!DNL Anaplan] documentatie.

## Distribueren naar [!DNL Workfront Fusion]

Voltooi de volgende stappen om dit integratiescenario aan uw op te stellen [!DNL Fusion] account. Dit mag alleen gebeuren nadat de vereiste [!DNL Workfront] en [!DNL Anaplan] configuratie.

1. Ga naar de [!UICONTROL Templates] menu in [!DNL Workfront Fusion] en klik op de knop **[!UICONTROL Send Workfront actual hours updates to [!DNL Anaplan] list item]** scenario-sjabloon.
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
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>De naam van de lijst in uw [!DNL Anaplan] en de geselecteerde werkruimte en het geselecteerde model.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL File Name: Actual Hours Import]</td> 
      <td> <p>De naam van het bestand dat de werkelijke gegevens over de projecturen ontvangt.</p> <p> (Voorbeeld: WorkfrontUpdateLinkedprojects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Actual Hours Import]</td> 
      <td> <p>De naam van het proces dat de invoer van de gegevens van projecturen zal uitvoeren.</p> <p>(Voorbeeld: WF Int - projecturen laden op rol)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Subdomein]</td> 
      <td>Het subdomein van uw [!DNL Workfront] account. Hiermee maakt u een koppeling naar uw [!DNL Workfront] in een notitie die kan worden gegenereerd.</td> 
     </tr> 
    </tbody> 
   </table>

   In het dialoogvenster [!DNL Anaplan] installatiedocumentatie.

1. Een [!DNL Anaplan] verbindingsprofiel.
1. Alle resterende bijwerken [!DNL Anaplan] modules met een [!DNL Anaplan] verbinding, wanneer hierom wordt gevraagd.
1. Selecteer of voeg een [!DNL Workfront] verbindingsprofiel.
1. Alle resterende bijwerken [!DNL Workfront] modules met een [!DNL Workfront] verbinding, wanneer hierom wordt gevraagd.

## Andere aanbevolen scènemasjablonen

Dit scenario malplaatje wordt gecomplimenteerd door het volgende speer malplaatjes van het optimalisatiescenario die ook kunnen worden opgesteld:

* [[!UICONTROL Send [!DNL Adobe Workfront] projectupdates voor een [!DNL Anaplan] lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] uitgaven voor een [!DNL Anaplan] lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Aanvullende scenario&#39;s voor het koppelen van begrotingsaanvragen:

* [[!UICONTROL Create an [!DNL Anaplan] lijstitem uit een [!DNL Adobe Workfront] begrotingsverzoek]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] begrotingstoewijzing aan een [!DNL Adobe Workfront] project]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Aanvullende scenario&#39;s voor het koppelen van campagneverzoeken:

* [[!UICONTROL Create an [!DNL Anaplan] lijstitem uit een [!DNL Adobe Workfront] campagneverzoek]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] begrotingstoewijzing aan een [!DNL Adobe Workfront] campagneverzoek of campagneproject]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
