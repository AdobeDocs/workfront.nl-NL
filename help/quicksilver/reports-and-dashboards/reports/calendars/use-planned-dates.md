---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Geplande datums gebruiken in een kalenderrapport
description: Een kalenderrapport is een dynamisch rapport dat een visuele vertegenwoordiging van uw werk verstrekt. U kunt de Geplande gebieden van de Datum in een kalenderrapport voor taken, kwesties, en projecten gebruiken.
author: Lisa
feature: Reports and Dashboards
exl-id: 27bf6f03-2f6b-4556-a715-75c4a21bfbbb
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# [!UICONTROL Planned Dates] gebruiken in een kalenderrapport

Een kalenderrapport is een dynamisch rapport dat een visuele vertegenwoordiging van uw werk verstrekt. U kunt [!UICONTROL Planned Date] -velden in een kalenderrapport gebruiken voor de volgende objecten:

* Taken
* Problemen
* Projecten

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>[!UICONTROL Edit] toegang tot [!UICONTROL Reports] , [!UICONTROL Dashboards] en [!UICONTROL Calendars]</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de [!DNL Workfront] -beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>[!UICONTROL Manage] toegang tot het kalenderverslag</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## De groep items instellen

U kunt kiezen hoe de groep items moet worden weergegeven in uw kalender.

1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in [!DNL Adobe Workfront] en klik vervolgens op **[!UICONTROL Calendars]** .

1. Selecteer de kalender waaraan u een nieuwe groep items wilt toevoegen.\
   of\
   Klik op **[!UICONTROL + New Calendar]** en voer de naam van de kalender in.

   >[!NOTE]
   >
   >U moet Edit toegang tot Rapporten, Dashboards, en Kalenders in uw toegangsniveau hebben om een kalenderrapport tot stand te brengen.

1. Klik links in het scherm op **[!UICONTROL Add to Calendar]** en klik vervolgens op **[!UICONTROL Add advanced items]** .

1. Geef het volgende op:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Name this group of items]</strong></td>
      <td>Typ een naam voor de groep items.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Color]</strong></td>
      <td>Selecteer een kleur voor de groep items. Alle items worden in de geselecteerde kleur in het kalenderrapport weergegeven.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Date Field]</strong></td>
      <td><p>Kies <strong>[!UICONTROL Planned dates]</strong> . Voor meer informatie over geplande data raadpleegt u </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">Overzicht van de geplande begindatum van het project</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Overzicht van de geplande startdatum van de taak</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Overzicht van de geplande voltooiing van de taak</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Geplande afsluitdatum van project instellen</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Kies in de kalender de optie</strong></td>
      <td><p>Kies hoe u de datums wilt weergeven:</p>
       <ul>
        <li><strong>[!UICONTROL Start Date Only]</strong>: In de kalender wordt het object op één datum weergegeven.</li>
        <li><strong>[!UICONTROL End Date Only]</strong>: In de kalender wordt het object op één datum weergegeven.</li>
        <li><strong>[!UICONTROL Duration] (Begin aan Eind) </strong>: De kalender toont het voorwerp over een spanwijdte van dagen.</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL Switch to actual dates when available]</strong></td>
      <td><p>De kalender schakelt automatisch over naar de werkelijke datums wanneer deze beschikbaar zijn. <br> Kies <strong>[!UICONTROL Yes]</strong> of <strong>[!UICONTROL No]</strong> om over te schakelen op werkelijke datums, indien beschikbaar. Zie voor meer informatie over de werkelijke datums</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">Overzicht van het project Werkelijke Begindatum </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Overzicht van het project Werkelijke uitvoeringsdatum </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. Ga verder naar de volgende sectie.

## Objecten toevoegen aan de groep items

Nadat u hebt ingesteld hoe de items moeten worden weergegeven, moet u de objecten die u in de kalender wilt zien, aan de groep toevoegen.

1. Selecteer in de sectie **[!UICONTROL What would you like to add to the calendar?]** de optie

   * **[!UICONTROL Tasks]**
   * **[!UICONTROL Projects]**
   * **[!UICONTROL Issues]**

1. Klik op **[!UICONTROL Add Tasks]** , **[!UICONTROL Add Projects]** of **[!UICONTROL Add Issues]** , afhankelijk van het objecttype dat u aan de kalender toevoegt.\
   ![ Uitgezochte voorwerp voor kalender ](assets/field-name.png)

1. Typ in het keuzemenu eerst de veldnaam en selecteer vervolgens de veldbron van het object dat u in de kalender wilt weergeven (bijvoorbeeld **[!UICONTROL Late Tasks]** ).
1. Stel een voorwaardelijke instructie in voor de kalendergroep.

   ![ verklaring van de Voorwaarde ](assets/condition-statement-calendar.png)

   Om over het plaatsen van voorwaarden te leren, zie [ Filter en voorwaardenbepalingen ](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Optioneel) Geef aanvullende objecten voor de kalendergroep op door stap 1-4 te herhalen.
1. Selecteer in het veld **[!UICONTROL Set the Tasks/Projects/Issues labels to be the...]** hoe de objecten in deze kalendergroep worden gelabeld in de kalender.

   >[!NOTE]
   >
   >Als de standaardlabelopties niet beschikbaar zijn voor een bepaald object, wordt in plaats daarvan de naam van het object weergegeven. Wanneer u bijvoorbeeld het label [!UICONTROL Parent Task] hebt geselecteerd en er geen bovenliggende taak aan het object is gekoppeld, geeft [!DNL Adobe Workfront] de objectnaam weer die u in de kalender weergeeft.

1. Klik op **[!UICONTROL Save]**.
