---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Bepaal uurtypes en beschikbaarheid voor timesheets
description: Een Type van Uur is een etiket dat u toestaat om tijdingang te categoriseren. Afhankelijk van de rapporteringsvereisten van uw organisatie voor uren, kan dit een essentieel deel van registrerentijd zijn.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '1240'
ht-degree: 0%

---

# Bepaal uurtypes en beschikbaarheid voor timesheets

Een Type van Uur is een etiket dat u toestaat om tijdingang te categoriseren. Afhankelijk van de rapporteringsvereisten van uw organisatie voor uren, kan dit een essentieel deel van registrerentijd zijn.

Adobe Workfront kent twee uurtypen:

* **Algemene uren:** Uren die niet aan een project, zoals zieke tijd of toediening worden geassocieerd. U kunt algemene uren slechts op timesheet registreren.
* **Projectspecifieke uren:** Uren die projecten, taken, en kwesties het programma werden geopend. U kunt project-specifieke uren van om het even welke plaatsen registreren waar u tijd kunt registreren.

Wanneer het registreren van tijd in Workfront, de project-specifieke uurtypes die beschikbaar zijn afhangen van configuratieopties die bij het systeem, het project, en gebruikersniveaus worden geplaatst. (De volgende standaardproject-specifieke uurtypes zijn altijd beschikbaar: de Tijd van het project, de Tijd van de Taak, en Tijd van de Uitgave.)

De uurtypes die beschikbaar zijn om te selecteren wanneer het registreren tijd (op projecten, taken, en kwesties) eerst door de uurtypes worden bepaald die systeem-breed door de systeembeheerder ter beschikking worden gesteld, en dan door de uurtypes die op het project en gebruikersniveaus worden geselecteerd.

