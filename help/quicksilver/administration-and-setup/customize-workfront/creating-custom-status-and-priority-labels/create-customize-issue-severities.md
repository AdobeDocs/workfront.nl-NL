---
title: Uitgiftecontroles maken of aanpassen
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Uw gebruikers kunnen serienummers gebruiken om te bepalen hoe ernstig een probleem is. U kunt een van de vijf standaardserienummers in Adobe Workfront aanpassen of een nieuwe ernst maken voor uw gebruikers.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# Uitgiftecontroles maken of aanpassen

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

Uw gebruikers kunnen serienummers gebruiken om te bepalen hoe ernstig een probleem is. U kunt een van de vijf standaardserienummers in Adobe Workfront aanpassen of een nieuwe ernst maken voor uw gebruikers.

>[!NOTE]
>
>Taken en projecten hebben geen verificaties.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ingebouwde uitgaven

Workfront beschikt over vijf ingebouwde uitgavesecties:

* Cosmetisch
* Verwardheid
* Fout met tijdelijke oplossing
* Fout zonder tijdelijke oplossing
* Fatale fout

<p>U kunt het volgende bewerken voor deze controles:</p>

* Naam
* Kleur

   De kleur van een ernst blijft behouden in een diagramrapport als u de resultaten groepeert op Issue Severity. Voor informatie over grafiekrapporten raadpleegt u [Een diagram toevoegen aan een rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Welke strengheid is het gebrek

   Voor meer informatie over standaardwaarden raadpleegt u [Ernst van uitgaven maken of bewerken](#create-or-edit-an-issue-severity) in dit artikel.
* Beschrijving
* Of een ernst verborgen is in Workfront

   Zie voor meer informatie over het verbergen van een ernst [Ernst van uitgaven maken of bewerken](#create-or-edit-an-issue-severity")

* Ernst verwijderen

   Wanneer u dit doet, moet u een vervangingsstrengheid selecteren.

## Ernst van uitgaven maken of bewerken {#create-or-edit-an-issue-severity}

Als Workfront-beheerder kunt u uitgiftesetters maken en bewerken die zijn afgestemd op de behoeften van uw gebruikers.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Projectvoorkeuren** > **Ernst**.

1. Als u een nieuwe ernst maakt, klikt u op **Een nieuwe prioriteit toevoegen**.
1. Vorm de volgende opties voor de nieuwe strengheid of geef hen voor bestaande uit:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ernstnaam</td> 
      <td>Typ een naam voor de ernst</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Belang</td> 
      <td>Verhoog of verlaag de ernst die oorspronkelijk door Workfront is toegewezen.
      <p>Het belangrijke aantal voor elke strengheid moet uniek zijn. Het hoogste getal komt overeen met het hoogste niveau van ernst.</p> <p>U kunt dit nummer niet bewerken nadat u de ernst hebt opgeslagen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kleur</td> 
      <td> <p>Kies een kleur voor de ernst.</p> 
      <p>De kleur van de ernst wordt gebruikt in grafiekrapporten wanneer u uw resultaten groepeert door de Ernst van de Uitgave. Voor informatie over grafiekrapporten raadpleegt u <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Een diagram toevoegen aan een rapport</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standaardernst</td> 
      <td>Selecteer de ernst die Workfront automatisch moet selecteren voor alle nieuwe uitgaven.</p>
      <p>Cosmetisch is de standaardernst voor problemen in Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td>Typ een beschrijving voor de ernst om de functie uit te leggen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verbergen</td> 
      <td> Verberg een ernst die u niet meer nodig hebt. 
      <p>Een verborgen ernst wordt nergens in Workfront weergegeven, dus gebruikers kunnen deze optie niet kiezen voor hun uitgaven.</p> 
      <p><b>BELANGRIJK</b>: In plaats van de controles te verwijderen die u niet meer wilt gebruiken, raden we u aan ze te verbergen. Op deze manier houdt u al uw historische gegevens over objecten die al met de ernst zijn voltooid, en voorkomt u dat mensen in de toekomst de ernst van de zaak zullen gebruiken.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Wijzig de volgorde van de aanbiedingen door deze in de gewenste volgorde te slepen.

   Dit verandert de orde waarin zij voor kwesties tonen. Het verandert niets aan **Belang** getal.

1. Klikken **Opslaan**.

Ga voor meer informatie over hoe u versies kunt gebruiken tijdens het werken met problemen naar [Ernst van probleem bijwerken](../../../manage-work/issues/issue-information/update-issue-severity.md).
