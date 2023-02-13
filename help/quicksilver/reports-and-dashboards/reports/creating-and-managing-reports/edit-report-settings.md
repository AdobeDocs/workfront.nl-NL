---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Rapportinstellingen bewerken
description: U kunt de montages van een rapport uitgeven om te bepalen hoe het voor andere gebruikers toont, of welk soort informatie gebruikers voor kan roepen alvorens zij het rapport in werking stellen.
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Rapportinstellingen bewerken

U kunt de montages van een rapport uitgeven om te bepalen hoe het voor andere gebruikers toont, of welk soort informatie gebruikers voor kan roepen alvorens zij het rapport in werking stellen.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Hoe kan ik-stappen

1. Maak een rapport door naar de **Hoofdmenu** > **Rapporten** selecteert u vervolgens het object van het rapport.

   of

   Open een bestaand rapport en klik vervolgens op **Handelingen rapporteren** > **Bewerken**.

1. Klikken **Rapportinstellingen** in de hoger-juiste hoek van de rapportaannemer.
1. Vorm de volgende rapportmontages:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Rapporttitel</td> 
      <td>Geef een titel op voor het rapport.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td>Specificeer een verklaring beschrijvend het doel en het gebruik van het rapport.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dit rapport uitvoeren met de toegangsrechten van</td> 
      <td>Selecteer de gebruiker van wie de toegangsrechten u dit rapport wilt gebruiken wanneer het tonen voor andere gebruikers. Raadpleeg het artikel voor meer informatie over het uitvoeren van een rapport met de toegangsrechten van een andere gebruiker <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Een rapport uitvoeren en leveren met de toegangsrechten van een andere gebruiker</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wanneer het rapport wordt geladen, geeft u de opdracht</td> 
      <td>Selecteer het standaardlusje dat voor alle gebruikers wordt getoond wanneer het rapport laadt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wanneer het rapport op een dashboard laadt, toon... items</td> 
      <td>Geef het aantal items op dat voor alle gebruikers wordt weergegeven wanneer het rapport op een dashboard wordt geladen. De standaardwaarde is 15 items en het maximumaantal items is 200.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">De weergave Bronraster weergeven op het tabblad Details</td> 
      <td> <p>(Alleen gebruikersrapport) Selecteer deze optie om het Resource Grid op het tabblad Details van het rapport weer te geven.</p> <p>Opmerking: Wanneer het toepassen van de mening van het Net van het Middel op een gebruikersrapport, toont het rapport slechts projecten die in de Huidige status zijn. Als u projecten in een andere status wilt zien, kunt u het Lusje van het Gebruik van de Gebruiker in het gebied van Mensen van de Globale Bar van de Navigatie gebruiken, en de Mening van het Net van het Middel daar toepassen. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een speciale weergave weergeven op het tabblad Details</td> 
      <td>(Alleen projectrapport) Geef het type weergave op dat gebruikers zien wanneer ze deze informatie openen op het tabblad Details. U kunt bijvoorbeeld een mijlpaal- of Gantt-weergave selecteren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dit rapport standaard weergeven in een Gantt-weergave</td> 
      <td>(Alleen projectrapport en taakrapport) Selecteer deze optie als u de Gantt-weergave automatisch wilt inschakelen wanneer gebruikers het tabblad Details in dit rapport weergeven.<br>Voor meer informatie over het bekijken van de grafiek van Gantt in projectrapporten en taakrapporten, zie de sectie "de taakomschrijving van de Mening in de projectenlijst Gantt Grafiek"in het artikel <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Informatie weergeven in de Gantt-grafiek </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Weergave wijzigen in rapport toestaan</td> 
      <td>Selecteer deze optie als u wilt dat gebruikers de weergave kunnen wijzigen wanneer ze het rapport uitvoeren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Groep toestaan om op het rapport te worden gewijzigd</td> 
      <td>Selecteer deze optie om gebruikers toe te staan om de Groep te veranderen wanneer het runnen van het rapport.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Filter wijzigen in rapport toestaan</td> 
      <td>Selecteer deze optie om gebruikers toe te staan om de Filter te veranderen wanneer het runnen van het rapport.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Prompts rapporteren** aan opstelling om het even welke herinneringen voor het rapport.\
   Voor meer informatie over het toevoegen van herinneringen aan een rapport, zie het artikel [Een vraag toevoegen aan een rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Klikken **Gereed,** klik vervolgens op **Opslaan + Sluiten**.

## Aanvullende informatie

Zie ook:

* [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program)
* [Aan de slag met rapporten in Adobe Workfront](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Ingebouwde Adobe Workfront-rapporten gebruiken](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
