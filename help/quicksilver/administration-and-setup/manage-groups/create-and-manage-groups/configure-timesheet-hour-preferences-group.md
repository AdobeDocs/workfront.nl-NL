---
user-type: administrator
product-area: system-administration;user-management
keywords: groep,voorkeuren,taak,groepen,uitgave,ontgrendelen
navigation-topic: create-and-manage-groups
title: De voorkeuren voor tijdbladen en uren voor een groep configureren
description: Op systeemniveau, kan een beheerder van Adobe Workfront de timesheet en de sectie van de uurvoorkeur Algemene Voorkeur ontgrendelen en pre-bevolkt timesheets met. Hierdoor kunnen groepsbeheerders de opties in die secties onafhankelijk voor hun eigen groepen configureren.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '1358'
ht-degree: 0%

---

# Voorkeuren voor tijdschriften en uren voor een groep configureren

Een beheerder van Adobe Workfront kan de volgende secties van timesheet en uurvoorkeur op systeemniveau ontgrendelen zodat de groepsbeheerders hen voor hun eigen groepen onafhankelijk kunnen vormen:

* Algemene voorkeuren
* Waar gebruikers tijd kunnen vastleggen
* Vooraf ingevulde tijdbladen

Als er groepen zijn boven de groep die u beheert, kunnen hun beheerders dit ook voor uw groep doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

De volgende secties op de pagina van de Voorkeur van Timesheet en van Uren zijn configureerbaar slechts op het systeemniveau en kunnen niet voor groepen worden ontgrendeld:

* Verwijderde projecten, taken en problemen

