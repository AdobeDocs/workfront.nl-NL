---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Overzicht van labeltypen
description: Lag is de hoeveelheid tijd die na de voltooiing van gedwongen voorganger moet overgaan tot de afhankelijke taak (Positieve Lag) kan beginnen, of de hoeveelheid tijd dat een afhankelijke taak kon beginnen alvorens voorganger (Negatieve Lag) begint.
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '1385'
ht-degree: 0%

---

# Overzicht van labeltypen

Lag is de hoeveelheid tijd die na de voltooiing van gedwongen voorganger moet overgaan tot de afhankelijke taak (Positieve Lag) kan beginnen, of de hoeveelheid tijd dat een afhankelijke taak kon beginnen alvorens voorganger (Negatieve Lag) begint.

De geplande, voorspelde en geschatte data van de vervolgtaken worden berekend met inachtneming van de vertraging en de geplande, voorspelde en geraamde aanvangsdata (Voltooiing) van de voorgaande taken.

## Toegangsvereisten

<!--drafted - replace table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de taken en het project beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Lag- en labeltypen aangeven voor taken

U kunt vlagtypes op taken wijzen wanneer u hun voorgangersverhoudingen bepaalt.

* [Wijs op de Types van Lag in de Predecessors sectie van een taak](#indicate-lag-types-in-the-predecessors-section-of-a-task)
* [Wijs op de Types van Lag in een taaklijst](#indicate-lag-types-in-a-task-list)

### Wijs op de Types van Lag in de Predecessors sectie van een taak {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. Ga naar een taak waarvoor u voorganger en het Type van Lag wilt bepalen.
1. Klikken **Predecessors** in het linkerdeelvenster. Mogelijk moet u op **Meer weergeven** en vervolgens **Predecessors**.
1. Klikken **Voorganger toevoegen**.
1. (Optioneel) Als u een voorganger voor meerdere projecten wilt toevoegen, vervangt u de opdracht **Bovenliggend project** naam met een ander project.
1. Typ de naam van de voorgaande taak en selecteer deze wanneer deze in de lijst wordt weergegeven.
1. Selecteer **Type afhankelijkheid**.

   Voor meer informatie over de Types van Afhankelijkheid van predecessor, zie [Overzicht van typen taakafhankelijkheid](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Geef een **Lag** hoeveelheid met een numerieke waarde. U kunt negatieve getallen opgeven om een negatieve vertraging aan te geven.
1. Selecteer uit de volgende opties het type vertraging dat u voor uw voorganger wilt opgeven:

   * **Dagen**
   * **Kalenderdagen**
   * **Percentage**
   * **Dag van de week**
   * **Dag van de week (niet nul)**

      Voor meer informatie over deze Types van Lag en hoe zij worden berekend, zie de sectie [Overzicht van typen labels](#lag-types-overview) in dit artikel.

1. Klikken **Opslaan**.

### Wijs op de Types van Lag in een taaklijst  {#indicate-lag-types-in-a-task-list}

1. Ga naar een takenlijst en selecteer de **Standaard** Weergeven vanuit de **Weergave** vervolgkeuzemenu.

1. Klik in het dialoogvenster **Predecessors** kolom die overeenkomt met de taak waarvoor u een voorganger en een hoeveelheid vertraging wilt opgeven.
1. Voer het volgende in zonder spaties:

   * het aantal van de taak u als voorganger van de geselecteerde taak wilt wijzen
   * de afkorting voor het gebiedstype u tussen de taken wilt wijzen

      Voor meer informatie over de afkortingen voor de Types van Afhankelijkheid, zie [Overzicht van typen taakafhankelijkheid](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * ofwel **+** voor een positieve vertraging of een **-** voor een negatieve vertraging

   * de omvang van de vertraging
   * De afkorting voor het Laagtype dat u wilt gebruiken.

      Voor meer informatie over de afkortingen voor de Types van Lag, zie de sectie [Overzicht van typen labels](#lag-types-overview) in dit artikel.
   Als u bijvoorbeeld wilt aangeven dat een taak een voorganger en een positieve vertraging van twee dagen heeft, voert u

   ```
   1fs+2d
   ```

   in de kolom Voorgangers.

1. Klik op Enter op het toetsenbord om de wijzigingen in uw taak op te slaan.

## Overzicht van typen labels {#lag-types-overview}

Een voorbeeld van een taak die een vertragingstijd zou vereisen zou bomen in aantal kunnen zaaien. Als het versnipperde hout moet drogen voordat het kan worden geknipt, zou er een vertraging optreden tussen het kappen van de bomen en het zaaien ervan in de bomen.

De volgende tabel illustreert de typen labels en hoe u de hoeveelheid tijd voor elke Lag kunt aangeven:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Waarde</strong> </p> </td> 
   <td> <p><strong>Beschrijving</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dagen (d)</p> </td> 
   <td> <p>De vertraging tussen twee taken die verband houden met afhankelijkheid wordt gemeten in werkdagen. Dit is het standaardlabeltype. </p> <p>Als er bijvoorbeeld een eindstartafhankelijkheid is met een vertraging van twee werkdagen en de voorganger op vrijdag klaar is, begint de afhankelijke taak op woensdag. De weekenddagen tellen niet als deel van de vertraging. </p> <p>Opmerking: De maximale vervallimiet voor dagen is 366.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Kalenderdagen (c)</p> </td> 
   <td> <p>De vertraging tussen twee taken wordt gemeten in kalenderdagen, met inbegrip van feestdagen en weekends. </p> <p>Opmerking: Hoewel dit type vertraging niet-werkdagen telt als onderdeel van de vertraging, kan een afhankelijke taak nooit beginnen op een niet-werkdag. Als dit vlagtype de afhankelijke taak op een niet-werkende dag laat beginnen, is de Geplande Datum van het Begin van de afhankelijke taak gepland voor de volgende werkdag. </p> <p>Bijvoorbeeld, als er een eind-begin gebiedsdeel met een 2 kalenderdagvertraging is en de voorgangerstaak op Donderdag eindigt, begint de afhankelijke taak op Maandag in plaats van een Zondag. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Percentage (p of pe)</p> </td> 
   <td> <p>De vertraging wordt uitgedrukt als percentage van de geschatte tijd om de voorganger te voltooien. </p> <p>Bijvoorbeeld, als er een eind-begin gebiedsdeel met bij 20% vertraging tussen op een 10 dagvoorgangertaak is, zal het systeem berekenen hoeveel dagen 20% van de voorgangerstaakwandduur is en gebruikt dat als vertraging. In dit geval duurt het twee dagen nadat de taak is voltooid. </p> <p>Opmerking: De maximale vervallimiet voor procenten is 2000%.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dag van de week (w) </p> </td> 
   <td> <p>De vertraging tussen twee taken wordt gemeten door de dagen van de week voor de week aan te geven die de geplande Voltooiingsdatum van de voorganger bevat.</p> <p>Voor dit Type van Lag, wordt elke dag van de week geassocieerd met een aantal:</p> 
    <ul> 
     <li>Zondag=1</li> 
     <li>Maandag=2</li> 
     <li>Dinsdag 3</li> 
     <li>Woensdag=4</li> 
     <li>Donderdag=5</li> 
     <li>Vrijdag=6</li> 
     <li>Zaterdag=7</li> 
    </ul> <p>Als u wilt erop wijzen dat de Geplande Datum van het Begin van de opvolger op een Dinsdag van de huidige week zou moeten vallen, en de Dinsdag is v????r de Geplande Datum van de Voltooiing van de voorganger, zou u uw opvolger met de volgende formule coderen: </p> <p><code style="font-style: normal;">4fs-3w</code> </p> <p>Opmerking: Als de Dinsdag voor de week van de Geplande VoltooiingsDatum van de voorganger inging, dan is de Geplande Datum van het Begin van de opvolgertaak de eerste beschikbare werkdag van die week. </p> <p>Als u wilt erop wijzen dat de vertraging op een Zaterdag van de huidige week zou moeten vallen, en de Zaterdag is na de Geplande Datum van Voltooiing van de voorganger, zou u uw opvolger met de volgende formule coderen:</p> <p><code style="font-style: normal;">4fs+7w</code> </p> <p>Als zaterdag een niet-werkdag is, wordt de volgende beschikbare dag na zaterdag (om positieve vertraging aan te geven) geselecteerd als de geplande begindatum van de opvolger. </p> <p>Als u het verloop of de komende weken wilt aangeven, kunt u een getal v????r het dagnummer toevoegen voor het type vertraging. </p> <p>Als u bijvoorbeeld de maandag van 10 weken geleden wilt aangeven, kunt u deze code gebruiken om de voorganger van uw opvolger aan te geven:</p> <p><code>4fs-102w</code> </p> <p>10 geeft 10 weken geleden aan en 2 is het nummer dat is toegewezen aan maandag. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dag van de week Niet nul (k)</p> </td> 
   <td> <p>De vertraging tussen twee taken wordt bepaald identiek aan de Dag van het type van de Verlag van de Week, behalve als de tijd van de voorganger op de zelfde dag van de gespecificeerde week be??indigt. De vertragingstijd wordt vervolgens berekend aan de aangrenzende week (+/-). </p> <p>In dit geval kan de vertragingstijd nooit 0 zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Overzicht van negatieve labels

U kunt een negatieve Lag gebruiken om op de behoefte of de capaciteit te wijzen voor de taak om te beginnen alvorens de voorgangertaak die be??indigt.

Houd rekening met de volgende regels wanneer u negatieve vlaggen gebruikt:

* De negatieve Lag kan niet de begin/einddata van een taak dwingen om v????r of na de Geplande Begin/be??indigingsdata van het project te zijn. Deze data worden gespecificeerd in het Programma van gebied op het project.

   Overweeg in dit geval het volgende:

   * Plan het project vanaf de voltooiingsdatum.
   * De laatste taak op het project zou moeten gebruiken moet op de Beperking van de Taak be??indigen. Aanbevolen wordt de taak voldoende lang te maken om rekening te houden met alle taken in verband met het project. De resterende taken werken goed met de restrictie Zo snel mogelijk.

* Het gebruik van een voorganger-relatie Voltooien met taken kan een foutbericht veroorzaken.

   Overweeg in dit geval het volgende:

   * Stel een voorgangerrelatie tussen taken in die bestaat uit Voltooien.
   * De duur van de opvolgertaak moet gelijk zijn aan of groter zijn dan het geplande aantal dagen tussen taken.
