---
title: Velden maken
description: In de Planning van Adobe Workfront, kunt u douanevelden voor elk type van verslag tot stand brengen. U kunt het gebied met de verslagen van de Planning van Workfront dan associëren.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7e2bb0ee-5f25-4307-9fec-876590c0ae1a
source-git-commit: a2062658110792689c0a15dd1c616c58ebf7e07a
workflow-type: tm+mt
source-wordcount: '3390'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Create fields
description: In Adobe Workfront Planning, you can create custom fields for each kind of operational record type or taxonomy. You can then associate the field with records.
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

{{planning-important-intro}}

In Adobe Workfront Planning kunt u aangepaste velden maken voor recordtypen. U kunt de gebieden met de verslagen van de Planning van Workfront dan associëren om verslaginformatie te verbeteren.

U moet recordtypen maken voordat u velden kunt maken die u hieraan wilt koppelen. Voor informatie, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

U kunt velden op de volgende manieren maken in Workfront Planning:

* Van kras
* Door recordtypen aan te sluiten
* Door recordtypen te importeren met een Excel- of CSV-bestand
* Door een recordtype te maken
* Een werkruimte maken op basis van een sjabloon

Voor meer informatie over de planningsgebieden van Workfront, zie [ Overzicht van het Gebied ](/help/quicksilver/planning/fields/fields-overview.md).

## Toegangsvereisten

+++ Breid uit om toegangsvereisten voor de Planning van Workfront te bekijken.

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
<p>Uw organisatie moet zijn ingeschreven in de vroege toegangsfase voor Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-plan</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td>
   <td>
   <p>Nieuw: Standaard</p> 
   <p>Huidig: Plan</p>
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>Er is geen toegangsniveaucontrole voor de Planning van Workfront</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>Rechten beheren in een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt.</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het planningsgebied toevoegen aan uw lay-outsjabloon. Voor informatie, zie <a href="/help/quicksilver/planning/access/access-overview.md"> overzicht van de Toegang </a>. </p>  
</td>
  </tr>

</tbody>
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## geheel nieuwe velden maken {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de records wilt maken waarvoor u velden wilt maken.

   De werkruimte wordt geopend en de recordtypen worden weergegeven.

1. Klik op de kaart van een recordtype.

   Alle bestaande records die aan het recordtype zijn gekoppeld, worden in de rijen van de tabelweergave weergegeven.

   >[!TIP]
   >
   >    Als er nog geen records worden weergegeven, hebt u mogelijk nog geen records of hebt u een filter toegepast dat beperkt wat u op het scherm ziet.

   Alle bestaande velden die aan het recordtype zijn gekoppeld, worden weergegeven in de kolommen van de tabelweergave.

   >[!TIP]
   >
   >    Sommige velden zijn mogelijk verborgen. Klik op Velden en schakel de modus Velden in die u als kolommen wilt weergeven in de tabelweergave.

1. Klik op het pictogram **+** rechtsboven in de tabelweergave

   of

   Beweeg over de kopbal van om het even welke kolom, klik de naar beneden wijzende pijl na de gebiedsnaam, dan klik links **of** Tussenvoegsel rechts **om het nieuwe gebied toe te voegen.**
