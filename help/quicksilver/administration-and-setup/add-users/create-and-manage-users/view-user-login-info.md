---
title: Aanmeldingsgegevens gebruiker weergeven
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: U kunt zien hoe vaak de gebruikers zich bij Workfront aanmelden, evenals de laatste tijd zij het programma hebben geopend, door erop te wijzen dat u deze informatie in de mening van een lijst van gebruikers, of in een rapport voor gebruikers wilt omvatten.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: 1c11be2d6de471bf456107b5c86a599766583f74
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# Aanmeldingsgegevens van gebruikers weergeven

U kunt zien hoe vaak de gebruikers zich bij Adobe Workfront aanmelden, evenals de laatste tijd zij het programma hebben geopend, door erop te wijzen dat u deze informatie in de mening van een lijst van gebruikers, of in een rapport voor gebruikers wilt omvatten.

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
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p><p>of</p><p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau voor systeembeheerders. </li> 
     <li> <p><b> Gebruikers </b> het plaatsen in uw toegangsniveau dat aan <b> wordt gevormd geeft </b> toegang uit, met <b> creeert </b> en minstens één van de twee <b> die gebruikers Admin </b> opties onder <b> worden toegelaten verfijnen uw montages </b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Van deze twee opties, als <b> Admin van de Gebruiker (de Gebruikers van de Groep) </b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hoe Workfront aanmeldingsgegevens registreert

Workfront registreert de volgende informatie over gebruikers die zich aanmelden bij het systeem:

* **Login Telling**: Workfront telt een gebruiker die aan de toepassing het programma opent eens om de 24 uur. Als een gebruiker zich meerdere keren aanmeldt met verschillende browsers, computers of mobiele apparaten, telt Workfront alle logins die zich op één dag hebben voorgedaan als één aanmelding. Het aantal aanmelding bevat gegevens die beginnen bij het maken van de gebruiker.
* **Laatste Login Datum**: De laatste datum toen een gebruiker het programma opende. De datum van elke aanmelding van een browser, mobiel apparaat of andere toepassingen wordt in dit veld vastgelegd.

Aanmelden bij Workfront op een van de volgende manieren telt als aanmelding bij Workfront:

* De Workfront-webtoepassing
* De Workfront Mobile-apps (iOS- of Android-apparaten)
* Elke ondersteunde Workfront-integratie met een andere toepassing van derden (zoals Slack)
* Elke aangepaste integratie tussen Workfront en een andere toepassing van derden.
* De Workfront API

  >[!NOTE]
  >
  >Aanmelden bij Workfront via de Workfront API is alleen beschikbaar voor organisaties die nog niet zijn aangemeld bij het Adobe Business Platform.

## Gebruiksgegevens weergeven in een gebruikerslijst of rapport

U kunt het Aantal Login en de Laatste gebieden van de Datum van Aanmelding in de mening van een lijst van gebruikers, of in een rapport voor gebruikers tonen.\
Voor meer informatie over het creëren van een rapport, zie [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

Gebruiksinformatie weergeven in de weergave van een lijst met gebruikers:

1. Ga naar een lijst met gebruikers in Workfront.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. Klik **toevoegen Kolom** dichtbij de laag-juiste hoek van het scherm.
1. In **toon in dit kolom** gebied, begin **Login Telling** te typen, dan het te selecteren wanneer het in de lijst onder **Gebruiker** verschijnt.

1. Klik **toevoegen opnieuw Kolom**.
1. In **toon in het kolom** gebied, begin **Laatste Login Datum** te typen, dan het te selecteren wanneer het in de lijst onder **Gebruiker** verschijnt.

1. (Facultatief) klik **Geavanceerde Opties**, dan selecteren a **Formaat van het Gebied** van het drop down menu om de tijd of de dag van de week van laatste login in uw kolom te omvatten.

1. Klik **sparen Mening**.\
   De weergave bevat informatie over het aantal keren dat de gebruikers zich hebben aangemeld en het tijdstip waarop ze zich voor het laatst hebben aangemeld.
