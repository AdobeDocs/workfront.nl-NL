---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Verzenden [!DNL Adobe Workfront] uitgaven voor een [!DNL Anaplan] lijstitem
description: Dit integratiescenario deelt op kosten betrekking hebbende details van een [!DNL Adobe Workfront] met een [!DNL Anaplan] begrotingspost. Door deze informatie te delen kunt u beter profiteren van de optimalisatie van uitgaven en de financiële analyse die [!DNL Anaplan] verstrekt.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---

# Verzenden [!DNL Adobe Workfront] uitgaven voor een [!DNL Anaplan] lijstitem

Dit integratiescenario deelt op kosten betrekking hebbende details van een [!DNL Adobe Workfront] met een [!DNL Anaplan] begrotingspost. Door deze informatie te delen kunt u beter profiteren van de optimalisatie van uitgaven en de financiële analyse die [!DNL Anaplan] verstrekt.

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
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
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

* Een gebruikersprofiel in [!DNL Workfront] benoemd *[!UICONTROL *[!DNL Anaplan] Integration]**, dat de rechten van de systeembeheerder heeft.

   Voor informatie over het maken van een gebruiker in [!DNL Workfront], zie [Gebruikers toevoegen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL Campaign Brief]** aangepast formulier dat is gekoppeld aan het projectobject, voor het opslaan van aangepaste gegevenswaarden die u wilt verzenden naar [!DNL Anaplan].

   Het formulier moet de volgende velden bevatten:

   | Veldnaam | Veldtype |
   |---|---|
   | [!UICONTROL Last Transmission Date] | Datum |
   | [!UICONTROL Integration Notes] | Alineatekstveld |

   Voor informatie over het maken van aangepaste formulieren raadpleegt u [Een aangepast formulier maken of bewerken](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Verwacht [!DNL Anaplan] Configuratie

U moet het volgende opgeven in [!DNL Anaplan] om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Anaplan] benoemd **[!UICONTROL [!DNL Workfront ] Integration]**, die beheerdersrechten voor het systeem heeft.
* De [!DNL Anaplan] Model dat u voor dit scenario wilt gebruiken.
* De lijst in de [!DNL Anaplan] Model dat u campagnebegrotingen wilt vastleggen.
* An **[!UICONTROL Anaplan Actual Expense Import]** bestand dat de volgende kolommen bevat, in deze volgorde:

   1. [!UICONTROL [!DNL Workfront] Expense GUID]

   2. [!UICONTROL [!DNL Workfront] Project GUID]

   3. [!UICONTROL Actual Amount]

   4. [!UICONTROL Description]

   5. [!UICONTROL Expense Type]

   6. [!UICONTROL Effective Date]

   7. [!UICONTROL Campaign Name]

   8. [!UICONTROL [!DNL Anaplan] List Item ID]
   Om het [!UICONTROL [!DNL Anaplan] Actual Expense Import] bestand:

   1. Kopieer en plak het volgende in een teksteditor of [!DNL Excel].
   1. Sla het bestand op in een CSV-indeling.
   1. Het bestand uploaden naar [!DNL Anaplan].

      Zie voor instructies de [!DNL Anaplan] documentatie over het invoeren van gegevens in modules van een dossier.

   1. Noteer de naam die u aan het bestand hebt gegeven; het zal worden gebruikt tijdens de inzet van [!UICONTROL Fusion] scenario-sjabloon.

   Voorbeeld-CSV-inhoud

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

