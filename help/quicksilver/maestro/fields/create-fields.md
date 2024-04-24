---
title: Velden maken
description: In de Planning van Adobe Workfront, kunt u douanevelden voor elk type van verslag tot stand brengen. U kunt het gebied met de verslagen van de Planning van Workfront dan associëren.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7e2bb0ee-5f25-4307-9fec-876590c0ae1a
source-git-commit: 2f8a5b2d2183090029966a13c7af37f20eb44fd0
workflow-type: tm+mt
source-wordcount: '3283'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!---
title: Create fields
description: In Adobe Maestro, you can create custom fields for each kind of operational record type or taxonomy. You can then associate the field with Maestro records.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--Should the structure of this article be like this one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

<!--Do we need this for FORMULAS: when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula - not sure is needed??-->

# Velden maken

{{maestro-important-intro}}

In Adobe Workfront Planning kunt u aangepaste velden maken voor recordtypen. U kunt de gebieden met de verslagen van de Planning van Workfront dan associëren om verslaginformatie te verbeteren.

U moet recordtypen maken voordat u velden kunt maken die u hieraan wilt koppelen. Zie voor meer informatie [Recordtypen maken](../architecture/create-record-types.md).

U kunt velden op de volgende manieren maken in Maestro:

* Van kras
* Door recordtypen aan te sluiten
* Door recordtypen te importeren met een Excel- of CSV-bestand
* Door een recordtype te maken
* Een werkruimte maken op basis van een sjabloon

