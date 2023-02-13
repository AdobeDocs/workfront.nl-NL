---
title: Prioriteiten maken en aanpassen
description: U kunt de prioriteiten voor projecten, taken, en kwesties in het gebied van de Opstelling van Workfront controleren. Prioriteiten geven belang aan uw projecten, taken of problemen in Adobe Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Prioriteiten maken en aanpassen

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

U kunt de prioriteiten voor projecten, taken, en kwesties in het gebied van de Opstelling van Workfront controleren. Prioriteiten geven belang aan uw projecten, taken of problemen in Adobe Workfront.

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

## Bestaande prioriteiten aanpassen

Als beheerder van Workfront, kunt u de volgende wijzigingen in de standaardprioriteiten aanbrengen die in Workfront worden verstrekt:

* Naam van prioriteiten wijzigen.
* Herstel de prioriteiten.

   Ga voor meer informatie over het aanpassen van prioriteiten naar [Een prioriteit maken voor een projecttaak of uitgave](#create-a-priority-for-a-project-task-or-issue).

* Wijzig de standaardprioriteit.

   Voor meer informatie over de functionaliteit om de standaardprioriteit te veranderen, zie [Een prioriteit maken voor een projecttaak of uitgave](#create-a-priority-for-a-project-task-or-issue).

* Bewerk de beschrijving van de prioriteiten.
* Stel een kleur in voor elke prioriteit.

   De kleur van de prioriteit wordt gebruikt in grafiekrapporten, wanneer u uw resultaten door groepeert **Prioriteit**.

   Voor meer informatie over grafiekrapporten, zie [Een diagram toevoegen aan een rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Prioriteiten verwijderen.

   Wanneer u een bestaande prioriteit verwijdert, moet u een vervangende prioriteit selecteren.

* Prioriteiten verbergen.

   Ga voor meer informatie over de functionaliteit van het verbergen van prioriteiten naar [Een prioriteit maken voor een projecttaak of uitgave](#create-a-priority-for-a-project-task-or-issue).

   >[!NOTE]
   >
   >U moet voor elk object ten minste één prioriteit in uw Workfront-account hebben.

De prioriteiten die standaard worden opgegeven voor elk objecttype (project, taak en uitgave) zijn identiek:

* Geen
* Laag
* Normaal
* Hoog
* Dringend

## Een prioriteit maken voor een projecttaak of uitgave {#create-a-priority-for-a-project-task-or-issue}

Naast de standaardprioriteiten in Workfront kunt u ook uw eigen prioriteiten toevoegen om aan de behoeften van uw organisatie te voldoen.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Projectvoorkeuren** > **Prioriteiten**.

1. Klik op de tab voor het objecttype waarvoor u een prioriteit wilt maken (**Project**, **Taak**, of **Probleem**).
1. Klikken **Een nieuwe prioriteit toevoegen**.
1. Geef de volgende informatie op voor de nieuwe prioriteit:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Prioriteitsnaam</td> 
      <td>Typ een naam voor uw prioriteit.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Belang</td> 
      <td> <p>Wanneer het toevoegen van een nieuwe prioriteit, wordt een aantal toegewezen aan het door gebrek. Bewerk dit nummer als het niet aan uw wensen voldoet.</p> <p>De <strong>Belang</strong> Het nummer voor elke prioriteit moet uniek zijn voor het object dat u hebt geselecteerd.<br>Het nummer van de prioriteit geeft het belang van het project, de taak of het vraagstuk weer: het hoogste aantal komt overeen met de hoogste prioriteit .</p> <p><b>OPMERKING</b>: U kunt het belangrijke nummer niet meer bewerken nadat u de prioriteit hebt opgeslagen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kleur</td> 
      <td> <p>Kies een kleur voor uw prioriteit.</p> <p>De kleur van de prioriteit wordt gebruikt in grafiekrapporten en de Montages van het Team van de Gelijkheid. Voor meer informatie over grafiekrapporten, zie <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Een diagram toevoegen aan een rapport</a>.</p> <p>Voor meer informatie over de Montages van het Team van de Geldige, zie in.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standaardprioriteit</td> 
      <td> <p>Bepaal of dit een standaardprioriteit moet zijn of niet door het keuzerondje te selecteren.</p> <p>Indien een prioriteit wordt aangewezen als de <strong>Standaardprioriteit</strong>, wordt deze automatisch gekozen voor alle projecten, taken of problemen in Workfront. <strong>Normaal</strong> is de standaardprioriteit voor alle objecten in Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td>Voeg een beschrijving voor uw prioriteit toe om zijn functie te verklaren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verbergen</td> 
      <td> <p>Selecteer dit vakje als u de prioriteit wilt verbergen.</p><p>Wanneer u <b>Verbergen</b> -optie, wordt de prioriteit nergens in Workfront weergegeven en kunnen gebruikers deze niet kiezen voor hun projecten, taken en problemen.</p> 
      <p><b>BELANGRIJK</b>: We raden u aan de prioriteiten die u niet meer wilt gebruiken, te verbergen in plaats van ze te verwijderen. Door ze te verbergen, houdt u nog steeds al uw historische gegevens bij, van objecten die met deze prioriteit zijn voltooid, en voorkomt u dat mensen in de toekomst deze prioriteit kiezen. </p>
      <p>U kunt desgewenst de volgorde van uw prioriteiten wijzigen door deze in de gewenste volgorde te slepen. Dit verandert de orde waarin zij voor projecten, taken, en kwesties tonen. Dit verandert niets aan <b>Belang</b> getal. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Opslaan**.

Zie de volgende artikelen voor instructies over het toepassen van prioriteiten op projecten, taken en kwesties:

* [De projectprioriteiten begrijpen en bijwerken](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Taakprioriteit bijwerken](../../../manage-work/tasks/task-information/task-priority.md)
* [Prioriteit van probleem bijwerken](../../../manage-work/issues/issue-information/update-issue-priority.md)
