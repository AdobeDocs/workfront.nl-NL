---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: toegang, model, trechter, diagram, niveaus, toestemmingen
navigation-topic: access-levels
title: Ingebouwde toegangsniveaus in Adobe Workfront
description: Elk van de zes ingebouwde toegangsniveaus wordt ontworpen voor een bepaald type van gebruiker, met inbegrip van de Beheerder van het Systeem, de Planner, de Arbeider, de Recensent, de Aanvrager, en Externe Gebruiker. Met deze toegangsniveaus kunt u bepalen welke gebruikers in het systeem kunnen bewerken en weergeven. Als u een aangepast toegangsniveau nodig hebt, kunt u het ingebouwde toegangsniveau kopiëren en de hoeveelheid toegang bepalen die u voor de verschillende Workfront-objecttypen wilt toestaan.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 1bd454246419e199e5cfd0d8d1d73cd30c0b13b1
workflow-type: tm+mt
source-wordcount: '1515'
ht-degree: 0%

---

# Ingebouwde oudere toegangsniveaus in Adobe Workfront

Elk van de zes ingebouwde niveaus van de erfenistoegang worden ontworpen voor een bepaald type gebruiker:

* Systeembeheerder
* Planner
* Worker
* Revisor
* Aanvrager
* Externe gebruiker

Afhankelijk van het oude toegangsniveau zijn maximaal drie instellingen beschikbaar voor de meeste Workfront-objecttypen:

<table style="table-layout:auto">
    <tr>
        <td>Bewerken</td>
        <td>Gebruikers kunnen het Workfront-object maken, bewerken, verwijderen en delen</td>
    </tr>
    <tr>
        <td>Weergave</td>
        <td>Gebruikers kunnen het Workfront-object bekijken en delen</td>
    </tr>
    <tr>
        <td>Geen toegang</td>
        <td>Gebruikers hebben geen toegang tot het Workfront-object</td>
    </tr>
</table>

