---
title: Configureerbare toegang tot functionaliteit voor elk objecttype (verouderd)
description: Dit artikel verklaart wat u als beheerder van Adobe Workfront voor elk objecten type, op elk toegangsniveau kunt toestaan. Het verklaart ook wat de standaardconfiguratie voor elk type van toegangsniveau is.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '3510'
ht-degree: 0%

---

# Configureerbare toegang tot functionaliteit voor elk objecttype (verouderd)

>[!NOTE]
>
>De informatie in dit artikel verwijst naar de oudere toegangsniveaus. Voor informatie over de huidige toegangsniveaus, zie [&#x200B; Nieuw overzicht van toegangsniveaus &#x200B;](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

Wanneer het vormen van een toegangsniveau voor uw organisatie, kunt u bepalen welke specifieke acties aan het toegangsniveau beschikbaar zijn.

In dit artikel worden de opties uitgelegd die een Adobe Workfront-beheerder voor elk objecttype op elk toegangsniveau kan selecteren. Het verklaart ook wat de standaardconfiguratie voor elk type van toegangsniveau is.

Bijvoorbeeld, als een beheerder van Workfront &quot;Mening&quot;voor projecten in een bepaald toegangsniveau selecteert, zullen de gebruikers met dat toegangsniveau projecten kunnen slechts bekijken, niet hen uitgeven.

Voor informatie over alle functionaliteit beschikbaar voor een objecten type in elk toegangsniveau, zie [&#x200B; Functionaliteit beschikbaar voor elk objecten type &#x200B;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Projecten

In elk toegangsniveau, kunt u de volgende opties voor projecten vormen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Toegangsniveau</th> 
   <th>Opties</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planner (licentietype abonnement)</td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li><p> <b> Mening </b></p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om projecten te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot projecten toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Kopiëren</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Weergave</p> </li> 
       <li> <p>Delen</p> </li> 
       <li> <p>Delen op het hele systeem</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Worker </td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li><p> <b> Mening </b></p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om projecten te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat beperkte het uitgeven toegang tot projecten toe. Om te zien hoe de Edit toegang in een de toegangsniveau van de Arbeider in vergelijking met een de toegangsniveau van de Planner (dat volledige toegang tot projecten) toestaat, zie de sectie <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref"> Projecten </a> in de artikel <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref"> Functionaliteit beschikbaar voor elk objecten type </a>.</p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om projecten te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de Edit knoop, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li> <b> Mening </b> (standaardselectie) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aanvrager</td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li><p> <b> Mening </b></p> (standaardselectie) <p>De toegang van de mening is beperkt omdat u niet het kunt verfijnen om project het delen toe te laten of onbruikbaar te maken.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externe gebruiker</td> 
   <td> <p>Toegang tot projecten is niet beschikbaar. Externe gebruikers kunnen Workfront alleen gebruiken om documenten te bekijken en te downloaden en om kalenders te bekijken die met hen worden gedeeld.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Taken

In elk toegangsniveau, kunt u de volgende opties voor taken vormen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Toegangsniveau</th> 
   <th>Opties</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planner </td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li><p> <b> Mening </b></p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om taken te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot taken toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
       <li> <p>Delen op het hele systeem</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Worker </td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li><p> <b> Mening </b></p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om taken te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot taken toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li> <b> Mening </b> (standaardselectie) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aanvrager</td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li><p> <b> Mening </b></p> (standaardselectie)<p>De toegang van de mening is beperkt omdat u niet het kunt verfijnen om project het delen toe te laten of onbruikbaar te maken.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externe gebruiker</td> 
   <td> <p>Toegang tot taken is niet beschikbaar. Externe gebruikers kunnen Workfront alleen gebruiken om documenten te bekijken en te downloaden en om kalenders te bekijken die met hen worden gedeeld.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problemen

In elk toegangsniveau, kunt u de volgende opties voor kwesties vormen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Toegangsniveau</th> 
   <th>Opties</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planner </td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li> <p><b>Weergave</b></p><p>Om dit te verfijnen, kunt u de capaciteit vormen om kwesties te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot kwesties toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
       <li> <p>Delen op het hele systeem</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Worker </td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li><p> <b> Mening </b></p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om kwesties te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot kwesties toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li><p> <b> Mening </b></p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om kwesties te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot kwesties toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aanvrager</td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li><p> <b> Mening </b></p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om kwesties te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot kwesties toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externe gebruiker</td> 
   <td> <p>Toegang tot problemen is niet beschikbaar. Externe gebruikers kunnen Workfront alleen gebruiken om documenten te bekijken en te downloaden en om kalenders te bekijken die met hen worden gedeeld.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Portfolio&#39;s

In elk toegangsniveau, kunt u de volgende opties voor portefeuilles vormen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Toegangsniveau</th> 
   <th>Opties</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planner </td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li><p> <b> Mening </b></p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om portefeuilles te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot portefeuilles toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
       <li> <p>Delen op het hele systeem</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Worker </td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li> <b> Mening </b> (standaardselectie) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li> <b> Mening </b> (standaardselectie)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aanvrager</td> 
   <td> <p>Toegang tot portfolio's is niet beschikbaar.</p> </td> 
  </tr> 
  <tr> 
   <td>Externe gebruiker</td> 
   <td> <p>Toegang tot portfolio's is niet beschikbaar. Externe gebruikers kunnen Workfront alleen gebruiken om documenten te bekijken en te downloaden en om kalenders te bekijken die met hen worden gedeeld.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Programma&#39;s

In elk toegangsniveau, kunt u de volgende opties voor programma&#39;s vormen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Toegangsniveau</th> 
   <th>Opties</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planner </td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li><p> <b> Mening </b></p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om programma's te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot programma's toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
       <li> <p>Delen op het hele systeem</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Worker </td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li> <b> Mening </b> (standaardselectie) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li> <b> Mening </b> (standaardselectie)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aanvrager</td> 
   <td> <p>Toegang tot programma's is niet beschikbaar.</p> </td> 
  </tr> 
  <tr> 
   <td>Externe gebruiker</td> 
   <td> <p>Toegang tot programma's is niet beschikbaar. Externe gebruikers kunnen Workfront alleen gebruiken om documenten te bekijken en te downloaden en om kalenders te bekijken die met hen worden gedeeld.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Rapporten, dashboards en kalenders

In elk toegangsniveau, kunt u de volgende opties voor rapporten, dashboards, en kalenders vormen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Toegangsniveau</th> 
   <th>Opties</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planner </td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li> <p><b>Weergave</b></p><p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop) uit, dan maak of laat om het even welke volgende acties onbruikbaar. Beide zijn standaard ingeschakeld:</p> 
      <ul> 
       <li> <p>Ingebouwde rapporten weergeven</p> </li> 
       <li> <p>Delen</p> </li> 
      </ul> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot rapporten, dashboards, en kalenders toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek behalve <b> Mening Ingebouwde Rapporten </b>, <b> de Rapporten van het Aandeel </b>, en <b> het systeembrede Aandeel </b>.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Ingebouwde rapporten weergeven</p> </li> 
       <li> <p>Delen</p> </li> 
       <li> <p>Rapporten openbaar (extern) delen</p> </li> 
       <li> <p>Delen op het hele systeem</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Worker </td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li><p> <b> Mening </b></p> (standaardselectie)<p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende acties onbruikbaar. Beide zijn standaard ingeschakeld:</p> 
      <ul> 
       <li> <p>Ingebouwde rapporten weergeven</p> </li> 
       <li> <p>Delen</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li> <p><b> Mening </b> (standaardselectie)<p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende acties onbruikbaar. Alleen de optie Delen is standaard ingeschakeld.</p> 
      <ul> 
       <li> <p>Ingebouwde rapporten weergeven</p> </li> 
       <li> <p>Delen</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aanvrager</td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li> <p><b> Mening </b> (standaardselectie): Staat mening-slechts toegang tot rapporten, dashboards, en kalenders toe die met hen zijn gedeeld.</p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om ingebouwde rapporten te bekijken. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de <b> Mening </b> knoop, dan onbruikbaar maken of toelaten <b> Gebouwd Mening </b> (onbruikbaar gemaakt door gebrek).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externe gebruiker</td> 
   <td> <p>Toegang tot rapporten, dashboards en kalenders is niet beschikbaar. Externe gebruikers kunnen Workfront alleen gebruiken om documenten te bekijken en te downloaden en om kalenders te bekijken die met hen worden gedeeld.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Filters, weergaven en groepen

In elk toegangsniveau, kunt u de volgende opties voor filters, meningen, en groeperingen vormen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Toegangsniveau</th> 
   <th>Opties</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planner </td> 
   <td> 
    <ul> 
     <li> <p><b>Weergave</b></p><p>Om dit te verfijnen, kunt u de capaciteit vormen om filters, meningen, en groeperingen te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot filters, meningen, en groeperingen toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
       <li> <p>Delen op het hele systeem</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Worker </td> 
   <td> 
    <ul> 
     <li> <p><b>Weergave</b></p><p>Om dit te verfijnen, kunt u de capaciteit vormen om filters, meningen, en groeperingen te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot filters, meningen, en groeperingen toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
       <li> <p>Delen op het hele systeem</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li><p> <b> Mening </b></p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om filters, meningen, en groeperingen te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot filters, meningen, en groeperingen toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
       <li> <p>Delen op het hele systeem</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aanvrager</td> 
   <td> 
    <ul> 
     <li> <p><b> Mening </b>:</p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om filters, meningen, en groeperingen te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot filters, meningen, en groeperingen toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
       <li> <p>Delen op het hele systeem</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externe gebruiker</td> 
   <td> <p>Er is geen toegang tot filters, weergaven en groepen. Externe gebruikers kunnen Workfront alleen gebruiken om documenten te bekijken en te downloaden en om kalenders te bekijken die met hen worden gedeeld.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Documenten

In elk toegangsniveau, kunt u de volgende opties voor documenten vormen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Toegangsniveau</th> 
   <th>Opties</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planner </td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li><p> <b> Mening </b></p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om documenten te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): staat volledige het uitgeven toegang tot documenten toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek behalve <b> Documenten van het Aandeel Openbaar </b> en <b> het systeembrede Aandeel </b>.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
       <li> <p>Documenten openbaar (extern) delen</p> </li> 
       <li> <p>Delen op het hele systeem</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Worker </td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li> <p><b>Weergave</b></p><p>Om dit te verfijnen, kunt u de capaciteit vormen om documenten te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): staat volledige het uitgeven toegang tot documenten toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek behalve <b> Documenten van het Aandeel Openbaar </b> en <b> het systeembrede Aandeel </b>.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
       <li> <p>Documenten openbaar (extern) delen</p> </li> 
       <li> <p>Delen op het hele systeem</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li><p> <b> Mening </b></p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om documenten te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): staat volledige het uitgeven toegang tot documenten toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende acties onbruikbaar. Al hen worden toegelaten door gebrek behalve de laatste twee, <b> Documenten van het Aandeel Openbaar </b> en <b> het systeembrede Aandeel </b>.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
       <li> <p>Documenten openbaar (extern) delen</p> </li> 
       <li> <p>Delen op het hele systeem</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aanvrager</td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li> <p><b>Weergave</b></p><p>Om dit te verfijnen, kunt u de capaciteit vormen om documenten te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): staat volledige het uitgeven toegang tot documenten toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externe gebruiker</td> 
   <td> <p>De toegang tot documenten is niet configureerbaar in dit toegangsniveau. Maar externe gebruikers kunnen Workfront gebruiken om documenten weer te geven, te bekijken en te downloaden.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Gebruikers

