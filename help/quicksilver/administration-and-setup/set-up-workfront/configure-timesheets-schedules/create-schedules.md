---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Een schema maken
description: U kunt de werkweken van uw gebruikers bepalen met programma's. U kunt een programma met een gebruiker of een project associëren. Dit staat  [!DNL Workfront]  toe om chronologie en gebruikersbeschikbaarheid te berekenen.
author: Lisa, Alina
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# Een schema maken

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

Als [!DNL Adobe Workfront] beheerder, kunt u uw werkweek met programma&#39;s bepalen. U kunt een programma met een gebruiker of een project associëren. Hierdoor kunnen in [!DNL Workfront] tijdlijnen en de beschikbaarheid van de gebruiker worden berekend.

Wanneer u gebruikers hebt die in verschillende tijdzones werken, zorgt het creëren van een programma in elk van de tijdzones en het associëren van het met die gebruikers ervoor dat hun werk in [!DNL Workfront] in echt - tijd wordt geregistreerd en dat hun beschikbaarheid altijd nauwkeurig volgens is wanneer zij werken.

Voor informatie over het associëren van programma&#39;s met gebruikers en projecten, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven en [ projecten ](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

De beheerders van de groep kunnen ook programma&#39;s tot stand brengen die met de groepen worden geassocieerd zij leiden. Voor meer informatie, zie [ creeer en wijzig de programma&#39;s van een groep ](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

Voor informatie over het gebruiken van programma&#39;s om gebruikers te helpen in [!DNL Workfront] over tijdstreken samenwerken, zie [ Werkend over tijdstreken ](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

Voor informatie over hoe de programma&#39;s in middel planning worden gebruikt, zie [ Overzicht van Programma&#39;s ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md) en [ overzicht van de Planner van het Middel ](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td><p>Nieuw: [!UICONTROL Standard]</p>
       <p>of</p>
       <p>Huidige: [!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td>  
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een schema maken

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Schedules]**.
1. Klik op **[!UICONTROL New Schedule]**.
1. Voer een naam in voor het schema.
1. (Optioneel) Selecteer **[!UICONTROL Default Schedule]** om dit schema aan te duiden als uw standaard.

   U moet minstens één schema in [!DNL Workfront] hebben. Als u slechts één hebt, wordt het aangewezen als standaardprogramma.

   U kunt meer dan één programma hebben, maar u kunt slechts één standaardprogramma hebben.

   >[!NOTE]
   >
   >U kunt geen programma als standaardprogramma aanwijzen als u een groepsbeheerder bent. Alleen een [!DNL Workfront] -beheerder kan een schema aanwijzen als standaard voor het systeem.

   ![ Nieuw programma ](assets/new-schedule.png)

1. Selecteer op het tabblad **[!UICONTROL Schedule]** een dagelijks schema door de blauwe omtrek over uurblokken te slepen om deze te markeren.

   We raden u aan 8 blokken van een uur te selecteren over een periode van 9 uur. Dit is geschikt voor lunch of andere onderbrekingen.

   ![ blokken van de Tijd op een programma ](assets/new-schedule-with-exceptions.png)

1. Voer op het tabblad **[!UICONTROL Details]** de volgende informatie in:

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL Group with Administration Access]</td>
     <td><p>Selecteer de groep waarvan de beheerders machtigingen hebben om dit schema te bewerken.</p>
     <p><b> BELANGRIJK </b>:</p>
      <ul>
       <li>
       <p>Als u een groepsbeheerder bent die een programma creeert, is dit gebied verplicht.</p>
       <p>Als groepsbeheerder, kunt u een programma tot stand brengen slechts als het voor een groep of subgroep wordt aangewezen waarvoor u als beheerder wordt aangewezen.</p>
       <p>Als u slechts één groep beheert, wordt die groep standaard in dit veld geselecteerd.</p>
       <p>Als u meerdere groepen beheert, moet u een groep in dit veld selecteren voordat u het schema kunt opslaan.</p></li>
       <li>Als u een [!DNL Workfront] -beheerder bent die een schema maakt, is dit veld optioneel. Wanneer u een programma creeert zonder het met een groep te associëren, wordt het bewaard als systeem-vlakke programma en kan niet door een groepsbeheerder van om het even welke groep worden beheerd.
       <p>De programma's die aan rekeningen of projecten worden toegewezen zijn zichtbaar aan alle gebruikers die deze voorwerpen kunnen uitgeven. Dit geldt voor zowel systeem-niveau als groep-vlakke programma's.</p>
       </li>
       <p>Het specificeren van een Groep met de Toegang van het Beleid voor een programma wijst niet het programma aan de gebruikers in de groep toe; het staat slechts de groepsbeheerders in de groep toe om, het programma uit te geven te schrappen en te kopiëren.</p>
       <p>De Beheerders van de groep kunnen geen systeem-vlakke programma's uitgeven, schrappen of kopiëren. Voor meer informatie, zie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref"> de beheerders van de Groep </a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Groups with View Access]</td>
     <td><p>Selecteer de groepen met [!UICONTROL View] toegang die dit schema kunnen zien.</p>
     <p>Alleen de gebruikers in de groepen die u hier opgeeft, kunnen het schema in het keuzemenu vinden wanneer zij het aan gebruikers of projecten toewijzen.</p></tr>
    <tr>
     <td>[!UICONTROL Time Zone]</td>
     <td><p>Selecteer de tijdzone voor het programma.</p>
     <p>Als u het programma met een gebruiker associeert, adviseren wij dat de tijdzone van het programma dat van de gebruiker aanpast. Voor informatie over de tijdstreken van de gebruiker, zie <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref"> het profiel van een gebruiker uitgeven.
     </td>
    </tr>
   </table>


1. Geef op het tabblad **[!UICONTROL Exceptions]** eventuele uitzonderingen op het schema op.

   Uitzonderingen zijn volledige of halve dagen die van de planning moeten worden uitgesloten, zoals feestdagen of bedrijfsgebeurtenissen.

   >[!NOTE]
   >
   >Als u reeds weet wat uw terugkomende programmauitzonderingen zijn, kunt u uw planningsuitzonderingen voor vele jaren in de toekomst bepalen.

   Volledige of gedeeltelijke dagen kunnen van het werkschema worden uitgesloten. Klik op de datum om deze als uitzondering te selecteren en selecteer vervolgens het veld **[!UICONTROL All day]** om aan te geven of de uitzondering een volledige dag is of niet.

   ![ Alle daguitzondering ](assets/schedule-adding-an-all-day-exception.png)

1. Ga de begin en eindtijd voor de gedeeltelijke daguitzonderingen in.

   ![ Gedeeltelijke daguitzondering ](assets/partial-day-exception-on-schedules.png)

1. Klik **[!UICONTROL Save]**, dan klik **[!UICONTROL Save]Veranderingen**.

1. (Optioneel) Koppel het schema aan een gebruiker.

   Voor informatie, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

1. (Optioneel) Koppel het programma aan een project.

   Voor informatie, zie [ projecten ](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.
