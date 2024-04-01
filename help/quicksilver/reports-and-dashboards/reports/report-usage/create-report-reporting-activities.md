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
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Rapport maken over bestaande rapporten {#create-the-report-about-existing-reports}

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) rechtsboven in Adobe Workfront.
1. Klikken **Rapporten** vervolgens **Nieuw rapport**.
1. In de **Nieuw rapport** vervolgkeuzemenu, selecteren **Rapport** een verslag op te stellen over bestaande verslagen.

1. In de **Kolommen (weergave)** voegt u de kolommen toe die u in het rapport wilt opnemen.\
   Een aantal van de volgende velden kan nuttig zijn:

   | Veld | Beschrijving |
   |---|---|
   | **Als gebruiker uitvoeren: naam** | Dit is de gebruiker die is opgegeven in het dialoogvenster **Voer dit rapport uit met de toegangsrechten van:** in het verslag. Als deze gebruiker wordt gedeactiveerd, toont een rapport niet voor iedereen het rapport wordt gedeeld met. |
   | **Gedeeld met** | Dit zijn alle entiteiten waarmee het rapport wordt gedeeld. |
   | **Ingevoerd door** | Dit is de eigenaar van het rapport. |
   | **Datum van laatste weergave** | Dit is de datum en tijd waarop het rapport voor het laatst door een gebruiker is bekeken. |

   {style="table-layout:auto"}

1. (Optioneel) U kunt als volgt uw lijst met rapporten beperken tot specifieke gedeactiveerde gebruikers:

   1. Selecteer de **Filters** tab, en klik vervolgens op **Filterregel toevoegen**.

   1. Het filter toevoegen **Uitvoeren als gebruikersnaam** > **Gelijk**.

   1. Typ de naam van de gedeactiveerde gebruiker die u aan het filter wilt toevoegen en klik vervolgens op de naam wanneer deze in de lijst wordt weergegeven.
   1. Herhaal Stap C tot u alle gedeactiveerde gebruikers hebt geselecteerd u in het rapport wilt omvatten.

1. (Optioneel) U kunt als volgt uw lijst met rapporten beperken tot geplande rapporten:

   1. Selecteer de **Filters** tab, en klik vervolgens op **Filterregel toevoegen**.

   1. Het filter toevoegen **Geplande rapport-id** > **Is niet leeg**.

1. Klikken **Opslaan + Sluiten** typt u vervolgens een naam voor het rapport en klikt u op **Rapport opslaan**.

   Uw rapportgegevens worden weergegeven.

1. (Optioneel) Exporteer dit rapport naar Excel en sla het op uw computer op.\
   Voor informatie over het exporteren van een rapport raadpleegt u [Gegevens exporteren](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

## Informatie over een rapport bijwerken

Nadat u uw rapport hebt gemaakt, kunt u uw rapporten naar wens bijwerken.

1. Ga naar het rapport dat u wilt bijwerken.
1. Voer afhankelijk van de actie die u wilt uitvoeren een van de volgende handelingen uit:

   * Werk de **Voer dit rapport uit met de toegangsrechten van:** veld voor een actieve gebruiker: zie voor meer informatie [Een rapport uitvoeren en leveren met de toegangsrechten van een andere gebruiker](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

   * Een kopie van het rapport maken: zie voor meer informatie [Een kopie van een rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).
   * Een rapport verwijderen: raadpleeg de [Een exacte kopie van een rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2) artikel [Een kopie van een rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

   * Een rapport delen: Zie voor meer informatie [Een rapport delen in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

1. (Voorwaardelijk) als u de originele rapporten kopieert, gebruik de informatie van het rapport u in creeerde [Rapport maken over bestaande rapporten](#create-the-report-about-existing-reports) om de nieuwe kopieën te delen met dezelfde entiteiten als de oorspronkelijke rapporten.
