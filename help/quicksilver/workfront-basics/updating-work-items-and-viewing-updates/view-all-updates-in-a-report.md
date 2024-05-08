---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Alle updates in een notitierapport weergeven
description: Alle updates in een notitierapport weergeven
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 36bdacb5f6d04245552aeeb4ab82d210597645a2
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Alle updates in een notitierapport weergeven

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

In het gedeelte Updates van een object wordt standaard maximaal 200 updates weergegeven. Als u alle updates wilt zien die een van de gebruikers voor een object heeft ingevoerd, kunt u een notitierapport maken waarin alle updates worden weergegeven.

>[!NOTE]
>
>U kunt een rapport bouwen om updates op voorwerpen in Voorproef met het de ingangsrapport van het Dagboek te bekijken. Zie voor meer informatie [Rapport over het gebied Updates](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td> <p>Nieuw: Standaard </p>
   <p>Huidig: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau</strong></td> 
   <td> <p>Toegang bewerken tot:</p> 
    <ul> 
     <li> <p>Rapporten, dashboards en kalenders maken</p> </li> 
     <li> <p>Filters, weergaven en groepen maken</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Weergave</p> <p><b>OPMERKING</b></p>
   <p>Als u geen toestemming van de Mening of hoger aan een voorwerp hebt, toont de informatie voor dat voorwerp niet in het rapport.</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Zie voor meer informatie [Toegangsvereisten in Adobe Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Een notitierapport maken

Het maken van een rapport voor Notities voor elk object is identiek, ongeacht het object.

Bijvoorbeeld, om een rapport van de Nota voor alle nota&#39;s op een project tot stand te brengen:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) rechtsboven in Adobe Workfront.

1. Klikken **Rapporten**.
1. Klikken **Nieuw rapport** en kiest u **Opmerking**.

1. (Optioneel) Klik op **Weergaven** vervolgens **Kolom toevoegen** om de **Naam** van de **Project** volgens het verslag . 

1. (Optioneel) Klik op **Groepen** vervolgens **Groepering toevoegen** om te groeperen door **Projectnaam** als u meerdere projecten tegelijk rapporteert.\
   Dit zorgt ervoor dat de nota&#39;s door hun respectieve projecten worden gegroepeerd, die het rapport gemakkelijker maken te lezen. 

1. (Optioneel) Klik op **Filters,** dan **Filterregel toevoegen**.
1. Een filter toevoegen voor **Opmerking** > **Notititie** > **Is niet leeg**.

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Als een projectveld is bijgewerkt maar er geen notitie is toegevoegd op het moment van de update, wordt het **Notititie** van de update wordt weergegeven als **(Geen tekst toegevoegd om bij te werken)**.


1. (Optioneel) Voeg een ander filter toe voor **Project** > **Naam** > **Gelijk aan** en voeg een of meer projectnamen toe waarvoor u notities wilt weergeven.
1. Klikken **Opslaan + Sluiten**.\
   Alle updates ingegaan op het project door alle gebruikers met toestemmingen om het project minstens te bekijken worden getoond in het rapport.