Als u een douanepanager, de Arbeider, de Vraag, of het toegangsniveau van de Recensent nodig hebt, kunt u het ingebouwde niveau van de erfenistoegang kopiëren en de hoeveelheid toegang bepalen u het voor de diverse objecten van Workfront wilt toestaan. Voor informatie bij het creëren van een niveau van de douanetoegang of het wijzigen van één van de ingebouwde niveaus van de erfenistoegang, zie [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Wij adviseren sterk dat u de ingebouwde niveaus van de erfenistoegang onveranderd laat zodat u naar hen kunt verwijzen nadat u opstelling uw gebruikers.

Voor algemene informatie over deze toegangsniveaus, zie [Overzicht van toegangsniveaus](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Toegangsniveau van systeembeheerder

Dit ingebouwde toegangsniveau dat is gekoppeld aan de licentie voor abonnementen, is ontworpen voor een gebruiker die het Adobe Workfront-systeem beheert. U kunt dit ingebouwde toegangsniveau niet wijzigen.

Gebruikers met het toegangsniveau voor systeembeheerders kunnen alles doen binnen Workfront. Ze kunnen alle Workfront-objecten en informatie die door alle andere gebruikers in Workfront is ingevoerd, weergeven en bewerken.

Zij hebben ook toegang tot het volledige gebied van de Opstelling, waar zij om het even welk plaatsen op het systeemniveau kunnen veranderen. En ze hebben toegang tot alle gebieden in het hoofdmenu ![](assets/main-menu-icon.png).

Zie voor meer informatie [Volledige administratieve toegang verlenen aan een gebruiker](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Toegangsniveau van oudere installer

Dit toegangsniveau is ook gekoppeld aan de licentie voor abonnementen en is bedoeld voor:

* Managers van groepen, teams, projecten, en middelen
* Iedereen die verantwoordelijk is voor het plannen, maken en beheren van taken, projecten, portfolio&#39;s en programma&#39;s
* Iedereen die verantwoordelijk is voor het toewijzen van werk (taken en problemen) aan andere gebruikers
* Gebruikers die rapporten maken en die tijdbladen, werkitems en documenten goedkeuren
* Gebruikers die toegang tot alle gebieden in het hoofdmenu nodig hebben ![](assets/main-menu-icon.png)

U kunt een aangepaste versie van het ingebouwde oudere toegangsniveau van de Planner maken en de mate van toegang bepalen die het toestaat voor de verschillende objecttypen van Workfront. Zie voor meer informatie [Ingebouwde toegangsniveaus in Adobe Workfront](#Customiz) in dit artikel.

Hieronder ziet u de hoogste toegangsinstellingen die beschikbaar zijn voor objecten in het verouderde toegangsniveau van de Planner:

| Workfront-objecttype | Geen toegang | Toegang weergeven | Toegang bewerken |
|---|---|---|---|
| Projecten |   |   | ✓ |
| Taken |   |   | ✓ |
| Problemen |   |   | ✓ |
| Portfolio |   |   | ✓ |
| Programma&#39;s |   |   | ✓ |
| Rapporten (inclusief dashboards en kalenderrapporten) |   |   | ✓ |
| Filters, weergaven en groepen |   |   | ✓ |
| Documenten |   |   | ✓ |
| Gebruikers |   |   | ✓ |
| Sjablonen |   |   | ✓ |
| Financiële gegevens |   |   | ✓ |
| Bronbeheer |   |   | ✓ |
| Scenario Planner |   |   | ✓ (De standaardinstelling is Geen toegang.) |
| Workfront-doelen |   |   | ✓ (De standaardinstelling is Geen toegang.) |

{style="table-layout:auto"}

## Toegangsniveau voor oudere werknemers

Dit toegangsniveau is gekoppeld aan de werklicentie en is bedoeld voor gebruikers die het werk in Workfront uitvoeren. Zij plannen het werk niet; ze maken het af .

Gebruikers met dit toegangsniveau:

* Wordt toegewezen aan werkitems waar ze kunnen bijdragen en waarvan de logtijd kan worden vastgelegd
* Werk en documenten kunnen worden goedgekeurd, maar geen timesheets
* Kan rapporten openen en delen
* Kan communiceren met andere gebruikers in het systeem
* Alle gebieden in het hoofdmenu zijn toegankelijk ![](assets/main-menu-icon.png), maar hun gebied &quot;Gebruikers&quot; heet Teams. In het gebied van Teams, kunnen de gebruikers met dit toegangsniveau slechts teams bekijken die zij tot behoren, samen met het werk dat aan die teams wordt toegewezen.
* Heb beperkte capaciteit om tot voorwerp-zij tot stand te brengen geen projecten, portefeuilles, programma&#39;s, of rapporten kunnen leiden.

U kunt een aangepaste versie maken van het ingebouwde toegangsniveau van de Worker voor oudere gebruikers en de mate van toegang bepalen die dit mogelijk maakt voor de verschillende Workfront-objecttypen. Zie voor meer informatie [Ingebouwde toegangsniveaus in Adobe Workfront](#Customiz) in dit artikel.

Hieronder ziet u de hoogste toegangsinstellingen die beschikbaar zijn voor objecten op het toegangsniveau van Worker:

| Workfront-objecttype | Geen toegang | Toegang weergeven | Toegang bewerken |
|---|---|---|---|
| Projecten |   |   | ✓ (beperkt): gebruikers kunnen het project alleen delen, taken en problemen in het project maken en gegevens bewerken in aangepaste formulieren die er al aan zijn gekoppeld.) |
| Taken |   |   | ✓ |
| Problemen |   |   | ✓ |
| Portfolio |   | ✓ (De standaardinstelling is Geen toegang.) |   |
| Programma&#39;s |   | ✓ (De standaardinstelling is Geen toegang.) |   |
| Rapporten (inclusief dashboards en kalenderrapporten) |   | ✓ |   |
| Filters, weergaven en groepen |   |   | ✓ |
| Documenten |   |   | ✓ |
| Gebruikers |   |   | ✓ |
| Sjablonen | ✓ |   |   |
| Financiële gegevens |   | ✓ (De standaardinstelling is Geen toegang. Met de instelling Weergave kan de gebruiker alleen het gebied Financiën in Projectdetails bekijken.) |   |
| Bronbeheer |   | ✓ |   |
| Scenario Planner |   |   | ✓ (De standaardinstelling is Geen toegang.) |
| Workfront-doelen |   |   | ✓ (De standaardinstelling is Geen toegang.) |

{style="table-layout:auto"}

## Revisor verouderd toegangsniveau

Dit toegangsniveau is gekoppeld aan de Revisielicentie en is ontworpen voor managers die werk aanvragen bij andere gebruikers en die het werk beoordelen en goedkeuren. Dit zijn geen projecteigenaars of teamleden, maar ze hebben toegang tot Workfront nodig om de werkitems te kunnen zien waarop ze toezicht houden.

Een belanghebbende met dit toegangsniveau kan zich bijvoorbeeld aanmelden bij Workfront om deel te nemen aan een doorlopende revisie van marketingmaterialen, werkupdates te bekijken en documenten, goedkeuringen, rapporten en kalenders te beoordelen.

Gebruikers met het toegangsniveau van de Revisor:

* Kan geen werkitems toewijzen of tijdbladen goedkeuren
* Kan aanvragen en documenten openen in het hoofdmenu ![](assets/main-menu-icon.png).
* Heb beperkte capaciteit om tot voorwerp-zij tot stand te brengen geen projecten, portefeuilles, programma&#39;s, of rapporten kunnen leiden.

U kunt een aangepaste versie van het ingebouwde, oudere toegangsniveau van Reviewer maken en bepalen hoeveel toegang er wordt verleend voor de verschillende Workfront-objecttypen. Zie voor meer informatie [Ingebouwde toegangsniveaus in Adobe Workfront](#Customiz) in dit artikel.

Beperkt voor projecten en taken tot het toegangsniveau van de Worker, zijn de hoogste toegangsmontages beschikbaar voor voorwerpen in het de toegangsniveau van de Recensent:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Workfront-objecttype</th> 
   <th>Geen toegang</th> 
   <th>Toegang weergeven</th> 
   <th>Toegang bewerken</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projecten</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Taken</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problemen</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programma's</td> 
   <td> </td> 
   <td>✓ (De standaardinstelling is Geen toegang.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Rapporten (inclusief dashboards en kalenderrapporten)</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Filters, weergaven en groepen</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Documenten</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Gebruikers</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Sjablonen</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Financiële gegevens</td> 
   <td> </td> 
   <td> <p>✓ (De standaardinstelling is Geen toegang. Met de instelling Weergave kan de gebruiker alleen het gebied Financiën in Projectdetails bekijken.)</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bronbeheer</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Scenario Planner </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (De standaardinstelling is Geen toegang.)</td> 
  </tr> 
  <tr> 
   <td>Workfront-doelen </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (De standaardinstelling is Geen toegang.)</td> 
  </tr> 
 </tbody> 
</table>

## Verouderde toegangsniveau aanvragen

Dit toegangsniveau, gekoppeld aan de aanvraaglicentie, is ontworpen voor gebruikers die eenvoudige werkverzoeken indienen en ontvangen in Workfront. Deze zijn standaard beperkt tot het gebied Verzoeken.

Bijvoorbeeld, kan een gebruiker kwesties aan de rij van het de hulpbureauverzoek van uw organisatie registreren.

Gebruikers met dit toegangsniveau:

* Kan verzoeken indienen en deze aanvragen bijwerken
* Documenten uploaden en goedkeuren
* Kan de status van de verzonden problemen bekijken
* Kan niet toewijzen aan werkitems
* Alleen toegang tot aanvragen via het hoofdmenu ![](assets/main-menu-icon.png). Voor meer informatie over verzoekrijen, zie [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

U kunt een aangepaste versie van het ingebouwde oudere toegangsniveau van de Vraag tot stand brengen en de hoeveelheid toegang bepalen het voor de diverse objecten van Workfront toelaat. Zie voor meer informatie [Ingebouwde toegangsniveaus in Adobe Workfront](#Customiz) in dit artikel.

Hieronder ziet u de hoogste toegangsinstellingen die beschikbaar zijn voor objecten op het toegangsniveau van de aanvrager:

| Workfront-objecttype | Geen toegang | Toegang weergeven | Toegang bewerken |
|---|---|---|---|
| Project |   | ✓ (Alleen de pagina Projectdetails) |   |
| Taak |   | ✓ (Alleen de pagina Details) |   |
| Probleem |   |   | ✓ |
| Portfolio | ✓ |   |   |
| Programma&#39;s | ✓ |   |   |
| Rapporten (inclusief dashboards en kalenderrapporten) |   | ✓ (Alleen de pagina Details) |   |
| Filters, weergaven en groepen |   |   | ✓ |
| Document |   |   | ✓ |
| Gebruiker |   | ✓ |   |
| Sjabloon | ✓ |   |   |
| Financiële gegevens | ✓ |   |   |
| Bronbeheer | ✓ |   |   |
| Scenario Planner | ✓ |   |   |
| Workfront-doelen |   |   | ✓ (De standaardinstelling is Geen toegang.) |

{style="table-layout:auto"}

## Toegangsniveau externe gebruiker

Dit toegangsniveau is niet gekoppeld aan een betaalde Workfront-licentie. Het is het meest beperkende toegangsniveau, dat hoofdzakelijk voor medewerkers zoals externe adviseurs wordt ontworpen die zich niet bij Workfront aanmelden, maar moet, af en toe documenten herzien downloaden of bekijken.

Workfront-gebruikers kunnen taken toewijzen aan externe gebruikers, ook al kunnen externe gebruikers zich niet aanmelden bij het systeem. Maar wij raden ons hiertegen aan, omdat dat werk in het systeem onopgelost zou blijven.

Gebruikers met het toegangsniveau voor externe gebruikers:

* Alleen documenten en kalenderrapporten weergeven die met hen worden gedeeld
* Zie gebruikers die documenten en kalenderrapporten met hen delen
* De documenten goedkeuren die met hen worden gedeeld

U kunt dit toegangsniveau niet wijzigen.

>[!IMPORTANT]
>
>De externe Gebruiker is beschikbaar slechts als de optie &quot;met mensen zonder de rekeningen van Workfront samenwerken door hun e-mailadres te gebruiken&quot;in het gebied van de Voorkeur van het Systeem in Opstelling wordt toegelaten. Zie voor meer informatie [Beveiligingsvoorkeuren voor het systeem configureren](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

Hieronder ziet u de hoogste toegangsinstellingen die beschikbaar zijn voor objecten op het toegangsniveau van de externe gebruiker.

| Workfront-objecttype | Geen toegang | Toegang weergeven | Toegang bewerken |
|---|---|---|---|
| Project | ✓ |   |   |
| Taak | ✓ | ✓ |   |
| Probleem | ✓ |   |   |
| Portfolio | ✓ |   |   |
| Programma&#39;s | ✓ |   |   |
| Rapporten (inclusief dashboards en kalenderrapporten) |   | ✓ (alleen voor kalenderverslagen; geen mogelijkheid om rapporten te delen) |   |
| Filters, weergaven en groepen | ✓ |   |   |
| Document |   | ✓ (zonder de mogelijkheid om documenten te delen) |   |
| Gebruiker |   | ✓ |   |
| Sjabloon | ✓ |   |   |
| Financiële gegevens | ✓ |   |   |
| Bronbeheer | ✓ |   |   |
| Scenario Planner | ✓ |   |   |
| Workfront-doelen | ✓ |   |   |
