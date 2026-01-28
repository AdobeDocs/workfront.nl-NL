---
title: Overzicht van toegangsniveaus
user-type: administrator
content-type: reference
product-area: system-administration
keywords: toegang,niveau,systeem,beheerder,standaard,licht,contribuant
navigation-topic: access-levels
description: Elke gebruiker moet een toegangsniveau hebben om zich aan te melden en in Workfront te werken. Met het toegangsniveau kunt u bepalen wat een gebruiker kan zien en doen met bepaalde Workfront-objecten en -gebieden.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d297d8a4-5a4e-418f-983a-19545aeb0668
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '1747'
ht-degree: 0%

---

# Overzicht van toegangsniveaus

>[!NOTE]
>
>De informatie in dit artikel verwijst naar de huidige toegangsniveaus. Voor informatie over de niveaus van de erfenistoegang, zie [ overzicht van de niveaus van de Toegang ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Als beheerder van Adobe Workfront, wijst u een toegangsniveau aan een gebruiker voor twee doeleinden toe:

* Elke gebruiker moet een toegangsniveau hebben om zich aan te melden en in Workfront te werken.
* Met het toegangsniveau kunt u bepalen wat een gebruiker kan zien en doen met bepaalde Workfront-objecten en -gebieden.

## Nieuwe ingebouwde toegangsniveaus in Adobe Workfront {#built-in-access}

Workfront heeft vijf nieuwe ingebouwde toegangsniveaus:

* Systeembeheerder
* Standard
* Licht
* Medewerker
* Extern

Afhankelijk van het toegangsniveau zijn maximaal drie machtigingen beschikbaar voor de meeste Workfront-objecttypen:

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

Als u een aangepast toegangsniveau nodig hebt, kunt u het ingebouwde toegangsniveau kopiëren en de hoeveelheid toegang aanpassen die u voor de verschillende Workfront-objecttypen wilt gebruiken. Voor informatie bij het creëren van een niveau van de douanetoegang, zie [ tot douanetoegangsniveaus ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

>[!IMPORTANT]
>
>Wij adviseren sterk dat u de ingebouwde toegangsniveaus onveranderd laat zodat u naar hen kunt verwijzen nadat u opstelling uw gebruikers.

### Toegangsniveau van systeembeheerder

Dit ingebouwde toegangsniveau is gekoppeld aan de standaardlicentie en is ontworpen voor een gebruiker die het Adobe Workfront-systeem beheert. U kunt dit ingebouwde toegangsniveau niet wijzigen.

Gebruikers met het toegangsniveau voor systeembeheerders kunnen alles doen in Workfront. Ze kunnen alle Workfront-objecten en informatie die door alle andere gebruikers in Workfront is ingevoerd, weergeven en bewerken.

Zij hebben ook toegang tot het volledige gebied van de Opstelling, waar zij om het even welk plaatsen op het systeemniveau kunnen veranderen, en zij kunnen tot alle gebieden in het Belangrijkste Menu toegang hebben.

Voor meer informatie, zie [ een gebruiker volledige administratieve toegang verlenen ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### Standaardtoegangsniveau

Dit toegangsniveau is ook gekoppeld aan de standaardlicentie en is bedoeld voor gebruikers die:

* Alle projecten op één locatie plannen, maken en traceren
* Automatische routinematige processen
* Bronnen beheren
* Bijhouden en samenwerken aan verzoeken
* Spoor en rapporteer de projectfinanciën
* Kickoff binnenkomende werkverzoeken
* Samenwerken aan projecten, taken en problemen

>[!NOTE]
>
>U kunt een aangepaste versie van het standaard ingebouwde toegangsniveau maken en de mate van toegang aanpassen die dit toestaat voor de verschillende Workfront-objecttypen. Voor informatie bij het creëren van een niveau van de douanetoegang, zie [ tot douanetoegangsniveaus ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

#### **de details van de Toegang**

Hieronder ziet u de hoogste toegangsinstellingen die beschikbaar zijn voor objecten op het niveau Standaard:

| Workfront-objecttype | Geen toegang | Toegang weergeven | Toegang bewerken |
|---|---|---|---|
| Projecten |   |   | ✓ |
| Taken |   |   | ✓ |
| Problemen |   |   | ✓ |
| Portfolio&#39;s |   |   | ✓ |
| Programma&#39;s |   |   | ✓ |
| Rapporten (inclusief dashboards en kalenderrapporten) |   |   | ✓ |
| Filters, weergaven en groepen |   |   | ✓ |
| Documenten |   |   | ✓ |
| Gebruikers |   |   | ✓ |
| Sjablonen |   |   | ✓ |
| Financiële gegevens |   |   | ✓ |
| Bronbeheer |   |   | ✓ |
| Scenario Planner |   |   | ✓ (Standaard is Geen toegang ingesteld.) |
| Doelen |   |   | ✓ |

{style="table-layout:auto"}

### Lichttoegangsniveau

Dit toegangsniveau is gekoppeld aan de Lichte licentie en is ontworpen voor gebruikers die:

* Alle items en updates weergeven die zijn gekoppeld aan werk
* Projecten, taken en problemen goedkeuren
* dashboards en rapporten weergeven
* De tijd van het spoor op projecten, taken, en kwesties en keurt timeshesheets goed
* Problemen maken en beheren

Gebruikers met het toegangsniveau Licht:

* Kan aan werkitems worden toegewezen, maar deze kunnen niet worden voltooid.
* Kan aanvragen en documenten openen in het hoofdmenu.
* Heb beperkte capaciteit om tot voorwerp-zij tot stand te brengen geen projecten, portefeuilles, programma&#39;s, of rapporten kunnen leiden.
* Kan tijd op het projectniveau slechts registreren wanneer Edit toegang wordt toegelaten. Ze kunnen geen projecten maken, bewerken, verwijderen of delen.

>[!NOTE]
>
>U kunt een aangepaste versie maken van het ingebouwde toegangsniveau Licht en de mate van toegang aanpassen die dit toestaat voor de verschillende Workfront-objecttypen. Voor informatie bij het creëren van een niveau van de douanetoegang, zie [ tot douanetoegangsniveaus ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

#### **de details van de Toegang**

Hieronder ziet u de hoogste toegangsinstellingen die beschikbaar zijn voor objecten in het toegangsniveau Licht:

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
   <td> </td> 
   <td>✓ (voor logboektijd op het projectniveau)</td> 
  </tr> 
  <tr> 
   <td>Taken</td> 
   <td> </td> 
   <td></td> 
   <td>✓ (beperkt)</td> 
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
   <td></td> 
   <td> <p>✓ (de standaardinstelling is Geen toegang)</p> </td> 
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
   <td>Doelen </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (De standaardinstelling is Geen toegang)</td> 
 </tbody> 
</table>

### Toegangsniveau van contribuant

Dit toegangsniveau is gekoppeld aan de bijdragelicentie en is bedoeld voor gebruikers die:

* Verzoeken verzenden
* Aanvragen bijhouden
* Aanvragen voor bijwerken en controleren
* Aanvragen goedkeuren

Gebruikers met dit ingebouwde toegangsniveau:

* Kan verzoeken indienen en deze aanvragen bijwerken
* Documenten uploaden en goedkeuren
* Kan projecten, taken en problemen goedkeuren

  >[!NOTE]
  >
  >Medewerkers kunnen deelnemen aan goedkeuringen, maar hebben geen toegang tot het tabblad Goedkeuringen om goedkeuringsprocessen te bekijken of te beheren.

* Kan de status van de verzonden problemen bekijken
* Kan worden toegewezen aan werkitems maar kan deze niet voltooien
* U hebt alleen toegang tot aanvragen via het hoofdmenu. Voor meer informatie over verzoekrijen, zie [ een Rij van het Verzoek ](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.

>[!NOTE]
>
>U kunt een aangepaste versie van het ingebouwde toegangsniveau van de Medewerker maken en de mate van toegang aanpassen die het toestaat voor de verschillende Workfront-objecttypen. Voor informatie bij het creëren van een niveau van de douanetoegang, zie [ tot douanetoegangsniveaus ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

#### **de details van de Toegang**

Hieronder ziet u de hoogste toegangsinstellingen die beschikbaar zijn voor objecten op het toegangsniveau van de Contribute-medewerker:

| Workfront-objecttype | Geen toegang | Toegang weergeven | Toegang bewerken |
|---|---|---|---|
| Project |   | ✓ (beperkt) |   |
| Taak |   | ✓ (beperkt) |   |
| Probleem |   |   | ✓ |
| Portfolio&#39;s |   | ✓ |   |
| Programma&#39;s |   | ✓ |   |
| Rapporten (inclusief dashboards en kalenderrapporten) |   | ✓ (Alleen het tabblad Details) |   |
| Filters, weergaven en groepen |   |   | ✓ |
| Document |   |   | ✓ |
| Gebruiker |   | ✓ |   |
| Teams |   | ✓ |   |
| Sjablonen | ✓ |   |   |
| Financiële gegevens | ✓ |   |   |
| Bronbeheer | ✓ |   |   |
| Scenario Planner | ✓ |   |   |
| Doelen |   |   | ✓ (De standaardinstelling is Geen toegang) |

{style="table-layout:auto"}

>[!IMPORTANT]
>
>Vanaf de release 24.7 hebben contribuanten standaard toegang tot programma&#39;s en portfolio&#39;s.
>
> 
>Medewerkers die vóór de release 24.7 zijn geactiveerd, hebben standaard nog steeds geen toegang tot programma&#39;s en portfolio&#39;s. U kunt de toegang van de gebruiker tot de weergave indien nodig handmatig bijwerken.

### Toegangsniveau externe gebruiker

Dit toegangsniveau is niet gekoppeld aan een betaalde Workfront-licentie. Het is het meest restrictieve toegangsniveau, dat hoofdzakelijk voor medewerkers zoals externe adviseurs wordt ontworpen die zich niet bij Workfront aanmelden, maar moet, af en toe documenten herzien downloaden of bekijken.

Gebruikers met het toegangsniveau voor externe gebruikers:

* Alleen documenten en kalenderrapporten weergeven die met hen worden gedeeld
* Gebruikers weergeven die documenten en kalenderrapporten met hen delen
* De documenten goedkeuren die met hen worden gedeeld

Externe gebruikers kunnen niet worden toegewezen aan werkitems.

U kunt dit toegangsniveau niet wijzigen.

>[!IMPORTANT]
>
>De externe Gebruiker is beschikbaar slechts als de optie &quot;met mensen zonder de rekeningen van Workfront samenwerken door hun e-mailadres te gebruiken&quot;in het gebied van de Voorkeur van het Systeem in Opstelling wordt toegelaten. Voor meer informatie, zie [ de voorkeur van de systeemveiligheid ](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md) vormen.

#### **de details van de Toegang**

Hieronder ziet u de hoogste toegangsinstellingen die beschikbaar zijn voor objecten op het toegangsniveau van de externe gebruiker.

| Workfront-objecttype | Geen toegang | Toegang weergeven | Toegang bewerken |
|---|---|---|---|
| Project | ✓ |   |   |
| Taak | ✓ |   |   |
| Probleem | ✓ |   |   |
| Portfolio&#39;s | ✓ |   |   |
| Programma&#39;s | ✓ |   |   |
| Rapporten (inclusief dashboards en kalenderrapporten) |   | ✓ (Alleen voor kalenderrapporten; geen rapporten kunnen worden gedeeld) |   |
| Filters, weergaven en groepen | ✓ |   |   |
| Document |   | ✓ (kan geen documenten delen) |   |
| Gebruiker |   | ✓ |   |
| Teams | ✓ |   |   |
| Sjablonen | ✓ |   |   |
| Financiële gegevens | ✓ |   |   |
| Bronbeheer | ✓ |   |   |
| Scenario Planner | ✓ |   |   |
| Doelen | ✓ |   |   |


## Hoe de toegangsniveaus en de toestemmingen samenwerken

De niveaus van de toegang bepalen wat de gebruikers kunnen zien en doen met algemene objecten types en gebieden in het systeem, zoals projecten, taken, en kwesties. De toestemmingen bepalen wat u tot op specifieke voorwerpen toegang hebt die door andere mensen in het systeem als een project worden gecreeerd om een marketing campagne in werking te stellen.

In de volgende tabel wordt de algemene toegang van een gebruiker tot objecten (gedefinieerd door het toegangsniveau van de gebruiker) tot machtigingen voor een specifiek gezamenlijk object vergeleken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>Toegangsniveau </th> 
   <th>Machtigingen </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Door een Workfront-beheerder toegekend op het toegangsniveau van een gebruiker</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Toegewezen door een gebruiker die een object op objectniveau deelt</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Overgenomen van een gezamenlijk object met een hogere positie 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

De activiteiten een gebruiker met een voorwerp kan doen worden bepaald door een combinatie van hun toegangsniveau en de toestemmingen die aan hen worden gegeven.

![ het modelhiërarchie van de Veiligheid ](assets/security-model-hierachy-copy.png)

### Rechten verlenen via het delen van objecten

Gebruikers krijgen toegang tot afzonderlijke objecten wanneer andere gebruikers bepaalde machtigingen voor die objecten delen en verlenen.

>[!NOTE]
>
>* Als een gebruiker een object deelt met bepaalde machtigingen en dat object onderliggende objecten eronder heeft, erft de ontvanger dezelfde machtigingen voor die onderliggende objecten.
>* Als een toegangsniveau gebruikers beperkt om bepaalde voorwerpen te schrappen, houdt dit hen niet van het schrappen van kindvoorwerpen die in die voorwerpen bevat zijn.

Een gebruiker kan de ontvanger een van de volgende machtigingen verlenen aan het afzonderlijke object:

* **Mening**: Dit niveau van toestemming staat de ontvanger toe om het voorwerp op één van de volgende manieren te delen:

   * In het hele systeem, zodat alle gebruikers het kunnen zien (niet beschikbaar voor alle objecten)
   * Met externe gebruikers zonder Workfront-licentie (niet beschikbaar voor alle objecten)
   * Met een e-mailadres (alleen beschikbaar voor documenten en kalenders)

* **draag** bij: (niet beschikbaar voor alle voorwerpen)
* **beheert**: Wanneer iemand een voorwerp deelt, worden de rechten van de ontvanger op het voorwerp bepaald door een combinatie van het de toegangsniveau van de ontvanger en de toestemmingen aan het voorwerp die door de aandeelhouder werden verleend. De laagste toegangsgraad beschikbaar in die combinatie is wat bepaalt wat de ontvanger met het voorwerp kan doen.

### Voorbeeldscenario&#39;s

#### **Scenario 1**

Als het de toegangsniveau van de ontvanger project het uitgeven niet toestaat, kan die persoon geen project uitgeven of schrappen zelfs als de aandeelhouder toestemmingen verleende om het te beheren.

Of, als het de toegangsniveau van de ontvanger project het uitgeven toestaat, maar aandeelhouder verleende mening-slechts toestemmingen aan een project, kan de gebruiker niet het project uitgeven of schrappen.

#### **Scenario 2**

Wanneer Olivia een Workfront-project deelt met Tony, wordt de toegang van Tony tot het project bepaald door een combinatie van twee dingen:

* Tony&#39;s toegangsniveau, toegewezen door de beheerder van Workfront
* Tony&#39;s machtigingen voor het project, gespecificeerd door Olivia

Tony&#39;s acties met betrekking tot het project kunnen verder worden beperkt op het project, maar ze kunnen niet onbeperkt zijn tot wat op zijn toegangsniveau is toegestaan:

* Als het toegangsniveau van Tony hem niet toestaat om taken tot stand te brengen, kan hij geen taken aan het project toevoegen, zelfs als Olivia hem toestemmingen gaf om taken aan het toe te voegen.
* Als het de toegangsniveau van Tony hem toestaat om taken tot stand te brengen, maar Olivia verleende geen toestemmingen om taken aan het project toe te voegen, kan hij geen taken aan dat project toevoegen, maar hij kan taken aan andere projecten toevoegen waar hij toestemmingen heeft gekregen om dit te doen.