Zie voor meer informatie over Maestro-velden [Overzicht van veld](/help/quicksilver/maestro/fields/fields-overview.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven voor het bètaprogramma Adobe Workfront Planning. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-plan</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>Er is geen toegangsniveaucontrole voor de Planning van Workfront</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Machtigingen beheren in een werkruimte</a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt.</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>

</tbody>
</table>


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## geheel nieuwe velden maken {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

{{step1-to-maestro}}

De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Vouw de pijl omlaag naar rechts uit, rechts van de naam van een bestaande werkruimte, selecteer de werkruimte waarvan u recordtypen wilt maken en klik op het recordtype.

   Alle bestaande records die aan het recordtype zijn gekoppeld, worden in de rijen van de tabelweergave weergegeven.

   >[!TIP]
   >
   >    Als er nog geen records worden weergegeven, hebt u mogelijk nog geen records of hebt u een filter toegepast dat beperkt wat u op het scherm ziet.

   Alle bestaande velden die aan het recordtype zijn gekoppeld, worden weergegeven in de kolommen van de tabelweergave. <!--caveat this for when we can hide the fields; mention that they can be hidden if they are not visible by default-->


1. Klik op de knop **+** in de rechterbovenhoek van de tabelweergave om nieuwe velden toe te voegen.
1. In de **Nieuw veld** tabblad, zoekt u naar een veldtype in het dialoogvenster **Veldtype** of selecteer een van de volgende veldtypen:

   * [Tekst met één regel](#single-line-text)
   * [Alinea](#paragraph)
   * [Meerdere selecties](#multi-select)
   * [Enkel selecteren](#single-select)
   * [Datum](#date)
   * [Getal](#number)
   * [Percentage](#percentage)
   * [Valuta](#currency)
   * [Selectievakje](#checkbox)
   * [Formule](#formula)
   * [Mensen](#people)
   * [Gemaakt door](#created-by)
   * [Aanmaakdatum](#created-date)
   * [Laatst gewijzigd door](#last-modified-by)
   * [Laatst gewijzigd](#last-modified-date)

   >[!IMPORTANT]
   >
   >    U kunt het veldtype van het veld niet wijzigen nadat u het hebt opgeslagen.

1. Ga verder met het toevoegen van elk veld, zoals beschreven in de volgende secties.

### Tekst met één regel {#single-line-text}

Tekstvelden van één regel bevatten beperkte alfanumerieke informatie. U kunt bijvoorbeeld de gegevens van de eigenaar, de belanghebbende, het team of de organisatie-eenheid vastleggen in een tekstveld met één regel. De inhoud van een tekstveld met één regel kan maximaal 250 tekens bevatten. <!-- asked Lilit if we can change this to "Single-line" since this can have numbers and text.-->

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Tekst met één regel** veldtype.

   ![](assets/single-line-text-field-type.png)

1. Voeg de volgende informatie toe in de **Nieuw veld** tab:
   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de pagina Details van de record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolomkop van het veld in een tabel plaatst.
1. Klikken **Maken**.

   Het nieuwe veld met één regel wordt toegevoegd als een kolom aan het recordtype en de waarden ervan kunnen aan records worden gekoppeld.


### Alinea {#paragraph}

In alineasvelden wordt aanvullende alfanumerieke informatie over een record vastgelegd, vergelijkbaar met het veld Beschrijving.

>[!TIP]
>
>* De inhoud van een alinea-veld kan maximaal 1000 tekens bevatten.
>
>* U kunt RTF-opmaak gebruiken om de inhoud van alineasvelden te verbeteren wanneer deze worden weergegeven in de tabelweergave of op de pagina Details van een record. Zie voor meer informatie [Records bewerken](/help/quicksilver/maestro/records/edit-records.md).

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Alinea** veldtype.

   ![](assets/paragraph-field-type.png)


1. Voeg de volgende informatie toe in de **Nieuw veld** tab:
   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de pagina Details van de record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
1. Klikken **Maken**.

   Het nieuwe paragraafgebied wordt toegevoegd als kolom aan het verslagtype, en zijn waarden kunnen met verslagen worden geassocieerd.


### Meerdere selecties {#multi-select}

U kunt een veld met meerdere selecties gebruiken om aanvullende informatie in elke gewenste indeling vast te leggen door meerdere opties in een vervolgkeuzemenu te selecteren.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Meerdere selecties** veldtype.

   ![](assets/multi-select-field-type.png)


1. Voeg de volgende informatie toe in de **Nieuw veld** tab:
   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de pagina Details van de record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Keuzen**: De opties die beschikbaar zijn om in het keuzemenu te selecteren nadat het veld is opgeslagen. U kunt zowel cijfers als letters voor de naam van elke keus hebben.
1. Klikken **Keuze toevoegen** om zoveel opties toe te voegen als nodig is. Er geldt geen limiet voor het aantal keuzen dat u kunt toevoegen aan een veld met meerdere selecties.
1. (Optioneel) Sleep een keuze handmatig in de gewenste volgorde of selecteer de optie
   **Keuzen A-Z sorteren** als u wilt dat de keuzen automatisch in alfabetische volgorde worden weergegeven. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. (Optioneel) Als u een keuze wilt verwijderen, klikt u op **x** rechts van het pictogram.
1. Klik op het kleurstaal links van een keuze om de kleurkiezer uit te vouwen en de kleur van elke optie aan te passen.
1. Klikken **Maken**.

   Het nieuwe multi-select gebied wordt toegevoegd als kolom aan het verslagtype, en zijn waarden kunnen met verslagen worden geassocieerd.

### Enkel selecteren {#single-select}

Met velden die een enkele selectie maken, wordt aanvullende informatie in elke gewenste indeling vastgelegd door een optie in een vervolgkeuzemenu te selecteren.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Enkel selecteren** veldtype.

   ![](assets/single-select-field-type.png)


1. Voeg de volgende informatie toe in de **Nieuw veld** tab:
   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de pagina Details van de record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Keuzen**: De opties die beschikbaar zijn om in het keuzemenu te selecteren nadat het veld is opgeslagen. U kunt zowel cijfers als letters voor de naam van elke keus hebben.

1. Klikken **Keuze toevoegen** om zoveel opties toe te voegen als nodig is. Er geldt geen limiet voor het aantal keuzen dat u kunt toevoegen aan een veld voor één keuze.
1. (Optioneel) Sleep een keuze handmatig in de gewenste volgorde of selecteer de optie **Keuzen A-Z sorteren** als u wilt dat de keuzen automatisch in alfabetische volgorde worden weergegeven. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. (Optioneel) Als u een keuze wilt verwijderen, klikt u op **x** rechts van het pictogram.
1. Klik op het kleurstaal links van een keuze om de kleurkiezer uit te vouwen en de kleur van elke optie aan te passen.
1. Klikken **Maken**.

   Het nieuwe veld Eén keuze wordt toegevoegd als kolom aan het recordtype en de waarden ervan kunnen aan records worden gekoppeld.

### Datum {#date}

U kunt een datumveld gebruiken om aanvullende informatie vast te leggen in de datum- en tijdnotatie.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Datum** veldtype.

   ![](assets/date-field-type.png)


1. Voeg de volgende informatie toe in de **Nieuw veld** tab:
   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de recordpagina. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Datumnotatie**: Het type datumnotatie dat u in dit veld wilt weergeven. <!--update this casing - submitted bug for it-->

     Selecteer een van de volgende indelingen:
      * **Landinstelling**: Komt overeen met de landinstelling van de browser.
      * **Standaard** 16-05-2023
      * **Lang**: 16 mei 2023
      * **Europees** Debat : 16 mei 2023
      * **ISO** 2023-05-16
   * **Een tijdveld opnemen**: Selecteer deze optie als u een tijdstempel wilt opnemen. Deze optie is standaard uitgeschakeld. <!--update this setting name - submitted bug for it to be changed-->

     Selecteer een van de volgende opties:

      * **24 uur**: Bijvoorbeeld: 18:00
      * **12 uur**: Bijvoorbeeld: 6:00 PM

1. Klikken **Maken**.

   Het nieuwe datumveld wordt toegevoegd als een kolom aan het recordtype en de waarden ervan kunnen worden gekoppeld aan records.

### Getal {#number}

Met een getalveldtype wordt informatie vastgelegd in een getalnotatie.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Getal** veldtype.

   ![](assets/number-field-type.png)
1. Voeg de volgende informatie toe in de **Nieuw veld** tab:

   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de recordpagina.
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Precisie**: Het aantal decimalen dat u voor het veld wilt opnemen. U kunt maximaal 6 decimalen weergeven.
   * **Negatieve getallen toestaan**: Selecteer deze optie als u negatieve getallen in dit veld wilt toestaan. Deze optie is standaard uitgeschakeld.

   >[!NOTE]
   >
   >    Als u negatieve getallen toestaan selecteert en negatieve waarden worden opgeslagen in de records waaraan het veld is gekoppeld, kunt u de instelling in de toekomst niet meer uitschakelen.

1. Klikken **Maken**.

   Het nieuwe nummerveld wordt als kolom toegevoegd aan het recordtype en de waarden ervan kunnen aan records worden gekoppeld.

### Percentage {#percentage}

Percentageveldtypen leggen informatie vast in een getalnotatie gevolgd door een percentageteken.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Percentage** veldtype.

   ![](assets/percentage-field-type.png)

1. Voeg de volgende informatie toe in de **Nieuw veld** tab:
   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de recordpagina.
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Precisie**: Het aantal decimalen dat u voor het veld wilt opnemen. U kunt maximaal 6 decimalen weergeven.
   * **Negatieve getallen toestaan**: Selecteer deze optie als u negatieve percentagewaarden in dit veld wilt toestaan. Deze optie is standaard uitgeschakeld.

   >[!NOTE]
   >
   >    Als u negatieve getallen toestaan selecteert en negatieve waarden worden opgeslagen in de records waaraan het veld is gekoppeld, kunt u de instelling in de toekomst niet meer uitschakelen.

1. Klikken **Maken**.

   Het nieuwe percentageveld wordt toegevoegd als kolom aan het verslagtype, en zijn waarden kunnen met verslagen worden geassocieerd.

### Valuta {#currency}

Valutatypen leggen informatie vast in een getalnotatie voorafgegaan door een valutasymbool.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Valuta** veldtype.

   ![](assets/currency-field-type.png)

1. Voeg de volgende informatie toe in de **Nieuw veld** tab:
   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de recordpagina. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Valuta**: Het type valuta dat u in dit veld wilt weergeven. Dit is een lijst van valuta&#39;s volgens de Internationale Organisatie voor Normalisatie (ISO).
   * **Precisie**: Het aantal decimalen dat u voor het veld wilt opnemen. U kunt maximaal 6 decimalen weergeven.
   * **Negatieve getallen toestaan**: Selecteer deze optie als u negatieve valutawaarden wilt toestaan in dit veld. Deze optie is standaard uitgeschakeld.

   >[!NOTE]
   >
   >    Als u negatieve getallen toestaan selecteert en negatieve waarden worden opgeslagen in de records waaraan het veld is gekoppeld, kunt u de instelling in de toekomst niet meer uitschakelen.

1. Klikken **Maken**.

   Het nieuwe valutaveld wordt toegevoegd als een kolom aan het recordtype en de waarden ervan kunnen aan records worden gekoppeld.

### Selectievakje

Met het veldtype Selectievakje kunt u één optie voor het selectievakje aan een record toevoegen. U kunt dit veld gebruiken om een specifiek kenmerk of een specifieke status voor die specifieke record aan te geven. U kunt deze bijvoorbeeld gebruiken als vlag voor het bijhouden van voltooiing, goedkeuring of een ander binair kenmerk voor elke record.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Selectievakje** veldtype.

   ![](assets/checkbox-field-type.png)

1. Voeg de volgende informatie toe in de **Nieuw veld** tab:
   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de recordpagina. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
1. Klikken **Maken**.

   Het nieuwe selectievakje wordt als kolom toegevoegd aan het recordtype en de waarden ervan kunnen aan records worden gekoppeld.

### Formule

Formulervelden genereren een nieuwe waarde met behulp van bestaande waarden uit andere velden in een recordtype en een functie die aangeeft hoe de bestaande waarden moeten worden berekend.

Zie voor meer informatie [Overzicht van formuliervelden](/help/quicksilver/maestro/fields/formula-fields.md).

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Formule** veldtype.

   ![](assets/new-formula-field-with-list-of-expressions.png)

1. Voeg de volgende informatie toe in de **Nieuw veld** tab:

   * **Naam**: Voer een naam in voor het nieuwe veld.
   * **Beschrijving**: Voeg informatie toe over het nieuwe veld.
   * **Formule**: Typ ten minste één teken om toegang te krijgen tot een expressie en selecteer het teken wanneer het in de lijst wordt weergegeven.

1. Klik op de geselecteerde expressie om de definitie weer te geven en de opmaak weer te geven.

   ![](assets/description-of-formula-expression.png)

   Ga voor meer informatie over welke expressies worden ondersteund naar [Overzicht van formuliervelden](/help/quicksilver/maestro/fields/formula-fields.md)

1. Voeg veldnamen toe zoals deze worden weergegeven in Workfront Planning om ernaar te verwijzen in een formule.

   >[!NOTE]
   >
   > U kunt geen multiselect-tekstvelden toevoegen aan een formule.



1. Klikken **Maken**.

   Het nieuwe formuleveld wordt toegevoegd als kolom aan het verslagtype, en zijn waarden kunnen met verslagen worden geassocieerd.


### Mensen

U kunt het veldtype Mensen gebruiken om een gebruiker toe te voegen <!--, job role, or team--> naar een record. Dit is een typeveld en u kunt alleen gebruikers toevoegen<!--, roles, or teams--> die al in je Workfront-exemplaar bestaan.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Mensen** veldtype.

   ![](assets/people-field-type.png)

1. Voeg de volgende informatie toe in de **Nieuw veld** tab:
   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de recordpagina.
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Meerdere waarden toestaan**: Selecteer deze optie als u wilt toestaan dat gebruikers meer dan één gebruiker toevoegen in dit veld. Deze optie is standaard uitgeschakeld.

   >[!NOTE]
   >
   >    Als u Meerdere waarden toestaan selecteert en meerdere gebruikers zijn opgeslagen in de records waaraan het veld is gekoppeld, kunt u de instelling in de toekomst niet meer uitschakelen wanneer u dit veld bewerkt.

1. Klikken **Maken**.

   Het nieuwe Mensen-type gebied wordt toegevoegd als kolom aan het verslagtype, en zijn waarden kunnen met verslagen worden geassocieerd.

### Gemaakt door

U kunt het veld Gemaakt op veldtype gebruiken om de gebruiker die de record heeft gemaakt, toe te voegen aan een record. Dit is een alleen-lezen veld en het veld wordt automatisch gevuld met de naam van de gebruiker die is aangemeld toen de record werd gemaakt.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Gemaakt door** veldtype.

   ![](assets/created-by-field-type.png)

1. Voeg de volgende informatie toe in de **Nieuw veld** tab:

   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de recordpagina. <!--this might change and they might prepopulate it with "Created by"-->
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.

1. Klikken **Maken**.

   Het nieuwe veld Gemaakt door type wordt toegevoegd als kolom aan het recordtype en de waarden ervan worden voorgevuld met de naam van de gebruiker die elke record heeft gemaakt.


### Aanmaakdatum

Met het veldtype Gemaakt datum kunt u de datum toevoegen waarop de record is gemaakt aan een record. Dit is een alleen-lezen veld en het veld wordt automatisch gevuld met de datum (en eventueel met de tijd) waarop de record is gemaakt.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Aanmaakdatum** veldtype.

   ![](assets/created-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Voeg de volgende informatie toe in de **Nieuw veld** tab:

   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de recordpagina. <!--this might change and they might prepopulate it with "Created date"-->
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Datumnotatie**: Kies een van de volgende indelingen:

      * **Landinstelling**: Komt overeen met de landinstelling van de browser.
      * **Standaard** 16-05-2023
      * **Lang**: 16 mei 2023
      * **Europees** Debat : 16 mei 2023
      * **ISO** 2023-05-16
   * **Een tijdveld opnemen**: Selecteer deze optie als u een tijdstempel wilt opnemen. Deze optie is standaard uitgeschakeld. <!--submitted a UI text change for this - check the UI-->

     Selecteer een van de volgende opties:

      * **24 uur**: Bijvoorbeeld: 18:00
      * **12 uur**: Bijvoorbeeld: 6:00 PM

1. Klikken **Maken**.

   Het nieuwe datumtekstveld Gemaakt wordt toegevoegd als een kolom aan het recordtype en de waarden ervan worden voorgevuld met de datum (of datum en tijd) waarop de record is gemaakt.


### Laatst gewijzigd door

U kunt de Laatst gewijzigd op veldtype gebruiken om de gebruiker die de record het laatst heeft gewijzigd, toe te voegen aan een record. Dit is een alleen-lezen veld en het veld wordt automatisch gevuld met de naam van de gebruiker die is aangemeld toen de record voor het laatst werd bijgewerkt.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Laatst gewijzigd door** veldtype.

   ![](assets/last-modified-by-field-type.png)

1. Voeg de volgende informatie toe in de **Nieuw veld** tab:

   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de recordpagina. <!--this might change and they might prepopulate it with "Created by"-->
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.

1. Klikken **Maken**.

   Het nieuwe subtekstveld Laatst gewijzigd wordt toegevoegd als een kolom aan het recordtype en de waarden ervan worden voorgevuld met de naam van de gebruiker die elke record het laatst heeft gewijzigd.


### Laatst gewijzigd

Met het veldtype Laatst gewijzigd kunt u de datum toevoegen waarop een record voor het laatst is gewijzigd in een record. Dit is een alleen-lezen veld en het veld wordt automatisch gevuld met de datum (en eventueel met de tijd) waarop de record voor het laatst is gewijzigd.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Aanmaakdatum** veldtype.

   ![](assets/last-modified-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Voeg de volgende informatie toe in de **Nieuw veld** tab:

   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de recordpagina. <!--this might change and they might prepopulate it with "Created date"-->
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Datumnotatie**: Kies een van de volgende indelingen:

      * **Landinstelling**: Komt overeen met de landinstelling van de browser.
      * **Standaard** 16-05-2023
      * **Lang**: 16 mei 2023
      * **Europees** Debat : 16 mei 2023
      * **ISO** 2023-05-16
   * **Een tijdveld opnemen**: Selecteer deze optie als u een tijdstempel wilt opnemen. Deze optie is standaard uitgeschakeld. <!--submitted a UI text change for this - check the UI-->

     Selecteer een van de volgende opties:

      * **24 uur**: Bijvoorbeeld: 18:00
      * **12 uur**: Bijvoorbeeld: 6:00 PM

1. Klikken **Maken**.

   Het nieuwe datum-type veld Laatst gewijzigd wordt toegevoegd als kolom aan het recordtype en de waarden ervan worden voorgevuld met de datum (of datum en tijd) waarop de record voor het laatst is gewijzigd.

## Velden maken door recordtypen aan te sluiten

U kunt gekoppelde recordvelden maken wanneer u een nieuwe verbinding toevoegt tussen twee recordtypen van Maestro, of een recordtype en een objecttype vanuit andere toepassingen.

Voor informatie over het verbinden van de registratietypen van de Planning van Workfront, zie [Verbind recordtypen](../architecture/connect-record-types.md)

## Velden maken door recordtypen te importeren met een Excel- of CSV-bestand

Zie voor meer informatie [Recordtypen maken](../architecture/create-record-types.md).

## Velden maken door een recordtype te maken

Wanneer u een recordtype maakt, worden ook een aantal velden die aan het nieuwe recordtype zijn gekoppeld, standaard gemaakt. Zie voor meer informatie [Recordtypen maken](../architecture/create-record-types.md).

## Velden maken door een werkruimte te maken van een sjabloon

Adobe Workfront Planning maakt velden voor recordtypen wanneer u een werkruimte maakt op basis van een sjabloon.

Zie voor meer informatie [Werkruimten maken](/help/quicksilver/maestro/architecture/create-workspaces.md).