---
user-type: administrator
product-area: system-administration
keywords: kickstart,trap-start,kickstart,trap-start
navigation-topic: use-kick-starts
title: Gegevens naar Adobe Workfront importeren met een Kick-startsjabloon
description: Kick-start zijn speciaal opgemaakte Excel-werkboeken die u kunt vullen met gegevens die u in Workfront wilt importeren. Adobe Workfront beschikt over een Kick-Start-sjabloon die u kunt gebruiken om dit te doen, zoals wordt uitgelegd in Kick-Starts data importer.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '2515'
ht-degree: 0%

---

# Gegevens naar Adobe Workfront importeren met een Kick-startsjabloon

Kick-start zijn speciaal opgemaakte Excel-werkboeken die u kunt vullen met gegevens die u in Workfront wilt importeren. Adobe Workfront beschikt over een Kick-Start-sjabloon die u kunt gebruiken om dit te doen, zoals wordt uitgelegd in [Kick-start gegevensimporteur](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md).

Dit proces wordt opgedeeld in drie hoofdtaken:

* Eerst exporteert u een Kick-Start-sjabloon als een spreadsheetbestand
* Ten tweede vult u het werkblad met uw gegevens
* Tot slot importeert u de gevulde spreadsheet in Workfront

Elk van deze procedures wordt geschetst in de juiste orde in dit artikel.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>:</p> 
   <p> Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Beperkingen

U kunt grote aantallen voorwerpen in Workfront invoeren gebruikend een Kick-Begin malplaatje. Houd echter rekening met de volgende beperkingen:

* Als u gegevens op deze manier importeert, wordt er geen informatie bijgewerkt over records die al in Workfront bestaan
* U kunt alleen nieuwe records en de bijbehorende gegevens importeren
* Er kunnen niet meer dan 2000 records tegelijk worden geïmporteerd om ervoor te zorgen dat er geen time-out optreedt bij het importeren

## Een Kick-startsjabloon exporteren als een spreadsheetbestand

Wanneer u een malplaatje van het Kick-Begin uitvoert ontvangt u een leeg werkboek van het spreadsheet van Excel. In verdere procedures in dit artikel, zult u het werkboek met uw informatie bevolken en dan het terug in Workfront invoeren.

Een Kick-Start-sjabloon exporteren:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Systeem** > **Gegevens exporteren (Kick-start)**.