In elk toegangsniveau, kunt u de volgende opties voor gebruikers vormen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Toegangsniveau</th> 
   <th>Opties</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planner </td> 
   <td> 
    <ul> 
     <li> <p><b>Weergave</b></p><p>Om dit te verfijnen, kunt u de capaciteit vormen om de contactinformatie van gebruikers te bekijken. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de <b> Mening </b> knoop, dan maak of laat de <b> optie van het Contact van de Mening </b> (toegelaten door gebrek) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot gebruikers toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende acties onbruikbaar. Slechts worden de eerste twee opties, <b> creëren </b> en <b> Schrapping </b>, toegelaten door gebrek.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li>Gebruikersbeheerder (alle gebruikers)</li> 
       <li> <p>Gebruikersbeheerder (Groepgebruikers)</p> </li> 
      </ul> <p>Voor informatie over de twee opties van Admin van de Gebruiker, zie de sectie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref"> toegang van gebruikers om gebruikers uit te geven gebruikend een niveau van de douanetoegang </a> in het artikel <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> toegang van de Verlening tot gebruikers </a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Worker </td> 
   <td> 
    <ul> 
     <li><p> <b> Mening </b> (slechts beschikbare optie)</p><p>Om dit te verfijnen, kunt u de capaciteit vormen om de contactinformatie van gebruikers te bekijken. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de <b> Mening </b> knoop, dan maak of laat de <b> optie van het Contact van de Mening </b> (toegelaten door gebrek) onbruikbaar toe.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li><p> <b> Mening </b> (slechts beschikbare optie)</p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om de contactinformatie van gebruikers te bekijken. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de <b> 2&rbrace; knoop van de Mening &lbrace;, dan toelaten of onbruikbaar maken de </b> Info van het Contact van de Mening <b> optie (door gebrek).</b></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aanvrager</td> 
   <td> 
    <ul> 
     <li> <p><b> Mening </b> (slechts beschikbare optie)</p><p>Om dit te verfijnen, kunt u de capaciteit vormen om de contactinformatie van gebruikers te bekijken. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de <b> 2&rbrace; knoop van de Mening &lbrace;, dan toelaten of onbruikbaar maken de </b> Info van het Contact van de Mening <b> optie (door gebrek).</b></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externe gebruiker</td> 
   <td> <p>Toegang tot gebruikers is niet beschikbaar. Externe gebruikers kunnen Workfront alleen gebruiken om documenten te bekijken en te downloaden en om kalenders te bekijken die met hen worden gedeeld.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Teams

