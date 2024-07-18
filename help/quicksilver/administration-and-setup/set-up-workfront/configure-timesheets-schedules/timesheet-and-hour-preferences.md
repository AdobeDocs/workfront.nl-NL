---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Voorkeuren voor tijdpagina's en uren configureren
description: Als  [!DNL Adobe Workfront]  beheerder, kunt u voorkeur voor timesheets en uren in  [!DNL Workfront]  specificeren om te bepalen welke punten de timesheets met kunnen pre-bevolken en welke punten gebruikers tijd kunnen registreren aan.
author: Alina and Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 66e6c96ca51a159f6e9a16178f06dd016217c7d8
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 0%

---

# Voorkeuren voor tijdpagina&#39;s en uren configureren

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als [!DNL Adobe Workfront] -beheerder kunt u voorkeuren opgeven voor tijdbladen en uren in [!DNL Workfront] om te definiëren met welke items de tijdbladen vooraf kunnen worden ingevuld en welke items gebruikers zich kunnen aanmelden.

>[!IMPORTANT]
>
>Naast de punten die een timesheet volgens de voorwaarden vooraf invullen die in dit artikel worden beschreven, tonen de volgende punten ook op timesheets, door gebrek:
>
>* Punten waarvoor u tijd tijdens het tijdkader van timesheet registreerde
>* Items die zijn vastgezet aan de tijdpagina
>* Items die u zoekt en die u handmatig toevoegt aan de tijdpagina. Items die handmatig worden toegevoegd, worden standaard vastgezet.
>
>Voor meer informatie, zie [ tijd van het Logboek ](../../../timesheets/create-and-manage-timesheets/log-time.md) en [ overzicht van de Tijdopnemer ](/help/quicksilver/timesheets/timesheets/timesheets-overview.md).



Alle wijzigingen die u aanbrengt in tijdbladen, zijn van invloed op alle tijdbladen die in de toekomst worden gemaakt.

## Toegangsvereisten

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
   <td><p>Huidige:[!UICONTROL Plan]</p>
   of
   <p>Nieuw: Standaard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder zijn.</p>  </td>
</tr> 
 </tbody> 
</table>

*Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voorkeuren voor tijdbladen en uren instellen

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Timesheet & Hours]** > **[!UICONTROL Preferences]** .

   De pagina Voorkeuren tijdbladen en uren wordt weergegeven.

