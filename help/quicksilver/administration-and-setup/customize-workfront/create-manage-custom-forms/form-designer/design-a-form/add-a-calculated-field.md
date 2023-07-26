---
title: Berekende velden toevoegen met de formulierontwerper
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: U kunt een berekend aangepast veld toevoegen waarin bestaande gegevens worden gebruikt om nieuwe gegevens te genereren wanneer het aangepaste formulier aan een object wordt gekoppeld.
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 407aae49-4bc3-4364-a794-7e170a57a6d3
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '2317'
ht-degree: 0%

---

# Berekende velden toevoegen met de formulierontwerper

U kunt een berekend aangepast veld toevoegen waarin bestaande gegevens worden gebruikt om nieuwe gegevens te genereren wanneer het aangepaste formulier aan een object wordt gekoppeld.

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
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> <p>Ga voor informatie over hoe Workfront-beheerders deze toegang verlenen naar <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, type licentie of configuraties op toegangsniveau u hebt.

## Een bestaand berekend aangepast veld opnieuw gebruiken in een aangepast formulier

U kunt hetzelfde berekende aangepaste veld gebruiken voor aangepaste formulieren die bij verschillende objecten horen. U kunt bijvoorbeeld het berekende veld Winst gebruiken dat u voor het aangepaste formulier voor het project hebt gemaakt, op een aangepaste taakvorm.

Als u een bestaand berekend aangepast veld gebruikt, wordt de berekening niet overgedragen naar het nieuwe formulier. U moet de berekening opnieuw toevoegen in hetzelfde veld op het nieuwe aangepaste formulier.

U kunt ook een andere berekening voor hetzelfde veld uitvoeren op het nieuwe formulier. Als u dezelfde naam voor het berekende aangepaste veld behoudt, bent u verzekerd van consistentie en consistentie in de naamgevingsconventie.

>[!IMPORTANT]
>
>Door wijzigingen in berekende expressies kan de veldwaarde van objecten verouderd raken. Voer een van de volgende handelingen uit om ervoor te zorgen dat u altijd de bijgewerkte berekening in deze velden weergeeft:
>
>* Nadat u een object hebt opgeslagen waar u gegevens hebt bewerkt in een aangepast formulier, klikt u op het pictogram Meer ![](assets/more-icon.png) op de hoofdpagina van het object en vervolgens Aangepaste expressies opnieuw berekenen.
>* Selecteer de optie Aangepaste expressies opnieuw berekenen wanneer u objecten bulksgewijs bewerkt.
>* Selecteer de optie Vorige berekeningen bijwerken wanneer u een berekend aangepast veld op een aangepast formulier bewerkt.

Een bestaand berekend aangepast veld opnieuw gebruiken:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Aangepaste Forms** in het linkerdeelvenster.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Klikken **Nieuw aangepast formulier.**
1. Selecteer de objecttypen waaraan u het aangepaste formulier wilt koppelen en klik vervolgens op **Doorgaan**.

1. Klik in de linkerbovenhoek van het scherm op **Veldbibliotheek**.

   ![](assets/field-library.png)

1. Gebruik het zoekvak of vouw de **Berekend** om het berekende veld te zoeken dat u nodig hebt en sleep het veld naar de plaats waar u het wilt weergeven in het aangepaste formulier.

1. (Optioneel) Herhaal de vorige stap om andere velden toe te voegen.

   >[!NOTE]
   >
   >U kunt maximaal 500 velden en widgets toevoegen aan één aangepast formulier. De prestaties kunnen echter afnemen wanneer er meer dan 100 formulieren op een formulier staan, afhankelijk van de complexiteit ervan.
   >
   >
   >Voorbeelden van complexe formulieren zijn formulieren met trapsgewijze parameters, berekende aangepaste gegevensvelden en opties voor meerdere waarden in één veld.

1. Als u de wijzigingen wilt opslaan, klikt u op **Toepassen** en ga naar een andere sectie om door te gaan met het samenstellen van uw formulier.

   of

   Klikken **Opslaan en sluiten**.

## Een nieuw berekend veld toevoegen