In elk toegangsniveau, kunt u de volgende opties voor teams vormen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Toegangsniveau</th> 
   <th>Opties</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planner </td> 
   <td> 
    <ul> 
     <li><b> Mening </b> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de <b> 2&rbrace; knoop van de Mening &lbrace;, dan maak of laat om het even welke volgende opties* onbruikbaar toe. </b> Beide zijn standaard uitgeschakeld.</p> 
      <ul> 
       <li>Alle teams weergeven</li> 
       <li> <p>Aan mijn groepen gekoppelde teams weergeven</p> </li> 
      </ul> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot teams toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de <b> 2&rbrace; knoop van de Mening &lbrace;, dan maak of laat om het even welke volgende opties* onbruikbaar toe. </b> Al hen worden toegelaten door gebrek, behalve <b> uitgeeft teams ik </b> ben.</p> 
      <ul> 
       <li>Maken</li> 
       <li>Verwijderen</li> 
       <li> <p>Teams bewerken die ik heb ingeschakeld</p> </li> 
       <li> <p>Teams bewerken in groepen die ik beheer (alleen groepbeheerders)</p> </li> 
       <li> <p>Alle teams weergeven</p> </li> 
       <li> <p>Aan mijn groepen gekoppelde teams weergeven</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Worker </td> 
   <td> 
    <ul> 
     <li> <b> Mening </b>
      <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de <b> 2&rbrace; knoop van de Mening &lbrace;, dan maak of laat om het even welke volgende opties* onbruikbaar toe. </b> Beide zijn standaard ingeschakeld.</p> 
      <ul> 
       <li>Alle teams weergeven</li> 
       <li> <p>Aan mijn groepen gekoppelde teams weergeven</p> </li> 
      </ul> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot teams toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de <b> 2&rbrace; knoop van de Mening &lbrace;, dan maak of laat om het even welke volgende opties* onbruikbaar toe. </b> Slechts wordt de eerste optie, <b> uitgeeft teams I </b>, onbruikbaar gemaakt door gebrek.</p> 
      <ul> 
       <li> <p>Teams bewerken die ik heb ingeschakeld</p> </li> 
       <li> <p>Alle teams weergeven</p> </li> 
       <li> <p>Aan mijn groepen gekoppelde teams weergeven</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <p><b> Mening </b> (slechts beschikbare optie)</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de <b> 2&rbrace; knoop van de Mening &lbrace;, dan maak of laat om het even welke volgende opties* onbruikbaar toe. </b> Beide zijn standaard ingeschakeld.</p> 
      <ul> 
       <li> <p>Alle teams weergeven</p> </li> 
       <li>Aan mijn groepen gekoppelde teams weergeven</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aanvrager</td> 
   <td> 
    <ul> 
     <li> <p><b> Mening </b> (slechts beschikbare optie)</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de <b> 2&rbrace; knoop van de Mening &lbrace;, dan maak of laat om het even welke volgende opties* onbruikbaar toe. </b> Beide zijn standaard ingeschakeld.</p> 
      <ul> 
       <li> <p>Alle teams weergeven</p> </li> 
       <li>Aan mijn groepen gekoppelde teams weergeven</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externe gebruiker</td> 
   <td> <p>Toegang tot teams is niet beschikbaar. Externe gebruikers kunnen Workfront alleen gebruiken om documenten te bekijken en te downloaden en om kalenders te bekijken die met hen worden gedeeld.</p> </td> 
  </tr> 
 </tbody> 
