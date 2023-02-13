---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Een [!DNL Anaplan] lijstitem uit een [!DNL Adobe Workfront] begrotingsverzoek
description: Dit integratiescenario verbindt [!DNL Adobe Workfront] project (campagne) met een [!DNL Anaplan] begrotingspost. Dit wordt bereikt door een begrotingsverzoek toe te voegen aan de [!DNL Workfront] een project waarvoor financiering nodig is. In dit scenario wordt gezocht naar onverwerkte begrotingsaanvragen en wordt vervolgens een proces uitgevoerd om een lege begrotingspost te maken in [!DNL Anaplan] de procedures voor de toewijzing van begrotingsmiddelen in Anaplan op te starten.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Een [!DNL Anaplan] lijstitem uit een [!DNL Adobe Workfront] begrotingsverzoek

Dit integratiescenario verbindt [!DNL Adobe Workfront] project (campagne) met een [!DNL Anaplan] begrotingspost. Dit wordt bereikt door een begrotingsverzoek toe te voegen aan de [!DNL Workfront] een project waarvoor financiering nodig is. In dit scenario wordt gezocht naar onverwerkte begrotingsaanvragen en wordt vervolgens een proces uitgevoerd om een lege begrotingspost te maken in [!DNL Anaplan] om de procedures voor begrotingstoewijzing te starten in [!DNL Anaplan].

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
   <td role="rowheader" [!DNL>Adobe Workfront Fusion]-licentie**</td> 
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr>
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

&#42;&#42;Voor informatie over[!DNL  Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Triginggebeurtenis

Dit scenario wordt gepland om de 15 minuten uit te voeren.

## Verwacht [!DNL Workfront] Configuratie

U moet het volgende opgeven in [!DNL Workfront] om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Workfront] benoemd *[!UICONTROL *[!DNL Anaplan] Integration]**, dat de rechten van de systeembeheerder heeft.

   Voor informatie over het maken van een gebruiker in [!DNL Workfront], zie [Gebruikers toevoegen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL Budget Request]** aangepast formulier dat is gekoppeld aan het [!UICONTROL Request] object.

   De volgende vereiste velden moeten in het aangepaste formulier worden opgenomen om te helpen bij het in kaart brengen van gegevens naar [!DNL Anaplan]:

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

   Voor informatie over het maken van aangepaste formulieren raadpleegt u [Een aangepast formulier maken of bewerken](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* Projectsjablonen die campagnes en andere projecten vertegenwoordigen waarvoor financiering vereist is, geconfigureerd met een [!UICONTROL Budget Request] onderwerp in wachtrij. De [!UICONTROL Budget Request] het rijonderwerp wordt toegewezen om te gebruiken [!UICONTROL Budget Request] aangepast formulier.
* A **[!UICONTROL Campaign Brief]** formulier voor het projectobject.

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

   Voor informatie over het maken van aangepaste formulieren raadpleegt u [Een aangepast formulier maken of bewerken](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Verwacht [!DNL Anaplan] Configuratie

U moet het volgende opgeven in [!DNL Anaplan] om dit scenario te gebruiken:

* Een gebruikersprofiel in [!DNL Anaplan] benoemd **[!UICONTROL [!DNL Workfront] Integration]**, die beheerdersrechten voor het systeem heeft.
* De [!DNL Anaplan] Model dat u voor dit scenario wilt gebruiken.
* De lijst in de [!DNL Anaplan] Model dat campagnebudgetten vastlegt.

   De module van de lijst moet het ontvangen van de volgende attributen steunen:

   * [!UICONTROL Workfront Project GUID]
   * [!UICONTROL Campaign Name]
   * [!UICONTROL Requested Labor Funds]
   * [!UICONTROL Requested Expense Funds]
   * [!UICONTROL Budget Request Type]
   * [!UICONTROL Reason for Funding Adjustment]

   In deze lijst en module moeten aanvullende gegevens worden opgeslagen die nodig zijn voor de normale functionaliteit van [!DNL Anaplan], met inbegrip van de mogelijkheid om een begroting vast te stellen en te melden dat de begrotingspost gereed is om te worden gesynchroniseerd naar [!DNL Workfront].

Voor instructies over een van deze handelingen raadpleegt u de [!DNL Anaplan] documentatie.

## Distribueren naar [!DNL Workfront Fusion]

Voltooi de volgende stappen om dit integratiescenario aan uw op te stellen [!DNL Fusion] account. Dit mag alleen gebeuren nadat de vereiste [!DNL Workfront] en [!DNL Anaplan] configuratie.

1. Ga naar de [!UICONTROL Templates] menu in [!DNL Workfront Fusion] en klik op de knop **[!UICONTROL Create an [!DNL Anaplan] list item from a Workfront budget request]** scenario-sjabloon.
1. De waarden van variabelen vervangen voor het volgende [!DNL Anaplan] variabelen:

   | Naam variabele | Waarde vervangen door |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] Workspace ID] | De id van een werkruimte van uw [!DNL Anaplan] account. |
   | [!UICONTROL [!DNL Anaplan] Model ID] | De id van een model van uw [!DNL Anaplan] en de geselecteerde werkruimte. |
   | [!UICONTROL [!DNL Anaplan] Module Name] | De naam van de module die de campagnekenmerken in de geselecteerde [!DNL Anaplan] Lijst. |
   | [!UICONTROL Campaign List Name] | De naam van de lijst in uw [!DNL Anaplan] en de geselecteerde werkruimte en het geselecteerde model. |

   {style=&quot;table-layout:auto&quot;}

   In het dialoogvenster [!DNL Anaplan] installatiedocumentatie.

1. Een [!DNL Anaplan] verbindingsprofiel.
1. Alle resterende bijwerken [!DNL Anaplan] modules met een [!DNL Anaplan] verbinding, wanneer hierom wordt gevraagd.
1. Selecteer of voeg een [!DNL Workfront] verbindingsprofiel.

   Na het opstellen van het malplaatje, is dit de module u zult bijwerken om douanegebiedsverwijzingen aan de waarde van het gebiedsbezit toe te voegen of te verwijderen als u de standaard in kaart gebrachte gebieden wilt veranderen aan [!DNL Anaplan].

1. Alle resterende bijwerken [!DNL Workfront] modules met een [!DNL Workfront] verbinding, wanneer hierom wordt gevraagd.

## Andere aanbevolen scènemasjablonen

Om het werkschema te voltooien door dit malplaatje wordt vertegenwoordigd, moet u het volgende extra malplaatje ook opstellen dat:

* [[!UICONTROL Apply an [!DNL Anaplan] begrotingstoewijzing aan een [!DNL Adobe Workfront] project]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Aanvullende scenario&#39;s voor optimalisatie van uitgaven zijn:

* [[!UICONTROL Send [!DNL Adobe Workfront] projectupdates voor een [!DNL Anaplan] lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] de daadwerkelijke uren updates aan een [!DNL Anaplan] lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] uitgaven voor een [!DNL Anaplan] lijstitem]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