1. Klikken **Meer opties** Selecteer vervolgens de soorten gegevens die u wilt opnemen.

   Elke optie die u selecteert, vertegenwoordigt een verzameling meerdere tabbladen in het geëxporteerde werkblad. Als u bijvoorbeeld de optie Rapport selecteert, worden alle benodigde objecten voor het maken van een rapport opgenomen in het werkblad (weergaven, filters, groepen, rapporten).

   U kunt alle hieronder vermelde objecttypen gebruiken om gegevens te importeren in Workfront. (De enige uitzondering is de optie Toegangsniveaus. Het gegevensblad van Niveaus van de Toegang in de uitvoer wordt verstrekt voor verwijzingsdoeleinden-het staat u toe om een toegangsniveau aan een nieuw gebruikersrekening door identiteitskaart toe te wijzen.)

   De sjabloon voor elk objecttype kan in de volgende bestandsindelingen worden geëxporteerd en bevat de volgende bladen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Object</strong> </p> </th> 
      <th> <p><strong>Exporteren als</strong> </p> </th> 
      <th> <p><strong>Werkbladen in het geëxporteerde werkblad</strong> </p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col"> <p>Dashboard</p> <p>Alle dashboards in het systeem zijn beschikbaar om te exporteren. U kunt maximaal 100 specifieke dashboards selecteren in één export.</p> </td> 
      <td scope="col">Exporteren als ZIP-bestand</td> 
      <td scope="col"> <p>Parameter</p> <p>Parameteroptie</p> <p>Parametergroep</p> <p>Categorieparameter</p> <p>Categorie</p> <p>Rapport</p> <p>Sectie tabblad Portal</p> <p>Dashboard</p> <p>Voorkeuren</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Rapport</p> <p>Alle rapporten in het systeem zijn beschikbaar om te exporteren. U kunt maximaal 100 specifieke rapporten selecteren in één exportbewerking.</p> </td> 
      <td scope="col">Exporteren als ZIP-bestand </td> 
      <td scope="col"> <p scope="col">Parameter</p> <p scope="col">Parameteroptie</p> <p scope="col">Parametergroep</p> <p scope="col">Categorieparameter</p> <p scope="col">Categorie</p> <p scope="col">Rapport</p> <p scope="col">Voorkeuren</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Goedkeuring</p> </td> 
      <td scope="col"> <p>Exporteren als Excel-bestand</p> </td> 
      <td scope="col"> <p>Stap fiatteur</p> <p>Goedkeuringsstap</p> <p>Goedkeuring</p> <p>Goedkeuringsproces</p> <p>Voorkeuren</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Aangepaste gegevens</p> </td> 
      <td scope="col"> <p>Exporteren als Excel-bestand</p> </td> 
      <td scope="col"> <p>Parameter</p> <p>Parameteroptie</p> <p>Parametergroep</p> <p>Categorieparameter</p> <p>Categorie</p> <p>Voorkeuren</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Type uitgave</p> </td> 
      <td scope="col"> <p>Exporteren als Excel-bestand</p> </td> 
      <td> <p>Type uitgave</p> <p>Voorkeuren</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Uurtype</p> </td> 
      <td scope="col"> <p>Exporteren als Excel-bestand</p> </td> 
      <td> <p>Uurtype</p> <p>Voorkeuren</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Team</p> </td> 
      <td scope="col"> <p>Exporteren als Excel-bestand</p> </td> 
      <td> <p> Teamlid</p> <p>Team</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td> <p>Gebruiker</p> </td> 
      <td> <p>Exporteert als Excel-bestand. Klik op <strong>Meer opties</strong>.</p> </td> 
      <td> <p>Gebruiker</p> <p>Voorkeuren</p> </td> 
     </tr> 
     <tr> 
      <td>Toegangsniveau</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p>Toegangsniveau</p> <p>Voorkeuren</p> </td> 
     </tr> 
     <tr> 
      <td>Toewijzing</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p>Toewijzing</p> <p>Voorkeuren</p> </td> 
     </tr> 
     <tr> 
      <td>Bedrijf</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p> Bedrijf</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>E-mailsjabloon</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p>E-mailsjabloon</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Kosten</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p> Kosten"</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Externe pagina</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p> Externe pagina</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Filter</td> 
      <td>Exporteert als een ZIP-bestand</td> 
      <td> <p> Filter</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Groep</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p> Groep</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Groepering</td> 
      <td>Exporteert als een ZIP-bestand</td> 
      <td> <p> Groepering</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Uur</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p> Uur</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Probleem</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p> Probleem</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Functie</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p> Functie</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Mijlpad</td> 
      <td> Exporteren als Excel-bestand</td> 
      <td> <p> Mijlsteen</p> <p>Mijlpad</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Opmerking</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p> Opmerking</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Portfolio</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p> Portfolio</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Project</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p> Wachtrij</p> <p>Project</p> <p>Routeringsregel</p> <p>Onderwerp van wachtrij</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Bronschatting</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p> Bronschatting</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Bronpool</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p> Bronpool</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Risico</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p> Risico</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Type risico</td> 
      <td> Exporteren als Excel-bestand</td> 
      <td> <p> Type risico</p> <p>Voorkeuren</p> </td> 
     </tr> 
     <tr> 
      <td>Scorecard</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p>Scorecard-vragen</p> <p>Scorecard-optie</p> <p>Scorecard</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Taak</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p> Taak</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Sjabloon</td> 
      <td> Exporteren als Excel-bestand</td> 
      <td> <p> Wachtrij</p> <p>Sjabloon</p> <p>Routeringsregel</p> <p>Onderwerp van wachtrij</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Sjabloontoewijzing</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p> Sjabloontoewijzing</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Sjabloontaak</td> 
      <td>Exporteren als Excel-bestand</td> 
      <td> <p> Sjabloontaak</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Tijdschema</td> 
      <td> Exporteren als Excel-bestand</td> 
      <td> <p> Tijdbladprofiel</p> <p>Tijdschema</p> <p>Voorkeuren </p> </td> 
     </tr> 
     <tr> 
      <td>Weergave </td> 
      <td> <p>Exporteren als ZIP-bestand</p> </td> 
      <td> <p> Weergave</p> <p>Voorkeuren </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Downloaden**.
