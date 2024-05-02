---
title: Een tabelkolom configureren in het rapportcanvas
description: Een tabelkolom configureren in het rapportcanvas
hidefromtoc: true
hide: true
exl-id: ce33888f-344d-4f69-b527-9679340d134b
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 0%

---

# Een tabelkolom configureren in het rapportcanvas

De kolommen in een lijst kunnen voor vertoning worden gevormd. U kunt de volgende aspecten van een kolom wijzigen:

* Naam
* Sorteren
* Machtiging bewerken
* Tekst boven
* Samenvoeging
* Voorwaardelijke opmaak

## Vereisten

Alvorens u begint, moet u in de bèta van het Canvas van de Rapportering inschrijven. Zie voor meer informatie [Bewerken van canvas melden: overzicht](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Kolommen in een tabel wijzigen

1. Ga naar een bestaand rapport, klik op de knop **Meer menu** pictogram ![](assets/more-icon.png) in de rapportkopbal, dan selecteer **Bewerken**.
1. Voor de lijstkopbal in het rapport, klik **Bewerken** pictogram ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Als u de tabel hebt gemaakt en nog geen velden hebt toegevoegd, klikt u in plaats daarvan op de knop Bewerken in het midden van de tabel.

1. (Optioneel) Voeg kolommen in de tabel toe, verplaats deze of verwijder deze. Zie voor meer informatie over het bewerken van de velden in een tabel [Een tabelblok toevoegen of bewerken in het rapportcanvas](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md)

   | Een nieuwe kolom toevoegen | Als u een kolom aan een tabel wilt toevoegen, klikt u op een veld en sleept u het veld van het gereedschap **Velden** rechts van de pagina op de tabel waar u de pagina wilt plaatsen of dubbelklik op een veld om de pagina toe te voegen als de meest rechtse kolom. |
   |---|---|
   | Een kolom verplaatsen | Als u de volgorde van kolommen in een tabel wilt wijzigen, klikt u op de naam van een kolom en sleept u deze naar een nieuwe locatie. |
   | Een kolom verwijderen | Als u een kolom uit een tabel wilt verwijderen, klikt u op de kolom die u wilt verwijderen en klikt u op de x aan de rechterkant van de kolomnaam. |

   {style="table-layout:auto"}

1. Als u een kolom wilt configureren, klikt u op de naam van de kolom die u wilt wijzigen in de koptekstrij van de tabel en vervolgens op een van de volgende tabbladen in het rechterdeelvenster:

   <table style="table-layout:auto"> 
    <col> class="TableStyle-TableStyle-List-options-in-stappen-Column-Column1" /&gt;
    <tbody>
     <tr data-mc-conditions="">
      <th role="rowheader" colspan="2">Tabblad Gegevens</th>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Geaggregeerd op basis van</td>
      <td><p> Als u de gegevens in een kolom wilt samenvoegen (samenvatten in de koptekst), selecteert u het gewenste type samenvoeging in het dialoogvenster <strong>Geaggregeerd op basis van</strong> vervolgkeuzelijst. Welke opties beschikbaar zijn, is afhankelijk van het type gegevens in de kolom.</p><p>Als u groepen in de tabel gebruikt, wordt de samengevoegde waarde weergegeven in de groepstrij boven de kolomnaam in plaats van naast de kolomnaam.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Veldindeling</td>
      <td><p>(Alleen beschikbaar als de kolom datum-, percentage-, valuta- of tijdgegevens bevat, niet tekst.) Selecteer de gewenste indeling voor de gegevens in het dialoogvenster <b>Veldindeling</b> vervolgkeuzelijst. U kunt bijvoorbeeld percentagetekens weergeven na de getallen in een kolom of de manier wijzigen waarop datums worden weergegeven.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Veld kan worden bewerkt</td>
      <td><span>De optie <strong>Veld kan worden bewerkt</strong> als u wilt toestaan dat gebruikers die de tabel weergeven de naam van de kolom kunnen bewerken.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Sorteren</strong></td>
      <td><p>Standaard sorteert de tabel op basis van de gegevens in oplopende volgorde in de kolom helemaal links. Als u op de geselecteerde kolom wilt sorteren, klikt u op de pijl-omlaag naast <strong>Sorteren</strong>en klik vervolgens op het selectievakje <b>Sorteren op deze kolom</b>. U kunt vervolgens een <strong>Sorteren</strong> richting (oplopende of aflopende waarden) en een <strong>Sorteervolgorde</strong> (de relatieve sorteerprioriteit van deze kolom in vergelijking met andere sorteerkolommen in de tabel).</p><p>U kunt dit proces herhalen om de tabel met maximaal vijf verschillende kolommen te sorteren. Zorg ervoor dat elke kolom de juiste waarde heeft <strong>Sorteervolgorde</strong> ten opzichte van eventuele nieuwe kolommen die u selecteert om te sorteren.</p><p>Opmerking: als u een kolom verwijdert die is geselecteerd om een tabel te sorteren en er een andere kolom is geselecteerd om te sorteren, wordt die kolom gebruikt om de tabel in aflopende volgorde te sorteren. Als er geen andere kolommen zijn geselecteerd om te sorteren, keert de lijst aan het gebrek terug: sorterend door zijn eerste kolom.</p><p>Wanneer u een kolom aanwijst om de tabel te sorteren, wordt naast de kolomnaam een klein vak weergegeven met een getal dat de relatieve prioriteit van die kolom aangeeft bij het sorteren van de tabel (de tabel wordt eerst gesorteerd op 1, vervolgens op 2, enzovoort) en een pijl om aan te geven of de sorteerrichting oplopend of aflopend is. </p><p><img src="assets/sorting-indicator-350x170.png" style="width: 350;height: 170;"></p></td>
     </tr>
    </tbody>
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <th role="rowheader" colspan="2">Het tabblad Stijl</th> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aangepast kolomlabel</strong> </td> 
      <td>Voer een nieuwe weergavenaam in voor de kolom (maximaal 100 tekens).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hoektekst tonen</td> 
      <td> <p>Bepaal of u verklarende tekst wilt tonen wanneer iemand over een kolomnaam beweegt.</p> <p>Deze optie is standaard uitgeschakeld.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tekst boven</td> 
      <td>(Alleen beschikbaar als <strong>Hoektekst tonen</strong> is ingeschakeld.) Pas de verklarende tekst aan die toont wanneer iemand over een kolomnaam beweegt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Voorwaardelijke opmaak</strong> </td> 
      <td> 
       <ol data-mc-continue="false"> 
        <li value="1"> <p>Toevoegen <img src="assets/add-rule.png">, bewerken <img src="assets/edit-icon.png">, of verwijderen <img src="assets/delete.png"> een regel die cellen in de kolom formatteert wanneer hun waarden aan criteria voldoen u specificeert.</p> <p>U kunt bijvoorbeeld een regel maken die het lettertype in het veld Projectstatus wijzigt in vet paars wanneer de waarde van dat veld gelijk is aan "Samenstellen".</p> <p>Of u kunt <b>Pictogram weergeven</b> om een groen vlagpictogram aan elk punt in de kolom toe te voegen dat de "Huidige"status heeft.</p> <p> <img src="assets/conditional-formatting-options.png"> </p> <p>Opmerking: als u <strong>Pictogram weergeven</strong>, zijn de andere opmaakopties niet beschikbaar.</p> <p>U kunt <strong>Toepassen op de hele rij</strong> als u het formatteren de volledige rij van een cel wilt beïnvloeden die aan de voorwaarde van uw regel voldoet. U kunt bijvoorbeeld projecten markeren die na een bepaalde datum worden uitgevoerd door een gele achtergrondkleur toe te passen op niet alleen de datumcellen in de kolom "Vereist", maar op de hele rij waar die datums voorkomen.</p> <p>Tip: als u opmaakopties aan een regel toevoegt, wordt de resulterende celopmaak weergegeven onder <strong>Voorvertoning</strong> onder aan het deelvenster.</p> </li> 
        <li value="2">Wanneer u klaar bent met het toevoegen van een regel, klikt u op <strong>Opslaan</strong>.</li> 
        <li value="3"> <p>(Optioneel) Klik op <b>+ Regel toevoegen</b> om extra regels aan de zelfde kolom toe te voegen.</p> <p>Meerdere regels voor voorwaardelijke opmaak in een tabel worden in de volgende volgorde toegepast:</p> 
         <ul> 
          <li> <p>De regels die op volledige rijen van toepassing zijn worden eerst geëvalueerd, van links naar rechts voor elke kolom en dan van boven naar onder binnen een kolom.</p> <p>Opmerking: Rijopmaak heeft voorrang op andere voorwaardelijke opmaak voor cellen in die rij, zelfs als ze anders aan de voorwaarde van de regel van een andere kolom zouden voldoen.</p> </li> 
          <li> <p>Andere regels worden hierna geëvalueerd, van boven naar beneden aangezien zij in het juiste paneel voor een kolom worden vermeld. U kunt slepen <img src="assets/drag-object-icon.png"> opgeslagen regels in dat deelvenster om de volgorde te wijzigen.</p> <p>Opmerking: cellen worden opgemaakt op basis van de eerste voorwaarde waaraan ze voldoen en worden niet verder opgemaakt, zelfs niet als ze aan andere voorwaarden voldoen.</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op de knop **Terug** pijl in de linkerbovenhoek van het scherm om naar uw rapport terug te keren.
