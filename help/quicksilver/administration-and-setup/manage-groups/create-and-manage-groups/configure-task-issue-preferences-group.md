---
title: Taak- en uitgavevoorkeuren voor een groep configureren
user-type: administrator
product-area: system-administration;user-management;setup
keywords: groep,voorkeuren,taak,uitgave,ontgrendelen
navigation-topic: create-and-manage-groups
description: Als de groepen in uw organisatie een taak of een uitgiftevoorkeur onafhankelijk van de manier moeten vormen het op het systeemniveau wordt gevormd, kan een beheerder van Adobe Workfront de voorkeur ontgrendelen. Dan, als groepsbeheerder, kunt u de voorkeur voor uw groep vormen en het zal alle taken of kwesties beïnvloeden verbonden aan uw groep.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '1894'
ht-degree: 0%

---

# Taak- en uitgavevoorkeuren voor een groep configureren

Als de groepen in uw organisatie een taak of een uitgiftevoorkeur onafhankelijk van de manier moeten vormen het op het systeemniveau wordt gevormd, kan een beheerder van Adobe Workfront de voorkeur ontgrendelen. Dan, als groepsbeheerder, kunt u de voorkeur voor uw groep vormen en het zal alle taken of kwesties beïnvloeden verbonden aan uw groep.

Als er groepen zijn boven de groep die u beheert, kunnen hun beheerders dit ook voor uw groep doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

