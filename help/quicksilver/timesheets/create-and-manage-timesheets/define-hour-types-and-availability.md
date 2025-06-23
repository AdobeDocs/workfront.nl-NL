---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Bepaal de Types en Beschikbaarheid van Uur
description: Een Type van Uur is een etiket dat u toestaat om tijdingang te categoriseren. Afhankelijk van de rapporteringsvereisten van uw organisatie voor uren, kan dit een essentieel deel van registrerentijd zijn.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '1487'
ht-degree: 0%

---

# De types en beschikbaarheid van uren bepalen

<!--Audited: 6/2025-->

Een Type van Uur is een etiket dat u toestaat om tijdingang te categoriseren. Afhankelijk van de rapporteringsvereisten van uw organisatie voor uren, kan dit een essentieel deel van registrerentijd zijn.

Adobe Workfront kent twee uurtypen:

* **Algemene uren**: Uren die niet met een project, zoals zieke tijd of beleid worden geassocieerd. U kunt algemene uren slechts op timesheet registreren.
* **project-specifieke uren**: De uren het programma geopend projecten, taken, en kwesties. U kunt project-specifieke uren van om het even welke plaats registreren waar u tijd kunt registreren.

Wanneer het registreren van tijd in Workfront, de project-specifieke uurtypes die beschikbaar zijn afhangen van configuratieopties die bij het systeem, het project, en gebruikersniveaus worden geplaatst. (De volgende standaardproject-specifieke uurtypes zijn altijd beschikbaar: de Tijd van het project, de Tijd van de Taak, en Tijd van de Uitgave.)

De uurtypes die beschikbaar zijn om te selecteren wanneer het registreren tijd (op projecten, taken, en kwesties) eerst door de uurtypes worden bepaald die systeem-breed door de systeembeheerder ter beschikking worden gesteld, en dan door de uurtypes die op het project en gebruikersniveaus worden geselecteerd.