>[!IMPORTANT]
>
>Voordat u een nieuw berekend aangepast veld maakt, moet u de bestaande velden identificeren die u wilt opnemen, zodat u zeker weet dat de gegevens die nodig zijn voor de berekening aanwezig zijn in Workfront.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Aangepaste Forms** in het linkerdeelvenster.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Klikken **Nieuw aangepast formulier.**
1. Selecteer de objecttypen waaraan u het aangepaste formulier wilt koppelen en klik vervolgens op **Doorgaan**.

1. Op de linkerkant van het scherm, vind **Berekend** en sleep het naar een sectie op het canvas.

   ![](assets/drag-field-to-section.png)

1. Configureer rechts in het scherm de opties die beschikbaar zijn voor het type aangepast veld dat u toevoegt:

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
      <li><p>Als herinnering aan wat de formule is en hoe het werkt. Dit is vooral handig als u dit berekende aangepaste veld wilt gebruiken op meerdere formulieren.</p> </li> 
      <li> <p>Als knopinfo kunnen gebruikers zien wanneer ze de muisaanwijzer op het veld plaatsen. U voegt hier alle tekst toe die u in de knopinfo wilt zien.</p> <p>Als u niet wilt dat zij de formule in tooltip zien, wat voor hen verwarrend zou kunnen zijn, kunt u het verbergen.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Indeling</td> 
      <td> <p>De indeling waarin u de resultaten van het veld wilt opslaan en weergeven.</p> <p>Als het veld wordt gebruikt in wiskundige berekeningen, moet u altijd een <strong>Getal</strong> of <strong>Valuta</strong> gebruiken. Als u Getal of Valuta selecteert, wordt het systeem automatisch gebruikt voor het afkappen van getallen die met 0 beginnen.</p> 
      <p><b>BELANGRIJK</b>: Voordat u een indeling kiest, moet u rekening houden met de juiste indeling voor het nieuwe veld. Het indelingsveld kan niet worden bewerkt nadat het aangepaste formulier is opgeslagen. En het selecteren van het verkeerde formaat kon toekomstige berekeningen en samengevoegde waarden in rapport en lijstgroepen beïnvloeden.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. In de **Berekening** begint met het maken van uw berekening:
   1. Klikken **Maximaliseren** om de Rekeningeditor te openen en uw berekening samen te stellen.</p>
Een berekening begint gewoonlijk met een expressie, gevolgd door haakjes die de velden bevatten waarnaar u wilt verwijzen wanneer het aangepaste formulier aan een object is gekoppeld.

      Elk veld moet met accolades zijn omgeven. Wanneer u de naam van een veld begint te typen, doet het systeem suggesties en kunt u er een selecteren om het veld in de berekening in te voegen.