</table>


## Sjablonen

In elk toegangsniveau, kunt u de volgende opties voor malplaatjes vormen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Toegangsniveau</th> 
   <th>Opties</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planner </td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li><p> <b> Mening </b></p> <p>Om dit te verfijnen, kunt u de capaciteit vormen om malplaatjes te delen. Klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de knoop van de Mening, dan maak of laat <b> Aandeel </b> optie (die door gebrek wordt toegelaten) onbruikbaar toe.</p> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot malplaatjes toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Al hen worden toegelaten door gebrek.</p> 
      <ul> 
       <li> <p>Maken</p> </li> 
       <li> <p>Verwijderen</p> </li> 
       <li> <p>Delen</p> </li> 
       <li> <p>Delen op het hele systeem</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Worker </td> 
   <td> 
    <ul> 
     <li> <p><b> Geen toegang </b> (slechts beschikbare optie)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <p><b> Geen toegang </b> (slechts beschikbare optie)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aanvrager</td> 
   <td> 
    <ul> 
     <li> <p><b> Geen toegang </b> (slechts beschikbare optie)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externe gebruiker</td> 
   <td> <p>Toegang tot sjablonen is niet beschikbaar. Externe gebruikers kunnen Workfront alleen gebruiken om documenten te bekijken en te downloaden en om kalenders te bekijken die met hen worden gedeeld.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Financiële gegevens

