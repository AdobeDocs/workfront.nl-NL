---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Verzenden [!DNL Adobe Workfront] projectupdates voor een [!DNL Anaplan] lijstitem
description: Dit integratiescenario deelt vooruitgang, status, en belangrijkste planningsdetails van een [!DNL Adobe Workfront] met een [!DNL Anaplan] begrotingspost. Door deze informatie te delen kunt u beter profiteren van de optimalisatie van uitgaven en de financiële analyse die [!DNL Anaplan] verstrekt.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# Verzenden [!DNL Adobe Workfront] projectupdates voor een [!DNL Anaplan] lijstitem

Dit integratiescenario deelt vooruitgang, status, en belangrijkste planningsdetails van een [!DNL Adobe Workfront] met een [!DNL Anaplan] begrotingspost. Door deze informatie te delen kunt u beter profiteren van de optimalisatie van uitgaven en de financiële analyse die [!DNL Anaplan] verstrekt.

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

* Een gebruikersprofiel in [!DNL Workfront] benoemd **[!UICONTROL [!DNL Anaplan] Integration]**, die beheerdersrechten voor het systeem heeft.

   Voor informatie over het maken van een gebruiker in [!DNL Workfront], zie [Gebruikers toevoegen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL Campaign Brief]** aangepast formulier dat aan het projectobject is gekoppeld, om aangepaste gegevenswaarden op te slaan die u naar Anaplan wilt verzenden.

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

   Voor informatie over het maken van aangepaste formulieren raadpleegt u [Een aangepast formulier maken of bewerken](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## Verwacht [!DNL Anaplan] Configuratie

U moet het volgende opgeven in [!DNL Anaplan] om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Anaplan] benoemd **[!UICONTROL [!DNL Workfront] Integration]**, die beheerdersrechten voor het systeem heeft.
* De [!DNL Anaplan] Model dat u voor dit scenario wilt gebruiken.
* De lijst in de [!DNL Anaplan] Model dat u voor dit scenario wilt gebruiken.
* A **[!UICONTROL Project Update Import]** bestand dat de volgende kolommen bevat, in deze volgorde:

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

Om het [!UICONTROL [!DNL Anaplan] Planned Expense Import] bestand:

1. Kopieer en plak het volgende in een teksteditor of [!DNL Excel]
1. Het bestand opslaan in een CSV-indeling
1. Upload het bestand naar Anaplan.

   Zie voor instructies de [!DNL Anaplan] documentatie over het invoeren van gegevens in modules van een dossier.

1. Noteer de naam die u aan het bestand hebt gegeven; het zal worden gebruikt tijdens de inzet van [!UICONTROL Fusion] scenario-sjabloon.

Voorbeeld-CSV-inhoud

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

1. [!UICONTROL Campaign Overview]

2. [!UICONTROL Key Message]

3. [!UICONTROL In Market Start Date]

4. [!UICONTROL In Market End Date]

5. [!UICONTROL Target Audience]

Neem ook alle andere velden op die u in de toewijzing wilt instellen.

* A **[!UICONTROL Project Update Import]** proces voorbereid om de invoer van gegevens uit te voeren die in een dossier worden geleverd uploadt.

Voor instructies over een van deze handelingen raadpleegt u de [!DNL Anaplan] documentatie.

## Distribueren naar [!DNL Workfront Fusion]

Voer de volgende stappen uit om dit integratiescenario in te zetten op uw Fusion-account. Dit mag alleen gebeuren nadat de vereiste [!DNL Workfront] en [!DNL Anaplan] configuratie.

1. Ga naar de [!UICONTROL Templates] menu in [!DNL Workfront Fusion] en klik op de knop **[!UICONTROL Send Workfront project updates to [!DNL Anaplan] list item]** scenario-sjabloon.
1. De waarden van variabelen vervangen voor het volgende [!DNL Anaplan] variabelen:

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
      <td role="rowheader">[!UICONTROL File Name: Project Update Import]</td> 
      <td>De naam van het bestand dat de projectupdategegevens ontvangt.<p>(Voorbeeld: WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Project Update Import]</td> 
      <td> <p>De naam van het proces dat de invoer van projectgegevens zal uitvoeren.</p> <p>(Voorbeeld: WF Int - Informatie over campagnes bijwerken)</p> </td> 
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

   Het filter wordt gevormd om in al onvolledig verbonden project en die projecten te trekken die in de laatste 29 minuten werden voltooid. Als u de frequentie van de [!DNL Fusion] Het scenario u zal deze waarde willen bijwerken zodra het scenario malplaatje is opgesteld.

1. Op de **[!UICONTROL Build Projects Update CSV]** Voeg een nieuwe gegevensstructuur toe om de projectkenmerken toe te wijzen aan CSV-kolommen.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Alle resterende bijwerken [!DNL Workfront] modules met een [!DNL Workfront] verbinding, wanneer hierom wordt gevraagd.

## Andere aanbevolen scènemasjablonen

Dit scenario malplaatje wordt gecomplimenteerd door het volgende speer malplaatjes van het optimalisatiescenario die ook kunnen worden opgesteld:

* [[!UICONTROL Send [!DNL Adobe Workfront] de daadwerkelijke uren updates aan een [!DNL Anaplan] lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] uitgaven voor een [!DNL Anaplan] lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Aanvullende scenario&#39;s voor het koppelen van begrotingsaanvragen:

* [[!UICONTROL Create an [!DNL Anaplan] lijstitem uit een [!DNL Adobe Workfront] begrotingsverzoek]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] begrotingstoewijzing aan een [!DNL Adobe Workfront] project]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Aanvullende scenario&#39;s voor het koppelen van campagneverzoeken:

* [[!UICONTROL Create an [!DNL Anaplan] lijstitem uit een [!DNL Adobe Workfront] campagneverzoek]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] begrotingstoewijzing aan een [!DNL Adobe Workfront] campagneverzoek of campagneproject]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
