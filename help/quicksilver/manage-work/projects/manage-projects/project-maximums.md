---
title: Overzicht van projectlimieten
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront heeft limieten voor het aantal objecten dat aan een project kan worden gekoppeld. Projectlimieten zijn ingesteld om de productprestaties te verbeteren en uw ervaring met Workfront te verbeteren.
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# Overzicht van projectlimieten

Adobe Workfront heeft limieten voor het aantal objecten dat aan een project kan worden gekoppeld. Projectlimieten zijn ingesteld om de productprestaties te verbeteren en uw ervaring met Workfront te verbeteren.

De volgende voorwerpen verbonden aan projecten hebben de volgende grenzen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Taken</p></td> 
   <td>  <p>Het maximumaantal taken per project is 5.000. Er wordt een waarschuwingsbericht weergegeven wanneer het aantal taken dit maximum bereikt. Wanneer het maximum wordt bereikt, toont een foutenmelding en kunnen de extra taken niet aan het project worden toegevoegd.</p> <p>Verplaats taken die zijn gesloten voor een ander project dat is bestemd voor gesloten taken om te voorkomen dat u dit maximum bereikt. Het kan nodig zijn de verslagen over deze projecten aan te passen.</p>

<b> BELANGRIJK </b>

Voor projecten waar de taken veel gebiedsdelen hebben, zou een prestatiesdegradatie in het berekenen van de chronologie kunnen voorkomen of wanneer het werken in het project.

Daarom adviseren wij dat het aantal taken in projecten met complexe afhankelijkheden veel lager zou moeten zijn dan het toegestane maximum van 5.000 taken.

Enkele voorbeelden van taakgebiedsdelen die het opnieuw berekenen van de chronologie van het project zouden kunnen beïnvloeden of verhinderen zijn:

<ul><li>Aantal kinderen</li>
   <li>Meerdere niveaus voor taakinspringing</li>
   <li>Aantal voorgangers</li>
   <li>Meerdere toewijzingen</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Problemen</p></td> 
   <td>  <p>Het maximumaantal uitgaven per project is 10.000. Er wordt een waarschuwingsbericht weergegeven wanneer het aantal problemen dit maximum bereikt. Wanneer het maximum wordt bereikt, toont een foutenmelding en kunnen de extra kwesties niet aan het project worden toegevoegd.</p> <p>U kunt voorkomen dat dit maximum wordt bereikt door problemen die zijn gesloten, naar een ander project te verplaatsen dat is bedoeld voor afgesloten problemen. Het kan nodig zijn de verslagen over deze projecten aan te passen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Duur</p></td> 
   <td> <p>De maximale duur van een project moet 15 jaar zijn, zodat Workfront de tijdlijn automatisch kan berekenen. Er verschijnt een waarschuwingsbericht wanneer de projectduur het maximum bereikt. Wanneer het maximum is bereikt, wordt een waarschuwingsbericht weergegeven en vinden de automatische tijdlijnberekeningen niet meer plaats.</p> <p>De automatische tijdlijnberekeningen worden hervat zodra de duur van een project minder dan 15 jaar bedraagt, door de data van de taken in het project aan te passen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Tijdlijnberekeningen</p></td> 
   <td>Workfront voert geen automatische tijdlijnberekeningen uit voor projecten die niet in 6 maanden zijn bijgewerkt en zal niet hervat tot een update wordt gemaakt.<p>Voor projecten die niet in 3 maanden zijn bijgewerkt, voert Workfront wekelijks tijdlijnberekeningen uit in plaats van iedere avond.</p><p>Voor informatie over het berekenen van projectchronologie, zie <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref"> projectchronologie </a> opnieuw berekenen. </p></td> 
  </tr> 
    <tr> 
   <td role="rowheader"><p>Objecten omzetten </p></td> 
   <td>Workfront heeft een verwerkingslimiet van 5 minuten voor het omzetten van objecten. Als er een groot aantal documenten aan het object is gekoppeld, kan het zijn dat het object niet binnen de limiet van 5 minuten wordt omgezet. Mogelijk moet u enkele documenten verwijderen en het opnieuw proberen.</td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->