Voor informatie over hoe de Workfront-beheerder voorkeuren ontgrendelt, raadpleegt u [Projectvoorkeuren voor alle groepen in het systeem vergrendelen of ontgrendelen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>Configuratie op groepsniveau is ook mogelijk voor projectvoorkeuren. Zie voor meer informatie [Projectvoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* Een niet-vergrendelde voorkeur blijft meestal voor onbepaalde tijd ontgrendeld. Als de beheerder van Workfront het opnieuw sluit, wordt het systeem opnieuw plaatsend dat en de montages voor de voorkeur door de groepsbeheerders wordt gemaakt worden verloren.
>* De voorkeuren die zijn ingesteld voor de groep die is gekoppeld aan een project, hebben voorrang op de voorkeuren die zijn ingesteld voor de thuisgroep van de gebruiker die het project maakt.
>* Sommige voorkeuren op groepsniveau zijn van invloed op projectsjablonen die u voor de groep maakt. Zie de sectie voor meer informatie [De mening, het werk met, en creeert malplaatjes voor uw groep van het gebied van Groepen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) in het artikel [De projectsjablonen van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Nadat een beheerder van Workfront een voorkeur op het systeemniveau ontgrendelt, kunt u het vormen en dan het sluiten om ervoor te zorgen dat iedereen in uw groep en in zijn subgroepen de zelfde configuratie gebruikt. Dit is parallel aan de mogelijkheid dat een Workfront-beheerder een voorkeur voor iedereen in het systeem moet configureren en vergrendelen. Zie voor meer informatie [Een project, taak of uitgiftevoorkeur voor subgroepen vergrendelen of ontgrendelen](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-abonnement*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> <p>U moet een groepsbeheerder van de groep of een beheerder van Workfront zijn. Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Groepbeheerders</a> en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de Workfront-beheerder als u wilt weten welk abonnement- of licentietype u hebt.

## De ontgrendelde taak- en probleemvoorkeuren voor een groep op hoofdniveau configureren

>[!TIP]
>
>Als u een Workfront-beheerder bent, kunt u de stappen 1 tot en met 4 omzeilen door naar Instellingen > Projectvoorkeuren > Taken en problemen te gaan en vervolgens in het vak boven aan de pagina naar de naam van de groep te zoeken.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Groepen** ![](assets/groups-icon.png).

1. Klik op de naam van de groep waarvoor u de ontgrendelde taak en voorkeuren voor uitgaven wilt configureren.
1. Klik in het linkerdeelvenster op de pagina die voor de groep wordt weergegeven **Voorkeuren voor taken en problemen**.
1. Ga op de pagina die wordt weergegeven verder met een van de vijf onderstaande secties om instellingen voor de gebieden Nieuwe taakstandaardinstellingen, Problemen, Verwijderen, Werkelijke datums en Toegang te configureren. Klik vervolgens op **Opslaan**.

   Als u de muisaanwijzer boven het vergrendelingspictogram houdt ![](assets/lock-toggle-button-dimmed.png) voor een voorkeur die u moet vormen en de vertoningen van hulpmiddeluiteinde om u te vertellen dat gesloten is, kunt u uw beheerder van Workfront vragen om het voor alle groepen in de organisatie te ontgrendelen.

   Wanneer deze ontgrendeld is, kunnen u en andere groepsbeheerders deze afzonderlijk configureren voor uw eigen groepen. U kunt deze ook vergrendelen voor uw groep en voor alle subgroepen onder uw groep.

   * [Nieuwe taakstandaardinstellingen](#new-task-defaults)
   * [Problemen](#issues)
   * [Verwijderen](#deletion)
   * [Werkelijke datums](#actual-dates)

      <!--   
     <li><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>   
     -->

   * [Toegang](#access)

### Nieuwe taakstandaardinstellingen {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Begindatum voor nieuwe taken</td> 
      <td> <p>Bepaalt de standaardbegindatum voor nieuwe taken voor projectmanagers. De begindatum voor nieuwe taken kan ofwel de geplande startdatum van het project zijn, ofwel de dag waarop de taak wordt gemaakt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Duur </p> </td> 
      <td> <p>Bepaalt het verband tussen het aantal middelen (en hun toewijzingspercentage) en de duur of de totale inspanning voor de taak. Zie voor meer informatie <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">De Duur van de taak en de Types van Duur</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type inkomsten</td> 
      <td> <p>Berekent de geplande en werkelijke inkomstenramingen voor een taak. Wanneer de <strong>Type inkomsten</strong> is ingesteld op<strong>Niet opteerbaar</strong>de geplande uren en de werkelijk geregistreerde uren geen inkomstenraming voor de taak opleveren, en de werkzaamheden aan de taak dragen niet bij tot de ontvangsten op projectniveau.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kostensoort</td> 
      <td> <p>Berekent geplande en daadwerkelijke kostenramingen voor een taak. Wanneer ingesteld op <strong>Geen kosten</strong>de geplande uren en de werkelijk geregistreerde uren geen geplande of werkelijke kostenraming voor de taak opleveren en de werkzaamheden voor de taak dragen niet bij tot de kosten op projectniveau.</p> </td> 
     </tr> 
    </tbody> 
   </table>

### Problemen {#issues}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">De status van het opgeloste probleem automatisch bijwerken wanneer de status van het gevonden object verandert</td> 
      <td> <p>Wanneer iemand een kwestie in een project of een taak omzet, zowel worden de originele kwestie als het omgezette project of de taak het oplossen van voorwerpen. Met deze instelling kunt u de resolutie van het oorspronkelijke probleem correleren met de resolutie van het oplosbare object. Zie voor meer informatie over het omzetten van objecten <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overzicht van Oplossende en Oplosbare objecten </a>.</p> <p>Deze instelling heeft alleen effect als u <strong>Behoud het oorspronkelijke probleem en koppel de resolutie aan de taak</strong> moet worden geselecteerd.</p> 
       <ul> 
        <li>Wanneer deze instelling is ingeschakeld, kunt u aangepaste statussen maken met dezelfde sleutel voor zowel uitgaven als projecten of taken. Wanneer het project of de taak (als oplosbaar voorwerp) in de douanestatus verandert, weerspiegelt de verandering ook de status van de kwestie. De statussleutel moet gelijk zijn voor de uitgave en project- of taakstatus.</li> 
        <li>Als deze instelling is uitgeschakeld, wordt de status van het oplossen van objecten automatisch ingesteld op de standaardstatus in plaats van op de status Aangepast. Voor meer informatie over de standaardstatussen raadpleegt u <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Toegang krijgen tot de lijst met systeemuitgiftestatussen</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bij het converteren van een uitgave naar een taak</td> 
      <td> <p>Met de instellingen in dit gedeelte wordt bepaald wat er gebeurt tijdens het conversieproces van uitgave tot taak:</p> 
       <ul> 
        <li><strong>Behoud het oorspronkelijke probleem en koppel de resolutie aan de taak</strong>: Wanneer u de uitgave omzet, blijft het zichtbaar als kwestie tot de taak volledig is. De status van de uitgave wordt automatisch gewijzigd in Gesloten wanneer de taak is voltooid.</li> 
        <li><strong>Primaire contactpersoon toegang tot de taak geven</strong>: Geeft de primaire contactpersoon (maker van de uitgave) toegang tot de taak om de taak te beoordelen, updates uit te voeren en op de hoogte te blijven van de voortgang</li> 
        <li> <p><strong>Deze instellingen mogen tijdens de conversie worden gewijzigd</strong>: Hiermee kan de gebruiker die de uitgave converteert deze opties wijzigen tijdens de conversie van een uitgave naar een taak.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wanneer het omzetten van een kwestie in een project</td> 
      <td> <p>Met de instellingen in deze sectie wordt bepaald wat er gebeurt tijdens het conversieproces van uitgave naar project:</p> 
       <ul> 
        <li><strong>Behoud de oorspronkelijke kwestie en koppel zijn resolutie aan het project</strong>: Wanneer u de kwestie omzet, blijft het zichtbaar als kwestie tot het project volledig is. De status van de uitgave verandert automatisch in Gesloten wanneer het project voltooit.</li> 
        <li><strong>Primaire contactpersoon toegang tot het project geven</strong>: Geeft de primaire contactpersoon (maker van de uitgave) toegang tot het project om het project te beoordelen, updates uit te voeren en op de hoogte te blijven van de voortgang.</li> 
        <li><strong>Deze instellingen mogen tijdens de conversie worden gewijzigd</strong>: Staat de gebruiker toe die de kwestie omzet om de vermelde opties tijdens de omzetting van een kwestie in een project te veranderen.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Verwijderen {#deletion}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Gebruikers toestaan taken en problemen met geregistreerde uren te verwijderen</td> 
      <td> <p> Hiermee kunt u bepalen of u het verwijderen van taken of problemen toestaat waarbij uren worden geregistreerd. Deze optie is standaard ingeschakeld.</p> 
       <div> 
        <p><b>Tip</b>: Deze instelling is ook van toepassing op het verwijderen van projecten die taken of problemen hebben met het aantal uren dat is aangemeld. Deze instelling is niet van toepassing op het verwijderen van projecten waarbij de tijd rechtstreeks voor het project wordt vastgelegd. </p> 
        <p>Overweeg het volgende:</p> 
        <ul> 
         <li> <p>Als deze optie is geselecteerd, ontvangt u een informatieve waarschuwing wanneer u een taak of uitgave verwijdert. De waarschuwing herinnert u eraan dat als de taak of de kwestie uren het programma heeft geopend, zij of naar het project zullen worden verplaatst of worden geschrapt. U kunt vormen of de uren worden geschrapt of aan het project in het gebied van de Voorkeur van de Tijdopmaak &amp; van Uren van de Opstelling worden bewogen. Nadat u hebt bevestigd dat u de waarschuwing hebt gezien, wordt de taak of het probleem verwijderd. Voor meer informatie over het vormen van de Voorkeur van Timesheet &amp; van Uren, zie <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Voorkeuren voor tijdpagina's en uren configureren</a>. </p> <p>Tip: <span>Wanneer u een project met taken en kwesties schrapt die uren het programma geopend hebben, worden de geregistreerde uren of geschrapt of zij volgens de montages in het gebied van de Voorkeur van Timesheet &amp; van Uren van Opstelling behouden</span>. </p> </li> 
         <li><span>Wanneer u deze optie deselecteert, ontvangt u een belemmerende waarschuwing wanneer u een taak of een kwestie met geregistreerde uren schrapt, of wanneer u een project met uren schrapt die voor zijn taken of kwesties worden geregistreerd</span> <span>.</span> De waarschuwing geeft aan dat de beheerder het niet toestaat dat taken of problemen met geregistreerde uren worden verwijderd. De taken, kwesties<span>, of projecten die uren voor taken en kwesties hebben geregistreerd</span> kan niet worden verwijderd. </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

### Werkelijke datums {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Wanneer een taak of kwestie van "Nieuw"aan "Bezig"gaat plaats de Ware Datum van het Begin aan</td> 
      <td> <p>Selecteer een van de volgende opties als de Begindatum wordt vastgelegd in Workfront wanneer een taak of uitgave begint op <strong>Nieuw</strong> tot <strong>In uitvoering</strong>:</p> 
       <ul> 
        <li><strong>Nu:</strong> De werkelijke begindatum wordt ingesteld op de huidige datum.</li> 
        <li><strong>De geplande begindatum:</strong> De werkelijke begindatum wordt ingesteld op de geplande begindatum van de taak of uitgave.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wanneer een taak of kwestie wordt voltooid, plaats de Ware Datum van Voltooiing aan</td> 
      <td> <p>Selecteer een van de volgende opties als de datum van feitelijke voltooiing wordt vastgelegd in Workfront wanneer een taak of uitgave is voltooid:</p> 
       <ul> 
        <li><strong>Nu:</strong> De datum van werkelijke voltooiing is ingesteld op de huidige datum.</li> 
        <li> <p><strong>De geplande afsluitdatum:</strong> De datum van daadwerkelijke voltooiing wordt geplaatst aan de Geplande VoltooiingsDatum van de taak of de kwestie.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--
   This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it. Here's what Jeremy Flores says on 12/1/20:
   
   I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.
   You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.
   Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.

   To switch to the Start button:
   
   Select Change the Work On It button to a Start button to automatically update the status of an item. 
   In the lists of check boxes that display below this option, select one or more statuses for each work item type. With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item. 
     
   Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.
   If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.
   This setting is not currently available in
   
   The Workfront Mobile App
   Workfront for Office 365
   Workfront email notifications
   
   This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.
   If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.
   -->

### Toegang {#access}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Wanneer iemand is toegewezen aan een taak</td> 
      <td> 
       <ul> 
        <li><strong>Geef ze... toegang tot een taak</strong>: Definieert de standaardmachtigingen die een gebruiker heeft voor de taak waaraan hij of zij is toegewezen. Voor meer informatie over taaktoestemmingen, zie<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Toegang verlenen aan gebruikers</a>.</li> 
        <li> <p><strong>Ook verlenen zij ... toegang tot het project</strong>: Bepaalt de standaardtoestemming een gebruiker aan het project heeft waarop zij een taak hebben die aan hen wordt toegewezen. Voor meer informatie over projecttoestemmingen, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Projectvoorkeuren voor het hele systeem configureren</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wanneer iemand aan een kwestie wordt toegewezen</td> 
      <td> 
       <ul> 
        <li><strong>Geef ze... toegang tot een taak</strong>: Definieert de standaardmachtigingen die een gebruiker heeft voor de taak waaraan hij of zij is toegewezen. Voor meer informatie over taaktoestemmingen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</li> 
        <li> <p><strong>Ook verlenen zij ... toegang tot het project</strong>: Bepaalt de standaardtoestemming een gebruiker aan het project heeft waarop zij een taak hebben die aan hen wordt toegewezen. Voor meer informatie over projecttoestemmingen, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Projectvoorkeuren voor het hele systeem configureren</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wanneer iemand een verzoek indient</td> 
      <td> 
       <ul> 
        <li><strong>Geef ze... toegang tot de kwestie</strong>: Bepaalt de standaardtoestemming een gebruiker op een verzoek heeft zij voorgelegd. Zie voor meer informatie <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Een uitgave delen</a>.</li> 
        <li> <p><strong>De mensen van het zelfde bedrijf zullen de zelfde toestemmingen voor alle verzoeken erven</strong>: Staat gebruikers toe om verzoeken te zien die door andere gebruikers van het zelfde bedrijf worden voorgelegd zoals zij. Zij hebben de zelfde toestemmingen op die verzoeken zoals zij op hun hebben voorgelegd.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
