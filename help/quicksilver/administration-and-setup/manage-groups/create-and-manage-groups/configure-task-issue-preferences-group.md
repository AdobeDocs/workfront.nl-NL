---
title: Taak- en probleemvoorkeuren voor een groep configureren
user-type: administrator
product-area: system-administration;user-management;setup
keywords: groep,voorkeuren,taak,uitgave,ontgrendelen
navigation-topic: create-and-manage-groups
description: Als de groepen in uw organisatie een taak of een uitgiftevoorkeur onafhankelijk van de manier moeten vormen het op het systeemniveau wordt gevormd, kan een beheerder van Adobe Workfront de voorkeur ontgrendelen. Dan, als groepsbeheerder, kunt u de voorkeur voor uw groep vormen en het zal alle taken of kwesties beïnvloeden verbonden aan uw groep.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '2159'
ht-degree: 0%

---

# Taak- en uitgavevoorkeuren voor een groep configureren

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Als de groepen in uw organisatie een taak of een uitgiftevoorkeur onafhankelijk van de manier moeten vormen het op het systeemniveau wordt gevormd, kan een beheerder van Adobe Workfront de voorkeur ontgrendelen. Dan, als groepsbeheerder, kunt u de voorkeur voor uw groep vormen en het zal alle taken of kwesties beïnvloeden verbonden aan uw groep.

Als er groepen zijn boven de groep die u beheert, kunnen hun beheerders dit ook voor uw groep doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

