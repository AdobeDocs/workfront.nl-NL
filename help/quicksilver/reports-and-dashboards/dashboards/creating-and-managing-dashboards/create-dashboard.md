---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Een dashboard maken
description: U kunt dashboards tot stand brengen om tot informatie in Adobe Workfront snel toegang te hebben. Rapporten, kalenders en externe pagina's kunnen worden toegevoegd aan dashboards die u met anderen kunt delen voor een optimale samenwerking.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 39a8d670baa19aa37e29b0312e6c9a296569f44c
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 0%

---

# Een dashboard maken

<!--Audited: 01/2025-->

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Het is beschikbaar slechts in het milieu van de Voorproef voor alle klanten.</span>


U kunt dashboards tot stand brengen om tot informatie in Adobe Workfront snel toegang te hebben. U kunt maximaal 25 rapporten, kalenders en externe pagina&#39;s toevoegen aan dashboards die u met anderen kunt delen voor optimale samenwerking.

Meer over dashboards leren, zie [&#x200B; begonnen met dashboards &#x200B;](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

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
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards en kalenders bewerken</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>U krijgt beheermachtigingen voor de dashboards die u maakt</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

U moet de volgende objecten maken voordat u deze aan een dashboard kunt toevoegen:

* **Rapporten**: Voor informatie bij het creëren van rapporten, zie [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

* **Kalenders**: Voor informatie bij het creëren van kalenders, zie [&#x200B; overzicht van de rapporten van de Kalender &#x200B;](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

U kunt bestaande externe pagina&#39;s toevoegen aan een dashboard of u kunt een pagina maken van het nieuwe dashboard. Voor informatie bij het creëren van externe pagina&#39;s, zie [&#x200B; een externe Web-pagina in een dashboard &#x200B;](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md) inbedden.

## Een dashboard maken

{{step1-to-dashboards}}

1. Klik **Nieuw Dashboard**.\
   Het dialoogvenster Nieuw dashboard wordt weergegeven.

1. Geef het volgende op:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Naam</strong></td>
      <td><p>Dit is de naam van het dashboard. We raden u aan alleen UTF-8-tekens te gebruiken om compatibiliteitsproblemen te voorkomen.</p><p>Als u geen naam opgeeft, wordt de naam van het eerste rapport op het dashboard standaard de naam van het dashboard.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Beschrijving (optioneel)</strong></td>
      <td>Dit is een beschrijving van het dashboard.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>Valuta</strong></td>
      <td><span class="preview">Dit is het standaardvalutatype voor het dashboard. <br>
      <br> de Gebruikers kunnen tussen verschillende munttypes schakelen wanneer het filtreren van het dashboard. Voor meer informatie, zie <a href="/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/filter-canvas-dashboard.md"> een dashboard door munttype </a> filtreren.</span></td>
     </tr>
    </tbody>
   </table>

1. Selecteer een lay-out door het radioknoop te klikken die aan het bij de bovenkant van **Uitgezochte Lay-out/voegt Rapporten/toevoegt Calendars** sectie beantwoordt. Dit is de lay-out waarin de rapporten, kalenders, of externe pagina&#39;s op het dashboard zullen tonen.

   De lay-out met één kolom is de standaardinstelling.

   Voor informatie over rapportlay-out op dashboards, zie [&#x200B; begrijpen hoe de rapporten op een dashboard &#x200B;](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md) tonen.

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. In de **Beschikbare Rapporten &amp; Calendars** sectie, begin de naam van een rapport, een kalender, of een externe pagina in de onderzoeksbar te typen, dan belemmering en laat vallen het rapport, de kalender, of de externe pagina in de lay-outruit aan het recht.

   >[!NOTE]
   >
   >Wanneer het zoeken naar een punt, keert het onderzoek om het even welke 2000 onlangs gecreeerd rapporten terug. Rapportnamen met Unicode-tekens worden niet geretourneerd in zoekresultaten. U kunt het beste Unicode-tekens niet opnemen bij het benoemen van objecten in Workfront door namen te typen in plaats van namen van een andere bron te kopiëren en te plakken.

   ![&#x200B; Onderzoek naar rapporten &#x200B;](assets/unshimmed-dashboard-ui.png)

1. (Optioneel) Klik op **Externe pagina toevoegen** om een nieuwe externe pagina aan het dashboard toe te voegen.

   Voor meer informatie over het creëren van externe pagina&#39;s en het inbedden van hen in dashboards, zie [&#x200B; een externe Web-pagina in een dashboard &#x200B;](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md) inbedden.

1. Klik **sparen + Sluiten**.

   Een tijdstempel wordt in de rechterbovenhoek van het dashboard weergegeven. De tijdstempel bevat de datum, tijd en tijdzone waarop het dashboard voor het laatst is vernieuwd.
