---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Voorkeuren voor tijdpagina's en uren configureren
description: Als [!DNL Adobe Workfront] beheerder, kunt u voorkeur voor timesheets en uren in specificeren [!DNL Workfront] om te bepalen welke punten timesheets met kunnen vooraf invullen en welke punten gebruikers tijd aan registreren kunnen.
author: Courtney and Alina
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 3b0a82381d1c33d897b123a597df21ba54cc2565
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 0%

---

# Voorkeuren voor tijdpagina&#39;s en uren configureren

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als [!DNL Adobe Workfront] beheerder, kunt u voorkeur voor timesheets en uren in specificeren [!DNL Workfront] om te bepalen welke punten timesheets met kunnen vooraf invullen en welke punten gebruikers tijd aan registreren kunnen.

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder.</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## Voorkeuren voor tijdbladen en uren instellen

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik op **[!UICONTROL Timesheet & Hours]** > **[!UICONTROL Preferences]**.

1. Op de pagina die wordt weergegeven, in het dialoogvenster **[!UICONTROL General preferences]** configureren, configureert u een van de volgende opties:

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
       </ul> <p>Dit is nuttig wanneer de gebruikers van plan zijn weg van het bureau te zijn en die tijd willen vooraf registreren.</p> <p><b>OPMERKING</b>: U kunt niet voorkomen dat gebruikers zich aanmelden bij taken of problemen die zijn gesloten of geannuleerd. U kunt gebruikers slechts verhinderen om tijd op volledige of dode projecten te registreren. Wij adviseren dat u filters in lijsten van taken en kwesties gebruikt om degenen uit te sluiten die zijn voltooid of geannuleerd zichtbaar aan gebruikers zijn.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL Assign Job Roles to hour entries manually]</td> 
      <td> <p>Gebruikers toestaan handmatig een taakrol te selecteren die in hun gebruikersprofiel is toegewezen of aan het object is toegewezen.</p> <p><b>BELANGRIJK</b>:  
        <ul> 
         <li>Als u dit het plaatsen na het toewijzen van baanrollen aan uuringangen onbruikbaar maakt, moeten de gebruikers uren aanpassen die onder diverse rollen op worden geregistreerd [!UICONTROL Hours] tabblad van het project, de taak of de uitgave.</li> 
         <li>Als aan de gebruiker geen taakrol is toegewezen in zijn profiel en er een taak is toegewezen als de [!UICONTROL Task Owner] in de [!UICONTROL Advanced Assignments] wordt die taakrol weergegeven wanneer de gebruiker zich aanmeldt bij de taak.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restrict timesheet editing to owners and admins]</td> 
      <td> <p>Bewerken beperken tot eigenaars van tijdbladen en [!DNL Workfront] beheerders. Als deze optie is uitgeschakeld, kunt u tijdbladen ook bewerken door:</p> 
       <ul> 
        <li> <p>Gebruikers met beheerbare toegang tot timesheets en uren op hun toegangsniveau</p> </li> 
        <li> <p>Goedkeuringen van tijdspagina als "Kan uren uitgeven"op timesheet wordt toegelaten</p> </li> 
        <li> <p>De manager van de eigenaar van het timesheet</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restrict hour editing to owners and admins]</td> 
      <td>Bewerken beperken tot de gebruiker die de uren invoert en [!DNL Workfront] beheerders. Deze instelling is van toepassing op de [!UICONTROL Hours] in een project of in een rapport van Uren.</td> 
     </tr> 
    </tbody> 
   </table>