Nadat de aangewezen uurtypes zijn gevormd, kunt u tijd van veelvoudige plaatsen in Workfront registreren. Voor meer informatie, zie [ tijd van het Logboek ](../../timesheets/create-and-manage-timesheets/log-time.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Nieuw: Standaard</p> 
   <p>Huidig: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>De beheerdertoegang van het systeem om systeem-brede uurtypes te bepalen en alle gebruikers uit te geven</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>De toegang tot het project beheren om uurtypes op een project te bepalen</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Beschikbaarheid op systeemniveau bepalen

De systeembeheerder bepaalt welke project-specifieke uurtypes in het hele systeem ter beschikking worden gesteld. Voor meer informatie, zie [ de types van uren ](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md) leiden.

## Beschikbaarheid op projectniveau bepalen {#define-availability-at-the-project-level}

De projecteigenaar bepaalt of alle die uurtypes op het systeemniveau worden bepaald op het project (en taken en kwesties binnen het project) beschikbaar zijn, of slechts een ondergroep van die uurtypes beschikbaar zijn.

{{step1-to-projects}}

1. Voor de **pagina van Projecten**, selecteer het project u de beschikbaarheid van uurtypes voor wilt bepalen.
1. Klik het **Meer** pictogram ![ Meer pictogram ](assets/more-icon.png) naast de projectnaam in de kopbal, dan klik **uitgeven**. Het **geeft** paneel van het Project uit opent.

1. In de **sectie van de Montages van het Project**, bepaal de plaats van de **Types van Uur van de Filter**.

1. Selecteer **Nr** om alle project-specifieke uurtypes beschikbaar te maken op het project.

   of

   Selecteer **ja** om slechts een ondergroep van de project-specifieke uurtypes beschikbaar op het project te maken, dan de **Types van Uur** te selecteren u beschikbaar wilt maken. U kunt meerdere uurtypen selecteren.

   >[!NOTE]
   >
   >   Overweeg het volgende:
   >   
   >   * Als u **ja** selecteert, slechts worden de uurtypes u uitgezocht ter beschikking gesteld om te selecteren wanneer het registreren van uren op het project (of op taken en kwesties binnen het project).
   >   
   >   * Als u **ja** selecteert en geen uurtypes selecteert, toont het project slechts algemene uurtypes.
   >
   >   * De zelfde selecties moeten op het individuele gebruikersniveau worden gemaakt opdat de gebruiker deze uurtypeopties op het project ziet.
   >
   >   * Wanneer het Type van Uur van het Standaard van de gebruiker en een project Gefilterde Type van Uur aanpast, wordt dat uurtype geselecteerd door gebrek wanneer het registreren tijd.

1. Klik **sparen**.

## Beschikbaarheid op gebruikersniveau definiëren

U kunt uren voor een bepaald uurtype op projecten, taken, en kwesties registreren slechts als dat uurtype op het systeemniveau, projectniveau, en gebruikersniveau beschikbaar is gemaakt.

Als u een uurtype op het gebruikersniveau beschikbaar maakt zoals die in deze sectie wordt beschreven maar niet dat uurtype ziet wanneer het registreren van tijd op een project, een taak, of een kwestie, dat uurtype niet beschikbaar op het project is gemaakt. Voor meer informatie, zie de volgende sectie in dit artikel: [ bepaalt beschikbaarheid op het projectniveau ](#define-availability-at-the-project-level).

Om de uurtypes te bepalen die aan een gebruiker beschikbaar zijn:

1. Klik het **pictogram van het 1&rbrace; pictogram van het Belangrijkste Menu ![ ](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik uw gebruikersavatar in de upper-left hoek.**

   of

   Klik het **pictogram van het 1&rbrace; Belangrijkste Menu ![ pictogram van het Menu ](assets/adobe-main-menu.png) in de hoger-juiste hoek, als beschikbaar, dan klik** Profiel van Workfront **.**

1. Klik het **Meer** pictogram ![ Meer pictogram ](assets/more-icon.png) naast de gebruikersnaam, dan klik **uitgeven**. Het **geeft Persoon** vakje uit opent.

   >[!IMPORTANT]
   >
   >Alleen een systeembeheerder kan andere gebruikers bewerken. Als u een licentie voor abonnementen hebt, kunt u de uurtypen in uw eigen profiel bewerken.


1. In de **Planning van het Middel** sectie, in **Beschikbare types van Uur** drop-down menu, doe één van beiden van het volgende, afhankelijk van welke uurtypes u beschikbaar wilt maken wanneer het registreren van tijd op een project, een taak, of een kwestie:

   * **om alle uurtypes ter beschikking te stellen voor de gebruiker:** selecteer alle uurtypes.\
     Als u alle uurtypen niet selecteert, is dit technisch hetzelfde als het selecteren van alle uurtypen. Nochtans, in dit geval, zijn alle uurtype beschikbaar voor de gebruiker slechts op projecten, taken, en kwesties waar **Nr** in de **optie van de Types van Uur van de Filter** wordt geselecteerd wanneer het uitgeven van het project, zoals die in [ wordt beschreven bepaalt beschikbaarheid op het projectniveau ](#define-availability-at-the-project-level).
   * **om slechts een ondergroep van de uurtypes beschikbaar voor de gebruiker te maken:** selecteer slechts de uurtypes u beschikbaar wilt maken.

     Opdat de uurtypes u op het gebruikersniveau selecteert om op projecten, taken, en kwesties beschikbaar te zijn, moeten deze zelfde uurtypes ook in de **optie van de Types van Uur van de Filter** worden geselecteerd wanneer het uitgeven van het project, zoals die in [ wordt beschreven bepaalt beschikbaarheid op het projectniveau ](#define-availability-at-the-project-level).

1. (Facultatief) in het **drop-down menu van het Type van Uur 0&rbrace; Standaard, selecteer één uurtype.** Wanneer het Type van Uur van de gebruiker Standaard en een project Gefilterde Type van Uur aanpast, wordt dat uurtype geselecteerd door gebrek wanneer het registreren tijd.

1. Klik **sparen Veranderingen**. Nu, wanneer u uren op een project, een taak, of een kwestie registreert, zijn de uurtypes u uitgezocht beschikbaar als die zelfde uurtypes op het projectniveau beschikbaar zijn gemaakt.

## Hoe gebruiker-niveau en project-niveau de types van uren samenwerken

De volgende lijst beschrijft welke uurtypes tonen op een voorwerp nadat u zowel gebruiker-niveau als de project-vlakke uurtypes hebt aangepast en gefilterd wanneer u tijd op het voorwerp registreert:

* Nadat u het Type Standaarduren voor de gebruiker en de Gefilterde Types van Uur van Project aanpast, toont het drop-down menu van het Type van Uur één van de volgende uurtypes:

   * Wanneer de gebruiker een Type Standaarduren op hun profiel heeft en het project het zelfde Gefilterde Type van Uur heeft, toont dit Type van Uur als geselecteerd gebrek wanneer het registreren tijd; Project, Taak, of de Tijd van de Uitgave tonen als extra opties.

   * Wanneer de gebruiker geen Type van Uur Standaard heeft en het project heeft de Types van Uur gefilterd, het Type van Uur standaard wanneer het registreren tijd Project, Taak, of Tijd van de Uitgave is, maar de gefilterde Types van Uur van het project toont ook als extra opties.

   * Wanneer de gebruiker geen Type van Uur Standaard heeft en het project heeft geen Gefilterde Types van Uur, slechts tonen de de types van uren van het Project, van de Taak, of van de Tijd van de Uitgave als gebreken afhankelijk van het voorwerp u tijd aan registreert.

   * Wanneer de gebruiker een Type van Uur Standaard heeft en het project heeft geen Gefilterde Types van Uur, de vertoning van de Tijd van het Project, van de Taak, of van de Uitgave als gebreken wanneer het registreren van tijd op de voorwerpen, en geen andere Types van Uur zijn beschikbaar als opties, met inbegrip van het Type van Uur Standaard van de gebruiker.

* Nadat u de Types van Uur aanpast en Beschikbare Types van Uur voor uw gebruiker bepaalt of de Types van Uur voor een project filtreert, bestaan de volgende scenario&#39;s:

   * Wanneer u alle uurtypes voor het Beschikbare gebied van het Type van Uur in het profiel van uw gebruiker selecteerde en de Types van Uur van het project niet worden gefiltreerd, zult u alle beschikbare uurtypes zien wanneer u tijd registreert.
   * Wanneer u slechts een ondergroep van uurtypes voor het Beschikbare gebied van het Type van Uur in het profiel van uw gebruiker selecteerde en de Types van Uur van het project niet worden gefiltreerd, zult u slechts de types van uren van de gebruiker zien wanneer u tijd registreert.
   * Wanneer u alle uurtypes voor het Beschikbare gebied van het Type van Uur in het profiel van uw gebruiker selecteerde en de Types van Uur van het project worden gefiltreerd, zult u slechts de de uurtypes van het project en de standaarduurtypes zoals de Tijd van het Project, de Tijd van de Taak, de Tijd van de Uitgave afhankelijk van het voorwerp zien.
   * Wanneer u slechts een ondergroep van uurtypes voor het Beschikbare gebied van het Type van Uur in het profiel van uw gebruiker selecteerde en de Types van Uur van het project worden gefiltreerd, zult u slechts de uurtypes zien die voor de gebruiker en het project gemeenschappelijk zijn. Als geen uurtypes voor de gebruiker en het project gemeenschappelijk zijn, slechts de standaarduurtypes tonen (de Tijd van het Project, de Tijd van de Taak, de Tijd van de Uitgave).

>[!TIP]
>
>   Als u een ander Type van Uur dan het standaarduurtype voor een voorwerp selecteert, wordt het uurtype kleverig. De volgende keer dat u zich aanmeldt bij hetzelfde object, wordt het type uur automatisch ingesteld op het object dat u het laatst hebt geselecteerd.