+++ **Uitbreiden om de vereiste syntaxis in berekende aangepaste velden te bekijken**

      Voor elk veld moet de hieronder beschreven syntaxis worden gebruikt, met accolades rond elke veldnaam. Wanneer u de naam van een veld begint te typen, doet het systeem suggesties en kunt u er een selecteren om het veld in de berekening in te voegen. Als u onjuiste gegevens in een berekening invoert, verschijnt er een waarschuwingsbericht. U kunt het formulier alleen opslaan als u de berekening bewerkt en geldige velden en een geldige berekende expressie opgeeft.

      >[!NOTE]
      >
      >Het systeem doet momenteel alleen suggesties wanneer u de naam begint te typen van een veld waarnaar u wilt verwijzen op een object waaraan het aangepaste formulier wordt gekoppeld. Velden van het bovenliggende object worden niet voorgesteld.

      **Namen van ronde velden met accolades**

      * Als u wilt dat de berekening naar een ingebouwd veld verwijst, moet de naam van het veld tussen accolades staan.

        Bijvoorbeeld: `{actualRevenue}`

        Veldnamen zijn hoofdlettergevoelig en moeten in de berekening precies worden weergegeven hoe ze in het Workfront-systeem worden weergegeven.

        Ga naar de [Workfront API Explorer](https://developer.adobe.com/workfront/api-explorer/) om de veldnamen te identificeren die in berekeningen kunnen worden gebruikt.

      * Als u wilt dat de berekening naar een aangepast veld verwijst, moet de naam van het veld tussen accolades staan en door `DE:` tussen de haakjes.

        Bijvoorbeeld: `{DE:Profit}`

        In het systeem worden alle aangepaste velden weergegeven waaruit u kunt kiezen wanneer u typt `DE:`.

         * Als u wilt dat de berekening verwijst naar een veld dat gegevens uit het veld *parent* Als het aangepaste formulier aan een object is gekoppeld, moet u de veldnaam ook tussen accolades en het objecttype van het bovenliggende object plaatsen.

        Als het aangepaste formulier bijvoorbeeld is geconfigureerd voor taken en u wilt dat het veld de werkelijke inkomsten van het bovenliggende object berekent wanneer het formulier aan een taak is gekoppeld, moet u aangeven `Project` als het objecttype van het veld:

        `{project}.{actualRevenue}`

        Of als het een aangepast veld is:

        `{project}.{DE:profit}`

        **Afzonderlijke items met perioden**

        Wanneer u in een berekend aangepast veld naar een verwant object verwijst, moet u namen en kenmerken van objecten scheiden met punten.

        Als u bijvoorbeeld in een aangepast taaktype formulier de naam van de eigenaar van de Portfolio wilt weergeven in een berekend aangepast veld, typt u het volgende:

        `{project}.{porfolio}.{owner}`

        Dit zou het volgende bepalen: Van het voorwerp van het douaneformulier (een taak), kunt u tot het volgende voorwerp met betrekking tot de taak (een project) toegang hebben. Vanaf dat punt hebt u toegang tot het volgende verwante object voor het project (een portfolio) en kunt u vervolgens verwijzen naar de velden die zijn gedefinieerd voor het portfolioobject (de eigenaar)

        **Naamsyntaxis voor het verwijzen naar een aangepast veld**

        Wanneer u in een berekend aangepast veld naar een ander aangepast veld verwijst, moet u de naam van het veld invoeren die in de gebruikersinterface van Workfront wordt weergegeven.

        Als u bijvoorbeeld wilt verwijzen naar de geselecteerde optie in een aangepast veld met de naam Executive sponsor, typt u het volgende:

        `{DE:Executive sponsor}`

        >[!NOTE]
        >
        >De syntaxis voor een veld met een typekop is iets anders dan voor andere typen velden, omdat u deze moet toevoegen `:name` aan het einde.
        >
        >Als u bijvoorbeeld wilt verwijzen naar de geselecteerde optie in een aangepast tekstveld met de naam &quot;Executive sponsor&quot;, typt u:
        >
        >`{DE:Executive sponsor:name}`


        **Berekende aangepaste velden in aangepaste formulieren voor meerdere objecten**

        In een aangepast formulier met meerdere objecten moeten de geselecteerde objecttypen compatibel zijn met ten minste één veld waarnaar wordt verwezen in de berekende aangepaste velden van het formulier. Velden die niet compatibel zijn met het object, worden N.v.t. het formulier weergegeven.

        Als u er zeker van wilt zijn dat het berekende veld het juiste resultaat voor alle objecttypen weergeeft, moet u `$$OBJCODE` om een berekening te definiëren voor elk objecttype.

        >[!INFO]
        >
        >**Voorbeeld:**
        >
        >In een douaneformulier dat wordt gevormd om met projecten, taken, en kwesties te werken, kunt u de volgende formule gebruiken om het objecten type te tonen:
        >
        >`IF($$OBJCODE="PROJ","This is a project",IF($$OBJCODE="TASK","This is a task","This is an issue"))`
        >
        >Op een project zal het gebied &quot;Dit is een project&quot;tonen, op een taak zal het &quot;Dit is een taak&quot;tonen, en op een kwestie zal het &quot;Dit is een kwestie&quot;zeggen.


        >[!INFO]
        >
        >**Voorbeeld:** Hoewel er geen Toegewezen aan is: Het gebied van de Naam in projecten, is er een ingebouwd gebied van de Eigenaar (dat automatisch met de naam van de persoon invult die het project creeerde, tenzij iemand manueel dit verandert).
        >
        >In het veld Aangepast in lading kunt u dus `$$OBJCODE` zoals hieronder wordt getoond om naar het gebied van de Eigenaar te verwijzen wanneer het douaneformulier aan een project in bijlage is, en het Toegewezen aan: gebied van de Naam wanneer het formulier aan een taak in bijlage is:
        >
        >`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

        Voor meer informatie over variabelen zoals `$$OBJCODE,` zie [Variabelen van jokerfilter](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

        **Automatische updates van berekende aangepaste velden**

        Berekende aangepaste velden op een object worden automatisch opnieuw berekend wanneer het volgende gebeurt:

         * Er verandert iets op het object, zoals een dagelijkse tijdlijnberekening.
         * Iemand bewerkt een ander veld waarnaar wordt verwezen door een berekend aangepast veld op het object.
         * De berekende expressie is leeg en het veld bevat een waarde. Deze stelt de waarde in op null.

           >[!NOTE]
           >
           ><div>In een douaneformulier in bijlage aan een voorwerp, worden de datum en de tijdverklaringen in berekende douanevelden berekend en bewaard door Coordinated Universal Time (UTC), niet door de configuraties van de tijdzone die voor de instantie van uw organisatie en uw gebruikersprofiel worden geplaatst. Berekeningen in een aangepast formulier worden gegenereerd op basis van de afzonderlijke tijdzones van elke gebruiker.</div>

+++

   1. Klik in het grote tekstvak en klik vervolgens op **Expressies** en **Velden** die beschikbaar zijn om deze aan uw berekening toe te voegen.

      U kunt ook een expressie of veld in het grote tekstvak typen en deze selecteren wanneer deze wordt weergegeven. Elk item wordt weergegeven met een &#39;F&#39; voor een veld of een &#39;E&#39; voor een expressie.

      Als u een haakje openen typt, wordt het haakje sluiten automatisch toegevoegd.

+++ **Uitbreiden om nuttige tips weer te geven**
      >[!TIP]
      >
      >U kunt een van de volgende handelingen uitvoeren om hulp te krijgen bij uw berekening:
      > 
      >* Houd de muisaanwijzer boven een expressie in uw berekening om een beschrijving te bekijken, een voorbeeld van het gebruik ervan en een koppeling Meer informatie in het artikel [Berekende gegevensexpressies](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
      >  ![](assets/hover-expression-help-text.jpg)
      >* Gebruik de kleurcodering om de componenten te identificeren die u hebt toegevoegd. Expressies worden in blauw weergegeven en velden in groen.
      >  ![](assets/colors-fields-expressions.jpg)
      >* Zoek rekenfouten die roze gemarkeerd zijn. U kunt de muisaanwijzer boven een gemarkeerde fout plaatsen om een korte beschrijving van de oorzaak ervan weer te geven.
      >  ![](assets/error-help.png)
      >* Geef een voorvertoning van de resultaten weer in het gebied onder de berekening.
      ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
      >  ![](assets/preview-calc.jpg)
      >* Verwijzingsexpressies in een lange berekening met behulp van de regelnummers die aan de linkerkant worden weergegeven.

+++
   1. Klikken **Minimaliseren** als u klaar bent met het maken van de berekening voor het berekende aangepaste veld.

   1. (Optioneel) Gebruik een van de volgende opties om het berekende aangepaste veld verder te configureren:

      <table style="table-layout:auto">
   <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Logica toevoegen</td> 
      <td>U kunt DisplayLogic toevoegen om te bepalen of het berekende veld wordt weergegeven op basis van ten minste één keuze die een gebruiker maakt in een voorafgaand meerkeuzeveld (vervolgkeuzelijst, Selectievakjes of Keuzerondjes) bij het invullen van het formulier. <!-- For more information, see <a href="Need to add link for new article when it's written" class="MCXref xref">Add display logic and skip logic to a custom form</a>.--> <p>Dit is alleen beschikbaar als ten minste één selectievakje, keuzerondje of vervolgkeuzeveld voorafgaat aan het berekende aangepaste veld op het formulier. </p> <p>Logica overslaan is niet beschikbaar voor berekende aangepaste velden.</p> </td> 
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

1. Als u de wijzigingen wilt opslaan, klikt u op **Toepassen** en ga naar een andere sectie om door te gaan met het samenstellen van uw formulier.

   of

   Klikken **Opslaan en sluiten**.
