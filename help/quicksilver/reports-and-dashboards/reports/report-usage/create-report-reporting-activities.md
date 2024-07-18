---
product-area: reporting
keywords: wijziging,eigenaar,gedeeld,rapport,delen,gebruiker,toegang,rechten,ingevoerd,laatst,bekeken,datum,rapportage,activiteiten
navigation-topic: report-usage
title: Een rapport opstellen over rapportageactiviteiten
description: Wanneer u een rapport over rapporten creeert, kunt u specifieke rapportinformatie identificeren, die kan omvatten als de rapporten aan gedeactiveerde gebruikers worden toegewezen, als de rapporten om met toegangsrechten van een gedeactiveerde gebruiker worden geplaatst te lopen, als de gebruikers tot een rapport toegang hebben u, etc. van plan bent te schrappen.
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# Een rapport opstellen over rapportageactiviteiten

Wanneer u een rapport over rapporten creeert, kunt u specifieke rapportinformatie identificeren, die kan omvatten als de rapporten aan gedeactiveerde gebruikers worden toegewezen, als de rapporten om met toegangsrechten van een gedeactiveerde gebruiker worden geplaatst te lopen, als de gebruikers tot een rapport toegang hebben u, etc. van plan bent te schrappen.

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
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Rapport maken over bestaande rapporten {#create-the-report-about-existing-reports}

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront.
1. Klik **Rapporten**, dan **Nieuw Rapport**.
1. In het **Nieuwe drop-down menu van het Rapport**, uitgezochte **Rapport** om een rapport over bestaande rapporten tot stand te brengen.

1. In de **Kolommen (Mening)** tabel, voeg de kolommen toe u in uw rapport wilt.\
   Een aantal van de volgende velden kan nuttig zijn:

   | Veld | Beschrijving |
   |---|---|
   | **looppas als Gebruiker: Naam** | Dit is de gebruiker die in de **wordt gespecificeerd stel dit rapport met de Rechten van de Toegang van:** gebied op het rapport in werking. Als deze gebruiker wordt gedeactiveerd, toont een rapport niet voor iedereen het rapport wordt gedeeld met. |
   | **Gedeeld met** | Dit zijn alle entiteiten waarmee het rapport wordt gedeeld. |
   | **ingegaan door** | Dit is de eigenaar van het rapport. |
   | **Laatste Bekeken Datum** | Dit is de datum en tijd waarop het rapport voor het laatst door een gebruiker is bekeken. |

   {style="table-layout:auto"}

1. (Optioneel) U kunt als volgt uw lijst met rapporten beperken tot specifieke gedeactiveerde gebruikers:

   1. Selecteer het **lusje van Filters**, dan klik **een Regel van de Filter** toevoegen.

   1. Voeg de filter **Looppas als Gebruiker - identiteitskaart** > **Gelijk** toe.

   1. Typ de naam van de gedeactiveerde gebruiker die u aan het filter wilt toevoegen en klik vervolgens op de naam wanneer deze in de lijst wordt weergegeven.
   1. Herhaal Stap C tot u alle gedeactiveerde gebruikers hebt geselecteerd u in het rapport wilt omvatten.

1. (Optioneel) U kunt als volgt uw lijst met rapporten beperken tot geplande rapporten:

   1. Selecteer het **lusje van Filters**, dan klik **een Regel van de Filter** toevoegen.

   1. Voeg filter **Geplande identiteitskaart van het Rapport** toe > **is niet leeg**.

1. Klik **sparen + Sluiten**, dan typ een naam voor het rapport, en klik **sparen Rapport**.

   Uw rapportgegevens worden weergegeven.

1. (Optioneel) Exporteer dit rapport naar Excel en sla het op uw computer op.\
   Voor informatie bij het uitvoeren van een rapport, zie [ Gegevens van de Uitvoer ](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Informatie over een rapport bijwerken

Nadat u uw rapport hebt gemaakt, kunt u uw rapporten naar wens bijwerken.

1. Ga naar het rapport dat u wilt bijwerken.
1. Voer afhankelijk van de actie die u wilt uitvoeren een van de volgende handelingen uit:

   * Werk **in werking stelt dit rapport met de Rechten van de Toegang van:** gebied aan een actieve gebruiker bij: Voor meer informatie, zie [ Looppas en lever een rapport met de toegangsrechten van een andere gebruiker ](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * Creeer een exemplaar van het rapport: Voor meer informatie, zie [ een exemplaar van een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md) creëren.
   * Schrap een rapport: Voor meer informatie, zie [ een nauwkeurige exemplaar van een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) sectie van het artikel [ creëren een exemplaar van een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * Deel een rapport: Voor meer informatie, zie [ een rapport in Adobe Workfront ](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md) delen.

1. (Voorwaardelijk) als u de originele rapporten kopieert, gebruik de informatie van het rapport u in [ creeerde leidt tot het rapport over bestaande rapporten ](#create-the-report-about-existing-reports) om de nieuwe exemplaren met de zelfde entiteiten zoals de originele rapporten te delen.
