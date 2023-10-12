---
title: Velden maken
description: In Adobe Maestro, kunt u douanevelden voor elk soort van operationeel verslagtype of taxonomie tot stand brengen. U kunt het veld vervolgens koppelen aan Maestro-records.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7e2bb0ee-5f25-4307-9fec-876590c0ae1a
source-git-commit: 8be7534dfc0a1227bd2274ad093a88ae19b4691d
workflow-type: tm+mt
source-wordcount: '2600'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!--Should the structure of this article be like this one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

# Velden maken

>[!IMPORTANT]
>
>Adobe Maestro maakt momenteel deel uit van een bètaprogramma dat voor een beperkt aantal klanten toegankelijk is.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

In Adobe Maestro, kunt u douanevelden voor operationele verslagtypes of taxonomieën tot stand brengen. U kunt de velden vervolgens koppelen aan Maestro-records om de recordgegevens te verbeteren.

U moet recordtypen maken voordat u velden kunt maken die u hieraan wilt koppelen. Zie voor meer informatie [Recordtypen maken](../architecture-and-fields/create-record-types.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven voor het afgesloten bètaprogramma van de Adobe Maestro. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
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
   <td role="rowheader">Toegangsniveau</td>
   <td> <p>Alle</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Lay-outsjabloon</td>
   <td> <p>Uw systeembeheerder moet het gebied Maestro in uw lay-outmalplaatje toevoegen. Zie voor meer informatie <a href="../access/grant-access.md">Toegang verlenen tot Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Overwegingen over Maestro-velden

* U kunt alleen velden maken vanuit de tabelweergave van een recordtypepagina. Velden worden als kolommen weergegeven in de tabelweergave.

  Voor informatie over het beheren van lijstkolommen (of verslaggebieden), zie [De tabelweergave beheren](../views/manage-the-table-view.md).

  Zie ook de volgende artikelen voor informatie over het beheren van velden:

   * [Velden bewerken](../architecture-and-fields/edit-fields.md)
   * [Velden verwijderen](./delete-fields.md)

* De velden die aan een recordtype zijn gekoppeld, zijn beschikbaar om te worden gekoppeld aan alle records van dat type. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Aan een recordtype gekoppelde velden kunnen niet worden toegevoegd aan een ander recordtype. <!-- this will change when they open the Field library tab when creating a field-->

* U kunt velden handmatig of automatisch maken op de volgende manieren:

   * Handmatig:

      * Door kolommen toe te voegen in de mening van de Lijst van een verslagtype pagina. De kolommen van de lijst zijn de gebieden verbonden aan het verslagtype. Dit zijn dezelfde velden die worden weergegeven op de pagina Details van een record.

        U kunt geen velden maken op de pagina Details van een record.

        In dit artikel wordt beschreven hoe u handmatig velden kunt maken.

      * U kunt recordtypen koppelen. U kunt gekoppelde recordvelden maken wanneer u een nieuwe verbinding toevoegt tussen twee Mouse-recordtypen of een recordtype en een objecttype uit andere toepassingen.

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        Zie voor meer informatie over het verbinden van Maestro-recordtypen [Verbind recordtypen](../architecture-and-fields/connect-record-types.md).

      * Door recordtypen te importeren met een Excel- of CSV-bestand. Zie voor meer informatie [Recordtypen maken](../architecture-and-fields/create-record-types.md).

   * Automatisch:

      * Standaard elke keer dat u een recordtype maakt.

        Hieronder vindt u standaardvelden die standaard worden gemaakt voor elk nieuw type operationeel record:

         * Naam
         * Beschrijving
         * Begindatum
         * Einddatum
         * Status. De standaardwaarden voor recordstatussen zijn:
            * Ontwikkeling
            * Geplant
            * Actief
            * Voltooid
            * In de wachtstand

           U kunt meer waarden toevoegen of de naam van de bestaande waarden wijzigen.

        Hier volgen de standaardvelden die standaard worden gemaakt voor elk nieuw type taxonomy-record:

         * Naam <!--will more be added? If not, consider rephrasing this bullet-->

      * Wanneer u een werkruimte maakt op basis van een sjabloon. Maestro creeert gebieden voor operationele verslagtypes en taxonomieën wanneer u een werkruimte van een malplaatje creeert. Zie voor meer informatie [Werkruimten maken](../architecture-and-fields/create-workspaces.md).



* U kunt de instellingen weergeven en bijwerken voor de velden die u of een andere gebruiker heeft gemaakt. <!--this will change with access/ permissions-->

* U kunt maximaal 500 velden hebben voor één recordtype.

* Veldnamen kunnen maximaal 250 tekens bevatten.

* Wanneer u een operationeel recordtype, taxonomie of werkruimte verwijdert, worden alle bijbehorende velden en de waarden van de velden ook verwijderd en kunnen deze niet worden hersteld. <!-- this might change with a possible recycle bin solution?!-->


## geheel nieuwe velden maken {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-workfront.png) in de rechterbovenhoek van Workfront <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> klik vervolgens op **Maestro** ![](assets/maestro-icon.png).

   De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Vouw de pijl omlaag naar rechts uit, rechts van de naam van een bestaande werkruimte, selecteer de werkruimte waarvan u recordtypen wilt maken en klik op het recordtype.

   Alle bestaande records die aan het recordtype zijn gekoppeld, worden in de rijen van de tabelweergave weergegeven.

   >[!TIP]
   >
   >    Als er nog geen records worden weergegeven, hebt u mogelijk nog geen records of hebt u een filter toegepast dat beperkt wat u op het scherm ziet.

   Alle bestaande velden die aan het recordtype zijn gekoppeld, worden weergegeven in de kolommen van de tabelweergave. <!--caveat this for when we can hide the fields; mention that they can be hidden if they are not visible by default-->


1. Klik op de knop **+** in de rechterbovenhoek van de tabelweergave om nieuwe velden toe te voegen.
1. In de **Nieuw veld** selecteert u een van de volgende veldtypen:

   * [Tekst met één regel](#single-line-text)
   * [Alinea](#paragraph)
   * [Meerdere selecties](#multi-select)
   * [Enkel selecteren](#single-select)
   * [Datum](#date)
   * [Getal](#number)
   * [Percentage](#percentage)
   * [Valuta](#currency)
   * [Selectievakje](#checkbox)
     <!--* [People](#people)-->

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

   Het nieuwe veld met één regel wordt toegevoegd als een kolom aan het recordtype en de waarden ervan kunnen aan records worden gekoppeld. Het veld wordt ook weergegeven op de pagina Details van een record.


### Alinea {#paragraph}

In alineasvelden wordt aanvullende alfanumerieke informatie over een record vastgelegd, vergelijkbaar met het veld Beschrijving. De inhoud van een alinea-veld kan maximaal 1000 tekens bevatten.

<!-- remove the last sentence above and add this tip when we go to rich text: 

>[!TIP]
>
>* The content of a paragraph field can have up to 1,000 characters. 

* You can use Rich Text formatting to enhance the content of paragraph fields when they display in the table view or the Details page of a record. (********check to make sure this is true about Details page***********)

-->

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Alinea** veldtype.

   ![](assets/paragraph-field-type.png)


1. Voeg de volgende informatie toe in de **Nieuw veld** tab:
   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de pagina Details van de record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
1. Klikken **Maken**.

   Het nieuwe paragraafgebied wordt toegevoegd als kolom aan het verslagtype en zijn waarden kunnen met verslagen worden geassocieerd. Het veld wordt ook weergegeven op de pagina Details van een record.


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
1. Klik op de knop **x** rechts van een keuze om het te verwijderen.
1. Klik op het kleurstaal links van een keuze om de kleurkiezer uit te vouwen en de kleur van elke optie aan te passen.
1. Klikken **Maken**.

   Het nieuwe multi-select gebied wordt toegevoegd als kolom aan het verslagtype en zijn waarden kunnen met verslagen worden geassocieerd. Het veld wordt ook weergegeven op de pagina Details van een record.

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
1. Klik op de knop **x** rechts van een keuze om het te verwijderen.
1. Klik op het kleurstaal links van een keuze om de kleurkiezer uit te vouwen en de kleur van elke optie aan te passen.
1. Klikken **Maken**.

   Het nieuwe veld Eén keuze wordt toegevoegd als een kolom aan het recordtype en de waarden ervan kunnen aan records worden gekoppeld. Het veld wordt ook weergegeven op de pagina Details van een record.

### Datum {#date}

U kunt een datumveld gebruiken om aanvullende informatie vast te leggen in de datum- en tijdnotatie.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Datum** veldtype.

   ![](assets/date-field-type.png)


1. Voeg de volgende informatie toe in de **Nieuw veld** tab:
   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de pagina Details van de record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Datumnotatie**: Het type datumnotatie dat u in dit veld wilt weergeven.

     Selecteer een van de volgende indelingen:
      * **Landinstelling**: Komt overeen met de landinstelling van de browser.
      * **Standaard** 16-05-2023
      * **Lang**: 16 mei 2023
      * **Europees** Debat : 16 mei 2023
      * **ISO** 2023-05-16
   * **Een tijdveld opnemen**: Selecteer deze optie als u een tijdstempel wilt opnemen. Deze optie is standaard uitgeschakeld.

     Selecteer een van de volgende opties:

      * **24 uur**: Bijvoorbeeld: 18:00
      * **12 uur**: Bijvoorbeeld: 6:00 PM

1. Klikken **Maken**.

   Het nieuwe datumveld wordt toegevoegd als een kolom aan het recordtype en de waarden ervan kunnen worden gekoppeld aan records. Het veld wordt ook weergegeven op de pagina Details van een record.

### Getal {#number}

Met een getalveldtype wordt informatie vastgelegd in een getalnotatie.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Getal** veldtype.

   ![](assets/number-field-type.png)
1. Voeg de volgende informatie toe in de **Nieuw veld** tab:

   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de pagina Details van de record.
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Precisie**: Het aantal decimalen dat u voor het veld wilt opnemen. U kunt maximaal 6 decimalen weergeven.
   * **Negatieve getallen toestaan**: Selecteer deze optie als u negatieve getallen in dit veld wilt toestaan. Deze optie is standaard uitgeschakeld.

   >[!NOTE]
   >
   >    Als u negatieve getallen toestaan selecteert en negatieve waarden worden opgeslagen in de records waaraan het veld is gekoppeld, kunt u de instelling in de toekomst niet meer uitschakelen.

1. Klikken **Maken**.

   Het nieuwe nummerveld wordt toegevoegd als een kolom aan het recordtype en de waarden ervan kunnen aan records worden gekoppeld. Het veld wordt ook weergegeven op de pagina Details van een record.

### Percentage {#percentage}

Percentageveldtypen leggen informatie vast in een getalnotatie gevolgd door een percentageteken.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Percentage** veldtype.

   ![](assets/percentage-field-type.png)

1. Voeg de volgende informatie toe in de **Nieuw veld** tab:
   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de pagina Details van de record.
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Precisie**: Het aantal decimalen dat u voor het veld wilt opnemen. U kunt maximaal 6 decimalen weergeven.
   * **Negatieve getallen toestaan**: Selecteer deze optie als u negatieve percentagewaarden in dit veld wilt toestaan. Deze optie is standaard uitgeschakeld.

   >[!NOTE]
   >
   >    Als u negatieve getallen toestaan selecteert en negatieve waarden worden opgeslagen in de records waaraan het veld is gekoppeld, kunt u de instelling in de toekomst niet meer uitschakelen.

1. Klikken **Maken**.

   Het nieuwe percentageveld wordt toegevoegd als kolom aan het verslagtype en zijn waarden kunnen met verslagen worden geassocieerd. Het veld wordt ook weergegeven op de pagina Details van een record.

### Valuta {#currency}

Valutatypen leggen informatie vast in een getalnotatie voorafgegaan door een valutasymbool.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Valuta** veldtype.

   ![](assets/currency-field-type.png)

1. Voeg de volgende informatie toe in de **Nieuw veld** tab:
   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de pagina Details van de record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Valuta**: Het type valuta dat u in dit veld wilt weergeven. Dit is een lijst van valuta&#39;s volgens de Internationale Organisatie voor Normalisatie (ISO).
   * **Precisie**: Het aantal decimalen dat u voor het veld wilt opnemen. U kunt maximaal 6 decimalen weergeven.
   * **Negatieve getallen toestaan**: Selecteer deze optie als u negatieve valutawaarden wilt toestaan in dit veld. Deze optie is standaard uitgeschakeld.

   >[!NOTE]
   >
   >    Als u negatieve getallen toestaan selecteert en negatieve waarden worden opgeslagen in de records waaraan het veld is gekoppeld, kunt u de instelling in de toekomst niet meer uitschakelen.

1. Klikken **Maken**.

   Het nieuwe valutaveld wordt toegevoegd als een kolom aan het recordtype en de waarden ervan kunnen aan records worden gekoppeld. Het veld wordt ook weergegeven op de pagina Details van een record.

### Selectievakje

Met het veldtype Selectievakje kunt u één optie voor het selectievakje aan een record toevoegen. U kunt dit veld gebruiken om een specifiek kenmerk of een specifieke status voor die specifieke record aan te geven. U kunt deze bijvoorbeeld gebruiken als vlag voor het bijhouden van voltooiing, goedkeuring of een ander binair kenmerk voor elke record.

1. Een veld maken zoals wordt beschreven in de sectie [geheel nieuwe velden maken](#create-fields-from-scratch) in dit artikel selecteert u vervolgens de **Selectievakje** veldtype.

   ![](assets/checkbox-field-type.png)

1. Voeg de volgende informatie toe in de **Nieuw veld** tab:
   * **Naam**: De naam van het veldtype, zoals deze wordt weergegeven in een tabel of op de pagina Details van de record. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het veld. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
1. Klikken **Maken**.

   Het nieuwe selectievakje wordt als kolom toegevoegd aan het recordtype en de bijbehorende waarden kunnen aan records worden gekoppeld. Het veld wordt ook weergegeven op de pagina Details van een record.

<!--
### People

You can use the People field type to add a user, job role, or team to a record. This is a type-ahead field, and you can add only users, roles, or teams that already exist in Workfront.
 
1. Start creating a field as described in the section [Create fields from scratch](#create-fields-from-scratch) in this article, then select the **People** field type.
 
    ***************INSERT SCREEN SHOT HERE - DO YOU HAVE TO REPLACE OTHER SCREEN SHOTS ABOVE OR IN OTHER DOCS THAT SHOW ALL THE FIELDS, IN INCLUDE THE NEW ONE?! ***************

1. Add the following information in the **New field** tab:
     * **Name**: The name of the field type, as it will appear in a table or the Details page of the record. *************ensure they updated this; and update the screen shot: it used to be "Label"**********
     * **Description**: Additional information about the field. The description of a field displays when you hover over the field's column in a table.
1. Click **Create**.

    The new People-type field is added as a column to the record type and its values can be associated with records. The field also displays on the Details page of a record. 

-->

## Velden maken door recordtypen aan elkaar te koppelen

U kunt gekoppelde recordvelden maken wanneer u een nieuwe verbinding toevoegt tussen twee Mouse-recordtypen of een recordtype en een objecttype uit andere toepassingen.

Voor informatie over het verbinden van Marestro- recordtypes, zie [Verbind recordtypen](../architecture-and-fields/connect-record-types.md).

## Velden maken door recordtypen te importeren met een Excel- en CSV-bestand

Zie voor meer informatie [Recordtypen maken](../architecture-and-fields/create-record-types.md).

## Velden maken door een recordtype te maken

Wanneer u een recordtype maakt, worden ook een aantal velden die aan het nieuwe recordtype zijn gekoppeld, standaard gemaakt. Zie voor meer informatie [Recordtypen maken](../architecture-and-fields/create-record-types.md).

## Velden maken door een werkruimte te maken van een sjabloon

Maestro creeert gebieden voor operationele verslagtypes en taxonomieën wanneer u een werkruimte van een malplaatje creeert.

Zie voor meer informatie [Werkruimten maken](../architecture-and-fields/create-workspaces.md).