1. (Facultatief) in de **het onderzoekvakje van de Tijdopnamen en van de Huren van het Systeem**, begin de naam van een groep te typen, dan het te selecteren wanneer het in de lijst toont.

   ![](assets/search-for-group-box-in-timesheets-preferences-page.png)

   De pagina met voorkeuren voor tijdbladen en uren wordt bijgewerkt met de voorkeuren voor de groep die u hebt geselecteerd. Voorkeuren op systeemniveau moeten zijn ontgrendeld om voorkeuren op groepsniveau te kunnen wijzigen. Voor meer informatie, zie de sectie [ timesheet en uurvoorkeur voor groepen ](#unlock-timesheet-and-hour-preferences-for-groups) in dit artikel ontgrendelen.

1. Configureer in de sectie **[!UICONTROL General preferences]** een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Log time for future dates]</td> 
      <td> <p>Staat gebruikers toe om tijd voor toekomstige data door het systeem binnen te registreren:</p> 
       <ul> 
        <li>Om het even welke projecten, taken, en kwesties waar zij toegang tot logboektijd hebben</li> 
        <li>Hun tijdschema's als Algemene Tijd</li> 
       </ul> <p>Dit is nuttig wanneer de gebruikers van plan zijn om vanaf het bureau weg te zijn en die tijd willen vooraf registreren.</p> <p><b> NOTA </b>:</p> 
       <p>U kunt niet voorkomen dat gebruikers zich aanmelden bij taken of problemen die zijn gesloten of geannuleerd. U kunt gebruikers slechts verhinderen om tijd op volledige of dode projecten te registreren. Wij adviseren dat u filters in lijsten van taken en kwesties gebruikt om degenen uit te sluiten die zijn voltooid of geannuleerd zichtbaar aan gebruikers zijn.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL Assign Job Roles to hour entries manually]</td> 
      <td> <p>Gebruikers toestaan handmatig een taakrol te selecteren die in hun gebruikersprofiel is toegewezen of aan het object is toegewezen.</p> <p><b> BELANGRIJK </b>:  
        <ul> 
         <li>Als u deze instelling uitschakelt nadat u taakrollen hebt toegewezen aan uren, moeten gebruikers de uren aanpassen die zijn geregistreerd onder verschillende rollen op het tabblad [!UICONTROL Hours] van het project, de taak of de uitgave.</li> 
         <li>Als er geen taakrol is toegewezen aan de gebruiker in het profiel en er een taak is toegewezen als [!UICONTROL Task Owner] in het dialoogvenster [!UICONTROL Advanced Assignments] , wordt die taakrol weergegeven wanneer de gebruiker zich op de taak aanmeldt.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restrict timesheet editing to owners and administrators]</td> 
      <td> <p>Bewerken beperken tot eigenaars van tijdbladen en [!DNL Workfront] -beheerders. Als deze optie is uitgeschakeld, kunt u tijdbladen ook bewerken door:</p> 
       <ul> 
        <li> <p>Gebruikers met beheerbare toegang tot timesheets en uren op hun toegangsniveau</p> </li> 
        <li> <p>Goedkeuringen van tijdspagina als "Kan uren uitgeven"op timesheet wordt toegelaten</p> </li> 
        <li> <p>De manager van de eigenaar van het timesheet</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restrict hour editing to owners and administrators]</td> 
      <td>Beperk het bewerken tot de gebruiker die de uren invoert en tot [!DNL Workfront] -beheerders. Deze instelling is van toepassing op het tabblad [!UICONTROL Hours] in een project of in een Uren-rapport.</td> 
     </tr> 
    </tbody> 
   </table>

1. Configureer in de sectie **[!UICONTROL Where users can log time]** een van de volgende opties:

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Directly on projects]</td>
        <td>Hiermee kunnen gebruikers zich aanmelden bij het project (zowel op de tab [!UICONTROL Updates] als op het tijdblad). Als de gebruikers geen tijd op het projectniveau registreren, zouden deze opties ongecontroleerd moeten blijven.</td>
    </tr>
    <tr>
        <td>[!UICONTROL On projects that are complete]</td>
        <td>Staat gebruikers toe om tijd op een project te registreren dat volledig is gemerkt. Als deze optie is uitgeschakeld, kunnen gebruikers geen tijd opnemen voor het werk dat ze in de status [!UICONTROL Complete] aan projecten hebben voltooid.</td>
    </tr>
    <tr>
        <td>[!UICONTROL On projects that are dead]</td>
        <td>Wanneer deze optie is ingeschakeld, kunnen gebruikers uren aanmelden bij projecten met de status [!UICONTROL Dead] .</td>
    </tr>
   </table>

