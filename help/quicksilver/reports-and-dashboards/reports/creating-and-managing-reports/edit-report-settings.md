---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Rapportinstellingen bewerken
description: U kunt de montages van een rapport uitgeven om te bepalen hoe het voor andere gebruikers toont, of welk soort informatie gebruikers voor kan roepen alvorens zij het rapport in werking stellen.
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# Rapportinstellingen bewerken

<!-- Audited: 11/2024 -->

U kunt de montages van een rapport uitgeven om te bepalen hoe het voor andere gebruikers toont, of welk soort informatie gebruikers voor kan roepen alvorens zij het rapport in werking stellen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
      <p>Standard</p>
      <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuratie op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
 <td> <p>Machtigingen beheren voor een rapport</p></td>  
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Procedure

1. Begin creërend een rapport door naar het **Belangrijkste menu** te gaan > **Rapporten**, dan het voorwerp van uw rapport te selecteren.

   of

   Open een bestaand rapport, dan klik **de Acties van het Rapport** > **uitgeven**.

1. Klik **Montages van het Rapport** in de hoger-juiste hoek van de rapportbouwer.
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
      <td>Selecteer de gebruiker van wie de toegangsrechten u dit rapport wilt gebruiken wanneer het tonen voor andere gebruikers. Voor meer informatie over het runnen van een rapport met de toegangsrechten van een andere gebruiker, zie het artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref"> Looppas en lever een rapport met de toegangsrechten van een andere gebruiker </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wanneer het rapport wordt geladen, geeft u de opdracht</td> 
      <td>Selecteer het standaardlusje dat voor alle gebruikers wordt getoond wanneer het rapport laadt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wanneer het rapport op een dashboard wordt geladen, ... items tonen</td> 
      <td>Geef het aantal items op dat voor alle gebruikers wordt weergegeven wanneer het rapport op een dashboard wordt geladen. De standaardwaarde is 15 items en het maximumaantal items is 200.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">De weergave Bronraster weergeven op het tabblad Details</td> 
      <td> <p>(Alleen gebruikersrapport) Selecteer deze optie om het Resource Grid op het tabblad Details van het rapport weer te geven.</p> <p>Nota: Wanneer het toepassen van de mening van het Net van het Middel op een gebruikersrapport, toont het rapport slechts projecten die in de Huidige status zijn. Als u projecten in een andere status wilt zien, kunt u het Lusje van het Gebruik van de Gebruiker in het gebied van Mensen van de Globale Bar van de Navigatie gebruiken, en de Mening van het Net van het Middel daar toepassen. <!--
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
      <td>(Alleen projectrapport en taakrapport) Selecteer deze optie als u de Gantt-weergave automatisch wilt inschakelen wanneer gebruikers het tabblad Details in dit rapport weergeven.<br> voor meer informatie over het bekijken van de grafiek van Gantt in projectrapporten en taakrapporten, zie de sectie "de taakinformatie van de Mening in de van de projectlijst Gantt Grafiek"in de artikel <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref"> informatie van de Mening in de Grafiek van Gantt </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Weergave wijzigen in rapport toestaan</td> 
      <td>Selecteer deze optie als u wilt dat gebruikers de weergave kunnen wijzigen wanneer ze het rapport uitvoeren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Groep toestaan om op het rapport te worden gewijzigd</td> 
      <td>Selecteer deze optie als gebruikers de groep mogen wijzigen wanneer ze het rapport uitvoeren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Filter wijzigen in rapport toestaan</td> 
      <td>Selecteer deze optie om gebruikers toe te staan om de Filter te veranderen wanneer het runnen van het rapport.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **Vragen van het Rapport** aan opstelling om het even welke herinneringen voor het rapport.\
   Voor meer informatie over het toevoegen van herinneringen aan een rapport, zie het artikel [&#x200B; een herinnering aan een rapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md) toevoegen.

1. Klik **Gedaan,** dan klik **sparen + Sluiten**.

## Aanvullende informatie

Zie ook:

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [&#x200B; worden begonnen met rapporten &#x200B;](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [&#x200B; de ingebouwde rapporten van Adobe Workfront van het Gebruik &#x200B;](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