Nadat de aangewezen uurtypes zijn gevormd, kunt u tijd van veelvoudige plaatsen in Workfront registreren, zoals die in wordt beschreven [Logtijd](../../timesheets/create-and-manage-timesheets/log-time.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>De beheerdertoegang van het systeem om systeem-brede uurtypes te bepalen en alle gebruikers uit te geven</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>De toegang tot het project beheren om uurtypes op een project te bepalen</td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement- of licentietype u hebt.

## Beschikbaarheid op systeemniveau bepalen

De systeembeheerder bepaalt welke project-specifieke uurtypes beschikbaar worden gemaakt systeembreed, zoals die in wordt beschreven [Uurtypen beheren](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Beschikbaarheid op projectniveau bepalen {#define-availability-at-the-project-level}

De projecteigenaar bepaalt of alle die uurtypes op het systeemniveau worden bepaald op het project (en taken en kwesties binnen het project) beschikbaar zijn, of slechts een ondergroep van die uurtypes beschikbaar zijn. 

1. Ga naar het project waar u de beschikbaarheid van uurtypes wilt bepalen.
1. Klik op de knop **Meer** naast de naam van de taak klikt u op **Bewerken**.

1. Klikken **Project bewerken**.
1. In de **Instellingen** de sectie te zoeken **Rijtypen filteren** -optie.

1. Selecteren **Nee** om alle project-specifieke uurtypes op het project ter beschikking te stellen.

   of

   Selecteren **Ja** om slechts een ondergroep van de project-specifieke uurtypes beschikbaar te maken op het project, dan selecteer de uurtypes u beschikbaar wilt maken. (Houd Shift ingedrukt als u meerdere uurtypen wilt selecteren.)

   Als u deze optie selecteert, worden alleen de uurstypen die u selecteert, beschikbaar gemaakt om te selecteren wanneer u zich aanmeldt in uren voor het project (of voor taken en problemen binnen het project). Als u deze optie selecteert en u geen uurtypes selecteert, toont het project slechts algemene uurtypes.

   De zelfde selecties moeten op het individuele gebruikersniveau worden gemaakt opdat de gebruiker deze uurtypeopties op het project ziet.

1. Klikken **Wijzigingen opslaan**.

## Beschikbaarheid op gebruikersniveau definiëren

U kunt uren voor een bepaald uurtype op projecten, taken, en kwesties registreren slechts als dat uurtype op het systeemniveau, op het projectniveau, en op het gebruikersniveau beschikbaar is gemaakt.

Als u een uurtype op het gebruikersniveau beschikbaar maakt zoals die in deze sectie wordt beschreven, maar u ziet niet dat uurtype wanneer het registreren van tijd op een project, een taak, of een kwestie, dat uurtype niet beschikbaar op het project (zoals die in wordt beschreven [Beschikbaarheid op projectniveau bepalen](#define-availability-at-the-project-level)).

Om de uurtypes te bepalen die aan een gebruiker beschikbaar zijn:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) rechtsboven in Adobe Workfront.

1. Klik op de gebruikersavatar in de linkerbovenhoek.
1. Klik op de knop **Meer** naast de gebruikersnaam en klik vervolgens op **Bewerken**.

1. Alleen een systeembeheerder kan andere gebruikers bewerken. Als u een licentie voor abonnementen hebt, kunt u de uurtypen in uw eigen profiel bewerken.
1. In de **Bronplanning** in de **Beschikbare uurtypen** drop-down menu, doe één van beiden van het volgende, afhankelijk van welke uurtypes u beschikbaar wilt maken wanneer het registreren van tijd op een project, een taak, of een kwestie:

   * **Alle uurtypen beschikbaar maken voor de gebruiker:** Selecteer alle uurtypen.\
     Als u alle uurtypen niet selecteert, is dit technisch hetzelfde als het selecteren van alle uurtypen. In dit geval is het hele uurtype echter alleen beschikbaar voor de gebruiker bij projecten, taken en problemen waarbij **Nee** is geselecteerd in het dialoogvenster **Rijtypen filteren** optie bij het bewerken van het project, zoals beschreven in [Beschikbaarheid op projectniveau bepalen](#define-availability-at-the-project-level).
   * **Alleen een subset van de uurtypen beschikbaar maken voor de gebruiker:** Selecteer alleen de uurtypen die u beschikbaar wilt maken.

     Opdat de uurtypes u op het gebruikersniveau selecteert om op projecten, taken, en kwesties beschikbaar te zijn, moeten deze zelfde uurtypes ook in worden geselecteerd **Rijtypen filteren** optie bij het bewerken van het project, zoals beschreven in [Beschikbaarheid op projectniveau bepalen](#define-availability-at-the-project-level).

1. Klikken **Wijzigingen opslaan**.

   Nu wanneer u uren op een project, een taak, of een kwestie registreert, zijn de uurtypes u uitgezocht beschikbaar als die zelfde uurtypes op het projectniveau beschikbaar zijn gemaakt.


## Hoe gebruiker-niveau en project-niveau de types van uren samenwerken

De volgende lijst beschrijft welke uurtypes tonen op een voorwerp nadat u zowel gebruiker-niveau als de project-vlakke uurtypes hebt aangepast en gefilterd:

* Wanneer u een object opent om de tijd te registreren, wordt standaard in het vervolgkeuzemenu Type uur de standaarduurtypen weergegeven die aan de gebruiker zijn gekoppeld. Dit gebeurt wanneer u uw uurtypes niet aanpast.

* Nadat u de Types van Uur aanpast en Beschikbare Types van Uur voor uw gebruiker bepaalt of de Types van Uur voor een project filtreert, bestaan de volgende scenario&#39;s:

   * Als u alle uurtypes voor het Beschikbare gebied van het Type van Uur in het profiel van uw gebruiker selecteerde, en de Types van Uur van het project worden niet gefiltreerd, zult u alle beschikbare uurtypes zien wanneer u tijd registreert.
   * Als u slechts een ondergroep van uurtypes voor het Beschikbare gebied van het Type van Uur in het profiel van uw gebruiker selecteerde, en de Types van Uur van het project worden niet gefiltreerd, zult u slechts de types van uren van de gebruiker zien wanneer u tijd registreert.
   * Als u alle uurtypes voor het Beschikbare gebied van het Type van Uur in het profiel van uw gebruiker selecteerde, en de Types van Uur van het project worden gefiltreerd, zult u slechts de de uurtypes van het project en de standaarduurtypes zoals de Tijd van het Project, de Tijd van de Taak, de Tijd van de Uitgave afhankelijk van het voorwerp zien.
   * Als u slechts een ondergroep van uurtypes voor het Beschikbare gebied van het Type van Uur in het profiel van uw gebruiker selecteerde, en de Types van Uur van het project worden gefiltreerd, zult u slechts de uurtypes zien die voor de gebruiker en het project gemeenschappelijk zijn. Als geen uurtypes voor de gebruiker en het project gemeenschappelijk zijn, slechts de standaarduurtypes tonen (de Tijd van het Project, de Tijd van de Taak, de Tijd van de Uitgave).

>[!TIP]
>
>   Als u een ander Type van Uur eerder dan het standaarduurtype voor een voorwerp selecteert, wordt het uurtype kleverig. De volgende keer dat u zich aanmeldt bij hetzelfde object, wordt het type uur automatisch ingesteld op het object dat u het laatst hebt geselecteerd.

