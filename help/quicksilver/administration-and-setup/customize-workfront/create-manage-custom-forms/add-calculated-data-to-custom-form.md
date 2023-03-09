---
title: Berekende gegevens toevoegen aan een aangepast formulier met de oudere formulierbuilder
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: In een aangepast formulier kunt u een berekend aangepast veld maken waarmee berekeningen worden gegenereerd. Hiertoe maakt u een instructie die gegevensexpressies en de namen van bestaande velden gebruikt. Dit kunnen aangepaste velden, berekende aangepaste gegevensvelden en ingebouwde Workfront-velden zijn. Deze verklaring berekent de gegevens u ingaat en toont het resultaat in het nieuwe berekende douaneveld.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9174c4ef-3beb-4d47-9c5c-363f52105a2c
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '2573'
ht-degree: 0%

---

# Berekende gegevens toevoegen aan een aangepast formulier met de oudere formulierbuilder

In een aangepast formulier kunt u een berekend aangepast veld toevoegen waarin bestaande gegevens worden gebruikt om nieuwe gegevens te genereren wanneer het aangepaste formulier aan een object wordt gekoppeld.

Een berekend aangepast veld kan het volgende bevatten:

* Een eenvoudige verwijzing naar één ingebouwd veld.

   >[!INFO]
   >
   > **Voorbeeld:** Om de opbrengst te berekenen die door projecten en taken wordt geproduceerd, kon u een berekend douanegebied tot stand brengen dat de ingebouwde Ware Inkomsten van het gebied bevat. Wanneer iemand de douaneformulier aan een project of een taak vastmaakt, toont de opbrengst voor het project of de taak op het gebied.

* Een expressie die naar een of meer velden verwijst. Dit kunnen aangepaste velden, andere berekende aangepaste velden en ingebouwde velden zijn.

   >[!INFO]
   >
   >**Voorbeeld:** Om de winst te berekenen die door projecten en taken wordt geproduceerd, kon u een berekend gebied tot stand brengen genoemd Winst die een wiskundige uitdrukking bevat die kosten van opbrengst aftrekt.
   >
   >Hiervoor kunt u de wiskundige expressie SUB (subtract) gebruiken met de ingebouwde velden Werkelijke kosten en Werkelijke inkomsten van Workfront.
   >
   >In de onderstaande stappen kunt u zien hoe dit voorbeeld kan worden uitgevoerd.