Voor informatie over hoe een beheerder van Workfront een timesheet en een uurvoorkeur ontgrendelt, zie de sectie [ timesheet en de uurvoorkeur voor groepen ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) in het artikel [ vormen timesheet en uurvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>Configuratie op groepsniveau is ook mogelijk voor projectvoorkeuren en voor taak- en uitgavenvoorkeuren. Voor informatie, zie [ projectvoorkeur voor een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) vormen en [ vorm taak en geef voorkeur voor een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) uit.

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

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Groeptimesheet en voorkeuren voor uren

Overweeg de volgende informatie over het vormen van een ontgrendelde timesheet of uurvoorkeur voor een groep:

* Als u een groepsbeheerder bent en u een timesheet of een uurvoorkeur voor uw groep vormt, beïnvloedt het mensen die de groep als hun Groep van het Huis gebruiken.
* Een niet-vergrendelde voorkeur blijft meestal voor onbepaalde tijd ontgrendeld. Als de beheerder van Workfront het opnieuw sluit, wordt het systeem opnieuw plaatsend dat en de montages voor de voorkeur door de groepsbeheerders wordt gemaakt worden verloren.
* Een timesheet erft timesheet en de uurvoorkeur die voor de Groep van het Huis van de timesheet wordt gevormd.

  <!--
  Add example here?
  -->

* Nadat een beheerder van Workfront een voorkeur op het systeemniveau ontgrendelt en u het voor uw groep vormt, kunt u het dan sluiten om ervoor te zorgen dat iedereen in de groepen onder u de zelfde configuratie gebruikt. Dit is parallel aan de mogelijkheid dat een Workfront-beheerder een voorkeur voor iedereen in het systeem moet configureren en vergrendelen. Voor meer informatie, zie [ Slot of ontgrendel een groep timesheet en een uurvoorkeur ](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## Vorm een niet gesloten timesheet of een uurvoorkeur voor een groep

>[!TIP]
>
>Als u een Workfront-beheerder bent, kunt u de stappen 1 tot en met 4 omzeilen door naar Setup > Tijdblad en uren > Voorkeuren te gaan en vervolgens naar de naam van de groep te zoeken in het vak boven aan de pagina.

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen** ![](assets/groups-icon.png).

1. Klik de naam van de groep waarvan timesheet of uurvoorkeur u wilt vormen.
1. In het linkerpaneel, klik **Chronologie &amp; Uren**.

1. Op de pagina die, in de **Algemene voorkeur** sectie toont, vorm om het even welke volgende opties:

   >[!TIP]
   >
   >Als u de muisaanwijzer boven een voorkeur houdt en knopinfo wordt weergegeven om aan te geven dat deze vergrendeld is, kunt u de Workfront-beheerder vragen deze te ontgrendelen voor alle groepen in de organisatie.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Logtijd voor toekomstige datums</td> 
      <td> <p>Staat gebruikers toe om tijd voor toekomstige data door het systeem binnen te registreren:</p> 
       <ul> 
       <li>Om het even welke projecten, taken, en kwesties waar zij toegang tot logboektijd, ongeacht de groep van het project hebben</li> 
       <li>Hun tijdschema's als Algemene Tijd</li>
       </ul> 
       <p>Dit is nuttig wanneer de gebruikers van plan zijn om vanaf het bureau weg te zijn en die tijd willen vooraf registreren.</p> 
       <p><b> NOTA </b>: U kunt gebruikers niet verhinderen tijd op taken of kwesties te registreren die worden gesloten of geannuleerd. U kunt gebruikers slechts verhinderen om tijd op volledige of dode projecten te registreren. Wij adviseren dat u filters in lijsten van taken en kwesties gebruikt om degenen uit te sluiten die zijn voltooid of geannuleerd zichtbaar aan gebruikers zijn.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uitgaven toevoegen uit een tijdsplaat</td> 
      <td> <p>Laat gebruikers toe om zowel tijd als kosten in timesheet te registreren.</p> 
      <p>Wanneer deze voorkeur voor een groep wordt toegelaten en de groep als huisgroep voor bepaalde gebruikers wordt geplaatst, toont een uitgavenpictogram naast projecten en taken op die gebruikers timesheets. Gebruikers kunnen op dit pictogram klikken om uitgaven voor het project of de taak toe te voegen of te bewerken.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taken handmatig toewijzen aan uurwaarden</td> 
      <td> <p>Gebruikers toestaan handmatig een taakrol te selecteren die in hun gebruikersprofiel is toegewezen of aan het object is toegewezen.</p> <p><b> BELANGRIJK </b>:  
        <ul> 
         <li>Als u dit het plaatsen na het toewijzen van baanrollen aan uuringangen onbruikbaar maakt, moeten de gebruikers uren aanpassen die onder diverse rollen op het lusje van Uren van het project, de taak, of de kwestie worden geregistreerd.</li> 
         <li>Als de gebruiker geen taakrol heeft toegewezen in zijn profiel en er een taak is toegewezen als Taakeigenaar in het dialoogvenster Geavanceerde toewijzingen, wordt die taakrol weergegeven wanneer de gebruiker zich aanmeldt voor de taak.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Tijdschema's bewerken beperken tot eigenaars en beheerders</td> 
      <td> <p>Beperk het uitgeven tot timesheet eigenaars, ongeacht de groep van het project en de beheerders van Workfront. Als deze optie is uitgeschakeld, kunt u tijdbladen ook bewerken door:</p> 
       <ul> 
        <li> <p>Gebruikers met beheerbare toegang tot timesheets en uren op hun toegangsniveau</p> </li> 
        <li> <p>Goedkeuringen van tijdspagina als "Kan uren uitgeven"op timesheet wordt toegelaten</p> </li> 
        <li> <p>De manager van de eigenaar van het timesheet</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Uren bewerken beperken tot eigenaars en beheerders</td> 
      <td>Beperk het bewerken tot de gebruiker die de uren invoert en tot Workfront-beheerders. Deze instelling is van toepassing op het tabblad Uren in een project of in een Uren-rapport.</td> 
     </tr> 
    </tbody> 
   </table>

1. In **waar de gebruikers tijd** sectie kunnen registreren, om het even welke volgende opties vormen:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">De tijd van de logboek direct op projecten</td> 
      <td>Staat gebruikers toe om tijd op het project (zowel op het lusje van Updates als timesheet) te registreren. Als u uw gebruikers wilt beperken van opnametijd op projectniveau, verlaat deze optie ongecontroleerd.</td>
     </tr>
     <tr>
      <td role="rowheader">De tijd van het logboek op projecten die volledig zijn</td>
      <td>Staat gebruikers toe om tijd op een project te registreren dat volledig is gemerkt. Als deze optie is uitgeschakeld, kunnen gebruikers geen tijd vastleggen voor het werk dat zij in de status Voltooid hebben voltooid voor projecten.</td>
     </tr>
     <tr>
      <td role="rowheader">De tijd van het programma van de logboeken op projecten die dood zijn</td> 
      <td>Wanneer deze optie wordt toegelaten, kunnen de gebruikers uren op projecten met een Dode status registreren.</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Deze voorkeur wordt toegepast gebaseerd op configuratie van de voorkeur van de Groep van het Huis van de gebruiker. Als deze montages in de voorkeur van de Groep van het Huis van de gebruiker worden toegelaten, zullen zij tijd op projecten, met inbegrip van voltooide of dode projecten, kunnen direct registreren, ongeacht of de de groepsvoorkeur van het project het toestaat of niet.

1. In **pre-bevolkt timesheets** sectie, vorm om het even welke volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Werk dat binnen &lt;aantal weken&gt; van de het werkwaaier van timesheet is</td> 
      <td> <p>Bepaalt het aantal weken vóór en na de datumwaaier van timesheet die data van taken en kwesties bevat die aan de gebruiker worden toegewezen. De standaardinstelling is 1 week en u kunt dit bereik uitbreiden tot 4 weken. Dit betekent dat het tijdschema vooraf gevuld is met taken en kwesties die data tussen vier weken vóór de datumwaaier van timesheet hebben tot vier weken na de datumwaaier van timesheet, als u 4 weken voor uw waaier selecteert. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taken en problemen die zijn voltooid</td> 
      <td>Als de veelvoudige middelen typisch aan één enkele taak worden toegewezen, adviseren wij dit het plaatsen. Dit betekent wanneer één middel tijd tegen de taak registreert en het als volledig merkt, kunnen de andere middelen die aan de taak worden toegewezen nog de taak of de kwestie in hun timesheet vinden, om hun uren te registreren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taken en kwesties die Geplande Datums in timesheet's datumwaaier hebben</td> 
      <td> <p>Wanneer geselecteerd, omvat timesheet taken en kwesties die of een Geplande Datum van het Begin of een Datum van de Voltooiing hebben die binnen de datumwaaier van timesheet valt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> Taken die de Geprojecteerde Datums in de de datumwaaier van timesheet hebben</td> 
      <td> <p>Wanneer geselecteerd, omvat timesheet taken die of een Verwachte Datum van het Begin of een Datum van de Voltooiing hebben die binnen het tijdkader van het project valt, zelfs als de geplande datum van de kwestie of de taak buiten de timesheet datumwaaier valt.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **sparen**.
