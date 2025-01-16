---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Systeembrede taak- en probleemvoorkeuren configureren
description: U kunt systeembrede voorkeuren configureren voor taken en problemen. Deze voorkeuren zijn van invloed op de manier waarop gebruikers taken en problemen in Workfront maken.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: 0a65a18678bfc0aa2e080a0a983746040310b079
workflow-type: tm+mt
source-wordcount: '1884'
ht-degree: 0%

---

# Taak- en probleemvoorkeuren voor het hele systeem configureren

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


Als [!DNL Adobe Workfront] beheerder kunt u systeembrede voorkeuren configureren voor taken en problemen. Deze voorkeuren zijn van invloed op de manier waarop uw gebruikers taken en problemen maken in [!DNL Workfront] .

Standaard zijn taak- en probleemvoorkeuren vergrendeld en kunnen groepsbeheerders deze op groepsniveau niet wijzigen, tenzij u ze voor alle groepen in het systeem ontgrendelt. Voor meer informatie, zie de sectie [ taak van het Slot en geef voorkeur voor groepen ](#lock-task-and-issue-preferences-for-groups) in dit artikel uit.


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
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td><p>Nieuw: [!UICONTROL Standard]</p>
   of
   <p>Huidige: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

*For meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Taak- en probleemvoorkeuren configureren voor iedereen in [!DNL Workfront]

{{step-1-to-setup}}

1. In het linkerpaneel, klik **[!UICONTROL Project Preferences]** > **[!UICONTROL Tasks & Issues].**

1. Ga op de pagina die wordt weergegeven verder met een van de zes onderstaande secties om instellingen voor [!UICONTROL New Task Defaults] , [!UICONTROL Issues] , [!UICONTROL Deletion] , [!UICONTROL Actual Dates] en [!UICONTROL Access] te configureren:

   * [[!UICONTROL New Task Defaults]](#new-task-defaults)
   * [[!UICONTROL Issues]](#issues)
   * [[!UICONTROL Deletion]](#deletion)
   * [Verplaatsen](#move)
   * [[!UICONTROL Actual Dates]](#actual-dates)
   * [[!UICONTROL Delegation]](#delegation)
   * [[!UICONTROL Access]](#access)


### [!UICONTROL New Task Defaults] {#new-task-defaults}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Start Date]</td> 
    <td> <p>Bepaalt de standaardbegindatum voor nieuwe taken voor projectmanagers. De begindatum voor nieuwe taken kan ofwel de geplande startdatum van het project zijn, ofwel de dag waarop de taak wordt gemaakt.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader"> <p>[!UICONTROL Duration Type] </p> </td> 
    <td> <p>Bepaalt het verband tussen het aantal middelen (en hun toewijzingspercentage) en de duur of de totale inspanning voor de taak. Voor meer informatie, zie {de Duur van de Taak 0} en de Types van Duur </a><a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref"></p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Revenue Type]</td> 
    <td> <p>Berekent de geplande en werkelijke inkomstenramingen voor een taak. Wanneer <strong>[!UICONTROL Revenue Type]</strong> wordt geplaatst aan <strong>[!UICONTROL Not Billable]</strong>, produceren de geplande uren en de daadwerkelijke geregistreerde uren geen opbrengstraming voor de taak, en het werk aan de taak draagt niet aan project-vlakke opbrengst bij.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Cost Type]</td> 
    <td> <p>Berekent geplande en daadwerkelijke kostenramingen voor een taak. Wanneer deze waarde op <strong>[!UICONTROL No Cost]</strong> is ingesteld, genereren de geplande uren en de werkelijk geregistreerde uren geen geplande of feitelijke kostenraming voor de taak en dragen de werkzaamheden aan de taak niet bij aan de kosten op projectniveau.</p> </td> 
    </tr> 
  </tbody> 
</table>

### Problemen {#issues}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Automatically update Resolvable Issue status when the status of the Resolving Object changes]</td> 
    <td> <p>Wanneer iemand een kwestie in een project of een taak omzet, zowel worden de originele kwestie als het omgezette project of de taak het oplossen van voorwerpen. Met deze instelling kunt u de resolutie van het oorspronkelijke probleem correleren met de resolutie van het oplosbare object. Voor meer informatie over het oplossen van voorwerpen, zie <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref"> Overzicht van het Oplossen van en Oplosbare Voorwerpen </a>.</p> <p>Deze instelling heeft alleen effect als de optie <strong>[!UICONTROL Keep the original issue and tie its resolution to the task]</strong> is geselecteerd.</p> 
      <ul> 
      <li>Wanneer deze instelling is ingeschakeld, kunt u aangepaste statussen maken met dezelfde sleutel voor zowel uitgaven als projecten of taken. Wanneer het project of de taak (als oplosbaar voorwerp) in de douanestatus verandert, weerspiegelt de verandering ook de status van de kwestie. De statussleutel moet gelijk zijn voor de uitgave en project- of taakstatus.</li> 
      <li>Als deze instelling is uitgeschakeld, wordt de status van het oplossen van objecten automatisch ingesteld op de standaardstatus in plaats van op de status Aangepast. Voor meer informatie over de standaardstatussen, zie <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref"> Toegang tot de lijst van de statussen van de systeemkwestie </a>.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When converting an issue to a task]</td> 
    <td> <p>Met de instellingen in dit gedeelte wordt bepaald wat er gebeurt tijdens het conversieproces van uitgave tot taak:</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Keep the original issue and tie its resolution to the task]</strong>: Wanneer u de uitgave converteert, blijft deze zichtbaar als een uitgave totdat de taak is voltooid. De status van de uitgave verandert automatisch in [!UICONTROL Closed] wanneer de taak is voltooid. Als deze optie is uitgeschakeld, wordt de uitgave verwijderd.</p> <p><b> NOTA </b>:  <p>Gebruikers zonder toegang of machtigingen om problemen te verwijderen, kunnen de uitgave niet verwijderen omdat ze deze converteren, ongeacht de status van deze instelling. Voor informatie over toegang en toestemmingen tot kwesties, zie:</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref"> de toegang van de Verlening tot kwesties </a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref"> Een uitgave delen </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Allow Primary Contact to have access to the task]</strong>: Geeft de primaire contactpersoon (maker van de uitgave) toegang tot de taak om de taak te beoordelen, op de hoogte te blijven van de voortgang van de taak en opmerkingen te maken over de sectie Updates van de taak.</li> 
      <li> <p><strong>[!UICONTROL Allow these settings to be changed during conversion]</strong>: Hiermee kan de gebruiker die de uitgave converteert, deze opties wijzigen tijdens de conversie van een uitgave naar een taak.</p></li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When converting an issue to a project]</td> 
    <td> <p>Met de instellingen in deze sectie wordt bepaald wat er gebeurt tijdens het conversieproces van uitgave naar project:</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Keep the original issue and tie its resolution to the project]</strong>: Wanneer u de uitgave omzet, blijft het zichtbaar als een kwestie tot het project volledig is. De status van de uitgave verandert automatisch in [!UICONTROL Closed] wanneer het project is voltooid. Als deze optie is uitgeschakeld, wordt de uitgave verwijderd. </p> <p><b> NOTA </b>:  <p>Gebruikers zonder toegang of machtigingen om problemen te verwijderen, kunnen de uitgave niet verwijderen omdat ze deze converteren, ongeacht de status van deze instelling. Voor informatie over toegang en toestemmingen tot kwesties, zie:</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref"> de toegang van de Verlening tot kwesties </a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref"> Een uitgave delen </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Allow Primary Contact to have access to the project]</strong>: Geeft de primaire contactpersoon (maker van de uitgave) toegang tot het project om het project te beoordelen, op de hoogte te blijven van de voortgang van het project en opmerkingen te maken over de sectie Updates van het project.</li> 
      <li><strong>[!UICONTROL Allow these settings to be changed during conversion]</strong>: Hiermee kan de gebruiker die de uitgave converteert, de weergegeven opties wijzigen tijdens de conversie van een uitgave naar een project.</li> 
      </ul> </td>
    </tr> 
  </tbody> 
  </table>

### [!UICONTROL Deletion] {#deletion}

**[!UICONTROL Allow users to delete tasks and issues with logged hours]**: Hiermee kunt u bepalen of u het verwijderen van taken of problemen toestaat waarbij uren worden geregistreerd. Deze optie is standaard ingeschakeld.

>[!TIP]
>
>Deze instelling is ook van toepassing op het verwijderen van projecten die taken of problemen hebben met het aantal uren dat is aangemeld. Deze instelling is niet van toepassing op het verwijderen van projecten waarbij de tijd rechtstreeks voor het project wordt vastgelegd.

* Als deze optie is geselecteerd, ontvangt u een informatieve waarschuwing wanneer u een taak of uitgave verwijdert. De waarschuwing herinnert u eraan dat als de taak of de kwestie uren het programma heeft geopend, zij of naar het project zullen worden verplaatst of worden geschrapt. U kunt configureren of de uren worden verwijderd of naar het project worden verplaatst in het [!UICONTROL Timesheet & Hours Preferences] -gebied van [!UICONTROL Setup] . Nadat u hebt bevestigd dat u de waarschuwing hebt gezien, wordt de taak of het probleem verwijderd. Voor meer informatie over het vormen van de Voorkeur van Timesheet &amp; van Uren, zie [ timesheet en uurvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.

  >[!TIP]
  >
  >Wanneer u een project verwijdert met taken en problemen die het programma &#39;uren&#39; hebben geopend, worden de geregistreerde uren verwijderd of behouden volgens de instellingen in het [!UICONTROL Timesheet & Hours Preferences] -gebied van [!UICONTROL Setup] . Het waarschuwingsbericht wordt niet weergegeven wanneer u een project verwijdert.

* Wanneer u deze optie deselecteert, ontvangt u een prohibitieve waarschuwing wanneer u een taak of een kwestie met geregistreerde uren schrapt, of wanneer u een project met uren schrapt die voor zijn taken of kwesties worden geregistreerd. De waarschuwing geeft aan dat de beheerder het niet toestaat dat taken of problemen met geregistreerde uren worden verwijderd. De taken, de kwesties, of de projecten die uren hebben voor taken en kwesties worden geregistreerd kunnen niet worden geschrapt.

### Verplaatsen

**[!UICONTROL Allow users to move tasks and issues with logged hours]**: Hiermee kunt u bepalen of u het verplaatsen van taken of problemen toestaat waar uren worden vastgelegd. Deze optie is standaard ingeschakeld.

* Als deze optie is geselecteerd, kunt u taken en problemen met tijd verplaatsen. De uren bewegen zich ook met de taken of de kwesties.

* Wanneer u deze optie uitschakelt, ontvangt u een onophoudelijke waarschuwing wanneer u een taak of uitgave met geregistreerde uren naar een ander project verplaatst. De waarschuwing geeft aan dat de beheerder het verplaatsen van taken of problemen met geregistreerde uren niet toestaat. De taken of kwesties die uren het programma worden geopend kunnen niet worden verplaatst. U kunt taken binnen hetzelfde project verplaatsen, zelfs als deze optie is uitgeschakeld.

### [!UICONTROL Actual Dates] {#actual-dates}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL When a task or issue goes from "New" to "In Progress," set the Actual Start Date to]</td> 
    <td> <p>Selecteer een van de volgende opties wanneer de werkelijke begindatum wordt opgenomen in [!DNL Workfront] wanneer een taak of uitgave van <strong>[!UICONTROL New]</strong> naar <strong>[!UICONTROL In Progress]</strong> gaat:</p> 
      <ul> 
      <li><strong>[!UICONTROL Now]:</strong> De werkelijke begindatum wordt ingesteld op de huidige datum.</li> 
      <li><strong>[!UICONTROL The Planned Start Date]:</strong> De werkelijke begindatum wordt ingesteld op de geplande begindatum van de taak of uitgave.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When a task or issue is completed, set the Actual Completion Date to]</td> 
    <td> <p>Selecteer een van de volgende opties als de werkelijke afwerkingsdatum wordt opgenomen in [!DNL Workfront] wanneer een taak of uitgave is voltooid:</p> 
      <ul> 
      <li><strong>[!UICONTROL Now]:</strong> De datum van feitelijke voltooiing wordt geplaatst aan de huidige datum.</li> 
      <li> <p><strong>[!UICONTROL The Planned Completion Date]: </strong> De datum van daadwerkelijke voltooiing wordt geplaatst aan de Geplande Datum van Voltooiing van de taak of de kwestie.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

### Delegatie

Als u de instelling **[!UICONTROL Allow users to delegate their tasks and issues]** inschakelt, kunnen alle gebruikers in het systeem hun werk tijdelijk delegeren aan anderen.

Wanneer deze instelling is ingeschakeld, kunnen gebruikers het volgende zien:

* De [!UICONTROL **Afgevaardigde**] verbinding in hun [!UICONTROL My Work], [!UICONTROL My Tasks], of [!UICONTROL My Issues] widgets in het [!UICONTROL Home] gebied. Zij kunnen taak delegeren en taken van daar uitgeven.

  >[!NOTE]
  >
  >  De [!UICONTROL **toestemmingen van de Afgevaardigde**] verbinding wordt altijd toegelaten in het [!UICONTROL Home] gebied.

* Een indicatie dat een taak of kwestie aan een andere gebruiker in het [!UICONTROL Assignments and delegations] gebied in de taak of uitgiftekopbal wordt gedelegeerd.
* Een indicatie dat een taak of kwestie aan een andere gebruiker in hun [!UICONTROL My Work] widget in [!UICONTROL Home] wordt gedelegeerd.

  Als u de instelling [!UICONTROL Allow users to delegate their tasks and issues] uitschakelt, worden de delegaties die momenteel zijn gepland, gestopt en ontvangen de gedelegeerde gebruikers een e-mail met de melding dat de delegatie is gestopt.

Raadpleeg de volgende artikelen voor informatie over het delegeren van werk aan anderen:

* [Overzicht van werkzaamheden delegeren](../../../manage-work/delegate-work/delegate-work-overview.md)
* [Taken en problemen delegeren](../../../manage-work/delegate-work/how-to-delegate-work.md)


<!--
<p><strong>Work On It</strong></p>
This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it.</p>
Here's what Jeremy Flores says on 12/1/20:</p>
I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.</p>
<p>You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.</p>
<p>Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.</p>
<p>To switch to the Start button:</p>
<ol>
<li value="1"> <p>Select <strong>Change the Work On It button to a Start button to automatically update the status of an item</strong>.</p> </li>
<li value="2"> <p>In the lists of check boxes that display below this option, select one or more statuses for each work item type.</p> <p>With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item.</p> </li>
</ol> <note type="note">
<ul class="preview">
<li>Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.</li>
<li>If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.</li>
<li>This setting is not currently available in
<ul>
<li>The Workfront Mobile App</li>
<li>Workfront for Office 365</li>
<li>Workfront email notifications</li>
</ul></li>
<li>This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.</li>
<li>If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.</li>
</ul>
</note>
-->

### [!UICONTROL Access] {#access}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL When someone is assigned to a task]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Give them ... access to a task]</strong>: Definieert de standaardmachtigingen die een gebruiker heeft voor de taak waaraan hij of zij is toegewezen. Voor meer informatie over taaktoestemmingen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Toegang van de Verlening tot gebruikers </a>.</li> 
      <li> <p><strong>[!UICONTROL Also grant them ... access to the project]</strong>: Bepaalt de standaardtoestemming een gebruiker aan het project heeft waarop zij een taak hebben die aan hen wordt toegewezen. Voor meer informatie over projecttoestemmingen, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref"> systeem-brede projectvoorkeur </a> vormen.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When someone is assigned to an issue]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Give them ... access to a task]</strong>: Definieert de standaardmachtigingen die een gebruiker heeft voor de taak waaraan hij of zij is toegewezen. Voor meer informatie over taaktoestemmingen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Toegang van de Verlening tot gebruikers </a>.</li> 
      <li> <p><strong>[!UICONTROL Also grant them ... access to the project]</strong>: Bepaalt de standaardtoestemming een gebruiker aan het project heeft waarop zij een taak hebben die aan hen wordt toegewezen. Voor meer informatie over projecttoestemmingen, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref"> systeem-brede projectvoorkeur </a> vormen.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When someone submits a request]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Give them ... access to the issue]</strong>: Definieert de standaardmachtigingen die een gebruiker heeft op een verzoek dat hij of zij heeft ingediend. Voor meer informatie, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref"> een kwestie delen </a>.</li> 
      <li> <p><strong>[!UICONTROL People from the same company will inherit the same permissions for all requests]</strong>: Staat gebruikers toe verzoeken te zien die door andere gebruikers van het zelfde bedrijf worden voorgelegd zoals zij. Zij hebben de zelfde toestemmingen op die verzoeken zoals zij op hun hebben voorgelegd.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

1. Klik op **[!UICONTROL Save]**.

## Taak- en uitgavevoorkeuren voor groepen vergrendelen {#lock-task-and-issue-preferences-for-groups}

Als de groepen in uw organisatie een taak of uitgiftevoorkeur nodig hebben die verschillend voor hun unieke werkschema&#39;s wordt gevormd, kunt u de voorkeur voor alle groepen door de organisatie ontgrendelen zodat zij het op hun kunnen vormen. Wanneer een voorkeur wordt ontgrendeld en de groepsbeheerder het wijzigt, worden de taken of kwesties verbonden aan de groep beïnvloed door groep-niveau die voor de voorkeur plaatst in plaats van systeem-niveau het plaatsen.

Voor informatie over hoe een groepsbeheerder taak vormt en uit:geven voorkeur voor een groep, zie [ taak en uitgiftevoorkeur voor een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) vormen.

>[!NOTE]
>
>Nadat een [!DNL Workfront] beheerder een voorkeur op het systeemniveau ontgrendelt, kan om het even welke groepbeheerder het vormen en dan het sluiten om ervoor te zorgen dat iedereen in hun groep en subgroups hieronder de zelfde configuratie gebruikt. Dit is parallel aan de mogelijkheid dat een [!DNL Workfront] -beheerder een voorkeur voor iedereen in het systeem moet configureren en vergrendelen. Voor meer informatie, zie [ projectvoorkeur voor een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) en [ Slot of ontgrendel een project, een taak, of een uitgiftevoorkeur voor subgroups ](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md) vormen.

Een taak of een uitgiftevoorkeur vergrendelen of ontgrendelen zodat groepen deze kunnen configureren:

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Project Preferences]** > **[!UICONTROL Tasks & Issues]** .

1. Voer een van de volgende handelingen uit:

   * Als u wilt dat beheerders van groepen onder uw groep een voorkeur voor hun groepen kunnen vormen, ontgrendel het ![](assets/unlock-toggle-button.png).
   * Als u wilt dat de groep en alle onderliggende groepen uw configuratie voor een voorkeur gebruiken, moet u controleren of deze is vergrendeld (dit is de standaardinstelling).

     >[!IMPORTANT]
     >
     >Wij adviseren dat u met de beheerders en de gebruikers in groepen door het systeem communiceert om ervoor te zorgen dat alle behoeften rekenschap worden gegeven op de manier u een gesloten voorkeur vormt. Wanneer u het sluit, wordt uw configuratie voor het geërft door alle groepen in het systeem. En als de voorkeur voor om het even welke periode is ontgrendeld, vervangt uw configuratie die die groepsbeheerders zouden kunnen hebben gemaakt.

1. Klik op **[!UICONTROL Save]**.