1. Op het **Nieuwe gebied** lusje, onderzoek naar een gebiedstype op het **type van Gebied** vakje, of selecteer van de volgende gebiedstypes:

   * [Tekst met één regel](#single-line-text)
   * [Alinea](#paragraph)
   * [Meerdere selecties](#multi-select)
   * [Enkel selecteren](#single-select)
   * [Datum](#date)
   * [ Aantal ](#number)
   * [Percentage](#percentage)
   * [Valuta](#currency)
   * [ Checkbox ](#checkbox)
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

1. Begin creërend een gebied zoals die in de sectie [ wordt beschreven creeer gebieden van kras ](#create-fields-from-scratch) in dit artikel, dan selecteer het **single-line tekst** gebiedstype.

   ![](assets/single-line-text-field-type.png)

1. Voeg de volgende informatie op het **Nieuwe gebied** tabel toe:
   * **Naam**: De naam van het gebiedstype, aangezien het in een lijst of de pagina van Details van het verslag zal verschijnen. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het gebied. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolomkop van het veld in een tabel plaatst.
1. Klik **creëren**.

   Het nieuwe veld met één regel wordt toegevoegd als een kolom aan het recordtype en de waarden ervan kunnen aan records worden gekoppeld.


### Alinea {#paragraph}

In alineasvelden wordt aanvullende alfanumerieke informatie over een record vastgelegd, vergelijkbaar met het veld Beschrijving.

>[!TIP]
>
>* De inhoud van een alinea-veld kan maximaal 1000 tekens bevatten.
>
>* U kunt RTF-opmaak gebruiken om de inhoud van alineasvelden te verbeteren wanneer deze worden weergegeven in de tabelweergave of op de pagina Details van een record. Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/edit-records.md) uitgeven.

1. Begin creërend een gebied zoals die in de sectie [ wordt beschreven creeer gebieden van kras ](#create-fields-from-scratch) in dit artikel, dan selecteer het **3} gebiedstype van de Paragraaf {.**

   ![](assets/paragraph-field-type.png)


1. Voeg de volgende informatie op het **Nieuwe gebied** tabel toe:
   * **Naam**: De naam van het gebiedstype, aangezien het in een lijst of de pagina van Details van het verslag zal verschijnen. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het gebied. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
1. Klik **creëren**.

   Het nieuwe paragraafgebied wordt toegevoegd als kolom aan het verslagtype, en zijn waarden kunnen met verslagen worden geassocieerd.


### Meerdere selecties {#multi-select}

U kunt een veld met meerdere selecties gebruiken om aanvullende informatie in elke gewenste indeling vast te leggen door meerdere opties in een vervolgkeuzemenu te selecteren.

1. Begin creërend een gebied zoals die in de sectie [ wordt beschreven creeer gebieden van kras ](#create-fields-from-scratch) in dit artikel, dan selecteer het **multi-uitgezochte** gebiedstype.

   ![](assets/multi-select-field-type.png)


1. Voeg de volgende informatie op het **Nieuwe gebied** tabel toe:
   * **Naam**: De naam van het gebiedstype, aangezien het in een lijst of de pagina van Details van het verslag zal verschijnen. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het gebied. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Keuzen**: De opties beschikbaar om van het drop-down menu te selecteren nadat het gebied wordt bewaard. U kunt zowel cijfers als letters voor de naam van elke keus hebben.
1. Klik **toevoegen keus** om zo vele keuzen toe te voegen zoals nodig. Er geldt geen limiet voor het aantal keuzen dat u kunt toevoegen aan een veld met meerdere selecties.
1. (Optioneel) Sleep een keuze handmatig in de gewenste volgorde of selecteer de optie
   **de keuzen van de Soort a-z** optie als u de keuzen automatisch in alfabetische orde wilt worden vermeld. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. (Facultatief) om een keus te verwijderen, klik het **x** pictogram rechts van het.
1. Klik op het kleurstaal links van een keuze om de kleurkiezer uit te vouwen en de kleur van elke optie aan te passen.
1. Klik **creëren**.

   Het nieuwe multi-select gebied wordt toegevoegd als kolom aan het verslagtype, en zijn waarden kunnen met verslagen worden geassocieerd.

### Enkel selecteren {#single-select}

Met velden die een enkele selectie maken, wordt aanvullende informatie in elke gewenste indeling vastgelegd door een optie in een vervolgkeuzemenu te selecteren.

1. Begin creërend een gebied zoals die in de sectie [ wordt beschreven creeer gebieden van kras ](#create-fields-from-scratch) in dit artikel, dan selecteer het **enig-uitgezochte** gebiedstype.

   ![](assets/single-select-field-type.png)


1. Voeg de volgende informatie op het **Nieuwe gebied** tabel toe:
   * **Naam**: De naam van het gebiedstype, aangezien het in een lijst of de pagina van Details van het verslag zal verschijnen. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het gebied. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Keuzen**: De opties beschikbaar om van het drop-down menu te selecteren nadat het gebied wordt bewaard. U kunt zowel cijfers als letters voor de naam van elke keus hebben.

1. Klik **toevoegen keus** om zo vele keuzen toe te voegen zoals nodig. Er geldt geen limiet voor het aantal keuzen dat u kunt toevoegen aan een veld voor één keuze.
1. (Facultatief) sleep en laat manueel elke keus in de gewenste orde vallen, of selecteer de **optie van de Soort A-Z** als u de keuzen automatisch in alfabetische orde wilt worden vermeld. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. (Facultatief) om een keus te verwijderen, klik het **x** pictogram rechts van het.
1. Klik op het kleurstaal links van een keuze om de kleurkiezer uit te vouwen en de kleur van elke optie aan te passen.
1. Klik **creëren**.

   Het nieuwe veld Eén keuze wordt toegevoegd als kolom aan het recordtype en de waarden ervan kunnen aan records worden gekoppeld.

### Datum {#date}

U kunt een datumveld gebruiken om aanvullende informatie vast te leggen in de datum- en tijdnotatie.

1. Begin creërend een gebied zoals die in de sectie [ wordt beschreven creeer gebieden van kras ](#create-fields-from-scratch) in dit artikel, dan selecteer het **Datum** gebiedstype.

   ![](assets/date-field-type.png)


1. Voeg de volgende informatie op het **Nieuwe gebied** tabel toe:
   * **Naam**: De naam van het gebiedstype, aangezien het in een lijst of de verslagpagina zal verschijnen. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het gebied. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Formaat van de Datum**: Het type van datumformaat u op dit gebied wilt tonen. <!--update this casing - submitted bug for it-->

     Selecteer een van de volgende indelingen:
      * **Landinstelling**: Gelijke aan de scène van uw browser.
      * **Norm**: 05/16/2023
      * **Lang**: 16 mei, 2023
      * **Europees**: 16/05/2023
      * **ISO**: 2023-05-16
   * **omvat een tijdgebied**: Selecteer deze optie als u een tijdstempel wilt omvatten. Deze optie is standaard uitgeschakeld. <!--update this setting name - submitted bug for it to be changed-->

     Selecteer een van de volgende opties:

      * **24hr**: Bijvoorbeeld: 18:00
      * **12hr**: Bijvoorbeeld: 6:00 PM

1. Klik **creëren**.

   Het nieuwe datumveld wordt toegevoegd als een kolom aan het recordtype en de waarden ervan kunnen worden gekoppeld aan records.

### Getal {#number}

Met een getalveldtype wordt informatie vastgelegd in een getalnotatie.

1. Begin creërend een gebied zoals die in de sectie [ wordt beschreven creeer gebieden van kras ](#create-fields-from-scratch) in dit artikel, dan selecteer het **3} gebiedstype van het Aantal {.**

   ![](assets/number-field-type.png)
1. Voeg de volgende informatie op het **Nieuwe gebied** tabel toe:

   * **Naam**: De naam van het gebiedstype, aangezien het in een lijst of de verslagpagina zal verschijnen.
   * **Beschrijving**: Aanvullende informatie over het gebied. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Precisie**: Het aantal decimalen die u voor het gebied wilt registreren. U kunt maximaal 6 decimalen weergeven.
   * **sta negatieve aantallen** toe: selecteer deze optie als u negatieve aantallen op dit gebied wilt toestaan. Deze optie is standaard uitgeschakeld.

   >[!NOTE]
   >
   >    Als u negatieve getallen toestaan selecteert en negatieve waarden worden opgeslagen in de records waaraan het veld is gekoppeld, kunt u de instelling in de toekomst niet meer uitschakelen.

1. Klik **creëren**.

   Het nieuwe nummerveld wordt als kolom toegevoegd aan het recordtype en de waarden ervan kunnen aan records worden gekoppeld.

### Percentage {#percentage}

Percentageveldtypen leggen informatie vast in een getalnotatie gevolgd door een percentageteken.

1. Begin creërend een gebied zoals die in de sectie [ wordt beschreven creeer gebieden van kras ](#create-fields-from-scratch) in dit artikel, dan selecteer het **3} gebiedstype van het Percentage {.**

   ![](assets/percentage-field-type.png)

1. Voeg de volgende informatie op het **Nieuwe gebied** tabel toe:
   * **Naam**: De naam van het gebiedstype, aangezien het in een lijst of de verslagpagina zal verschijnen.
   * **Beschrijving**: Aanvullende informatie over het gebied. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Precisie**: Het aantal decimalen die u voor het gebied wilt registreren. U kunt maximaal 6 decimalen weergeven.
   * **sta negatieve aantallen** toe: selecteer deze optie als u negatieve percentagewaarden op dit gebied wilt toestaan. Deze optie is standaard uitgeschakeld.

   >[!NOTE]
   >
   >    Als u negatieve getallen toestaan selecteert en negatieve waarden worden opgeslagen in de records waaraan het veld is gekoppeld, kunt u de instelling in de toekomst niet meer uitschakelen.

1. Klik **creëren**.

   Het nieuwe percentageveld wordt toegevoegd als kolom aan het verslagtype, en zijn waarden kunnen met verslagen worden geassocieerd.

### Valuta {#currency}

Valutatypen leggen informatie vast in een getalnotatie voorafgegaan door een valutasymbool.

1. Begin creërend een gebied zoals die in sectie [ wordt beschreven creeer gebieden van kras ](#create-fields-from-scratch) in dit artikel, dan selecteer het **3} gebiedstype van de Valuta {.**

   ![](assets/currency-field-type.png)

1. Voeg de volgende informatie op het **Nieuwe gebied** tabel toe:
   * **Naam**: De naam van het gebiedstype, aangezien het in een lijst of de verslagpagina zal verschijnen. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het gebied. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Valuta**: Het type van munt u op dit gebied wilt tonen. Dit is een lijst van valuta&#39;s volgens de Internationale Organisatie voor Normalisatie (ISO).
   * **Precisie**: Het aantal decimalen die u voor het gebied wilt registreren. U kunt maximaal 6 decimalen weergeven.
   * **sta negatieve aantallen** toe: selecteer deze optie als u negatieve muntwaarden op dit gebied wilt toestaan. Deze optie is standaard uitgeschakeld.

   >[!NOTE]
   >
   >    Als u negatieve getallen toestaan selecteert en negatieve waarden worden opgeslagen in de records waaraan het veld is gekoppeld, kunt u de instelling in de toekomst niet meer uitschakelen.

1. Klik **creëren**.

   Het nieuwe valutaveld wordt toegevoegd als een kolom aan het recordtype en de waarden ervan kunnen aan records worden gekoppeld.

### Selectievakje

Met het veldtype Selectievakje kunt u één optie voor het selectievakje aan een record toevoegen. U kunt dit veld gebruiken om een specifiek kenmerk of een specifieke status voor die specifieke record aan te geven. U kunt deze bijvoorbeeld gebruiken als vlag voor het bijhouden van voltooiing, goedkeuring of een ander binair kenmerk voor elke record.

1. Begin creërend een gebied zoals die in de sectie [ wordt beschreven creeer gebieden van kras ](#create-fields-from-scratch) in dit artikel, dan selecteer het **CheckBox** gebiedstype.

   ![](assets/checkbox-field-type.png)

1. Voeg de volgende informatie op het **Nieuwe gebied** tabel toe:
   * **Naam**: De naam van het gebiedstype, aangezien het in een lijst of de verslagpagina zal verschijnen. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Beschrijving**: Aanvullende informatie over het gebied. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
1. Klik **creëren**.

   Het nieuwe selectievakje wordt als kolom toegevoegd aan het recordtype en de waarden ervan kunnen aan records worden gekoppeld.

### Formule

Formulervelden genereren een nieuwe waarde met behulp van bestaande waarden uit andere velden in een recordtype en een functie die aangeeft hoe de bestaande waarden moeten worden berekend.

Voor meer informatie, zie [ overzicht van de gebieden van de Formule ](/help/quicksilver/planning/fields/formula-fields.md).

1. Begin creërend een gebied zoals die in sectie [ wordt beschreven creeer gebieden van kras ](#create-fields-from-scratch) in dit artikel, dan selecteer het **Formule** gebiedstype.

   ![](assets/new-formula-field-with-list-of-expressions.png)

1. Voeg de volgende informatie op het **Nieuwe gebied** tabel toe:

   * **Naam**: Ga een naam voor het nieuwe gebied in.
   * **Beschrijving**: Voeg informatie over het nieuwe gebied toe.
   * **Formule**: Begin typend minstens één karakter om tot een uitdrukking toegang te hebben, dan selecteer het wanneer het in de lijst toont.

1. Klik op de geselecteerde expressie om de definitie weer te geven en de opmaak weer te geven.

   ![](assets/description-of-formula-expression.png)

   Voor meer informatie over welke uitdrukkingen worden gesteund, zie [ overzicht van de gebieden van de Formule ](/help/quicksilver/planning/fields/formula-fields.md).

1. Voeg veldnamen toe zoals deze worden weergegeven in Workfront Planning om ernaar te verwijzen in een formule.

   >[!NOTE]
   >
   >* U kunt geen multiselect-tekstvelden toevoegen aan een formule.
   >
   >* U kunt verwijzen naar een veld dat zich op maximaal 4 niveaus van het huidige recordtype bevindt. Bijvoorbeeld, als u een formuleringsgebied voor een type van het verslag van de Activiteit creeert, en de Activiteit wordt verbonden met het type van het Verslag van het Product dat met het verslagtype van de Campagne wordt verbonden dat met een Project van Workfront wordt verbonden, kunt u het Begroting van het project in de formule verwijzen u voor het type van het verslag van de Activiteit creeert.

<!--1. In the **Format** field, select from the following choices to identify the format of the result displayed in the formula-type field:

    * **Text**: The result of the formula field displays as plain text. 
    * **Number**: The result of the formula field displays as a number. 
    * **Percent**: The result of the formula field displays as a number followed by a percentage symbol.  
    * **Currency**: The result of the formula field displays as a number preceded or followed by a currency symbol.  
    * **Tags**: The result of the formula field displays as a tag with the object's name. 
    * **Date**: The result of the formula field displays as a date. 

        A preview of what the result will look like displays under the **Format** field. 

        ![](assets/formula-field-formats-list-with-tag-selected-highlighted.png)

        >[!WARNING]
        >
        >If the result of the formula does not match the selected format, the field will show an error message where it displays. 

-->
1. Klik **creëren**.

   Het nieuwe formuleveld wordt toegevoegd als kolom aan het verslagtype, en zijn waarden kunnen met verslagen worden geassocieerd.


### Mensen

Met het veldtype Personen kunt u een gebruiker <!--, job role, or team--> aan een record toevoegen. Dit is een type-vooruit gebied, en u kunt slechts gebruikers <!--, roles, or teams--> toevoegen die reeds in uw instantie van Workfront bestaan.

1. Begin creërend een gebied zoals die in de sectie [ wordt beschreven creeer gebieden van kras ](#create-fields-from-scratch) in dit artikel, dan selecteer het **3} gebiedstype van Mensen {.**

   ![](assets/people-field-type.png)

1. Voeg de volgende informatie op het **Nieuwe gebied** tabel toe:
   * **Naam**: De naam van het gebiedstype, aangezien het in een lijst of de verslagpagina zal verschijnen.
   * **Beschrijving**: Aanvullende informatie over het gebied. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **staat veelvoudige waarden** toe: Selecteer deze optie als u gebruikers wilt toestaan om meer dan één gebruiker op dit gebied toe te voegen. Deze optie is standaard uitgeschakeld.

   >[!NOTE]
   >
   >    Als u Meerdere waarden toestaan selecteert en meerdere gebruikers zijn opgeslagen in de records waaraan het veld is gekoppeld, kunt u de instelling in de toekomst niet meer uitschakelen wanneer u dit veld bewerkt.

1. Klik **creëren**.

   Het nieuwe Mensen-type gebied wordt toegevoegd als kolom aan het verslagtype, en zijn waarden kunnen met verslagen worden geassocieerd.

### Gemaakt door

U kunt het veld Gemaakt op veldtype gebruiken om de gebruiker die de record heeft gemaakt, toe te voegen aan een record. Dit is een alleen-lezen veld en het veld wordt automatisch gevuld met de naam van de gebruiker die is aangemeld toen de record werd gemaakt.

1. Begin creërend een gebied zoals die in de sectie [ wordt beschreven creeer gebieden van kras ](#create-fields-from-scratch) in dit artikel, dan selecteer **die door** gebiedstype wordt gecreeerd.

   ![](assets/created-by-field-type.png)

1. Voeg de volgende informatie op het **Nieuwe gebied** tabel toe:

   * **Naam**: De naam van het gebiedstype, aangezien het in een lijst of de verslagpagina zal verschijnen. <!--this might change and they might prepopulate it with "Created by"-->
   * **Beschrijving**: Aanvullende informatie over het gebied. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.

1. Klik **creëren**.

   Het nieuwe veld Gemaakt door type wordt toegevoegd als kolom aan het recordtype en de waarden ervan worden voorgevuld met de naam van de gebruiker die elke record heeft gemaakt.


### Aanmaakdatum

Met het veldtype Gemaakt datum kunt u de datum toevoegen waarop de record is gemaakt aan een record. Dit is een alleen-lezen veld en het veld wordt automatisch gevuld met de datum (en eventueel met de tijd) waarop de record is gemaakt.

1. Begin creërend een gebied zoals die in de sectie [ wordt beschreven creeer gebieden van kras ](#create-fields-from-scratch) in dit artikel, dan selecteer het **Gemaakt datum** gebiedstype.

   ![](assets/created-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Voeg de volgende informatie op het **Nieuwe gebied** tabel toe:

   * **Naam**: De naam van het gebiedstype, aangezien het in een lijst of de verslagpagina zal verschijnen. <!--this might change and they might prepopulate it with "Created date"-->
   * **Beschrijving**: Aanvullende informatie over het gebied. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Formaat van de Datum**: Uitgezocht van de volgende formaten:

      * **Landinstelling**: Gelijke aan de scène van uw browser.
      * **Norm**: 05/16/2023
      * **Lang**: 16 mei, 2023
      * **Europees**: 16/05/2023
      * **ISO**: 2023-05-16
   * **omvat een tijdgebied**: Selecteer deze optie als u een tijdstempel wilt omvatten. Deze optie is standaard uitgeschakeld. <!--submitted a UI text change for this - check the UI-->

     Selecteer een van de volgende opties:

      * **24hr**: Bijvoorbeeld: 18:00
      * **12hr**: Bijvoorbeeld: 6:00 PM

1. Klik **creëren**.

   Het nieuwe datumtekstveld Gemaakt wordt toegevoegd als een kolom aan het recordtype en de waarden ervan worden voorgevuld met de datum (of datum en tijd) waarop de record is gemaakt.


### Laatst gewijzigd door

U kunt de Laatst gewijzigd op veldtype gebruiken om de gebruiker die de record het laatst heeft gewijzigd, toe te voegen aan een record. Dit is een alleen-lezen veld en het veld wordt automatisch gevuld met de naam van de gebruiker die is aangemeld toen de record voor het laatst werd bijgewerkt.

1. Begin creërend een gebied zoals die in de sectie [ wordt beschreven creeer gebieden van kras ](#create-fields-from-scratch) in dit artikel, dan selecteer het **Laatst gewijzigd door** gebiedstype.

   ![](assets/last-modified-by-field-type.png)

1. Voeg de volgende informatie op het **Nieuwe gebied** tabel toe:

   * **Naam**: De naam van het gebiedstype, aangezien het in een lijst of de verslagpagina zal verschijnen. <!--this might change and they might prepopulate it with "Created by"-->
   * **Beschrijving**: Aanvullende informatie over het gebied. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.

1. Klik **creëren**.

   Het nieuwe subtekstveld Laatst gewijzigd wordt toegevoegd als een kolom aan het recordtype en de waarden ervan worden voorgevuld met de naam van de gebruiker die elke record het laatst heeft gewijzigd.


### Laatst gewijzigd

Met het veldtype Laatst gewijzigd kunt u de datum toevoegen waarop een record voor het laatst is gewijzigd in een record. Dit is een alleen-lezen veld en het veld wordt automatisch gevuld met de datum (en eventueel met de tijd) waarop de record voor het laatst is gewijzigd.

1. Begin creërend een gebied zoals die in de sectie [ wordt beschreven creeer gebieden van kras ](#create-fields-from-scratch) in dit artikel, dan selecteer het **Gemaakt datum** gebiedstype.

   ![](assets/last-modified-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Voeg de volgende informatie op het **Nieuwe gebied** tabel toe:

   * **Naam**: De naam van het gebiedstype, aangezien het in een lijst of de verslagpagina zal verschijnen. <!--this might change and they might prepopulate it with "Created date"-->
   * **Beschrijving**: Aanvullende informatie over het gebied. De beschrijving van een veld wordt weergegeven wanneer u de cursor op de kolom van het veld in een tabel plaatst.
   * **Formaat van de Datum**: Uitgezocht van de volgende formaten:

      * **Landinstelling**: Gelijke aan de scène van uw browser.
      * **Norm**: 05/16/2023
      * **Lang**: 16 mei, 2023
      * **Europees**: 16/05/2023
      * **ISO**: 2023-05-16
   * **omvat een tijdgebied**: Selecteer deze optie als u een tijdstempel wilt omvatten. Deze optie is standaard uitgeschakeld. <!--submitted a UI text change for this - check the UI-->

     Selecteer een van de volgende opties:

      * **24hr**: Bijvoorbeeld: 18:00
      * **12hr**: Bijvoorbeeld: 6:00 PM

1. Klik **creëren**.

   Het nieuwe datum-type veld Laatst gewijzigd wordt toegevoegd als kolom aan het recordtype en de waarden ervan worden voorgevuld met de datum (of datum en tijd) waarop de record voor het laatst is gewijzigd.

## Velden maken door recordtypen aan te sluiten

U kunt gekoppelde recordvelden maken wanneer u een nieuwe verbinding toevoegt tussen twee recordtypen of een recordtype en een objecttype vanuit andere toepassingen.

Voor informatie over het verbinden van het verslagtypes van de Planning van Workfront, zie [ Connect verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md)

## Velden maken door recordtypen te importeren met een Excel- of CSV-bestand

Voor meer informatie, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

## Velden maken door een recordtype te maken

Wanneer u een recordtype maakt, worden ook een aantal velden die aan het nieuwe recordtype zijn gekoppeld, standaard gemaakt. Voor meer informatie, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

## Velden maken door een werkruimte te maken van een sjabloon

Adobe Workfront Planning maakt velden voor recordtypen wanneer u een werkruimte maakt op basis van een sjabloon.

Voor informatie, zie [ werkruimten ](/help/quicksilver/planning/architecture/create-workspaces.md) creëren.