1. Configureer in de sectie **[!UICONTROL Pre-populate timesheets]** een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Work that is within] &lt;aantal weken&gt; [!UICONTROL of the timesheet's work range]</td> 
      <td> <p>Bepaalt het aantal weken vóór en na de datumwaaier van timesheet die data van taken en kwesties bevat die aan de gebruiker worden toegewezen.</p> 
      <p>De standaardinstelling is 1 week en u kunt dit bereik uitbreiden tot 4 weken.</p> 
      <p>Dit betekent dat het tijdschema vooraf gevuld is met taken en kwesties die data tussen vier weken vóór de datumwaaier van timesheet hebben tot vier weken na de datumwaaier van timesheet, als u 4 weken voor uw waaier selecteert. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tasks and issues that have been completed]</td> 
      <td>Als de veelvoudige middelen typisch aan één enkele taak worden toegewezen, adviseren wij dit het plaatsen. Dit betekent wanneer één middel tijd tegen de taak registreert en het als volledig merkt, kunnen de andere middelen die aan de taak worden toegewezen nog de taak of de kwestie in hun timesheet vinden, om hun uren te registreren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tasks and issues that have Planned Dates in timesheet's date range]</td> 
      <td> <p>Wanneer geselecteerd, omvat timesheet taken en kwesties die of een Geplande Datum van het Begin of een Datum van de Voltooiing hebben die binnen de datumwaaier van timesheet valt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL Tasks that have Projected Dates in timesheet's date range]</td> 
      <td> <p>Wanneer geselecteerd, omvat timesheet taken die of een Verwachte Datum van het Begin of een Datum van de Voltooiing hebben die binnen het tijdkader van het project valt, zelfs als de geplande datum van de kwestie of de taak buiten de timesheet datumwaaier valt.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Geef in de sectie **[!UICONTROL Deleted projects, tasks, and issues]** het volgende op:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> Bij het verwijderen van projecten</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Keep logged time already added to timesheets as general time]</strong>: Als dit project op een later tijdstip wordt hersteld, blijft de tijd op het tijdspad staan.</li> 
        <li><strong>[!UICONTROL Delete any logged time]</strong>: Als dit project later wordt hersteld, wordt de reeds geregistreerde tijd hersteld aan het project.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bij het verwijderen van taken of problemen</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Move any logged time to the project]</strong> waar de taak of uitgave zich bevindt: Als deze taak of uitgave later wordt hersteld, blijft de tijd op het project.<br></li> 
        <li> <p><strong>[!UICONTROL Delete any logged time]</strong>: Als deze taak of uitgave later wordt hersteld, wordt de geregistreerde tijd hersteld aan de taak of de kwestie.</p> <p>Zie <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Configure affect] Uren wanneer een object wordt verwijderd en hersteld </a> voor meer informatie over deze opties.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Save]**.

## Tijdschema en uurvoorkeuren voor groepen ontgrendelen

De groepen in uw organisatie zouden timesheets of de voorkeur van het uur kunnen nodig hebben verschillend voor hun unieke werkschema&#39;s wordt gevormd die. U kunt de voorkeur voor alle groepen door de organisatie ontgrendelen zodat zij het op hun kunnen vormen.

Wanneer een voorkeur wordt ontgrendeld en een groepsbeheerder het wijzigt, beïnvloedt het timesheet eigenaars als de groep hun Groep van het Huis is.

Voor informatie over hoe een groepsbeheerder timesheet en uurvoorkeur voor een groep vormt, zie [ timesheet en uurvoorkeur voor een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md) vormen.

>[!NOTE]
>
>Nadat een [!DNL Workfront] beheerder een voorkeur op het systeemniveau ontgrendelt, kan om het even welke groepbeheerder het vormen en dan het sluiten om ervoor te zorgen dat iedereen in hun groep en subgroups hieronder de zelfde configuratie gebruikt. Dit is parallel aan de mogelijkheid dat een [!DNL Workfront] -beheerder een voorkeur voor iedereen in het systeem moet configureren en vergrendelen. Voor meer informatie, zie [ Slot of ontgrendel een groep timesheet en een uurvoorkeur ](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

Een projectvoorkeur ontgrendelen zodat groepen deze kunnen configureren:

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **[!UICONTROL Timesheets & Hours]** en klik vervolgens op **[!UICONTROL Preferences]** .

1. Voer een van de volgende handelingen uit:

   * Als u groepsbeheerders een voorkeur voor hun groepen wilt kunnen vormen, klik **ontgrendelen** knevel ![](assets/unlock-toggle-button.png) om het te ontgrendelen.
   * Als u wilt dat alle groepen uw configuratie voor een voorkeur gebruiken, zorg ervoor dat het de knevel gesloten ![](assets/locked-preference-toggle.png) is (dit is het gebrek).

     >[!IMPORTANT]
     >
     >Wij adviseren dat u met de beheerders en de gebruikers in groepen door het systeem communiceert om ervoor te zorgen dat alle behoeften rekenschap worden gegeven op de manier u een gesloten voorkeur vormt.
     >
     >Wanneer u het sluit, wordt uw configuratie voor het geërft door alle groepen in het systeem. En als de voorkeur voor om het even welke periode is ontgrendeld, vervangt uw configuratie die die groepsbeheerders zouden kunnen hebben gemaakt.

1. Klik op **[!UICONTROL Save]**.
