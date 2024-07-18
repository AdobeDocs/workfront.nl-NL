---
product-area: reporting;user-management
keywords: opslaan,nieuw,rapport,kopiëren
navigation-topic: create-and-manage-reports
title: Een kopie van een rapport maken
description: U kunt een kopie maken van elk rapport waartoe u toegang hebt. U kunt of een nauwkeurige exemplaar van een douanerapport tot stand brengen of u kunt een nieuwe versie van een standaardrapport bewaren. Nadat u een rapport kopieert, wordt u de eigenaar van het gekopieerde rapport en het toont in de Mijn sectie van Rapporten.
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# Een kopie van een rapport maken

U kunt een kopie maken van elk rapport waartoe u toegang hebt. U kunt of een nauwkeurige exemplaar van een douanerapport tot stand brengen of u kunt een nieuwe versie van een standaardrapport bewaren. Nadat u een rapport kopieert, wordt u de eigenaar van het gekopieerde rapport en het toont in de Mijn sectie van Rapporten.

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
   <td> <p>Toestemmingen aan een rapport weergeven</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Een exacte kopie van een rapport maken

Ga als volgt te werk als u een kopie wilt maken van een rapport waarvan u de eigenaar bent:

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront.

1. Klik **Rapporten**, dan **Alle Rapporten**.
1. Open een rapport.
1. Klik **Acties van het Rapport**, toen **Exemplaar**.

   >[!TIP]
   >
   >Als het rapport een standaardrapport is, verschijnt de optie van het Exemplaar niet in het menu van de Acties van het Rapport.\
   >Voor informatie over hoe te om een exemplaar van een standaardrapport tot stand te brengen, zie [ een nieuwe versie van een rapport ](#create-a-new-version-of-a-report) creëren.

   ![ het rapport van het Exemplaar ](assets/nwe-fulllistofreportactions-2022.png)

   Een exemplaar van het originele rapport wordt gecreeerd met de standaardnaam van *Exemplaar van [ Naam van het originele rapport]*. Bijvoorbeeld, zou het rapport &quot;Q4 Voltooide Taken&quot;&quot;Exemplaar van Q4 Voltooide Taken&quot;als naam hebben.

1. (Optioneel) Als u de naam van het rapport wilt wijzigen, typt u een nieuwe naam.

   >[!TIP]
   >
   >Als u de titel deselecteert voordat u de nieuwe naam typt, selecteert u de rapporttitel, verwijdert u de naam en voert u de nieuwe naam in.

1. (Facultatief) om de nieuwe versie van het rapport met andere gebruikers te delen, klik **Acties van het Rapport**, toen **het Delen**.

   >[!NOTE]
   >
   >De delende informatie brengt niet naar het gekopieerde rapport over van de originele versie.\
   >Voor informatie over hoe te zien wie het vorige rapport met werd gedeeld, zie [ een rapport over het melden van activiteiten ](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify) creëren.

1. (Optioneel) Als u beheermachtigingen hebt voor het oorspronkelijke rapport en het oorspronkelijke rapport niet meer nodig is, kunt u het verwijderen om overbodige dubbele rapporten in Workfront te verwijderen.

   Ga als volgt te werk om het oorspronkelijke rapport te verwijderen:

   1. Navigeer naar het rapport.
   1. Klik **de Acties van het Rapport**, dan **Schrapping**.

   1. Klik **ja, schrap het** om te bevestigen dat u het rapport wilt schrappen.

## Een nieuwe versie van een rapport maken {#create-a-new-version-of-a-report}

Als u een exemplaar van een standaardrapport wilt tot stand brengen, doe het volgende:

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront.

1. Klik **Rapporten**, dan **Alle Rapporten**.
1. Klik op de naam van een standaardrapport om het te openen.
1. Klik **de Acties van het Rapport**, dan **uitgeven**.

   ![ geef rapport ](assets/nwe-reportactionsfordefaultreport-2022.png) uit

1. Breng om het even welke wijzigingen aan u in de volgende lusjes van het rapport moet aanbrengen:

   * **Kolommen (Mening)**: Voor meer informatie over het aanpassen van meningen, zie het artikel [ Overzicht van Meningen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **Groepen**: Voor meer informatie over het aanpassen van groeperingen, zie het artikel [ Overzicht van Groepen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **Filters**: Voor meer informatie over het aanpassen van filters, zie het overzicht van artikel [ Filters ](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **Grafiek**: Voor meer informatie over het aanpassen van een rapportgrafiek, zie het artikel [ een grafiek aan een rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md) toevoegen.

1. In de hoger-juiste hoek, klik **Montages van het Rapport**.
1. Op het **gebied van de Titel van het 0} Rapport, geef het rapport een nieuwe naam.**
1. Klik **Gedaan**.
1. Klik **sparen als Nieuw Rapport**.

   ![](assets/nwe-save-as-new-report-350x220.png)

1. (Facultatief) om de nieuwe versie van het rapport met andere gebruikers te delen, klik **Acties van het Rapport**, toen **het Delen**.