Voor informatie over het maken van aangepaste formulieren voor uw organisatie en het begrijpen van het type velden dat u ermee kunt koppelen, raadpleegt u [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

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
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> <p>Ga voor informatie over hoe Workfront-beheerders deze toegang verlenen naar <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, type licentie of configuraties op toegangsniveau u hebt.

## Een berekend veld toevoegen aan een aangepast formulier {#add-a-calculated-field-to-a-custom-form}

U kunt zowel ingebouwde Workfront-velden als aangepaste velden gebruiken die u al hebt gemaakt.

>[!IMPORTANT]
>
>Voordat u een nieuw berekend aangepast veld maakt, moet u de bestaande velden identificeren die u wilt opnemen, zodat u zeker weet dat de gegevens die nodig zijn voor de berekening aanwezig zijn in Workfront.

1. Beginnen met het maken of bewerken van een aangepast formulier, zoals beschreven in [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Op de **Veld toevoegen** tabblad, klikt u op **Berekend**.

   In het weergavegebied aan de rechterkant wordt het veld weergegeven *12345*. Dit is slechts een indicator om u eraan te herinneren dat het veld een berekend aangepast veld is terwijl u het aangepaste formulier maakt of bewerkt. Wanneer het formulier aan een object is gekoppeld en gebruikers het invullen, zien ze het resultaat van de berekening in het veld, nooit de waarde *12345* -indicator.

1. Geef de volgende informatie op voor het berekende veld:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td>Typ een label voor het veld. Dit is wat gebruikers zien wanneer ze het aangepaste formulier gebruiken. Het veld <b>Naam</b>, die automatisch invult, wordt door Workfront in rapporten genoemd.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" id="instructions">Instructies</td> 
      <td> Standaard wordt de formule die u voor het veld maakt hier opgeslagen. U kunt tekst toevoegen voor aanvullende informatie over het veld en de formule in het veld. Dit kan op twee manieren nuttig zijn: 
       <ul> 
        <li> <p>Als herinnering aan wat de formule is en hoe het werkt. Dit is vooral handig als u dit berekende aangepaste veld wilt gebruiken op meerdere formulieren.</p> </li> 
        <li> <p>Als knopinfo kunnen gebruikers zien wanneer ze de muisaanwijzer op het veld plaatsen. U voegt hier tekst toe die u in de knopinfo wilt zien.</p> <p>Als u niet wilt dat zij de formule in tooltip zien, wat voor hen verwarrend zou kunnen zijn, kunt u het verbergen. Zie de tabelrij "Formule weergeven in instructies" in de sectie voor instructies <a href="#build-the-calculation-for-your-calculated-custom-field" class="MCXref xref">De berekening maken voor het berekende aangepaste veld</a> in dit artikel.</p> </li> 
       </ul> <p>Voor informatie over het gebruik van hetzelfde berekende aangepaste veld op een nieuw formulier raadpleegt u <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md#using-an-existing-calculated-custom-field-on-a-new-form" class="MCXref xref">Een bestaand berekend aangepast veld opnieuw gebruiken in een aangepast formulier</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Indeling</td> 
      <td> <p>De indeling waarin u de resultaten van het veld wilt opslaan en weergeven.</p> <p>Als het veld wordt gebruikt in wiskundige berekeningen, moet u altijd een <strong>Getal</strong> of <strong>Valuta</strong> gebruiken. Als u Getal of Valuta selecteert, wordt het systeem automatisch gebruikt voor het afkappen van getallen die met 0 beginnen.</p> 
      <p><b>BELANGRIJK</b>: Voordat u een indeling kiest, moet u rekening houden met de juiste indeling voor het nieuwe veld. Het indelingsveld kan niet worden bewerkt nadat het aangepaste formulier is opgeslagen. En het selecteren van het verkeerde formaat kon toekomstige berekeningen en samengevoegde waarden in rapport en lijstgroepen beïnvloeden.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Doorgaan naar [De berekening maken voor het berekende aangepaste veld](#build-the-calculation-for-your-calculated-custom-field) in dit artikel.

## De berekening maken voor het berekende aangepaste veld {#build-the-calculation-for-your-calculated-custom-field}

1. Beginnen met het maken van het berekende aangepaste veld, zoals wordt uitgelegd in de sectie [Een berekend veld toevoegen aan een aangepast formulier](#add-a-calculated-field-to-a-custom-form) in dit artikel.

1. Klikken **Maximaliseren** om de **Rekeneditor** en maak uw berekening.

   >[!INFO]
   >
   >**Voorbeeld:** Gebruikend het voorbeeld in de inleiding aan dit artikel, kon u een berekend gebied tot stand brengen van de douane genoemd Winst in een douaneformulier voor projecten en taken. Dit veld kan een berekening bevatten die het verschil weergeeft tussen de werkelijke en de werkelijke kosten:
   >
   >`SUB({actualRevenue},{actualCost})`
   >
   >In dit voorbeeld: `SUB` is de expressie en de velden waarnaar wordt verwezen, zijn `actualRevenue` en `actualCost`.

   Een berekening begint gewoonlijk met een expressie, gevolgd door haakjes die de velden bevatten waarnaar u wilt verwijzen wanneer het aangepaste formulier aan een object is gekoppeld. Voor informatie over de beschikbare expressies raadpleegt u [Berekende gegevensexpressies](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Elk veld moet met accolades zijn omgeven, zoals in de sectie wordt uitgelegd [Syntaxis vereist in berekende aangepaste velden](#syntax-required-in-calculated-custom-fields) in dit artikel. Wanneer u de naam van een veld begint te typen, doet het systeem suggesties en kunt u er een selecteren om het veld in de berekening in te voegen.

   In een berekening kunt u naar elk type aangepast veld verwijzen, met uitzondering van twee: Tekstveld met opmaaktype en beschrijvende tekst. Zie voor informatie over de aangepaste veldtypen [Een aangepast veld toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)

1. Klik in het grote tekstvak en klik vervolgens op **Expressies** en **Velden** die beschikbaar zijn om deze aan uw berekening toe te voegen.

   U kunt ook een expressie of veld in het grote tekstvak typen en deze selecteren wanneer deze wordt weergegeven. Elk item wordt weergegeven met een &#39;F&#39; voor een veld of een &#39;E&#39; voor een expressie.

   Als u een haakje openen typt, wordt het haakje sluiten automatisch toegevoegd.

   >[!TIP]
   >
   >U kunt een van de volgende handelingen uitvoeren om hulp te krijgen bij uw berekening:
   > 
   >* Houd de muisaanwijzer boven een expressie in uw berekening om een beschrijving te bekijken, een voorbeeld van het gebruik ervan en een koppeling Meer informatie in het artikel [Berekende gegevensexpressies](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
      >  ![](assets/hover-expression-help-text.jpg)
   >* Gebruik de kleurcodering om de componenten te identificeren die u hebt toegevoegd. Expressies worden in blauw weergegeven en velden in groen.
      >  ![](assets/colors-fields-expressions.jpg)
   >* Zoek rekenfouten die roze gemarkeerd zijn. U kunt de muisaanwijzer boven een gemarkeerde fout plaatsen om een korte beschrijving van de oorzaak van de fout weer te geven.
      >  ![](assets/error-help.png)
   >* Geef een voorvertoning van de resultaten weer in het gebied onder de berekening.
      ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->

      >  ![](assets/preview-calc.jpg)
   >* Verwijzingsexpressies in een lange berekening met behulp van de regelnummers die aan de linkerkant worden weergegeven.


1. Klikken **Minimaliseren** als u klaar bent met het maken van de berekening voor het berekende aangepaste veld.

   >[!NOTE]
   >
   >In het weergavegebied aan de rechterkant wordt het veld weergegeven *12345.* Dit is slechts een indicator om u eraan te herinneren dat het veld een berekend aangepast veld is terwijl u het aangepaste formulier maakt of bewerkt. Wanneer het formulier aan een object is gekoppeld en gebruikers het invullen, zien ze het resultaat van de berekening in het veld, nooit de waarde *12345* -indicator.

1. (Optioneel) Gebruik een van de volgende opties om het berekende aangepaste veld verder te configureren:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Logica toevoegen</td> 
      <td>U kunt DisplayLogic toevoegen om te bepalen of het berekende veld wordt weergegeven op basis van ten minste één keuze die een gebruiker maakt in een voorafgaand meerkeuzeveld (vervolgkeuzelijst, Selectievakjes of Keuzerondjes) bij het invullen van het formulier. Zie voor meer informatie <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Weergavelogica toevoegen en logica overslaan naar een aangepast formulier</a>. <p>Dit is alleen beschikbaar als ten minste één selectievakje, keuzerondje of vervolgkeuzelijst voorafgaat aan het berekende aangepaste veld op het formulier. </p> <p>Logica overslaan is niet beschikbaar voor berekende aangepaste velden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vorige berekeningen bijwerken</td> 
      <td>Wanneer u een bestaand berekend aangepast veld bewerkt, kunt u deze optie selecteren om een update in de berekening te activeren wanneer u het aangepaste formulier opslaat. Dit gebeurt slechts eenmaal wanneer u het aangepaste formulier opslaat. De optie keert naar zijn gehandicapte staat terug nadat u dit doet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formule weergeven in instructies</td> 
      <td>Laat deze optie ingeschakeld als u wilt dat gebruikers die het aangepaste formulier invullen, de formule van het veld zien wanneer ze de muisaanwijzer op het veld plaatsen. Zie de informatie over <a href="#instructions" class="MCXref xref">Instructies</a> eerder in deze tabel.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Gereed** wanneer alle wijzigingen zijn voltooid in het berekende aangepaste veld.

   Of klik op **Toepassen** om uw wijzigingen tot nu toe op het formulier toe te passen als u aangepaste velden wilt blijven toevoegen aan het formulier.

   Of klik op **Opslaan + Sluiten** als alle wijzigingen zijn voltooid op het aangepaste formulier.
1. Als u wilt controleren of het berekende aangepaste veld correct werkt, koppelt u het aangepaste formulier aan een object en bekijkt u het resultaat in het berekende aangepaste veld.

   Voor instructies voor het bijvoegen van een aangepast formulier raadpleegt u [Een aangepast formulier toevoegen aan een object](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   Als u op andere manieren een aangepast formulier wilt maken, kunt u verdergaan met het samenstellen van een van de volgende artikelen:

   * [Een aangepast veld toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Aangepaste velden en widgets in een aangepast formulier plaatsen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Een middelenwidget toevoegen of bewerken in een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Een bestaand berekend aangepast veld opnieuw gebruiken in een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Weergavelogica toevoegen en logica overslaan naar een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Een aangepast formulier voorvertonen en invullen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## Syntaxis vereist in berekende aangepaste velden

Voor elk veld moet de hieronder beschreven syntaxis worden gebruikt, met accolades rond elke veldnaam. Wanneer u de naam van een veld begint te typen, doet het systeem suggesties en kunt u er een selecteren om het veld in de berekening in te voegen. Als u gegevens onjuist invoert in een berekening, verschijnt er een waarschuwing. U kunt het formulier alleen opslaan als u de berekening bewerkt en geldige velden en een geldige berekende expressie opgeeft.

>[!NOTE]
>
>Het systeem doet momenteel alleen suggesties wanneer u de naam begint te typen van een veld waarnaar u wilt verwijzen voor een object waaraan het aangepaste formulier wordt gekoppeld, niet voor het bovenliggende object van het object.

### Namen van ronde velden met accolades

* Als u wilt dat de berekening naar een ingebouwd veld verwijst, moet de naam van het veld tussen accolades staan.

Bijvoorbeeld: `{actualRevenue}`

Veldnamen zijn hoofdlettergevoelig en moeten in de berekening precies worden weergegeven hoe ze in het Workfront-systeem worden weergegeven.

* Als u wilt dat de berekening naar een aangepast veld verwijst, moet de naam van het veld tussen accolades staan en door `DE:` tussen de haakjes.

Bijvoorbeeld: `{DE:Profit}`

In het systeem worden alle aangepaste velden weergegeven waaruit u kunt kiezen wanneer u typt `DE:`.

* Als u wilt dat de berekening verwijst naar een veld dat gegevens uit het veld *parent* Als het aangepaste formulier aan een object is gekoppeld, moet u de veldnaam ook tussen accolades en het objecttype van het bovenliggende object plaatsen.

   Als het aangepaste formulier bijvoorbeeld is geconfigureerd om te werken met taken en u wilt dat het veld de werkelijke inkomsten van het bovenliggende object berekent wanneer het formulier aan een taak is gekoppeld, moet u aangeven `Project` als het objecttype van het veld:

   `{project}.{actualRevenue}`

   Of als het een aangepast veld is:

   `{project}.{DE:profit}`

   Als u niet zeker bent wat het objecttype van het oudervoorwerp zal zijn omdat de douane voor voor veelvoudige objecten types wordt gevormd, kunt u de variabele van de vervangingsfilter gebruiken `$$OBJCODE` om de berekening voor elk van de mogelijke typen te laten werken. Zie voor meer informatie [Berekende aangepaste velden in aangepaste formulieren voor meerdere objecten](#calculated-custom-fields-in-multi-object-custom-forms) in dit artikel.

### Afzonderlijke items met perioden

Wanneer u in een berekend aangepast veld naar een verwant object verwijst, moet u namen en kenmerken van objecten scheiden met punten.

Als u bijvoorbeeld in een aangepast taaktype formulier de naam van de eigenaar van de Portfolio wilt weergeven in een berekend aangepast veld, typt u het volgende:

`{project}.{porfolio}.{owner}`

Dit bepaalt het volgende: Via het object van het aangepaste formulier (een taak) hebt u toegang tot het volgende object dat betrekking heeft op de taak (een project). Van daar, kunt u tot het volgende verwante voorwerp aan het project (een portefeuille) toegang hebben, dan het volgende verwante voorwerp aan de portefeuille (de eigenaar).

### Naamsyntaxis voor het verwijzen naar een aangepast veld

Wanneer u in een berekend aangepast veld naar een ander aangepast veld verwijst, moet u de naam van het veld invoeren zoals dit wordt weergegeven in de gebruikersinterface van Workfront.

Als u bijvoorbeeld wilt verwijzen naar de geselecteerde optie in een aangepast veld met de naam Executive sponsor, typt u het volgende:

`{DE:Executive sponsor}`

>[!NOTE]
>
>De syntaxis voor een veld met een typekop is iets anders dan voor andere typen velden, omdat u deze moet toevoegen `:name` aan het einde.
>
>Als u bijvoorbeeld wilt verwijzen naar de geselecteerde optie in een aangepast tekstveld met de naam &quot;Executive sponsor&quot;, typt u:
>
>`{DE:Executive sponsor:name}`


## Berekende aangepaste velden in aangepaste formulieren voor meerdere objecten {#calculated-custom-fields-in-multi-object-custom-forms}

In een aangepast formulier met meerdere objecten moeten de geselecteerde objecttypen compatibel zijn met alle velden waarnaar wordt verwezen in de berekende aangepaste velden van het formulier. Als er sprake is van incompatibiliteit, wordt u gewaarschuwd dat u aanpassingen moet aanbrengen.

>[!INFO]
>
>**Voorbeeld:**
>
>In een aangepast formulier dat is geconfigureerd om te werken met het taakobjecttype, maakt u een berekend aangepast veld met de naam In Charge. U configureert de methode om te verwijzen naar het ingebouwde veld, zodat de naam van de primaire ontvanger die de leiding heeft, wordt weergegeven wanneer het formulier aan een taak is gekoppeld:
>
>`{assignedTo}.{name}`
>
>Later voegt u het objecttype Project toe aan het aangepaste formulier. Een waarschuwingsbericht geeft aan dat het objecttype Project niet compatibel is met het berekende aangepaste veld.

Wanneer dit voorkomt, kunt u één van het volgende doen:

* Verwijder een van de twee incompatibele items uit het aangepaste formulier. Dit is het objecttype of het berekende aangepaste veld waarnaar wordt verwezen.
* Beide items behouden en de filtervariabele voor jokertekens gebruiken `$$OBJCODE` als een voorwaarde in een IF-expressie om twee verschillende versies van het veld In laden te maken. Hierdoor werkt het veld goed, ongeacht het type object waaraan het formulier is gekoppeld.

>[!INFO]
>
>**Voorbeeld:** Er is echter geen toewijzing aan: Het gebied van de naam in projecten, is er een ingebouwd gebied van de Eigenaar (dat automatisch met de naam van de persoon invult die het project creeerde, tenzij iemand manueel dit verandert).
>
>In het veld Aangepast in lading kunt u dus `$$OBJCODE` zoals hieronder getoond om het gebied van de Eigenaar van verwijzingen te voorzien wanneer het douaneformulier aan een project in bijlage is, en toegewezen aan: Veld benoemen wanneer het formulier aan een taak is gekoppeld:
>
>`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

Voor meer informatie over variabelen zoals `$$OBJCODE,` zie [Variabelen van jokerfilter](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Automatische updates van berekende aangepaste velden

Berekende aangepaste velden op een object worden automatisch opnieuw berekend wanneer het volgende gebeurt:

* Er verandert iets op het object, zoals een dagelijkse tijdlijnberekening.
* Iemand bewerkt een ander veld waarnaar wordt verwezen door een berekend aangepast veld op het object.
* De berekende expressie is leeg en het veld bevat een waarde. Deze stelt de waarde in op null.

   >[!NOTE]
   >
   ><div>In een douaneformulier in bijlage aan een voorwerp, worden de datum en de tijdverklaringen in berekende douanevelden berekend en bewaard door Coordinated Universal Time (UTC), niet door de configuraties van de tijdzone die voor de instantie van uw organisatie en uw gebruikersprofiel worden geplaatst. Berekeningen in een aangepast formulier worden gegenereerd op basis van de afzonderlijke tijdzones van elke gebruiker.</div>