In elk toegangsniveau, kunt u de volgende opties voor financiële gegevens vormen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Toegangsniveau</th> 
   <th>Opties</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planner </td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li> <p><b> Mening </b>:</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de <b> 2&rbrace; knoop van de Mening &lbrace;, dan maak of laat om het even welke volgende opties* onbruikbaar toe. </b> Beide zijn standaard ingeschakeld.</p> 
      <ul> 
       <li>Rol- en kostenfacturering weergeven</li> 
       <li> <p>Facturering van gebruikers en kostentarieven weergeven</p> </li> 
      </ul> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot financiële gegevens toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op de <b> 2&rbrace; knoop van de Mening &lbrace;, dan maak of laat om het even welke volgende opties* onbruikbaar toe. </b> Slechts worden de laatste twee opties, <b> het Factureren van de Rol van de Mening &amp; Tarieven van Kosten </b> en <b> het Factureren van de Gebruiker van de Mening &amp; Tarieven van Kosten </b>, toegelaten door gebrek.</p> 
      <ul> 
       <li>Rollenfacturering en kostentarieven bewerken</li> 
       <li> <p>Facturering van gebruikers en kostentarieven bewerken</p> </li> 
       <li>Rol- en kostenfacturering weergeven</li> 
       <li> <p>Facturering van gebruikers en kostentarieven weergeven</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Worker </td> 
   <td> 
    <ul> 
     <li> <p><b> Geen toegang </b> (standaardselectie)</p> </li> 
     <li> <b> Mening </b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <p><b> Geen toegang </b> (standaardselectie)</p> </li> 
     <li><b> Mening </b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aanvrager</td> 
   <td> 
    <ul> 
     <li> <p><b> Geen toegang </b> (slechts beschikbare optie)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externe gebruiker</td> 
   <td> <p>Toegang tot financiële gegevens is niet beschikbaar. Externe gebruikers kunnen Workfront alleen gebruiken om documenten te bekijken en te downloaden en om kalenders te bekijken die met hen worden gedeeld.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; voor informatie over deze opties, zie [&#x200B; Overzicht van het Factureren en de Ontvangsten &#x200B;](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Bronbeheer

In elk toegangsniveau, kunt u de volgende opties voor het Beheer van het Middel vormen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Toegangsniveau</th> 
   <th>Opties</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planner </td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li> <b> Mening </b> </li> 
     <li> <p><b> geeft </b> uit (standaardselectie): Staat volledige het uitgeven toegang tot het Beheer van het Middel toe.</p> <p>Om dit te verfijnen, klik het tandwielpictogram <img src="assets/gear-icon-in-access-levels.png"> op <b> geef </b> knoop uit, dan maak of laat om het even welke volgende opties onbruikbaar. Slechts wordt de eerste optie, <b> geeft prioriteiten en begrotingsuren in de Planner </b> uit, toegelaten door gebrek.</p> 
      <ul> 
       <li> <p> Prioriteiten en begrotingstijden bewerken in de Planner</p> </li> 
       <li> <p>Bronnenpools beheren</p> <p><b> NOTA </b>: Om middelpools te beheren, heeft een gebruiker extra toegang tot financiële gegevens en toestemmingen aan projectfinanciën nodig. Als u de toegang van het Beheer van het Middel tot een gebruiker van de Planner verleent die geen toegang tot financiële gegevens heeft, kan de gebruiker nog de uurtoewijzingen in de Planner van het Middel zien, maar kan niet op de mening van Kosten schakelen of het BedrijfsGeval bekijken. Voor meer informatie, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref"> toegang van de Verlening tot financiële gegevens </a> en <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref"> de financiële toestemmingen van het Aandeel op een voorwerp </a>.</p> </li> 
       <li> <p>Geplande uren bijwerken in werklastbalans</p> <p><b> NOTA </b>: Om geplande uren in de Balancer van de Werkbelasting bij te werken, heeft een gebruiker toestemming nodig om aan het voorwerp bij te dragen, met de Toewijzingen van het Merk die onder Geavanceerde Montages worden toegelaten. Voor informatie, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref"> Overzicht van het delen van toestemmingen op voorwerpen </a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Worker </td> 
   <td> 
    <ul> 
     <li><b> Geen toegang </b> </li> 
     <li> <b> Mening </b> (standaardselectie) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> </li> 
     <li> <b> Mening </b> (standaardselectie)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aanvrager</td> 
   <td> 
    <ul> 
     <li> <b> Geen toegang </b> (slechts beschikbare optie) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Externe gebruiker</td> 
   <td> <p>Toegang is niet beschikbaar. Externe gebruikers kunnen Workfront alleen gebruiken om documenten te bekijken en te downloaden en om kalenders te bekijken die met hen worden gedeeld.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Scenario Planner, gebied

De standaardinstelling voor alle toegangsniveaus is Geen toegang. Een Workfront-beheerder kan dit wijzigen in Toegang weergeven of bewerken voor elke Planner, Worker en Reviewer.

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>De gebruikers kunnen een plan bekijken dat een andere gebruiker creeerde slechts als een verbinding aan het plan met hen wordt gedeeld.

## Gebied met Workfront-doelen

Alle zes van de standaardtoegangsniveaus (en alle 4 van de licentietypen) kunnen de Doelen van Workfront uitgeven en bekijken.

Bewerken is de standaardoptie.
