---
title: Een tabel filteren in Rapportcanvas
description: Een tabel filteren in Rapportcanvas
hidefromtoc: true
hide: true
source-git-commit: 350d64577bac677bb0cc9bcb804c32b0301bc5d4
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 0%

---


# Een tabel filteren in Rapportcanvas

Nadat u een lijstblok aan een rapport toevoegt, kunt u opstellingsfilters om de informatie te beperken die in de lijst toont.

Een filterregel bevat drie componenten:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Veld</td> 
   <td> <p>Het veld dat de informatie bevat waarmee u de tabel wilt filteren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Operator</td> 
   <td> <p>De manier waarop het filter bepaalt welke veldwaarden in de tabel worden opgenomen of van de tabel worden uitgesloten. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Waarde</td> 
   <td> <p>De waarden in het geselecteerde veld die worden geëvalueerd op basis van de operator.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Voorbeeld:** Als u de resultaten in uw rapport wilt beperken tot alleen weergaveprojecten die eigendom zijn van Jane Doe, kunt u een filterregel maken met het veld &quot;Projecteigenaar&quot;, de operator &quot;Gelijk aan&quot; en de waarde &quot;Jane Doe&quot;.

Of u kon slechts projecten tonen die een toegewezen projecteigenaar hebben, die het gebied &quot;de Eigenaar van het Project&quot;en de exploitant &quot;niet leeg zou hebben.&quot;

## Vereisten

Alvorens u begint, moet u in de bèta van het Canvas van de Rapportering inschrijven. Zie voor meer informatie [Bewerken van canvas melden: overzicht](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Filterregels voor een tabel configureren

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Rapportage**.

1. Klikken **Nieuw rapport**.

   of

   Ga naar een bestaand rapport, klik op de knop **Meer menu** pictogram ![](assets/more-icon.png) in de rapportkopbal, dan selecteer **Bewerken**.

1. Als u rijen op een nieuwe tabel wilt groeperen, sleept u een tabelblok naar het canvas of dubbelklikt u erop.

   of

   Als u rijen op een bestaande tabel wilt groeperen, klikt u op de knop **Bewerken** pictogram ![](assets/edit-icon.png) in de tabelkop.

1. Zoek in het rechterdeelvenster het veld waarmee u de tabel wilt filteren en sleep deze naar de sectie Filter.

   Er wordt een filterregelset weergegeven met de naam van het veld dat u hebt geselecteerd.

1. Selecteer de gewenste operator in het keuzemenu:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Gelijk aan</strong> </td> 
      <td> <p>Hiermee wordt alleen een exacte overeenkomst met de gezochte waarde geretourneerd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Niet gelijk aan</strong> </td> 
      <td> <p>Hiermee worden alleen resultaten geretourneerd die niet exact overeenkomen met de gezochte waarde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is leeg</strong> </td> 
      <td> <p>Het veld bestaat voor het object, maar aan het veld is nog geen waarde toegewezen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is niet leeg</strong> </td> 
      <td> <p>Het veld waarop u filtert, bestaat en heeft een waarde gekregen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is kleiner dan</strong> </td> 
      <td> <p>Hiermee zoekt u naar alle resultaten met een waarde die lager is dan de ingevoerde waarde, zonder de ingevoerde waarde op te nemen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>is kleiner dan of gelijk aan</strong> </td> 
      <td> <p>Hiermee zoekt u naar alle resultaten met een waarde die kleiner is dan of gelijk is aan de ingevoerde waarde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is groter dan</strong> </td> 
      <td> <p>Hiermee zoekt u naar alle resultaten met een waarde die groter is dan de ingevoerde waarde, zonder de ingevoerde waarde op te nemen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>is groter dan of gelijk aan</strong> </td> 
      <td> <p>Hiermee zoekt u naar alle resultaten met waarden die groter zijn dan of gelijk zijn aan de ingevoerde waarde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tussen</strong> </td> 
      <td> <p>Verstrekt 2 vereiste gebiedswaarden en onderzoeken naar alle resultaten binnen waaier van beide gebieden met inbegrip van de ingegaan waarden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Bevat</strong> </td> 
      <td> <p>Hiermee wordt naar de opgegeven tekst in een hele tekenreeks gezocht.</p> <p>Als u bijvoorbeeld "Bevat index" gebruikt, wordt er alles met "Inf" of "inf" vastgelegd, zoals het woord "Infinity".</p> <p>Opmerking: Adobe Workfront zoekt naar het volledige woord of de hele woordgroep die u voor elke filterregel invoert. Als u bijvoorbeeld velden zoekt met de uitdrukking "nieuw project" in de naam, geeft Workfront geen projecten weer die alleen "nieuw" of "project" in de naam hebben, of woorden die extra woorden bevatten tussen bijvoorbeeld "nieuw hoofdproject". Het filter vindt slechts projecten met de nauwkeurige uitdrukking "nieuw project"in de naam.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Bevat niet</strong> </td> 
      <td> <p>Hiermee worden items zonder opgegeven tekst gefilterd.</p> <p>Met 'bevat geen inf' worden bijvoorbeeld velden geretourneerd zonder 'Inf' of 'inf' in de naam.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Voer de laatste waarde in om de filterregel te voltooien op basis van de operator die u hebt geselecteerd.

   >[!NOTE]
   >
   >Hier ingevoerde waarden zijn **niet** hoofdlettergevoelig.

1. (Optioneel) Ga als volgt te werk om een andere filterregel aan de regelset toe te voegen:

   1. Sleep een ander veld naar de **Neerzetten om een andere regel toe te voegen** in de sectie Filters onder de andere regel.
   1. Herhaal stap 4-6.
   1. Selecteer in de linkerbenedenkeuzelijst van de operator van de nieuwe regel de optie **EN** of **OF**.

      <table style="table-layout:auto"> 
       <col> 
       </col> 
       <col> 
       </col> 
       <tbody> 
        <tr> 
         <td role="rowheader"> <p>EN</p> </td> 
         <td> <p>Wanneer u zich bij filterregels of regelreeksen met de operator AND aansluit, geeft u aan dat u aan alle regels op hetzelfde niveau wilt voldoen.</p> <p>Standaard worden de instructies in een filter samengevoegd met de operator AND.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"> <p>OF</p> </td> 
         <td> <p>Wanneer u zich bij filterregels of regelreeks met OR exploitant aansluit, wijst u erop dat u wilt <strong>ten minste</strong> één regel-of regel plaats-op dat niveau om te ontmoeten.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >EN OF de exploitanten op het zelfde niveau-verbindend of veelvoudige regels binnen een regelreeks of volledige regelreeksen samen-zullen altijd aanpassen. Als u bijvoorbeeld de operator wijzigt tussen twee regels binnen een regelset, worden alle andere operatoren in die regelset automatisch aangepast.

1. (Voorwaardelijk) Om een extra reeks van de filterregel toe te voegen, doe het volgende:

   1. Sleep het veld dat u wilt toevoegen aan het dialoogvenster **Een regelset toevoegen** gebied onder de andere filterregelsets.
   1. Herhaal stap 4-7.
   1. Selecteer in het keuzemenu links van de nieuwe regelset de optie **EN** of **OF**. Deze operatoren werken hetzelfde als in stap 7, maar zijn van toepassing op hele regelsets in tegenstelling tot afzonderlijke regels binnen een set.****