Voor informatie over hoe de beheerder van Workfront voorkeur ontgrendelt, zie [&#x200B; het Slot of ontgrendelt projectvoorkeur voor alle groepen in het systeem &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>Configuratie op groepsniveau is ook mogelijk voor projectvoorkeuren. Voor informatie, zie [&#x200B; projectvoorkeur voor een groep &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) vormen.

>[!NOTE]
>
>* Een niet-vergrendelde voorkeur blijft meestal voor onbepaalde tijd ontgrendeld. Als de beheerder van Workfront het opnieuw sluit, wordt het systeem opnieuw plaatsend dat en de montages voor de voorkeur door de groepsbeheerders wordt gemaakt worden verloren.
>* De voorkeuren die zijn ingesteld voor de groep die is gekoppeld aan een project, hebben voorrang op de voorkeuren die zijn ingesteld voor de thuisgroep van de gebruiker die het project maakt.
>* Sommige voorkeuren op groepsniveau zijn van invloed op projectsjablonen die u voor de groep maakt. Voor meer informatie, zie de sectie [&#x200B; Mening, werk met, en creeer malplaatjes voor uw groep van het gebied van Groepen &#x200B;](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) in het artikel [&#x200B; creeer en wijzig het projectmalplaatjes van een groep &#x200B;](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Nadat een beheerder van Workfront een voorkeur op het systeemniveau ontgrendelt, kunt u het vormen en dan het sluiten om ervoor te zorgen dat iedereen in uw groep en in zijn subgroepen de zelfde configuratie gebruikt. Dit is parallel aan de mogelijkheid dat een Workfront-beheerder een voorkeur voor iedereen in het systeem moet configureren en vergrendelen. Voor meer informatie, zie [&#x200B; Slot of ontgrendel een project, een taak, of een uitgiftevoorkeur voor subgroups &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>U moet een groepsbeheerder van de groep of een systeembeheerder zijn.</td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De ontgrendelde taak- en probleemvoorkeuren voor een groep op hoofdniveau configureren

>[!TIP]
>
>Als u een Workfront-beheerder bent, kunt u de stappen 1 tot en met 4 omzeilen door naar Instellingen > Projectvoorkeuren > Taken en problemen te gaan en vervolgens in het vak boven aan de pagina naar de naam van de groep te zoeken.

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen** ![&#x200B; pictogram van Groepen &#x200B;](assets/groups-icon.png).

1. Klik op de naam van de groep waarvoor u de ontgrendelde taak en voorkeuren voor uitgaven wilt configureren.
1. Op de pagina die voor de groep, in het linkerpaneel toont, klik **de Voorkeur van de Taak &amp; van de Kwestie**.
1. Op de pagina die verschijnt, ga met één van de 5 die secties onder deze stappen worden vermeld om montages voor de Gebieden Nieuwe Gebieden te vormen de Gebreken van de Taak, Kwesties, Schrapping, Ware Datums, en Toegang, dan klik **sparen**.

   Als u over het slotpictogram ![&#x200B; pictogram van het Slot &#x200B;](assets/lock-toggle-button-dimmed.png) voor een voorkeur beweegt die u moet vormen en toont van een hulpmiddeluiteinde om u te vertellen dat gesloten is, kunt u uw beheerder van Workfront vragen om het voor alle groepen in de organisatie te ontgrendelen.

   Wanneer deze ontgrendeld is, kunnen u en andere groepsbeheerders deze afzonderlijk configureren voor uw eigen groepen. U kunt deze ook vergrendelen voor uw groep en voor alle subgroepen onder uw groep.

   * [&#x200B; Nieuwe Gebreken van de Taak &#x200B;](#new-task-defaults)
   * [&#x200B; Kwesties &#x200B;](#issues)
   * [&#x200B; Schrapping &#x200B;](#deletion)
   * [Verplaatsen](#move)
   * [Werkelijke datums](#actual-dates)
   * [Delegatie](#delegation)
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
      <td> <p>Bepaalt het verband tussen het aantal middelen (en hun toewijzingspercentage) en de duur of de totale inspanning voor de taak. Voor meer informatie, zie {de Duur van 0} Taak en de Types van Duur: artikelindex </a><a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref"></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type inkomsten</td> 
      <td> <p>Berekent de geplande en werkelijke inkomstenramingen voor een taak. Wanneer het <strong> Type van Inkomsten </strong> aan <strong> niet Billable </strong> wordt geplaatst, produceren de geplande uren en de daadwerkelijke geregistreerde uren geen opbrengstschatting voor de taak, en het werk aan de taak draagt niet aan project-vlakke opbrengst bij.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kostensoort</td> 
      <td> <p>Berekent geplande en daadwerkelijke kostenramingen voor een taak. Wanneer geplaatst aan <strong> Geen Kosten </strong>, produceren de geplande uren en de daadwerkelijke geregistreerde uren geen geplande of daadwerkelijke kostenraming voor de taak, en het werk aan de taak draagt niet aan project-vlakke kosten bij.</p> </td> 
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
      <td> <p>Wanneer iemand een kwestie in een project of een taak omzet, zowel worden de originele kwestie als het omgezette project of de taak het oplossen van voorwerpen. Met deze instelling kunt u de resolutie van het oorspronkelijke probleem correleren met de resolutie van het oplosbare object. Voor meer informatie over het oplossen van voorwerpen, zie <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref"> Overzicht van het Oplossen van en Oplosbare Voorwerpen </a>.</p> <p>Opdat dit plaatsen om het even welk effect te hebben, moet de optie <strong> de originele kwestie houden en zijn resolutie aan de taak </strong> binden worden geselecteerd.</p> 
       <ul> 
        <li>Wanneer deze instelling is ingeschakeld, kunt u aangepaste statussen maken met dezelfde sleutel voor zowel uitgaven als projecten of taken. Wanneer het project of de taak (als oplosbaar voorwerp) in de douanestatus verandert, weerspiegelt de verandering ook de status van de kwestie. De statussleutel moet gelijk zijn voor de uitgave en project- of taakstatus.</li> 
        <li>Als deze instelling is uitgeschakeld, wordt de status van het oplossen van objecten automatisch ingesteld op de standaardstatus in plaats van op de status Aangepast. Voor meer informatie over de standaardstatussen, zie <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref"> Toegang tot de lijst van de statussen van de systeemkwestie </a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bij het converteren van een uitgave naar een taak</td> 
      <td> <p>Met de instellingen in dit gedeelte wordt bepaald wat er gebeurt tijdens het conversieproces van uitgave tot taak:</p> 
       <ul> 
        <li><strong> houd de originele kwestie en band zijn resolutie aan de taak </strong>: Wanneer u de kwestie omzet, blijft het zichtbaar als kwestie tot de taak volledig is. De status van de uitgave wordt automatisch gewijzigd in Gesloten wanneer de taak is voltooid.</li> 
        <li><strong> sta Primair Contact toe om toegang tot de taak </strong> te hebben: Verleent het primaire contact (de schepper van de kwestie) toegang tot de taak om de taak te herzien, updates te maken, en op de hoogte te blijven van zijn vooruitgang</li> 
        <li> <p><strong> laat deze montages toe om tijdens omzetting </strong> worden veranderd: Staat de gebruiker toe die de kwestie omzet om deze opties tijdens de omzetting van een kwestie in een taak te veranderen.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wanneer het omzetten van een kwestie in een project</td> 
      <td> <p>Met de instellingen in deze sectie wordt bepaald wat er gebeurt tijdens het conversieproces van uitgave naar project:</p> 
       <ul> 
        <li><strong> houd de originele kwestie en verbind zijn resolutie aan het project </strong>: Wanneer u de kwestie omzet, blijft het zichtbaar als kwestie tot het project volledig is. De status van de uitgave verandert automatisch in Gesloten wanneer het project voltooit.</li> 
        <li><strong> sta Primair Contact toe om toegang tot het project </strong> te hebben: Verleent de primaire contact (de schepper van de kwestie) toegang tot het project om het project te herzien, updates te maken, en van zijn vooruitgang op de hoogte te blijven.</li> 
        <li><strong> laat deze montages toe om tijdens omzetting </strong> worden veranderd: Staat de gebruiker toe die de kwestie omzet om de vermelde opties tijdens de omzetting van een kwestie in een project te veranderen.</li> 
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
        <p><b> Uiteinde </b>: Dit het plaatsen is ook op het schrappen van projecten van toepassing die taken of kwesties met uren hebben die hen worden het programma geopend. Deze instelling is niet van toepassing op het verwijderen van projecten waarbij de tijd rechtstreeks voor het project wordt vastgelegd. </p> 
        <p>Overweeg het volgende:</p> 
        <ul> 
         <li> <p>Als deze optie is geselecteerd, ontvangt u een informatieve waarschuwing wanneer u een taak of uitgave verwijdert. De waarschuwing herinnert u eraan dat als de taak of de kwestie uren het programma heeft geopend, zij of naar het project zullen worden verplaatst of worden geschrapt. U kunt vormen of de uren worden geschrapt of aan het project in het gebied van de Voorkeur van de Tijdopmaak &amp; van Uren van de Opstelling worden bewogen. Nadat u hebt bevestigd dat u de waarschuwing hebt gezien, wordt de taak of het probleem verwijderd. Voor meer informatie over het vormen van de Voorkeur van Timesheet &amp; van Uren, zie <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref"> timesheet en uurvoorkeur </a> vormen. </p> <p>Tip: <span> wanneer u een project met taken en kwesties schrapt die uren het programma hebben geopend, worden de geregistreerde uren of volgens de montages in het gebied van de Voorkeur van de Tijdopnemer &amp; van Uren van Opstelling </span> geschrapt. </p> </li> 
         <li><span> wanneer u deze optie schrapt, ontvangt u een verbodswaarschuwing wanneer u een taak of een kwestie met geregistreerde uren schrapt, of wanneer u een project met uren schrapt die voor zijn taken of kwesties </span> worden geregistreerd <span>.</span> De waarschuwing geeft aan dat de beheerder het niet toestaat dat taken of problemen met geregistreerde uren worden verwijderd. De taken, de kwesties <span>, of de projecten die uren hebben voor taken en kwesties </span> worden geregistreerd kunnen niet worden geschrapt. </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>


### Verplaatsen

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Gebruikers toestaan taken en problemen met geregistreerde uren te verplaatsen</td> 
      <td> <p> Hiermee kunt u bepalen of u de verplaatsing van taken of problemen toestaat waar uren worden geregistreerd. Deze optie is standaard ingeschakeld.</p> 
       <p>Overweeg het volgende:</p> 
        <ul> 
         <li> Als deze optie is geselecteerd, kunt u taken en problemen met tijd verplaatsen. De uren bewegen zich ook met de taken of de kwesties. </li>
      <li>Wanneer u deze optie uitschakelt, ontvangt u een verbodswaarschuwing wanneer u een taak of uitgave met geregistreerde uren verplaatst. De waarschuwing geeft aan dat de beheerder het verplaatsen van taken of problemen met geregistreerde uren niet toestaat. De taken of de kwesties die uren het programma worden geopend kunnen niet naar een ander project worden verplaatst. U kunt taken met geregistreerde uren binnen het zelfde project bewegen, zelfs met deze optie schrapt.  </li></ul>
      </td> 
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
      <td> <p>Selecteer één van de volgende opties voor wanneer de Ware Datum van het Begin in Workfront wordt geregistreerd wanneer een taak of een kwestie van <strong> Nieuw </strong> <strong> </strong> gaat.</p> 
       <ul> 
        <li><strong> nu:</strong> De Ware Datum van het Begin wordt geplaatst aan de huidige datum.</li> 
        <li><strong> de Geplande Datum van het Begin:</strong> de Ware Datum van het Begin wordt geplaatst aan de Geplande Datum van het Begin van de taak of de kwestie.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wanneer een taak of kwestie wordt voltooid, plaats de Ware Datum van Voltooiing aan</td> 
      <td> <p>Selecteer een van de volgende opties als de datum van feitelijke voltooiing wordt vastgelegd in Workfront wanneer een taak of uitgave is voltooid:</p> 
       <ul> 
        <li><strong> nu:</strong> De Ware Datum van de Voltooiing wordt geplaatst aan de huidige datum.</li> 
        <li> <p><strong> de Geplande Datum van de Voltooiing:</strong> de Ware Datum van de Voltooiing wordt geplaatst aan de Geplande Datum van de Voltooiing van de taak of kwestie.</p> </li> 
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

### Delegatie

Als u de instelling **[!UICONTROL Allow users to delegate their tasks and issues]** inschakelt, kunnen alle gebruikers in de groep hun werk tijdelijk delegeren aan anderen.

Wanneer deze instelling is ingeschakeld, kunnen groepsgebruikers het volgende zien:

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

### Toegang {#access}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Wanneer iemand is toegewezen aan een taak</td> 
      <td> 
       <ul> 
        <li><strong> geef hen ... toegang tot een taak </strong>: bepaalt de standaardtoestemming een gebruiker aan de taak heeft zij worden toegewezen aan. Voor meer informatie over taaktoestemmingen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> de toegang van de Verlening tot gebruikers </a>.</li> 
        <li> <p><strong> verleent hen ook... toegang tot het project </strong>: bepaalt de standaardtoestemming een gebruiker aan het project heeft waaraan zij een taak hebben die aan hen wordt toegewezen. Voor meer informatie over projecttoestemmingen, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref"> systeem-brede projectvoorkeur </a> vormen.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wanneer iemand aan een kwestie wordt toegewezen</td> 
      <td> 
       <ul> 
        <li><strong> geef hen ... toegang tot een taak </strong>: bepaalt de standaardtoestemming een gebruiker aan de taak heeft zij worden toegewezen aan. Voor meer informatie over taaktoestemmingen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Toegang van de Verlening tot gebruikers </a>.</li> 
        <li> <p><strong> verleent hen ook... toegang tot het project </strong>: bepaalt de standaardtoestemming een gebruiker aan het project heeft waaraan zij een taak hebben die aan hen wordt toegewezen. Voor meer informatie over projecttoestemmingen, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref"> systeem-brede projectvoorkeur </a> vormen.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wanneer iemand een verzoek indient</td> 
      <td> 
       <ul> 
        <li><strong> geef hen.. toegang tot de kwestie </strong>: Bepaalt de standaardtoestemming een gebruiker op een verzoek heeft zij voorgelegd. Voor meer informatie, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref"> een kwestie </a> delen.</li> 
        <li> <p><strong> de Mensen van het zelfde bedrijf zullen de zelfde toestemmingen voor alle verzoeken </strong> erven: Staat gebruikers toe om verzoeken te zien die door andere gebruikers van het zelfde bedrijf worden voorgelegd zoals zij. Zij hebben de zelfde toestemmingen op die verzoeken zoals zij op hun hebben voorgelegd.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
