---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: toegang, model, funnel, diagram, niveaus, toestemmingen
navigation-topic: access-levels
title: Ingebouwde toegangsniveaus (verouderd)
description: Elk van de zes huidige ingebouwde toegangsniveaus wordt ontworpen voor een bepaald type van gebruiker, met inbegrip van de Beheerder van het Systeem, de Planner, de Arbeider, de Recensent, de Aanvrager, en Externe Gebruiker. Met deze toegangsniveaus kunt u bepalen welke gebruikers in het systeem kunnen bewerken en weergeven. Als u een aangepast toegangsniveau nodig hebt, kunt u een ingebouwd toegangsniveau kopiëren en dit wijzigen op basis van de hoeveelheid toegang die u voor de verschillende Workfront-objecttypen wilt toestaan.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '1656'
ht-degree: 0%

---

# Ingebouwde toegangsniveaus (verouderd)

<!--Audited: 01/2024-->

>[!NOTE]
>
>De informatie in dit artikel verwijst naar de oudere toegangsniveaus. Voor informatie over de huidige toegangsniveaus, zie [&#x200B; Nieuw overzicht van toegangsniveaus &#x200B;](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).


Elk van de zes huidige ingebouwde toegangsniveaus wordt ontworpen voor een bepaald type van gebruiker. Met deze toegangsniveaus kunt u bepalen welke gebruikers in het systeem kunnen bewerken en weergeven.

Elk van de zes ingebouwde toegangsniveaus worden ontworpen voor de volgende types van gebruikers:

* Systeembeheerder
* Planner
* Worker
* Revisor
* Aanvrager
* Externe gebruiker

Afhankelijk van het toegangsniveau zijn maximaal drie instellingen beschikbaar voor de meeste Workfront-objecttypen:

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

Als u een douanepanager, de Arbeider, de Vraag, of het toegangsniveau van de Recensent nodig hebt, kunt u het ingebouwde toegangsniveau kopiëren en de hoeveelheid toegang bepalen u het voor de diverse objecten van Workfront wilt toestaan.

>[!TIP]
>
>U kunt de toegangsniveaus van de Systeembeheerder of de externe gebruiker niet wijzigen.

Voor informatie bij het creëren van een niveau van de douanetoegang of het wijzigen van één van de ingebouwde toegangsniveaus, zie [&#x200B; douanetoegangsniveaus &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) creëren en wijzigen.

>[!IMPORTANT]
>
>Wij adviseren sterk dat u de ingebouwde toegangsniveaus onveranderd laat zodat u naar hen kunt verwijzen nadat u opstelling uw gebruikers.

Voor algemene informatie over deze toegangsniveaus, zie [&#x200B; overzicht van de Niveaus van de Toegang &#x200B;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Toegangsniveau van systeembeheerder

Het ingebouwde toegangsniveau van de Beheerder van het Systeem, verbonden aan de vergunning van het Plan, wordt ontworpen voor een gebruiker die het systeem van Adobe Workfront beheert. U kunt dit ingebouwde toegangsniveau niet wijzigen.

Gebruikers met het toegangsniveau voor systeembeheerders kunnen alles doen in Workfront. Ze kunnen alle Workfront-objecten en informatie die door alle andere gebruikers in Workfront is ingevoerd, weergeven en bewerken.

Zij hebben ook volledige toegang tot het gebied van de Opstelling, waar zij om het even welk plaatsen op het systeemniveau kunnen veranderen. En zij kunnen tot alle gebieden in het Belangrijkste Menu ![&#x200B; Belangrijkste menupictogram &#x200B;](assets/main-menu-icon.png) of tot het Belangrijkste het menupictogram van het Menu ![&#x200B; toegang hebben &#x200B;](assets/main-menu-icon.png), als beschikbaar.

Voor meer informatie, zie [&#x200B; een gebruiker volledige administratieve toegang verlenen &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Toegangsniveau van planner

Het toegangsniveau van de Planner is ook gekoppeld aan de licentie voor abonnementen en is bedoeld voor:

* Managers van groepen, teams, projecten, en middelen
* Iedereen die verantwoordelijk is voor het plannen, maken en beheren van taken, projecten, portfolio&#39;s en programma&#39;s
* Iedereen die verantwoordelijk is voor het toewijzen van werk (taken en problemen) aan andere gebruikers
* Gebruikers die rapporten maken en die tijdbladen, werkitems en documenten goedkeuren
* Gebruikers die toegang tot alle gebieden in het Belangrijkste het menupictogram van het Menu ![&#x200B; Belangrijkste &#x200B;](assets/main-menu-icon.png) of het Belangrijkste het menupictogram ![&#x200B; Belangrijkste &#x200B;](assets/main-menu-icon.png) nodig hebben, als beschikbaar

U kunt een aangepaste versie van het ingebouwde toegangsniveau van de Planner maken en de mate van toegang bepalen die het toestaat voor de verschillende Workfront-objecttypen. Voor meer informatie, zie [&#x200B; douanetoegangsniveaus &#x200B;](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) creëren en wijzigen.

Hieronder ziet u de hoogste toegangsinstellingen die beschikbaar zijn voor objecten in het toegangsniveau van de Planner:

| Workfront-objecttype | Geen toegang | Toegang weergeven | Toegang bewerken |
|---|---|---|---|
| Projecten |   |   | ✓ |
| Taken |   |   | ✓ |
| Problemen |   |   | ✓ |
| Portfolio&#39;s |   |   | ✓ |
| Programma&#39;s |   |   | ✓ |
| Rapporten, dashboards en Kalenders |   |   | ✓ |
| Filters, Weergaven en Groepen |   |   | ✓ |
| Documenten |   |   | ✓ |
| Gebruikers |   |   | ✓ |
| Teams |   |   | ✓ |
| Sjablonen |   |   | ✓ |
| Financiële gegevens |   |   | ✓ |
| Bronbeheer |   |   | ✓ |
| Scenario Planner |   |   | ✓ (Standaard is Geen toegang ingesteld.) |
| Workfront-doelen |   |   | ✓ (Standaard is Geen toegang ingesteld.) |

{style="table-layout:auto"}

## Toegangsniveau voor werknemers

Het toegangsniveau van de Worker is gekoppeld aan de werklicentie en is ontworpen voor gebruikers die het werk in Workfront uitvoeren. Ze plannen het werk niet, ze voltooien het.

Gebruikers met dit toegangsniveau:

* Wordt toegewezen aan werkitems waar ze kunnen bijdragen en waarvan de logtijd kan worden vastgelegd
* Werk en documenten kunnen worden goedgekeurd, maar geen timesheets
* Kan rapporten openen en delen
* Kan communiceren met andere gebruikers in het systeem
* Kan tot alle gebieden in het Belangrijkste het menupictogram van het Menu ![&#x200B; Belangrijkste &#x200B;](assets/main-menu-icon.png) of tot het Belangrijkste het menupictogram van het Menu ![&#x200B; toegang hebben &#x200B;](assets/main-menu-icon.png), als beschikbaar, en hun &quot;Gebruikers&quot;gebied wordt genoemd Teams. In het gebied van Teams, kunnen de gebruikers met dit toegangsniveau slechts teams bekijken die zij tot behoren, samen met het werk dat aan die teams wordt toegewezen.
* Heb beperkte capaciteit om tot voorwerp-zij tot stand te brengen geen projecten, portefeuilles, programma&#39;s, of rapporten kunnen leiden.

U kunt een aangepaste versie van het ingebouwde toegangsniveau van de Worker maken en de mate van toegang bepalen die dit toestaat voor de verschillende Workfront-objecttypen. Voor meer informatie, zie [&#x200B; douanetoegangsniveaus &#x200B;](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) creëren en wijzigen.

Hieronder ziet u de hoogste toegangsinstellingen die beschikbaar zijn voor objecten op het toegangsniveau van Worker:

| Workfront-objecttype | Geen toegang | Toegang weergeven | Toegang bewerken |
|---|---|---|---|
| Projecten |   |   | ✓ (Beperkt: gebruikers kunnen het project alleen delen, er taken en problemen in maken en gegevens bewerken in aangepaste formulieren die er al aan zijn gekoppeld.) |
| Taken |   |   | ✓ |
| Problemen |   |   | ✓ |
| Portfolio&#39;s |   | ✓ (Standaard is Geen toegang ingesteld.) |   |
| Programma&#39;s |   | ✓ (Standaard is Geen toegang ingesteld.) |   |
| Rapporten, dashboards en Kalenders |   | ✓ |   |
| Filters, Weergaven en Groepen |   |   | ✓ |
| Documenten |   |   | ✓ |
| Gebruikers |   |   | ✓ |
| Teams |   |   | ✓ (beperkte toegang) |
| Sjablonen | ✓ |   |   |
| Financiële gegevens |   | ✓ (De standaardinstelling is Geen toegang. Met de instelling Weergave kan de gebruiker alleen het gebied Financiën bekijken   in projectdetails.) |   |
| Bronbeheer |   | ✓ |   |
| Scenario Planner |   |   | ✓ (Standaard is Geen toegang ingesteld.) |
| Workfront-doelen |   |   | ✓ (Standaard is Geen toegang ingesteld.) |

{style="table-layout:auto"}

## Toegangsniveau van revisor

Het toegangsniveau van de Revisor, gekoppeld aan de Revisiewer-licentie, is ontworpen voor managers die werk aanvragen bij andere gebruikers en die het werk beoordelen en goedkeuren. Dit zijn geen projecteigenaars of teamleden, maar ze hebben toegang tot Workfront nodig om de werkitems te kunnen zien waarop ze toezicht houden.

Een belanghebbende met dit toegangsniveau kan zich bijvoorbeeld aanmelden bij Workfront om deel te nemen aan een doorlopende revisie van marketingmaterialen, werkupdates te bekijken en documenten, goedkeuringen, rapporten en kalenders te beoordelen.

Gebruikers met het toegangsniveau van de Revisor:

* Kan geen werkitems toewijzen of tijdbladen goedkeuren
* Kan tot de gebieden van Verzoeken en van Documenten in het Belangrijkste Menu ![&#x200B; Belangrijkste menupictogram &#x200B;](assets/main-menu-icon.png) of het Belangrijkste het menupictogram van het Menu ![&#x200B; toegang hebben &#x200B;](assets/main-menu-icon.png), als beschikbaar
* Heb beperkte capaciteit om tot voorwerp-zij tot stand te brengen geen projecten, portefeuilles, programma&#39;s, of rapporten kunnen leiden.

U kunt een aangepaste versie van het ingebouwde toegangsniveau van Reviewer maken en bepalen hoeveel toegang er wordt verleend voor de verschillende Workfront-objecttypen. Voor meer informatie, zie [&#x200B; douanetoegangsniveaus &#x200B;](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) creëren en wijzigen.

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
   <td>Portfolio's</td> 
   <td> </td> 
   <td>✓ (De standaardinstelling is Geen toegang.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programma's</td> 
   <td> </td> 
   <td>✓ (De standaardinstelling is Geen toegang.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Rapporten, dashboards, kalenders</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Filters, Weergaven en Groepen</td> 
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
   <td>Teams</td> 
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
   <td> <p>✓ (De standaardinstelling is Geen toegang. Met de instelling Weergave kan de gebruiker alleen het gebied Financiën bekijken   in projectdetails.)</p> </td> 
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

## Toegangsniveau aanvrager

Het toegangsniveau voor de aanvrager dat is gekoppeld aan de aanvraaglicentie, is ontworpen voor gebruikers die eenvoudige werkverzoeken indienen en ontvangen in Workfront. Deze zijn standaard beperkt tot het gebied Verzoeken.

Bijvoorbeeld, kan een gebruiker kwesties aan de rij van het de hulpbureauverzoek van uw organisatie registreren.

Gebruikers met dit toegangsniveau:

* Kan verzoeken indienen en deze aanvragen bijwerken
* Documenten uploaden en goedkeuren
* Kan de status van de verzonden problemen bekijken
* Kan niet toewijzen aan werkitems
* Kan verzoeken slechts van het gebied van Verzoeken in het Belangrijkste het menupictogram van het Menu ![&#x200B; Belangrijkste &#x200B;](assets/main-menu-icon.png) of het Belangrijkste het menupictogram van het Menu ![&#x200B; toegang hebben &#x200B;](assets/main-menu-icon.png), als beschikbaar. Voor meer informatie over verzoekrijen, zie [&#x200B; een Rij van het Verzoek &#x200B;](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.

U kunt een aangepaste versie van het ingebouwde toegangsniveau voor de aanvrager maken en bepalen hoeveel toegang er wordt verleend voor de verschillende Workfront-objecttypen. Voor meer informatie, zie [&#x200B; douanetoegangsniveaus &#x200B;](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) creëren en wijzigen.

Hieronder ziet u de hoogste toegangsinstellingen die beschikbaar zijn voor objecten op het toegangsniveau van de aanvrager:

| Workfront-objecttype | Geen toegang | Toegang weergeven | Toegang bewerken |
|---|---|---|---|
| Project |   | ✓ (Alleen de pagina Projectdetails) |   |
| Taak |   | ✓ (Alleen de pagina Taakdetails) |   |
| Probleem |   |   | ✓ |
| Portfolio&#39;s | ✓ |   |   |
| Programma&#39;s | ✓ |   |   |
| Rapporten, dashboards en Kalenders |   | ✓ |   |
| Filters, weergaven en groepen |   |   | ✓ |
| Documenten |   |   | ✓ |
| Gebruiker |   | ✓ |   |
| Teams |   | ✓ |   |
| Sjablonen | ✓ |   |   |
| Financiële gegevens | ✓ |   |   |
| Bronbeheer | ✓ |   |   |
| Scenario Planner | ✓ |   |   |
| Workfront-doelen |   |   | ✓ (Standaard is Geen toegang ingesteld.) |

{style="table-layout:auto"}

## Toegangsniveau externe gebruiker

Het toegangsniveau voor externe gebruikers is niet gekoppeld aan een betaalde Workfront-licentie. Het is het meest beperkende toegangsniveau, dat hoofdzakelijk voor medewerkers zoals externe adviseurs wordt ontworpen die zich niet bij Workfront aanmelden, maar moet, af en toe documenten herzien downloaden of bekijken.

Workfront-gebruikers kunnen taken toewijzen aan externe gebruikers, ook al kunnen externe gebruikers zich niet aanmelden bij het systeem. Wij raden echter niet aan taken en problemen toe te wijzen aan externe gebruikers, omdat dat werk in het systeem onopgelost blijft.

Gebruikers met het toegangsniveau voor externe gebruikers:

* Alleen documenten en kalenderrapporten weergeven die met hen worden gedeeld
* Zie de gebruikers die documenten en kalenderrapporten met hen delen
* Kan de met hen gedeelde documenten goedkeuren

U kunt dit toegangsniveau niet wijzigen.

>[!IMPORTANT]
>
>De externe Gebruiker is beschikbaar slechts als de optie &quot;met mensen zonder de rekeningen van Workfront samenwerken door hun e-mailadres te gebruiken&quot;in het gebied van de Voorkeur van het Systeem in Opstelling wordt toegelaten. Voor meer informatie, zie [&#x200B; de voorkeur van de systeemveiligheid &#x200B;](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md) vormen.

Hoewel deze instellingen niet zichtbaar zijn in het gebied Toegangsniveaus voor het toegangsniveau van de externe gebruiker, heeft een gebruiker met deze toegang de volgende hoogste toegang tot de objecttypen van Workfront:

| Workfront-objecttype | Geen toegang | Toegang weergeven | Toegang bewerken |
|---|---|---|---|
| Project | ✓ |   |   |
| Taak | ✓ | |   |
| Probleem | ✓ |   |   |
| Portfolio&#39;s | ✓ |   |   |
| Programma&#39;s | ✓ |   |   |
| Rapporten, dashboards en Kalenders |   | ✓ (Alleen voor kalenderrapporten; geen rapporten kunnen worden gedeeld) |   |
| Filters, Weergaven en Groepen | ✓ |   |   |
| Documenten |   | ✓ (zonder de mogelijkheid om documenten te delen) |   |
| Gebruikers |   | ✓ |   |
| Teams |   | ✓ |   |
| Sjablonen | ✓ |   |   |
| Financiële gegevens | ✓ |   |   |
| Bronbeheer | ✓ |   |   |
| Scenario Planner | ✓ |   |   |
| Workfront-doelen | ✓ |   |   |
