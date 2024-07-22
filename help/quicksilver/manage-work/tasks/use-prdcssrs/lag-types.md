---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Overzicht van typen labels
description: Lag is de hoeveelheid tijd die na de voltooiing van gedwongen voorganger moet overgaan tot de afhankelijke taak (Positieve Lag) kan beginnen, of de hoeveelheid tijd dat een afhankelijke taak kon beginnen alvorens voorganger (Negatieve Lag) begint.
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: ed179058cfec1332384ef76cb04598278109291b
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 0%

---

# Overzicht van typen labels

<!-- Audited: 01/2024 -->

Lag is de hoeveelheid tijd die na de Geplande Voltooiing van een voorganger moet overgaan tot de afhankelijke taak (Positieve Lag) kan beginnen, of de hoeveelheid tijd die een afhankelijke taak kon beginnen alvorens voorganger (Negatieve Lag) begint.

De geplande, voorspelde en geschatte datums van de vervolgtaken worden berekend met inachtneming van de vertraging en de geplande, voorspelde en geschatte begindatums (Voltooiing) van de voorgaande taken.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan </p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de taken en het project beheren</p> </td> 
  </tr> 
 </tbody> 
</table>

*For meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Laagtypen {#lag-types}

Een voorbeeld van een taak die een vertragingstijd zou vereisen zou bomen in aantal kunnen zaaien. Als het versnipperde hout moet drogen voordat het kan worden geknipt, zou er een vertraging optreden tussen het kappen van de bomen en het zaaien ervan in de bomen.

De volgende tabel illustreert de typen labels en hoe u de hoeveelheid tijd voor elke Lag kunt aangeven:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong> Waarde </strong> </p> </td> 
   <td> <p><strong> Beschrijving </strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dagen (d of de)</p> </td> 
   <td> <p>De vertraging tussen twee taken die verband houden met afhankelijkheid wordt gemeten in werkdagen. Dit is het standaardlabeltype. </p> <p>Als er bijvoorbeeld een eindstartafhankelijkheid is met een vertraging van twee werkdagen en de voorganger op vrijdag klaar is, begint de afhankelijke taak op woensdag. De weekenddagen tellen niet als deel van de vertraging. </p> <p>Opmerking: de maximale vervallimiet voor dagen is 366.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Kalenderdagen (c of ce)</p> </td> 
   <td> <p>De vertraging tussen twee taken wordt gemeten in kalenderdagen, met inbegrip van feestdagen en weekends. </p> <p>Opmerking: hoewel dit type vertraging niet-werkdagen telt als onderdeel van de vertraging, kan een afhankelijke taak nooit beginnen op een niet-werkdag. Als dit vlagtype de afhankelijke taak op een niet-werkende dag laat beginnen, is de Geplande Datum van het Begin van de afhankelijke taak gepland voor de volgende werkdag. </p> <p>Bijvoorbeeld, als er een eind-begin gebiedsdeel met een 2 kalenderdagvertraging is en de voorgangerstaak op Donderdag eindigt, begint de afhankelijke taak op Maandag in plaats van een Zondag. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Percentage (p of pe)</p> </td> 
   <td> <p>De vertraging wordt uitgedrukt als percentage van de geschatte tijd om de voorganger te voltooien. </p> <p>Bijvoorbeeld, als er een eind-begin gebiedsdeel met een vertraging van 20% op een predecessor 10-dagtaak is, zal het systeem berekenen hoeveel dagen 20% van de de taakduur van de voorganger vertegenwoordigen en dat als vertraging gebruiken. In dit geval duurt het twee dagen nadat de taak is voltooid. </p>

<p><b>OPMERKING</b></p> De maximale vervallimiet voor procenten is 2000%.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dag van de week (b of wij) </p> </td> 
   <td> <p>De vertraging tussen twee taken wordt gemeten door de dagen van de week voor de week aan te geven die de geplande Voltooiingsdatum van de voorganger bevat.</p> <p>Voor dit Type van Lag, wordt elke dag van de week geassocieerd met een aantal:</p> 
    <ul> 
     <li>Zondag=1</li> 
     <li>Maandag=2</li> 
     <li>Dinsdag 3</li> 
     <li>Woensdag=4</li> 
     <li>Donderdag=5</li> 
     <li>Vrijdag=6</li> 
     <li>Zaterdag=7</li> 
    </ul> <p>Als u wilt erop wijzen dat de Geplande Datum van het Begin van de opvolger op een Dinsdag van de huidige week zou moeten vallen, en de Dinsdag is vóór de Geplande Datum van de Voltooiing van de voorganger, zou u uw opvolger met de volgende formule coderen: </p> <p><code style="font-style: normal;">4fs-3w</code> </p>

<p><b>OPMERKING</b></p>

Als de Datum van het Begin van de opvolger wordt berekend om een bepaalde Dinsdag te zijn en die dag die voor de huidige week wordt overgegaan, dan is de Geplande Datum van het Begin van de opvolgertaak de zelfde dag (Dinsdag) van de volgende week, als beschikbaar. </p> <p>Als u wilt erop wijzen dat de vertraging op een Zaterdag van de huidige week zou moeten vallen, en de Zaterdag is na de Geplande Datum van Voltooiing van de voorganger, zou u uw opvolger met de volgende formule coderen:</p> <p><code> 4fs+7w</code> </p> <p>Als zaterdag een niet-werkdag is, wordt de volgende beschikbare dag na zaterdag (om positieve vertraging aan te geven) geselecteerd als de geplande begindatum van de opvolger. </p>

<p>Dit is niet van toepassing op planningsuitzonderingen. Als een datum ook een kalenderuitzondering is en de Datum van het Begin van de opvolger wordt berekend om die dag te zijn, dan probeert het systeem om de dichtstbijzijnde beschikbare datum te vinden die de dag van de week is die in de voorgangersuitdrukking wordt gespecificeerd.</p>

<p>Bijvoorbeeld, als de Datum van het Begin wordt berekend om een bepaalde Dinsdag te zijn en die dag een planningsuitzondering is en de vertraging van voorganger positief is dan zal het volgende Dinsdag (als dat ook een werkdag is) als Datum van het Begin van de opvolger kiezen. Als de vertraging negatief is, kiest het systeem de vorige Dinsdag als Datum van het Begin.</p>

<p>Als u het verloop of de komende weken wilt aangeven, kunt u een getal vóór het dagnummer toevoegen voor het type vertraging. </p> <p>Als u bijvoorbeeld de maandag van 10 weken geleden wilt aangeven, kunt u deze code gebruiken om de voorganger van uw opvolger aan te geven:</p> <p><code>4fs-102w</code> </p> <p>10 geeft 10 weken geleden aan en 2 is het nummer dat is toegewezen aan maandag. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dag van de week Niet nul (k of ke)</p> </td> 
   <td> <p>De vertraging tussen twee taken wordt bepaald identiek aan de Dag van het type van de Verlag van de Week, behalve als de tijd van de voorganger op de zelfde dag van de gespecificeerde week beëindigt. De vertragingstijd wordt vervolgens berekend aan de aangrenzende week (+/-). </p> <p>In dit geval kan de vertragingstijd nooit 0 zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Negatieve tag

U kunt een negatieve Lag gebruiken om op de behoefte of de capaciteit te wijzen voor de taak om te beginnen alvorens de voorgangertaak die beëindigt.

Houd rekening met de volgende regels wanneer u negatieve vlaggen gebruikt:

* De negatieve Lag kan niet de begin/einddata van een taak dwingen om vóór of na de Geplande Begin/beëindigingsdata van het project te zijn. Deze data worden gespecificeerd in het Programma van gebied op het project.

  Overweeg in dit geval het volgende:

   * Plan het project vanaf de voltooiingsdatum.
   * De laatste taak op het project zou moeten gebruiken moet op de Beperking van de Taak beëindigen. Aanbevolen wordt de taak voldoende lang te maken om rekening te houden met alle taken in verband met het project. De resterende taken werken goed met de restrictie Zo snel mogelijk.

* Het gebruik van een voorgangerrelatie Voltooien-Begin met taken kan een foutbericht veroorzaken.

  Overweeg in dit geval het volgende:

   * Stel een voorgangerrelatie tussen taken in die bestaat uit Voltooien.
   * De duur van de opvolgertaak moet gelijk zijn aan of groter zijn dan het geplande aantal dagen tussen taken.

## Lag- en labeltypen aangeven voor taken

U kunt vlagtypes op taken wijzen wanneer u hun voorgangersverhoudingen bepaalt.

### Wijs op de Types van Lag in de Predecessors sectie van een taak {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. Ga naar een taak waarvoor u voorganger en het Type van Lag wilt bepalen.
1. Klik **Predecessors** in het linkerpaneel. U zou **kunnen moeten klikken tonen Meer**, en dan **Predecessors**.
1. Klik **toevoegen Voorganger**.
1. (Facultatief) als u een dwars-projectvoorganger wilt toevoegen, vervang de **naam van het Project van de ouder** {met een ander project.
1. Typ de naam van de voorgaande taak en selecteer deze wanneer deze in de lijst wordt weergegeven.
1. Selecteer het **Type van Afhankelijkheid**.

   Voor meer informatie over de Types van Afhankelijkheid van predecessor, zie [ Overzicht van de types van taakgebiedsdeel ](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Specificeer a **bedrag van de a** Lag gebruikend een numerieke waarde. U kunt negatieve getallen opgeven om een negatieve vertraging aan te geven.
1. Selecteer een van de volgende opties om het type vertraging aan te geven dat u voor uw voorganger wilt opgeven:

   * **Dagen**
   * **de Dagen van de Kalender**
   * **Percentage**
   * **Dag van de Week**
   * **Dag van de Week (Nul)**

     Voor meer informatie over deze Types van Lag en hoe zij worden berekend, zie de types van sectie [ Lag ](#lag-types) in dit artikel.

1. Klik **sparen**.

### Wijs op de Types van Lag in een taaklijst  {#indicate-lag-types-in-a-task-list}

1. Ga naar een taaklijst, en selecteer de **Standaard** mening.

1. Klik binnen de **1} kolom van Predecessors {die aan de taak beantwoordt waarvoor u een voorganger en een vertragingsbedrag wilt specificeren.**
1. Voer het volgende in zonder spaties:

   * het aantal van de taak u als voorganger van de geselecteerde taak wilt wijzen
   * de afkorting voor het gebiedstype u tussen de taken wilt wijzen

     Voor meer informatie over de afkortingen voor de Types van Afhankelijkheid, zie [ Overzicht van de types van taakgebiedsdeel ](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * of a **+** voor een positieve vertraging of a **-** voor een negatieve vertraging

   * de omvang van de vertraging
   * de afkorting voor het gewenste Laagtype

     Voor meer informatie over de afkortingen voor de Types van Lag, zie de sectie [ Types van Lag ](#lag-types) in dit artikel.

   Als u bijvoorbeeld wilt aangeven dat een taak een voorganger en een positieve vertraging van twee dagen heeft, typt u `1fs+2d` in de kolom Voorgangers.

1. Druk op Enter op het toetsenbord om de wijzigingen in uw taak op te slaan.