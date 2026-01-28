---
title: Hoe de Verouderde Niveaus van de Toegang en de Toestemmingen samen werken
user-type: administrator
content-type: reference
product-area: system-administration
keywords: toegang, model, funnel, diagram, niveaus, toestemmingen
navigation-topic: access-levels
description: De beheerder van Adobe Workfront bepaalt welk toegangsniveau elke gebruiker zou moeten hebben. Dat toegangsniveau bepaalt wat de gebruikers kunnen zien en met objecten types en gebieden in het systeem doen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Hoe de niveaus van de erfenistoegang en toestemmingen samenwerken

>[!NOTE]
>
>De informatie in dit artikel verwijst naar de oudere toegangsniveaus. Voor informatie over de huidige toegangsniveaus, zie [ Nieuw overzicht van toegangsniveaus ](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

De beheerder van Adobe Workfront bepaalt welk toegangsniveau elke gebruiker zou moeten hebben. Dat toegangsniveau bepaalt wat de gebruikers kunnen zien en met objecten types en gebieden in het systeem doen.

Gebruikers krijgen ook toegang tot afzonderlijke objecten wanneer andere gebruikers bepaalde machtigingen voor die objecten delen en verlenen.


![ het modelhiërarchie van de Veiligheid ](assets/security-model-hierachy.png)

Bijvoorbeeld, als uw toegangsniveau zegt dat u taken kunt tot stand brengen, maar de toestemmingen u op een specifiek project ontvangt staan u niet toe om taken aan het toe te voegen, kunt u geen taken op het project toevoegen alhoewel u taken elders in Workfront kunt tot stand brengen.

In dit artikel wordt uitgelegd hoe deze combinatie werkt.

## Toegangsniveau

Het toegangsniveau dat door een Workfront-beheerder aan elke gebruiker wordt toegewezen, is vereist voor aanmelding bij Workfront.

De standaardtoegangsniveaus zijn:

* Systeembeheerder (bijgevoegd bij de licentie voor abonnementen)
* Planner (als bijlage bij de planvergunning gevoegd)
* Worker (toegevoegd aan de arbeidsvergunning)
* Revisor (bijgevoegd bij de Revisielicentie)
* Aanvrager (als bijlage bij de aanvraagvergunning gevoegd)
* Externe gebruiker (toegevoegd aan de externe e-maillicentie)

De Workfront-licentie voor elk standaard toegangsniveau bepaalt wat beschikbaar en configureerbaar is in het toegangsniveau. Voor informatie over de vergunningen van Workfront, zie [ het vergunningsoverzicht van Adobe Workfront ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

Voor de gebruikers die aan het worden toegewezen, bepaalt een toegangsniveau wat zij met de volgende objecten types en gebieden in Workfront kunnen zien en doen:

* Projecten
* Taken
* Problemen
* Portfolio&#39;s
* Rapporten, dashboards en Kalenders
* Filters, Weergaven en Groepen
* Documenten
* Andere gebruikers
* Sjablonen
* Financiële gegevens
* Bronbeheer
* Scenario Planner
* Workfront-doelen

In een douanetoegangsniveau, kunt u de montages voor deze voorwerpen en gebieden vormen om te veranderen hoeveel toegang gebruikers tot hen hebben. Afhankelijk van de vergunning verbonden aan het toegangsniveau, evenals het type van het voorwerp of het gebied, kunt u het toegangsniveau vormen om geen toegang toe te staan, toegang te bekijken, of toegang tot een voorwerp of een gebied uit te geven.

>[!IMPORTANT]
>
>Wij adviseren sterk dat u de ingebouwde toegangsniveaus onveranderd laat zodat u naar hen kunt verwijzen nadat u opstelling uw gebruikers. Als u een toegangsniveau wilt aanpassen, kopieert u het standaardtoegangsniveau en wijzigt u de kopie. (U kunt dit voor elk toegangsniveau behalve de Beheerder van het Systeem en Externe Gebruiker doen.)

Voor een gedetailleerde verklaring van elk van de standaardtoegangsniveaus, zie [ Ingebouwde toegangsniveaus ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

Voor instructies bij het toewijzen van een toegangsniveau aan een gebruiker, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

## Machtigingen

Wanneer een gebruiker een object deelt met iemand in het systeem, kan hij of zij de ontvanger een van de volgende machtigingen voor het object verlenen.

* **Mening**: Dit niveau van toestemming staat de ontvanger toe om het voorwerp op één van de volgende manieren te delen:

   * In het hele systeem, zodat alle gebruikers het kunnen zien (niet beschikbaar voor alle objecten)
   * Met externe gebruikers zonder Workfront-licentie (niet beschikbaar voor alle objecten)
   * Met een e-mailadres (alleen beschikbaar voor documenten)

* **draag** bij: (niet beschikbaar voor alle voorwerpen)
* **beheert**: Wanneer iemand een voorwerp deelt, worden de rechten van de ontvanger op het voorwerp bepaald door een combinatie van het de toegangsniveau van de ontvanger en de toestemmingen aan het voorwerp die door de aandeelhouder werden verleend. De laagste toegangsgraad beschikbaar in die combinatie is wat bepaalt wat de ontvanger met het voorwerp kan doen.

  >[!INFO]
  >
  >**Voorbeeld:** als het de toegangsniveau van de ontvanger project het uitgeven niet toestaat, kan die persoon geen project uitgeven of schrappen zelfs als aandeelhouder toestemmingen verleende om het te beheren.
  >
  >Of, als het de toegangsniveau van de ontvanger project het uitgeven toestaat, maar aandeelhouder verleende mening-slechts toestemmingen aan een project, kan de gebruiker niet het project uitgeven of schrappen.

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

>[!NOTE]
>
>* Als een gebruiker een object deelt met bepaalde machtigingen en dat object onderliggende objecten eronder heeft, erft de ontvanger dezelfde machtigingen voor die onderliggende objecten.
>* Als een toegangsniveau gebruikers beperkt om bepaalde voorwerpen te schrappen, houdt dit hen niet van het schrappen van kindvoorwerpen die in die voorwerpen bevat zijn.
>

## Meer voorbeeldscenario&#39;s

Wanneer Olivia een Workfront-project deelt met Tony, wordt de toegang van Tony tot het project bepaald door een combinatie van twee dingen:

* Tony&#39;s toegangsniveau, toegewezen door de beheerder van Workfront
* Tony&#39;s machtigingen voor het project, gespecificeerd door Olivia

Tony&#39;s acties met betrekking tot het project kunnen verder worden beperkt op het project, maar ze kunnen niet onbeperkt zijn tot wat op zijn toegangsniveau is toegestaan:

* Als het toegangsniveau van Tony hem niet toestaat om taken tot stand te brengen, kan hij geen taken aan het project toevoegen, zelfs als Olivia hem toestemmingen gaf om taken aan het toe te voegen.
* Als het de toegangsniveau van Tony hem toestaat om taken tot stand te brengen, maar Olivia verleende geen toestemmingen om taken aan het project toe te voegen, kan hij geen taken aan dat project toevoegen, maar hij kan taken aan andere projecten toevoegen waar hij toestemmingen heeft gekregen om dit te doen.
