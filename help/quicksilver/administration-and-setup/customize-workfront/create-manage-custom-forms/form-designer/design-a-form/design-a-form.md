---
title: Een formulier ontwerpen met de formulierontwerper
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: U kunt een aangepast formulier ontwerpen met de formulierontwerper.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: b56cf20e054b2658ade8aef6c179128e001603c2
workflow-type: tm+mt
source-wordcount: '3803'
ht-degree: 0%

---


# Een formulier ontwerpen met de formulierontwerper

{{highlighted-preview-article-level}}

U kunt een aangepast formulier ontwerpen met de formulierontwerper. U kunt aangepaste formulieren aan verschillende Workfront-objecten koppelen om gegevens over die objecten vast te leggen.

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-abonnement*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td>
   <p>Huidig plan: Standaard</p>
   <p>of</p>
   <p>Ouder plan: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> <p>Ga voor informatie over hoe Workfront-beheerders deze toegang verlenen naar <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, type licentie of configuraties op toegangsniveau u hebt.

## Beginnen met het ontwerpen van een aangepast formulier

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Aangepaste Forms** in het linkerdeelvenster.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Klikken **Nieuw aangepast formulier.**
1. Selecteer de objecttypen waaraan u het aangepaste formulier wilt koppelen en klik vervolgens op **Doorgaan**.

   ![](assets/choose-object-type.jpg)

1. In de **Titel is vereist** in, typt u de aangepaste titel van het formulier.
1. (Optioneel) Als u meer objecttypen aan het formulier wilt toevoegen zodat het aan meer objecten kan worden gekoppeld, klikt u op de knop **Toevoegen** pictogram ![](assets/add-objects-icon.png) na **Objecttypen** Selecteer vervolgens de gewenste tekst in het menu dat wordt weergegeven. U kunt dit herhalen om zoveel objecttypen toe te voegen als u wilt.

   U kunt ook op de X op een objecttype klikken om het uit het formulier te verwijderen.

   >[!CAUTION]
   >
   >Als u een aangepast formulier verwijdert, worden ook alle aangepaste gegevens verwijderd over de objecten die aan het formulier zijn gekoppeld. De verwijderde gegevens kunnen niet worden hersteld. U kunt in plaats daarvan een aangepast formulier deactiveren. Wanneer u een aangepast formulier deactiveert dat u niet meer gebruikt, behoudt u alle bijbehorende historische gegevens.
   >
   >Zie voor meer informatie [Objecttypen verwijderen op een aangepast formulier](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).