1. Doorgaan met [De spreadsheetsjabloon vullen met uw gegevens](#populate-the-spreadsheet-template-with-your-data) om de sjabloon te vullen met uw gegevens.

## De spreadsheetsjabloon vullen met uw gegevens {#populate-the-spreadsheet-template-with-your-data}

* [Over de tabbladen (gegevensbladen) in het werkblad](#about-the-tabs-data-sheets-included-in-the-spreadsheet)
* [Een record importeren](#import-a-record)
* [Datums opnemen](#include-dates)
* [Jokertekens gebruiken](#use-wildcards)
* [Vervanging van kenmerknaam voor id&#39;s](#attribute-name-substitution-for-ids)

### Over de tabbladen (gegevensbladen) in het werkblad {#about-the-tabs-data-sheets-included-in-the-spreadsheet}

>[!TIP]
>
>Om beter te begrijpen hoe u de informatie in elke kolom zult moeten formatteren wanneer u het Kick-Begin malplaatje bevolkt, denk na handelend een praktijk door een Kick-Begin met bestaande gegevens van Workfront over de voorwerpen uit te voeren u probeert om in te voeren. Zie voor instructies [Gegevens exporteren uit Adobe Workfront via Kick-start](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

Wanneer u een leeg Kick-Begint malplaatje opent, zijn een aantal lusjes (gegevensbladen) beschikbaar. Ze zijn afhankelijk van de objecten die u hebt geselecteerd om te downloaden. Elk object vertegenwoordigt een object in de toepassing, zoals project, taken, uren, dashboard en gebruikers:

Wanneer u een van deze tabbladen opent, worden in rij 2 de velden weergegeven voor elk object dat tijdens het importeren kan worden ingesteld. In een kolomkop wordt na het woord &quot;set&quot; de naam van het veld weergegeven zoals deze in de database wordt weergegeven. Deze velden fungeren als kolomkoppen.

>[!IMPORTANT]
>
>Zorg voor het volgende om fouten te voorkomen:
>
>* Verwijder of wijzig deze velden op geen enkele manier. Wijzig bijvoorbeeld hun volgorde of naam niet.
>* Vul elk veld met een kolomkop die vet wordt weergegeven. Deze vertegenwoordigen vereiste velden.
>
>  Als een vereist veld echter een standaardwaarde bevat die is ingesteld in de systeemvoorkeuren, hoeft u deze waarde niet in te vullen.
>
>  Bijvoorbeeld op **PROJ Project** de **setCondition** en **setConditionType** velden kunnen leeg blijven, maar de **setGroupID** en **setName** kolommen kunnen niet.
>

### Een record importeren  {#import-a-record}

Elke rij van het blad komt overeen met een uniek object.

1. Voltooi de cel in het dialoogvenster **isNew** kolom:

   * Als het object dat u importeert nieuw is, typt u **TRUE** de gegevens in de rij importeren.
   * Als het object zich al in Workfront bevindt, typt u **FALSE** om de rij te negeren.

1. Voltooi de cel in het dialoogvenster **ID** kolom op een van de volgende manieren:

   * Als het object dat u importeert nieuw is (en u typt **TRUE** in de **isNew** (kolom), geeft u een willekeurig nummer voor de id op. Dit nummer moet uniek zijn in het werkblad.

   * Als het object dat u importeert al in het Workfront-systeem bestaat (en u typt **FALSE** in de **isNew** kolom), moet identiteitskaart de alpha-numerieke GUID zijn die in Workfront voor dat voorwerp bestaat.

     ![Voorbeeld-id voor een groep](assets/kick-start-group-example.png)

   * Wanneer u een project invoert, moet u op een identiteitskaart van de Groep wijzen.

      * Als de groep al in Workfront bestaat, moet u de unieke id ervan toevoegen aan de **setGroupID** veld voor het project.
      * Als de groep niet bestaat in Workfront, kunt u de opdracht **GROEP** blad naar uw importbestand instellen **isNew** veld naar **TRUE** op het groepsblad en geef een numerieke id op voor de nieuwe groep in de **ID** kolom. De **setGroupID** veld voor het nieuwe project moet overeenkomen met het numerieke veld **ID** voor de nieuwe groep.

     **Voorbeeld:** Voor een project, de waarde die in **setGroupID** kolom moet een van de volgende vermeldingen bevatten:

      * GUID voor een bestaande Groep in uw instantie van Workfront
      * De waarde (getal) in de kolom Id in het dialoogvenster **GROEP** blad als u tijdens het importeren een nieuwe groep maakt

1. Voer waarden in voor de vereiste velden en alle andere velden die u tijdens het importeren wilt vullen.
1. (Optioneel) Aangepaste gegevens toevoegen:

   * Maak een nieuwe kolom voor elk aangepast veld dat u wilt opnemen in het importproces.
   * Geef elke nieuwe kolom voor het bijbehorende aangepaste veld de volgende naam: **DE:[Naam van aangepast veld zoals wordt weergegeven in Workfront]**.
   * In de kolom **setCategorieID**, typ GUID van de bestaande douanevorm waarop dit douaneveld verblijft. Dit veld is vereist bij het importeren van aangepaste gegevens.
   * Als u meerdere gegevenswaarden in het aangepaste veld wilt toevoegen (zoals keuzerondjes, selectievakjes of lijsten), gebruikt u het verticale scheidingsteken voor aangepaste gegevens op de balk &quot;|&quot; in het tabblad Voorkeuren om de waarden van elkaar te scheiden.

     **Voorbeeld:** Typ A|D onder de kolom DE:Departementen om afdeling A en afdeling D in uw douaneformulier te bevolken.

### Datums opnemen  {#include-dates}

Workfront kan de meeste datumnotaties verwerken. U moet er echter voor zorgen dat de datumkolom in het spreadsheet is opgemaakt als een datum. Het importeren mislukt als de kolom is opgemaakt als algemeen, een getal of tekst.

>[!TIP]
>
>De meeste mensen vinden het het gemakkelijkst om het formaat van MM/DD/YYYY (bijvoorbeeld: 07/10/2022) te gebruiken.

Workfront accepteert ook tijdwaarden als onderdeel van de datum (bijvoorbeeld: 07/10/2022 01:30 of 07/10/2022 1:00 PM).

Als u een tijd in de datum weglaat, voert Workfront een van de volgende handelingen uit:

* Gaat om 12:00 uur. Om het datumresultaat te zien u verwacht, moet de systeemtijdzone uw tijdzone aanpassen.
* Als het zich op een voorwerp bevindt dat met een programma wordt geassocieerd, verschuift de tijd aan de vroegste tijd dat het programma toestaat.

>[!NOTE]
>
>Wanneer u een UNIX-tijdstempel gebruikt, moet u nog drie nullen aan het einde van de waarde toevoegen.
>
>Als uw tijdstempel bijvoorbeeld 7336899000 is, zou u 7336899000000 invoeren in de cel.

### Jokertekens gebruiken {#use-wildcards}

U kunt de volgende vervangingen gebruiken wanneer het bevolken van uw Kick-Begin malplaatjespreadsheet:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Jokerteken</strong> </p> </th> 
   <th> <p><strong>Gedrag</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>$$TODAY</p> </td> 
   <td> <p>Indien gebruikt op een <strong>setDate</strong> in dit veld wordt de datum ingesteld op middernacht op de dag waarop u Kick-Start importeert.</p> <p>U kunt het jokerteken wijzigen met de standaardsyntaxis die is toegestaan met het jokerteken op een filter.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span>Als u wilt dat een project begint op de maandag van de week waarop het wordt geïmporteerd, kunt u <strong>$$TODAYbw</strong>. Hierdoor wordt de geplande startdatum van uw project ingesteld op zondag 12:00 uur. Aangezien het programma voor het project op dat moment waarschijnlijk geen werk toelaat, zal het om 9:00 beginnen maandagochtend.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>Indien gebruikt op een <strong>setDate</strong> in dit veld wordt de datum ingesteld op basis van het tijdstip waarop u de record maakt tijdens het importeren Kick-Start.</p> <p>U kunt het jokerteken wijzigen met de standaardsyntaxis die is toegestaan met het jokerteken op een filter.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span>Als u wilt dat een project 3 uur na het importeren start, kunt u <strong>$$NOW+3h</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>Indien gebruikt op een <strong>setAssignedToID</strong> of een ander op userID gebaseerd veld, wijst dit jokerteken het werk toe of associeert de record op een andere manier met de persoon die de import uitvoert.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$CUSTOMER</p> </td> 
   <td> <p>Dit jokerteken is speciaal toegevoegd voor Kick-Start-invoer van gebruikers. Wanneer een Workfront-account wordt gemaakt, wordt een gebruiker met het toegangsniveau Systeembeheerder gemaakt. De gebruikersnaam die aan de standaardbeheerder is toegewezen, kan als voorvoegsel worden gebruikt bij het maken van andere gebruikers in de account.</p> <p>Omdat gebruikersnamen in alle klanten uniek moeten zijn, is dit nuttig wanneer u verscheidene individuen met zeer gemeenschappelijke gebruikersnamen zoals John Smith hebt, die een gebruikersbenaming "jsmith."zouden kunnen hebben Door de gebruikersnaamtoewijzing met de standaardbeheerdersgebruikersnaam voor te bereiden, garandeert u dat elke gebruikersnaam uniek is (bijvoorbeeld: <strong>$$CUSTOMER.jsmith</strong>).</p> <p>Tip: een elegantere manier om ervoor te zorgen dat gebruikersnamen in het hele systeem uniek zijn, is door het e-mailadres van het individu in te voeren in de <strong>setUserName</strong> veld.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Vervanging van kenmerknaam voor id&#39;s  {#attribute-name-substitution-for-ids}

Hoewel het aan te raden is om waar mogelijk id&#39;s te gebruiken, is het soms lastig om te verwijzen naar id&#39;s van het ene vel naar het andere bij het instellen van een **setAttributeID** waarde. U kunt eenvoudig naar waarden verwijzen door de kolomkop te wijzigen.

**Voorbeelden:**

* **(importeren van project)**

  Wanneer het invoeren van projecten, plaats **setGroupID** van de projecten door **GROEP** blad, nota nemend van de respectieve Groep IDs, en het kleven van hen in de correcte cellen (**setGroupID** kolom) op de **PROJ Project** blad.

  Dit is mogelijk wanneer u met slechts een paar groepen en projecten werkt, maar als u met verschillende groepen werkt, is het niet praktisch.

  Om de Vervanging van de Naam van Attributen voor het hierboven beschreven voorbeeld te doen, verandert u **setGroupID** kolomkop naar **#setGroupID GROUP***name**. U kunt dan de groep van elk project door naam van verwijzingen voorzien.

  >[!NOTE]
  >
  >De optie om Vervanging van de Naam van Attributen te gebruiken is beperkt tot verwijzingen voor bestaande slechts verslagen. U kunt naamvervanging niet gebruiken voor objecten die u in dezelfde importbewerking maakt.

* **(importeren door gebruiker)**

  Vul bij het importeren van gebruikers de **setRoleID** uit een lijst met rollen in het **ROL** tab.

  Sommige rol-id&#39;s zijn bedoeld voor records die al in de account staan, terwijl andere id&#39;s tijdens het importeren worden gemaakt.

  Voor de nieuwe gebruikersverslagen die aan bestaande rollen worden toegewezen, kunt u naamvervanging gebruiken. Voor de nieuwe gebruikersverslagen die aan onlangs ingevoerde rollen worden toegewezen, kunt u niet.

  Op deze manier kunt u beide methoden gebruiken voor hetzelfde importbestand:

   * Voeg een kolom in het spreadsheet links van toe **setRoleID** kolom.
   * Geef de nieuwe kolom een naam **#setRoleID ROLE name**.
   * Voor roltoewijzingen aan bestaande records voert u de rolnamen in het dialoogvenster **#setRoleID ROLE name** kolom.

     Voor roltoewijzingen aan nieuwe rolverslagen, input identiteitskaart u op het blad van de Rol van de ROL in setRoleID toewees.

     ![Rol-id voor gebruikers](assets/set-role-id.png)

## De spreadsheetgegevens importeren in Workfront

Nadat u de Excel-sjabloon met uw gegevens hebt gevuld, kunt u de Excel-sjabloon uploaden naar Workfront.

Het importeren Kick-Start ondersteunt de volgende bestandstypen:

* Op XML gebaseerde Excel (.xlsx)
* Oudere Excel (.xls)
* Zipped-bestand (.ZIP) (dat alleen .xlsx- of .xls-bestanden bevat)

  >[!NOTE]
  >
  >U moet een .ZIP dossier gebruiken wanneer het invoeren van de spreadsheets van Excel die de volgende voorwerpen van verwijzingen voorzien:
  >
  >* Rapporten
  >* Documenten
  >* Avatars
  >* Eigenschappenbestanden weergeven, filteren of groeperen.
  >
  >Wanneer u een gecomprimeerd importbestand gebruikt, moet het ZIP-bestand dezelfde naam hebben als het XSL- of XLS-bestand en moeten alle bestanden op hetzelfde structuurniveau staan (geen mappen).

De sjabloonspreadsheetgegevens importeren in Workfront:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Systeem** >**Gegevens importeren (Kick-start)**.

1. In de **Gegevens uploaden met werkblad Kick-Start** sectie, klikken **Bestand kiezen** Blader vervolgens naar de gevulde spreadsheet en selecteer deze.

1. Klikken **Uploaden.**

   Als het Excel-bestand langer dan 5 minuten duurt om naar Workfront te uploaden, wordt de toepassing uitgerekt en kan het bestand niet worden geüpload.

   Importeer de gegevens in kleinere batches met objecten.

1. (Voorwaardelijk) Als u Workfront Fusion gebruikt, kunt u nu FLO&#39;s of scenario&#39;s inschakelen.
