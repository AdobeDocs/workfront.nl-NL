---
title: Een tabel filteren in Rapportcanvas
description: Een tabel filteren in Rapportcanvas
hidefromtoc: true
hide: true
exl-id: 1838b142-d845-4795-b27f-80bfba18e9d4
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '871'
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

**Voorbeeld:** als u resultaten in uw rapport aan slechts vertoningsprojecten wilde beperken die door Jansen worden bezeten, kon u een filterregel met het gebied &quot;de Eigenaar van het Project,&quot;de exploitant &quot;Gelijk aan,&quot;en de waarde &quot;Jansen&quot;tot stand brengen.

Of u kon slechts projecten tonen die een toegewezen projecteigenaar hebben, die het gebied &quot;de Eigenaar van het Project&quot;en de exploitant &quot;niet leeg zou hebben.&quot;

## Vereisten

Alvorens u begint, moet u in de bèta van het Canvas van de Rapportering inschrijven. Voor meer informatie, zie [&#x200B; Rapporterend de bèta van het Canvas: overzicht &#x200B;](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Filterregels voor een tabel configureren

1. Klik het **pictogram van het 1&rbrace; pictogram van het Belangrijkste Menu ![&#x200B; &#x200B;](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik** Meldend **.**

1. Klik **Nieuw rapport**.

   of

   Ga naar een bestaand rapport, klik het **Meer pictogram van het Menu** ![&#x200B; Meer pictogram &#x200B;](assets/more-icon.png) in de rapportkopbal, dan uitgezocht **geef** uit.

1. Als u rijen op een nieuwe tabel wilt groeperen, sleept u een tabelblok naar het canvas of dubbelklikt u erop.

   of

   Om rijen op een bestaande lijst te groeperen, klik **uitgeven** pictogram ![&#x200B; pictogram &#x200B;](assets/edit-icon.png) in de lijstkopbal uitgeven.

1. Zoek in het rechterdeelvenster het veld waarmee u de tabel wilt filteren en sleep deze naar de sectie Filter.

   Er wordt een filterregelset weergegeven met de naam van het veld dat u hebt geselecteerd.

1. Selecteer de gewenste operator in het keuzemenu:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> Gelijk aan </strong> </td> 
      <td> <p>Hiermee wordt alleen een exacte overeenkomst met de gezochte waarde geretourneerd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> niet gelijk aan </strong> </td> 
      <td> <p>Hiermee worden alleen resultaten geretourneerd die niet exact overeenkomen met de gezochte waarde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> is leeg </strong> </td> 
      <td> <p>Het veld bestaat voor het object, maar aan het veld is nog geen waarde toegewezen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> is niet leeg </strong> </td> 
      <td> <p>Het veld waarop u filtert, bestaat en heeft een waarde gekregen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> is minder dan </strong> </td> 
      <td> <p>Hiermee zoekt u naar alle resultaten met een waarde die lager is dan de ingevoerde waarde, zonder de ingevoerde waarde op te nemen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> is minder dan of gelijk aan </strong> </td> 
      <td> <p>Hiermee zoekt u naar alle resultaten met een waarde die kleiner is dan of gelijk is aan de ingevoerde waarde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> is groter dan </strong> </td> 
      <td> <p>Hiermee zoekt u naar alle resultaten met een waarde die groter is dan de ingevoerde waarde, zonder de ingevoerde waarde op te nemen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> is groter dan of gelijk aan </strong> </td> 
      <td> <p>Hiermee zoekt u naar alle resultaten met waarden die groter zijn dan of gelijk zijn aan de ingevoerde waarde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> tussen </strong> </td> 
      <td> <p>Verstrekt 2 vereiste gebiedswaarden en onderzoeken naar alle resultaten binnen waaier van beide gebieden met inbegrip van de ingegaan waarden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> bevat </strong> </td> 
      <td> <p>Hiermee wordt naar de opgegeven tekst in een hele tekenreeks gezocht.</p> <p>Als u bijvoorbeeld "Bevat index" gebruikt, wordt er alles met "Inf" of "inf" vastgelegd, zoals het woord "Infinity".</p> <p>Opmerking: Adobe Workfront zoekt naar het volledige woord of de hele woordgroep die u voor elke filterregel invoert. Als u bijvoorbeeld velden zoekt met de uitdrukking "nieuw project" in de naam, geeft Workfront geen projecten weer die alleen "nieuw" of "project" in de naam hebben, of woorden die extra woorden bevatten tussen bijvoorbeeld "nieuw hoofdproject". Het filter vindt slechts projecten met de nauwkeurige uitdrukking "nieuw project"in de naam.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> bevat niet </strong> </td> 
      <td> <p>Hiermee worden items zonder opgegeven tekst gefilterd.</p> <p>Met 'bevat geen inf' worden bijvoorbeeld velden geretourneerd zonder 'Inf' of 'inf' in de naam.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Voer de laatste waarde in om de filterregel te voltooien op basis van de operator die u hebt geselecteerd.

   >[!NOTE]
   >
   >De waarden ingegaan hier zijn **niet** gevoelig geval.

1. (Optioneel) Ga als volgt te werk om een andere filterregel aan de regelset toe te voegen:

   1. Sleep een ander gebied aan de **Daling om een ander regel** gebied in de sectie van Filters onder uw andere regel toe te voegen.
   1. Herhaal stap 4-6.
   1. In de exploitant drop-down linkerzijde van de nieuwe regel, uitgezochte **EN** of **OF**.

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
         <td> <p>Wanneer u zich bij filterregels of regel aansluit die met OF exploitant wordt geplaatst wijst u erop dat u <strong> minstens </strong> één regel-of regel plaats-op dat niveau wilt om worden ontmoet.</p> </td> 
        </tr> 
       </tbody> 
      </table>

      >[!IMPORTANT]
      >
      >EN OF de exploitanten op het zelfde niveau-verbindend of veelvoudige regels binnen een regelreeks of volledige regelreeksen samen-zullen altijd aanpassen. Als u bijvoorbeeld de operator wijzigt tussen twee regels binnen een regelset, worden alle andere operatoren in die regelset automatisch aangepast.

1. (Voorwaardelijk) Om een extra reeks van de filterregel toe te voegen, doe het volgende:

   1. Sleep het gebied dat u aan **wilt toevoegen voegt een regelreeks** gebied onder uw andere reeksen van de filterregel toe.
   1. Herhaal stap 4-7.
   1. In de exploitant drop-down linkerzijde van de nieuwe regelreeks, uitgezochte **EN** of **OF**. Deze operatoren werken hetzelfde als in stap 7, maar zijn van toepassing op hele regelsets in tegenstelling tot afzonderlijke regels binnen een set.**&#x200B;**