1. In de **[!UICONTROL Where users can log time]** configureren, configureert u een van de volgende opties:

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Log time directly on projects]</td>
        <td>Staat gebruikers toe om tijd op het project (zowel op [!UICONTROL Updates] (en tijdblad). Als de gebruikers geen tijd op het projectniveau registreren, zouden deze opties ongecontroleerd moeten blijven.</td>
    </tr>
    <tr>
        <td>De tijd van het logboek op projecten die volledig zijn</td>
        <td>Staat gebruikers toe om tijd op een project te registreren dat volledig is gemerkt. Als deze optie is uitgeschakeld, kunnen gebruikers geen tijd vastleggen voor het werk dat zij hebben uitgevoerd voor projecten in het dialoogvenster [!UICONTROL Complete] status.</td>
    </tr>
    <tr>
        <td>De tijd van het programma van het programma op projecten die dood zijn</td>
        <td>Wanneer deze optie is ingeschakeld, kunnen gebruikers uren aanmelden bij projecten met een [!UICONTROL Dead] status.</td>
    </tr>
   </table>

1. In de **[!UICONTROL Pre-populate timesheets]** configureren, configureert u een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Work that is within] &lt;number of weeks&gt; [!UICONTROL of the timesheet's work range]</td> 
      <td> <p>Bepaalt het aantal weken vóór en na de datumwaaier van timesheet die data van taken en kwesties bevat die aan de gebruiker worden toegewezen. De standaardinstelling is 1 week en u kunt dit bereik uitbreiden tot 4 weken. Dit betekent dat het tijdschema vooraf gevuld is met taken en kwesties die data tussen vier weken vóór de datumwaaier van timesheet hebben tot vier weken na de datumwaaier van timesheet, als u 4 weken voor uw waaier selecteert. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tasks & Issues that have been completed]</td> 
      <td>Als de veelvoudige middelen typisch aan één enkele taak worden toegewezen, adviseren wij dit het plaatsen. Dit betekent wanneer één middel tijd tegen de taak registreert en het als volledig merkt, kunnen de andere middelen die aan de taak worden toegewezen nog de taak of de kwestie in hun timesheet vinden, om hun uren te registreren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tasks & Issues that have Planned Dates in timesheet's date range]</td> 
      <td> <p>Wanneer geselecteerd, omvat timesheet taken en kwesties die of een Geplande Datum van het Begin of een Datum van de Voltooiing hebben die binnen de datumwaaier van timesheet valt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL Tasks that have Projected Dates in timesheet's date range]</td> 
      <td> <p>Wanneer geselecteerd, omvat timesheet taken die of een Verwachte Datum van het Begin of een Datum van de Voltooiing hebben die binnen het tijdkader van het project valt, zelfs als de geplande datum van de kwestie of de taak buiten de timesheet datumwaaier valt.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. In de **[!UICONTROL Deleted projects, tasks, and issues]** in de sectie, geeft u het volgende op:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL When deleting projects]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Keep logged time already added to timesheets as general time]</strong>: Als dit project op een later tijdstip wordt hersteld, blijft de tijd op het tijdspad staan.</li> 
        <li><strong>[!UICONTROL Delete any logged time]</strong>: Als dit project later wordt hersteld, wordt de reeds geregistreerde tijd hersteld aan het project.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL When deleting tasks or issues]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Move any logged time to the project where the task or issue resides]</strong>: Als deze taak of kwestie later wordt hersteld, blijft de tijd op het project.<br></li> 
        <li> <p><strong>[!UICONTROL Delete any logged time]</strong>: Als deze taak of uitgave later wordt hersteld, wordt de geregistreerde tijd hersteld aan de taak of de kwestie.</p> <p>Zie voor meer informatie over deze opties <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Configure affect] op uren dat een object wordt verwijderd en hersteld</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Save]**.

## Tijdschema en uurvoorkeuren voor groepen ontgrendelen

De groepen in uw organisatie zouden een timesheet of een uurvoorkeur kunnen vereisen die verschillend voor hun unieke werkschema&#39;s wordt gevormd. U kunt de voorkeur voor alle groepen door de organisatie ontgrendelen zodat zij het op hun kunnen vormen.

Wanneer een voorkeur wordt ontgrendeld en een groepsbeheerder het wijzigt, beïnvloedt het timesheet eigenaars als de groep hun Groep van het Huis is.

Voor informatie over hoe een groepsbeheerder timesheet en uurvoorkeur voor een groep vormt, zie [Voorkeuren voor tijdschriften en uren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>Na een [!DNL Workfront] de beheerder ontgrendelt een voorkeur op systeemniveau, kan om het even welke groepsbeheerder het vormen en dan het sluiten om ervoor te zorgen dat iedereen in hun groep en subgroups hieronder de zelfde configuratie gebruikt. Dit is parallel aan de mogelijkheid dat een [!DNL Workfront] de beheerder moet een voorkeur voor iedereen in het systeem vormen en sluiten. Zie voor meer informatie [Een groepsoverzicht en uurvoorkeur vergrendelen of ontgrendelen](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

Om een projectvoorkeur te ontgrendelen zodat de groepen het kunnen vormen:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe] Workfront, klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **[!UICONTROL Timesheets & Hours]** en klik vervolgens op **[!UICONTROL Preferences]**.

1. Voer een van de volgende handelingen uit:

   * Als u wilt dat groepsbeheerders een voorkeur voor hun groepen kunnen vormen, ontgrendel het ![](assets/unlock-toggle-button.png).
   * Als u wilt dat alle groepen uw configuratie voor een voorkeur gebruiken, zorg ervoor dat het gesloten is (dit is het gebrek).

      >[!IMPORTANT]
      >
      >Wij adviseren dat u met de beheerders en de gebruikers in groepen door het systeem communiceert om ervoor te zorgen dat alle behoeften rekenschap worden gegeven op de manier u een gesloten voorkeur vormt. Wanneer u het sluit, wordt uw configuratie voor het geërft door alle groepen in het systeem. En als de voorkeur voor om het even welke periode is ontgrendeld, vervangt uw configuratie die die groepsbeheerders zouden kunnen hebben gemaakt.

1. Klik op **[!UICONTROL Save]**.