1. Vervolgens kunt u velden toevoegen aan uw aangepaste formulier. Zie de volgende secties:
   * [Een bestaand veld of een bestaande widget opnieuw gebruiken die al in een ander aangepast formulier wordt gebruikt](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Tekstvelden toevoegen](#add-text-fields)
   * [Berekende velden toevoegen](#add-calculated-fields)
   * [Keuzerondjes, groep selectievakjes en vervolgkeuzelijsten toevoegen](#add-radio-buttons-checkboxes-and-dropdowns)
   * [Velden voor typekop en datum toevoegen](#add-typeahead-and-date-fields)
   * [Afbeeldingen, PDF en video&#39;s toevoegen](#add-images-pdfs-and-videos)
   * [Adobe XD-bestanden toevoegen](#add-adobe-xd-files)

## Nieuwe of bestaande velden toevoegen aan uw aangepaste formulier

U kunt nieuwe of bestaande velden gebruiken bij het ontwerpen van uw aangepaste formulier.

## Een bestaand veld of een bestaande widget opnieuw gebruiken die al in een ander aangepast formulier wordt gebruikt

1. Klik in de linkerbovenhoek van het scherm op **Veldbibliotheek**.

1. Sleep het veld of de widget naar de gewenste positie in het aangepaste formulier.
1. (Optioneel) Herhaal de vorige stap om andere velden of widgets toe te voegen.

   >[!NOTE]
   >
   >U kunt maximaal 500 velden en widgets toevoegen aan ????n aangepast formulier. De prestaties kunnen echter afnemen wanneer er meer dan 100 formulieren op een formulier staan, afhankelijk van de complexiteit ervan.
   >
   >
   >Voorbeelden van complexe formulieren zijn formulieren met trapsgewijze parameters, berekende aangepaste gegevensvelden en opties voor meerdere waarden in ????n veld.

1. Klik op **Toepassen** en ga naar een andere sectie om door te gaan met het samenstellen van uw formulier.

   of

   Klikken **Opslaan en sluiten**.

### Tekstvelden toevoegen

U kunt verschillende tekstvelden toevoegen aan een aangepast formulier.

+++ **Uitbreiden om beschrijvingen van beschikbare tekstvelden weer te geven**

* **Tekstveld met ????n regel**: Hiermee kunnen gebruikers ????n regel tekst in het veld typen.
* **Alineatekstveld**: Hiermee kunnen gebruikers meerdere tekstregels in het veld typen.
* **Tekstveld met opmaak**: Hiermee kunnen gebruikers meerdere tekstregels in het veld typen en de tekst opmaken met vet, cursief, onderstrepen, opsommingstekens, nummering, hyperlinks en blokaanhalingstekens. Een tekenlimiet van 15.000 staat voor veel tekst en opmaak toe.

   Zie Opslag van rijke tekstvelden in de API voor informatie over toegang tot dit veld via de API.

   >[!NOTE]
   >
   >Tekstvelden met opmaak zijn niet beschikbaar voor mobiele Workfront-apps (beschikbaar in volgende versies).

* **Beschrijvende tekst**: Hiermee kunt u instructies en koppelingen naar pagina&#39;s buiten Workfront opnemen.

+++

Een tekstveld toevoegen:

1. Zoek links in het scherm een van de volgende tekstvelden en sleep deze naar een sectie op het canvas:

   * Tekst met ????n regel:
   * Alineatekst
   * Tekstveld met opmaak
   * Beschrijvende tekst

   ![](assets/drag-field-to-section.png)

1. Configureer rechts in het scherm de opties die beschikbaar zijn voor het type aangepast veld dat u toevoegt:

   <table>
    <tr>
    <td>Invoer naar</td>
    <td>Beschrijving</td>
    <td>Beschikbaar voor </td>
    </tr>
    <tr>
    <td>Grootte</td>
    <td><p>Wijzig de grootte van de tekstvelden op het formulier.<p>
   </td>
    <td><ul>
    <li>Tekst met ????n regel</li>
    <li>Alineatekst</li>
    <li>Tekst met opmaak</li>
    <li>Beschrijvende tekst - Binnenkort beschikbaar</li>
    </ul></td>
    </tr>
    <tr>
    <td>Label</td>
    <td><p>Typ een beschrijvend label dat boven de widget moet worden weergegeven. U kunt het label op elk gewenst moment wijzigen.<p>
    <p>BELANGRIJK: Gebruik geen speciale tekens in dit label. Ze worden niet correct weergegeven in rapporten.</p></td>
    <td><ul>
    <li>Tekst met ????n regel</li>
    <li>Alineatekst</li>
    <li>Tekst met opmaak</li>
    </ul></td>
    </tr>
    <tr>
     <td>Naam</td>
    <td><p>(Vereist) Met deze naam geeft het systeem het veld aan. Wanneer u de widget voor het eerst configureert en u typt het label, wordt het veld Naam automatisch aangepast. Maar de gebieden van het Etiket en van de Naam zijn niet gesynchroniseerd-dit geeft u de vrijheid om het etiket te veranderen dat uw gebruikers zien zonder het moeten de naam veranderen die het systeem ziet.</p>
    <p><b>BELANGRIJK</b>:   
      <ul> 
      <li>Hoewel dit mogelijk is, raden we u aan deze naam niet te wijzigen nadat u of andere gebruikers het aangepaste formulier in Workfront hebben gebruikt. Als u dat doet, herkent het systeem niet langer het aangepaste veld waar er nu naar wordt verwezen in andere gebieden van Workfront. <p>Bijvoorbeeld, als u het douanegebied aan een rapport toevoegt en later zijn naam verandert, herkent Workfront het niet in het rapport en het zal daar ophouden correct te werken tenzij u het aan het rapport gebruikend de nieuwe naam opnieuw toevoegt.</p> </li>
      <li> <p>We raden u aan geen naam te typen die al wordt gebruikt voor ingebouwde Workfront-velden.</p> </li>
      <li><p>We raden u aan het teken punt/punt niet te gebruiken in de aangepaste veldnaam om fouten te voorkomen bij het gebruik van het veld in verschillende gebieden van Workfront.</p></li>
    </td>
    <td><ul>
    <li>Tekst met ????n regel</li>
    <li>Alineatekst</li>
    <li>Tekst met opmaak</li>
    <li>Beschrijvende tekst</li>
    </ul></td>
    </tr>
    <tr>
    <td>Instructies</td>
    <td>Typ eventuele aanvullende informatie over de widget. Wanneer gebruikers het aangepaste formulier invullen, kunnen ze de muisaanwijzer boven het pictogram van het vraagteken plaatsen om knopinfo weer te geven met de informatie die u hier typt.
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>Tekst met ????n regel</li>
    <li>Alineatekst</li>
    <li>Tekst met opmaak</li>
    </ul></td>
    </tr>
    <tr>
    <td>Indeling</td>
    <td><p>Selecteer het type gegevens dat in het aangepaste veld wordt vastgelegd.</p> <p><b>OPMERKING</b>:   
    <ul> 
    <li>Dit veld kan niet worden bewerkt nadat het formulier is opgeslagen. Als u het veld wilt gebruiken voor wiskundige berekeningen, selecteert u een getal- of valutanotatie.<br></li> 
    <li>Als u Getal of Valuta selecteert, wordt het systeem automatisch gebruikt voor het afkappen van getallen die met 0 beginnen.</li> 
     </ul></p></td> </td>
    <td><ul>
    <li>Tekst met ????n regel</li>
    <li>Alineatekst</li>
    </ul></td>
    </tr>
    <tr>
    <td>Weergavetype</td>
    <td>Schakelen tussen tekstvelden met ????n regel en alineatekst.</td>
    <td><ul>
    <li>Tekst met ????n regel</li>
    <li>Alineatekst</li>
    </ul></td>
    </tr>
    <tr>
    <td>Hyperlink</td>
    <td> Als u een hyperlink wilt toepassen op de beschrijvende tekst die u hebt getypt, voegt u deze hier toe. De beschrijvende tekst wordt als een koppeling weergegeven op objecten waaraan het formulier is gekoppeld.</td>
    <td><ul><li>Beschrijvende tekst</li></ul></td>
    </tr>
   </table>

1. (Optioneel) Herhaal de vorige stap om andere velden of widgets toe te voegen.

   of

   Als u een veld wilt kopi??ren, plaatst u de muis boven een veld en klikt u op het pictogram Kopi??ren.

   ![pictogram kopi??ren](assets/copy-field.png)

1. Klik op **Toepassen** en ga naar een andere sectie om door te gaan met het samenstellen van uw formulier.

   of

   Klikken **Opslaan en sluiten**.

### Berekende velden toevoegen

In een aangepast formulier kunt u een berekend aangepast veld toevoegen waarin bestaande gegevens worden gebruikt om nieuwe gegevens te genereren wanneer het aangepaste formulier aan een object wordt gekoppeld.

Als u een berekend veld wilt toevoegen, raadpleegt u [Berekende velden toevoegen met de formulierontwerper](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### Keuzerondjes, selectievakjes en vervolgkeuzelijsten toevoegen

U kunt keuzerondjes, selectievakjes en vervolgkeuzelijsten toevoegen aan een aangepast formulier.

+++ **Uitbreiden om beschrijvingen van beschikbare velden weer te geven**

* **Keuzerondjes**: Gebruikers hoeven slechts ????n keuze te maken.
* **Groep selectievakjes**: Hiermee kunnen gebruikers meerdere keuzen selecteren.
* **Vervolgkeuzelijst**: Bevat een lijst met keuzemogelijkheden.

+++

Keuzerondjes en selectievakjes toevoegen:

1. Zoek links in het scherm een van de volgende velden en sleep deze naar een sectie op het canvas.

   * Keuzerondjes
   * Groep selectievakjes
   * Vervolgkeuzelijst

   ![](assets/drag-field-to-section.png)

1. Configureer rechts in het scherm de opties die beschikbaar zijn voor het type aangepast veld dat u toevoegt:

   <table style="table-layout:auto"> 
    <tbody> 
    <tr>
    <td>Invoer naar</td>
    <td>Beschrijving</td>
    <td>Beschikbaar voor </td>
    </tr>
    <tr> 
     <td role="rowheader">Label</td> 
     <td> <p>(Vereist) Typ een beschrijvend label dat boven het aangepaste veld wordt weergegeven. U kunt het label op elk gewenst moment wijzigen.</p> <p><b>BELANGRIJK</b>: Gebruik geen speciale tekens in dit label. Ze worden niet correct weergegeven in rapporten.</p> </td> 
     <td><ul>
    <li>Keuzerondjes</li>
    <li>Groep selectievakjes</li>
    <li>Vervolgkeuzelijst</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">Naam</td> 
     <td> <p>(Vereist) Met deze naam identificeert het systeem het aangepaste veld wanneer u het toevoegt aan verschillende gebieden in Workfront, zoals rapporten, Home- en API-interacties.</p> <p>Wanneer u het aangepaste veld voor het eerst configureert en u typt het label, wordt het veld Naam automatisch aangepast. Maar de gebieden van het Etiket en van de Naam zijn niet gesynchroniseerd-dit geeft u de vrijheid om het etiket te veranderen dat uw gebruikers zien zonder het moeten de naam veranderen die het systeem ziet.</p> 
    <p><b>BELANGRIJK</b>:   
     <ul> 
    <li>Hoewel dit mogelijk is, raden we u aan deze naam niet te wijzigen nadat u of andere gebruikers het aangepaste formulier in Workfront hebben gebruikt. Als u dat doet, herkent het systeem niet langer het aangepaste veld waar er nu naar wordt verwezen in andere gebieden van Workfront. <p>Bijvoorbeeld, als u het douanegebied aan een rapport toevoegt en later zijn naam verandert, herkent Workfront het niet in het rapport en het zal daar ophouden correct te werken tenzij u het aan het rapport gebruikend de nieuwe naam opnieuw toevoegt.</p> </li>
    <li> <p>We raden u aan geen naam te typen die al wordt gebruikt voor ingebouwde Workfront-velden.</p> </li>
     <li><p>We raden u aan het teken punt/punt niet te gebruiken in de aangepaste veldnaam om fouten te voorkomen bij het gebruik van het veld in verschillende gebieden van Workfront.</p></li>
     </ul> <p>Elke aangepaste veldnaam moet uniek zijn in het Workfront-exemplaar van uw organisatie. Op deze manier kunt u een formulier hergebruiken dat al voor een ander aangepast formulier is gemaakt. Zie voor meer informatie <a href="#Add" class="MCXref xref">Een aangepast veld toevoegen aan een aangepast formulier</a> in dit artikel.</p> </td>
     <td><ul>
    <li>Keuzerondjes</li>
    <li>Groep selectievakjes</li>
    <li>Vervolgkeuzelijst</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Instructies</td> 
    <td> <p>Typ eventuele aanvullende informatie over het aangepaste veld. Wanneer gebruikers het aangepaste formulier invullen, kunnen ze de muisaanwijzer boven het pictogram van het vraagteken plaatsen om knopinfo weer te geven met de informatie die u hier typt.</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>Keuzerondjes</li>
    <li>Groep selectievakjes</li>
    <li>Vervolgkeuzelijst</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Indeling</td> 
    <td> <p>Selecteer het type gegevens dat in het aangepaste veld wordt vastgelegd.</p> <p><b>OPMERKING</b>:   
     <ul> 
    <li>Dit veld kan niet worden bewerkt nadat het formulier is opgeslagen. Als u het veld wilt gebruiken voor wiskundige berekeningen, selecteert u een getal- of valutanotatie.<br></li> 
    <li>Als u Getal of Valuta selecteert, wordt het systeem automatisch gebruikt voor het afkappen van getallen die met 0 beginnen.</li> 
     </ul></p></td> 
     <td><ul>
    <li>Keuzerondjes</li>
    <li>Groep selectievakjes</li>
    <li>Vervolgkeuzelijst</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">Weergavetype</td> 
    <td>Schakel tussen keuzerondjes, groepen selectievakjes of vervolgkeuzelijsten voor het veld.</td> 
    <td><ul>
    <li>Keuzerondjes</li>
    <li>Groep selectievakjes</li>
    <li>Vervolgkeuzelijst</li>
    </ul></td>
    </tr> 
     <tr> 
    <td role="rowheader">Een vereist veld maken</td> 
    <td>Selecteer deze optie als u wilt dat het veld verplicht is zodat de gebruiker het aangepaste formulier kan invullen. </td> 
    <td><ul>
    <li>Keuzerondjes</li>
    <li>Groep selectievakjes</li>
    <li>Vervolgkeuzelijst</li>
    </ul></td>
     </tr> 
    <tr> 
    <td role="rowheader">Keuzen </td> 
    <td> 
    <ol> 
    <li> <p>Klikken <b>Opties</b>Schakel vervolgens een van de volgende opties in:</p> 
    <ul> 
    <li><strong>Waarden tonen</strong>: Hiermee worden de waarden van elke keuze in het veld weergegeven. Het label van elke keuze wordt standaard weergegeven.</li> 
     <li><strong>Keuzen A-Z sorteren</strong>: Hiermee sorteert u de opties die u alfabetisch in het veld toevoegt.</li> 
    </ul> 
    </li> 
    <li> <p>Voor elke keuze die u voor de gebruiker toevoegt, klikt u op het tandwielpictogram <img src="assets/gear-icon-settings.png">Selecteer vervolgens een van de volgende opties:</p> 
    <ul> 
    <li><strong>Standaard selecteren</strong>: Selecteer standaard de keuze in het veld.</li> 
    <li> <p><strong>Keuze verbergen</strong>: Verberg de keuze in het veld. Verborgen keuzen blijven beschikbaar in rapporten.</p> </li> 
    <li> <p><strong>Keuze verwijderen</strong>: De keuze uit het veld verwijderen.</p> <p><b>WAARSCHUWING</b>: Als deze optie wordt gebruikt voor huidige objecten, verwijdert u deze niet uit het veld. Als u deze regel verwijdert, gaan historische gegevens verloren. Selecteer in plaats daarvan de optie om deze te verbergen, zodat gebruikers deze optie in de toekomst niet meer kunnen selecteren.</p> </li> 
    </ul> 
     </li> 
    </ol> </td> 
    <td><ul>
    <li>Keuzerondjes</li>
    <li>Groep selectievakjes</li>
    <li>Vervolgkeuzelijst</li>
    </ul></td>
     </tr> 
    </tbody> 
    </table>

1. (Optioneel) Herhaal de vorige stap om andere velden of widgets toe te voegen.

   of

   Als u een veld wilt kopi??ren, plaatst u de muis boven een veld en klikt u op het pictogram Kopi??ren.

   ![pictogram kopi??ren](assets/copy-field.png)

1. Klik op **Toepassen** en ga naar een andere sectie om door te gaan met het samenstellen van uw formulier.

   of

   Klikken **Opslaan en sluiten**.

### Velden voor typekop en datum toevoegen

U kunt datum- en tekstvelden toevoegen aan een aangepast formulier.

+++ **Uitbreiden om beschrijvingen van beschikbare velden weer te geven**

* **Typeahead**: Hiermee kunnen gebruikers de naam typen van een object dat in Workfront bestaat. Er wordt een lijst met suggesties weergegeven wanneer de gebruiker begint te typen. Dit veldtype ondersteunt de volgende objecten:
   * Gebruiker
   * Groep
   * Functie
   * Portfolio
   * Programma
   * Project
   * Team
   * Sjabloon
   * Bedrijf
* **Datumveld**: Hiermee geeft u een kalender weer waarin gebruikers een datum en tijd kunnen selecteren.

+++

U voegt als volgt velden voor de typekop toe:

1. Zoek links in het scherm een van de volgende velden en sleep deze naar een sectie op het canvas.

   * Typeahead
   * Datumveld

   ![](assets/drag-field-to-section.png)

1. Configureer rechts in het scherm de opties die beschikbaar zijn voor het type aangepast veld dat u toevoegt:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr>
    <td>Veldinstelling</td>
    <td>Beschrijving</td>
    <td>Beschikbaar voor </td>
    </tr>
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Vereist) Typ een beschrijvend label dat boven het aangepaste veld wordt weergegeven. U kunt het label op elk gewenst moment wijzigen.</p> <p><b>BELANGRIJK</b>: Gebruik geen speciale tekens in dit label. Ze worden niet correct weergegeven in rapporten.</p> </td> 
       <td><ul>
    <li>Typeahead</li>
    <li>Datumveld</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Naam</td> 
      <td> <p>(Vereist) Met deze naam identificeert het systeem het aangepaste veld wanneer u het toevoegt aan verschillende gebieden in Workfront, zoals rapporten, Home- en API-interacties.</p> <p>Wanneer u het aangepaste veld voor het eerst configureert en u typt het label, wordt het veld Naam automatisch aangepast. Maar de gebieden van het Etiket en van de Naam zijn niet gesynchroniseerd-dit geeft u de vrijheid om het etiket te veranderen dat uw gebruikers zien zonder het moeten de naam veranderen die het systeem ziet.</p> 
      <p><b>BELANGRIJK</b>:   
      <ul> 
      <li>Hoewel dit mogelijk is, raden we u aan deze naam niet te wijzigen nadat u of andere gebruikers het aangepaste formulier in Workfront hebben gebruikt. Als u dat doet, herkent het systeem niet langer het aangepaste veld waar er nu naar wordt verwezen in andere gebieden van Workfront. <p>Bijvoorbeeld, als u het douanegebied aan een rapport toevoegt en later zijn naam verandert, herkent Workfront het niet in het rapport en het zal daar ophouden correct te werken tenzij u het aan het rapport gebruikend de nieuwe naam opnieuw toevoegt.</p> </li>
      <li> <p>We raden u aan geen naam te typen die al wordt gebruikt voor ingebouwde Workfront-velden.</p> </li>
      <li><p>We raden u aan het teken punt/punt niet te gebruiken in de aangepaste veldnaam om fouten te voorkomen bij het gebruik van het veld in verschillende gebieden van Workfront.</p></li>
      </ul> <p>Elke aangepaste veldnaam moet uniek zijn in het Workfront-exemplaar van uw organisatie. Op deze manier kunt u een formulier hergebruiken dat al voor een ander aangepast formulier is gemaakt. Zie voor meer informatie <a href="#Add" class="MCXref xref">Een aangepast veld toevoegen aan een aangepast formulier</a> in dit artikel.</p> </td>
         <td><ul>
    <li>Typeahead</li>
    <li>Datumveld</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Instructies</td> 
      <td> <p>Typ eventuele aanvullende informatie over het aangepaste veld. Wanneer gebruikers het aangepaste formulier invullen, kunnen ze de muisaanwijzer boven het pictogram van het vraagteken plaatsen om knopinfo weer te geven met de informatie die u hier typt.</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>Typeahead</li>
    <li>Datumveld</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Tijd van dag weergeven</td> 
      <td>Selecteer deze optie als u de tijd van dag samen met de datum in het gebied wilt tonen.</td> 
         <td><ul>
    <li>Datumveld</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Type object waarnaar wordt verwezen</td> 
      <td> <p>Selecteer het objecttype dat u aan het veld wilt koppelen.</p> <p>Nadat u op Toepassen of Opslaan+Sluiten hebt geklikt, kunt u het objecttype voor het veld niet meer wijzigen.</p> <p><b>OPMERKING</b>:   
        <ul> 
         <li>Als uw Workfront-beheerder de naam voor Portfolio, Programma's of Projecten heeft aangepast in de Workfront-gebruikersinterface, wordt de standaardnaam voor Workfront voor het object weergegeven in deze vervolgkeuzelijst en niet de aangepaste naam. Raadpleeg uw Workfront-beheerder als u hier hulp bij nodig hebt.<br></li> 
         <li>De volgende objecttypen worden ondersteund in de mobiele apps van iOS en Android Workfront: Gebruiker, Bedrijf, Groep, de Rol van de Baan, Portfolio, Programma, Project, en Malplaatje.</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>Typeahead</li>
    </ul></td>
     </tr>
     <tr> 
      <td role="rowheader">Een vereist veld maken</td> 
      <td>Selecteer deze optie als u wilt dat het veld verplicht is zodat de gebruiker het aangepaste formulier kan invullen. </td> 
       <td><ul>
    <li>Typeahead</li>
    <li>Datumveld</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Herhaal de vorige stap om andere velden of widgets toe te voegen.

   of

   Als u een veld wilt kopi??ren, plaatst u de muis boven een veld en klikt u op het pictogram Kopi??ren.

   ![pictogram kopi??ren](assets/copy-field.png)

1. Klik op **Toepassen** en ga naar een andere sectie om door te gaan met het samenstellen van uw formulier.

   of

   Klikken **Opslaan en sluiten**.

### Afbeeldingen, PDF en video&#39;s toevoegen

U kunt afbeeldingen, PDF en video&#39;s toevoegen aan een aangepast formulier. Gebruikers die werken met het object waaraan het aangepaste formulier is gekoppeld, kunnen de afbeelding, de PDF of de video alleen in de volgende gebieden bekijken:

* Het gebied van Details van het voorwerp (bijvoorbeeld, voor een project, het gebied van de Details van het Project)
* Het vak Bewerken voor het object als dit de nieuwe Adobe Workfront-ervaring bevat die er uitziet (bijvoorbeeld de vakken Project bewerken en Taak bewerken)

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:???
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

+++ **Uitbreiden om beschrijvingen van beschikbare velden weer te geven**

* **Afbeelding**: Hiermee kunnen gebruikers _____ afbeeldingsbestanden toevoegen.
* **PDF**: Hiermee kunnen gebruikers PDF toevoegen
* **Video&#39;s**: Hiermee kunnen gebruikers ____ videobestanden toevoegen.

+++

Een afbeelding, PDF of video toevoegen:

1. Zoek links in het scherm een van de volgende velden en sleep deze naar een sectie op het canvas.

   * Afbeelding
   * PDF
   * Video

   ![](assets/drag-field-to-section.png)

1. Typ of bewerk een van de volgende eigenschappen voor de widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Vereist) Typ een beschrijvend label dat boven de widget moet worden weergegeven. U kunt het label op elk gewenst moment wijzigen.</p> <p><b>BELANGRIJK</b>: Gebruik geen speciale tekens in dit label. Ze worden niet correct weergegeven in rapporten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Naam</td> 
      <td> <p>(Vereist) Met deze naam wordt de widget door het systeem ge??dentificeerd.</p> <p>Wanneer u de widget voor het eerst configureert en u typt het label, wordt het veld Naam automatisch aangepast. Maar de gebieden van het Etiket en van de Naam zijn niet gesynchroniseerd-dit geeft u de vrijheid om het etiket te veranderen dat uw gebruikers zien zonder het moeten de naam veranderen die het systeem ziet.</p> <p><b>BELANGRIJK</b>: Hoewel dit mogelijk is, raden we u aan deze naam niet te wijzigen nadat u of andere gebruikers het aangepaste formulier in de widget hebben gebruikt. Als u dat doet, herkent het systeem de widget niet meer waar er nu naar kan worden verwezen in andere gebieden van Workfront. </p> <p>Elke widgetnaam moet uniek zijn in het Workfront-exemplaar van uw organisatie. Op deze manier kunt u een formulier hergebruiken dat al voor een ander aangepast formulier is gemaakt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Vereist) Typ of plak de URL van de widget waar deze op internet is opgeslagen.</p> 
      <p>Als u een videowidget toevoegt, kunt u dit op dit moment doen door het volgende toe te voegen in het vak URL:</p> 
      <ul> 
      <li> <p>YouTube- of Vimeo-koppeling</p> </li> 
      <li> <p>Video-koppeling Google Drive</p> </li> 
      <li> <p>Koppeling maken naar video met MP4- en MOV-extensie</p> </li> 
      <li> <p>Koppeling maken naar video die al is ge??pload naar het gebied Documenten in uw Workfront-instantie. Zie voor instructies <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Een videowidget toevoegen aan een aangepast formulier vanuit het gebied Documenten</a> in dit artikel.</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructies</td> 
      <td> <p>Typ eventuele aanvullende informatie over de widget. Wanneer gebruikers het aangepaste formulier invullen, kunnen ze de muisaanwijzer boven het pictogram van het vraagteken plaatsen om knopinfo weer te geven met de informatie die u hier typt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grootte</td> 
      <td>Wijzig desgewenst de weergavegrootte van de widget.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Herhaal de vorige stap om andere velden of widgets toe te voegen.

   of

   Als u een veld wilt kopi??ren, plaatst u de muis boven een veld en klikt u op het pictogram Kopi??ren.

   ![pictogram kopi??ren](assets/copy-field.png)

1. Klik op **Toepassen** en ga naar een andere sectie om door te gaan met het samenstellen van uw formulier.

   of

   Klikken **Opslaan en sluiten**.

#### **Een videowidget toevoegen aan een aangepast formulier vanuit het gebied Documenten**{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Wanneer u op deze manier een video toevoegt aan een aangepast formulier, gelden alleen de machtigingen die voor het aangepaste formulier zijn ingesteld voor de video wanneer gebruikers het formulier openen op een object, niet de machtigingen die voor de video in het gebied Documenten zijn ingesteld.

1. Ga naar de video in het gebied Documenten en genereer een proefdruk, zoals beschreven in [Een interactieve proefdruk maken voor een website of andere webinhoud](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Open de proefdruk.
1. Klik met de rechtermuisknop ergens op de video en selecteer vervolgens **Videoadres kopi??ren**.
1. Plak het gekopieerde adres in het aangepaste formulier waar u de videowidget toevoegt **URL** doos.
1. Klik op **Toepassen** en ga naar een andere sectie om door te gaan met het samenstellen van uw formulier.

   of

   Klikken **Opslaan en sluiten**.

### Adobe XD-bestanden toevoegen

U kunt een Adobe XD-prototype rechtstreeks aan een aangepast formulier toevoegen. Gebruikers die werken met het object waaraan het aangepaste formulier is gekoppeld, kunnen het Adobe XD-bestand alleen in de volgende gebieden zien:

* Het gebied van Details van het voorwerp (bijvoorbeeld, voor een project, het gebied van de Details van het Project)
* Het vak Bewerken voor het object als dit de nieuwe Adobe Workfront-ervaring bevat die er uitziet (bijvoorbeeld de vakken Project bewerken en Taak bewerken)

Een Adobe XD-bestand toevoegen:

1. Op de linkerkant van het scherm, vind **Adobe XD** en sleep het naar een sectie op het canvas.
1. Typ of bewerk een van de volgende eigenschappen voor de widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Vereist) Typ een beschrijvend label dat boven de widget moet worden weergegeven. U kunt het label op elk gewenst moment wijzigen.</p> <p><b>BELANGRIJK</b>: Gebruik geen speciale tekens in dit label. Ze worden niet correct weergegeven in rapporten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Naam</td> 
      <td> <p>(Vereist) Met deze naam wordt de widget door het systeem ge??dentificeerd. Wanneer u de widget voor het eerst configureert en u typt het label, wordt het veld Naam automatisch aangepast. Maar de gebieden van het Etiket en van de Naam zijn niet gesynchroniseerd-dit geeft u de vrijheid om het etiket te veranderen dat uw gebruikers zien zonder het moeten de naam veranderen die het systeem ziet.</p>
    <p><b>BELANGRIJK</b>:   
      <ul> 
      <li>Hoewel dit mogelijk is, raden we u aan deze naam niet te wijzigen nadat u of andere gebruikers het aangepaste formulier in Workfront hebben gebruikt. Als u dat doet, herkent het systeem niet langer het aangepaste veld waar er nu naar wordt verwezen in andere gebieden van Workfront. <p>Bijvoorbeeld, als u het douanegebied aan een rapport toevoegt en later zijn naam verandert, herkent Workfront het niet in het rapport en het zal daar ophouden correct te werken tenzij u het aan het rapport gebruikend de nieuwe naam opnieuw toevoegt.</p> </li>
      <li> <p>We raden u aan geen naam te typen die al wordt gebruikt voor ingebouwde Workfront-velden.</p> </li>
      <li><p>We raden u aan het teken punt/punt niet te gebruiken in de aangepaste veldnaam om fouten te voorkomen bij het gebruik van het veld in verschillende gebieden van Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Vereist) Typ of plak een geldige XD prototypekoppeling.</p> 
      <p>Opmerking: De instelling voor Koppelingstoegang op het tabblad Delen in Adobe XD moet zijn ingesteld op Iedereen met de koppeling. Anders kunnen gebruikers het prototype niet bekijken. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instructies</td> 
      <td> <p>Typ eventuele aanvullende informatie over de widget. Wanneer gebruikers het aangepaste formulier invullen, kunnen ze de muisaanwijzer boven het pictogram van het vraagteken plaatsen om knopinfo weer te geven met de informatie die u hier typt.
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grootte</td> 
      <td>(Optioneel) Wijzig desgewenst de weergavegrootte van de widget.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Herhaal de vorige stap om andere velden of widgets toe te voegen.

   of

   Als u een veld wilt kopi??ren, plaatst u de muis boven een veld en klikt u op het pictogram Kopi??ren.

   ![pictogram kopi??ren](assets/copy-field.png)

1. Klik op **Toepassen** en ga naar een andere sectie om door te gaan met het samenstellen van uw formulier.

   of

   Klikken **Opslaan en sluiten**.

## Een formulier organiseren en een voorbeeld bekijken met de formulierontwerper

Voor informatie over het organiseren en bekijken van een voorbeeld van uw formulier raadpleegt u [Een formulier organiseren en een voorbeeld bekijken met de formulierontwerper](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).