* An **[!UICONTROL [!DNL Anaplan] Planned Expense Import]** bestand dat de volgende kolommen bevat, in deze volgorde:

   1. [!UICONTROL [!DNL Workfront] Expense GUID]

   2. [!UICONTROL [!DNL Workfront] Project GUID]

   3. [!UICONTROL Actual Amount]

   4. [!UICONTROL Description]

   5. [!UICONTROL Expense Type]

   6. [!UICONTROL Effective Date]

   7. [!UICONTROL Campaign Name]

   8. [!UICONTROL [!DNL Anaplan] List Item ID]
   Om het [!UICONTROL [!DNL Anaplan] Planned Expense Import] bestand:

   1. Kopieer en plak het volgende in een teksteditor of [!DNL Excel]
   1. Het bestand opslaan in een CSV-indeling
   1. Upload het bestand naar Anaplan.

      Zie voor instructies de [!DNL Anaplan] documentatie over het invoeren van gegevens in modules van een dossier.

   1. Noteer de naam die u aan het bestand hebt gegeven; het zal worden gebruikt tijdens de inzet van [!UICONTROL Fusion] scenario-sjabloon.

   Voorbeeld-CSV-inhoud

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>


* A **[!UICONTROL Project Update Import]** proces voorbereid om de invoer van gegevens uit te voeren die in een dossier worden geleverd uploadt.

>[!NOTE]
>
>Er zijn afzonderlijke invoerbestanden voor geplande en werkelijke uitgaven, zodat deze onafhankelijk kunnen worden gerapporteerd over de geplande en effectieve data.

Voor instructies over een van deze handelingen raadpleegt u de [!DNL Anaplan] documentatie.

## Distribueren naar [!DNL Fusion]

Voltooi de volgende stappen om dit integratiescenario aan uw op te stellen [!DNL Fusion] account. Dit mag alleen gebeuren nadat de vereiste [!DNL Workfront] en [!DNL Anaplan] configuratie.

1. Ga naar de [!UICONTROL Templates] menu in [!DNL Workfront Fusion] en klik op de knop **[!UICONTROL Send Workfront expenses updates to [!DNL Anaplan] list item]** scenario-sjabloon.
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
      <td>De id van de werkruimte van uw [!DNL Anaplan] account die u voor dit scenario wilt gebruiken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Model-id] </td> 
      <td>De id van het model van uw [!DNL Anaplan] en de geselecteerde werkruimte die u voor dit scenario wilt gebruiken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>De naam van de lijst in uw [!DNL Anaplan] en de geselecteerde werkruimte en het model die u voor dit scenario wilt gebruiken.</td> 
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

   In het dialoogvenster [!DNL Anaplan] installatiedocumentatie.

1. Een [!DNL Anaplan] verbindingsprofiel.
1. Alle resterende bijwerken [!DNL Anaplan] modules met een [!DNL Anaplan] verbinding, wanneer hierom wordt gevraagd.
1. Selecteer of voeg een [!DNL Workfront] verbindingsprofiel.
1. Alle resterende bijwerken [!DNL Workfront] modules met een [!DNL Workfront] verbinding, wanneer hierom wordt gevraagd.
1. Op de **[!UICONTROL Build Actual Expense CSV]** Voeg een nieuwe gegevensstructuur toe om de projectkenmerken toe te wijzen aan CSV-kolommen.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Op de **[!UICONTROL Build Planned Expense CSV]** Voeg een nieuwe gegevensstructuur toe om de projectkenmerken toe te wijzen aan CSV-kolommen.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

## Andere aanbevolen scènemasjablonen

Dit scenario malplaatje wordt gecomplimenteerd door het volgende speer malplaatjes van het optimalisatiescenario die ook kunnen worden opgesteld:

* [[!UICONTROL Send [!DNL Adobe Workfront] projectupdates voor een [!DNL Anaplan] lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] de daadwerkelijke uren updates aan een [!DNL Anaplan] lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

Aanvullende scenario&#39;s voor het koppelen van begrotingsaanvragen:

* [[!UICONTROL Create an [!DNL Anaplan] lijstitem uit een [!DNL Adobe Workfront] begrotingsverzoek]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] begrotingstoewijzing aan een [!DNL Adobe Workfront] project]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Aanvullende scenario&#39;s voor het koppelen van campagneverzoeken:

* [[!UICONTROL Create an [!DNL Anaplan] lijstitem uit een [!DNL Adobe Workfront] campagneverzoek]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] begrotingstoewijzing aan een [!DNL Adobe Workfront] campagneverzoek of campagneproject]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
