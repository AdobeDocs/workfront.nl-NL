---
product-area: reporting
navigation-topic: text-mode-reporting
title: Tekstmodus in een groep bewerken
description: '"OPMERKING: alle FVG-artikelen gelijk maken voor bewerking in tekstmodus)'''
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1559'
ht-degree: 0%

---

# Tekstmodus in een groep bewerken

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: make all FVG articles the same for editing in text mode)</p>
-->

U kunt een groepering in een lijst of een rapport uitgeven gebruikend tekstwijze om tot gebieden toegang te hebben die niet beschikbaar in de standaardinterface zijn en complexere groeperingen tot stand brengen.

>[!TIP]
>
>Wij adviseren dat u zoveel mogelijk van de groepering in standaardwijze bouwt, dan het in tekstwijze omzet om het uit te geven.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om groepen in een rapport te bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren om groepen in een rapport te bewerken</p> <p>Rechten voor een groep beheren om deze te bewerken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

Voordat u de tekstmodus in een rapport of lijst gaat gebruiken, moet u altijd op de hoogte zijn van de syntaxis in de tekstmodus van Workfront.

Zie voor meer informatie:

* [Overzicht van de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Overzicht van syntaxis in tekstmodus](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Voorbeelden van aangepaste weergaven, filters en groeperingen](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Tekstmodus in een groep bewerken

Het bewerken van een groep in de tekstmodus is identiek voor rapporten en lijsten. De toegang tot van de groepering van een rapport of van een lijst verschilt.

>[!NOTE]
>
>Groepen zijn een verplicht rapportageelement voor het maken van grafieken in rapporten. Groepen in tekstmodus worden niet ondersteund in grafieken. Voor informatie over het toevoegen van grafieken aan rapporten, zie [Een diagram toevoegen aan een rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

Voor meer informatie over bouwgroepen raadpleegt u [Groepen maken in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Voor informatie over het creëren van een rapport, zie [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Voer een van de volgende handelingen uit:

   1. Om tot de groepering van een rapport toegang te hebben, ga naar het rapport, dan klik **Handelingen rapporteren** > **Bewerken** > **Groepen** tab.
   1. Als u vanuit een lijst toegang wilt tot de groepering, gaat u naar de lijst en vanuit de **Groepering** vervolgkeuzelijst, houdt u de muis boven de groep die u wilt wijzigen en klikt u op de knop **Bewerken** pictogram ![](assets/edit-icon.png).

      De groeperingsbouwer wordt geopend.

1. Klikken **Groepering toevoegen** om de groepen toe te voegen, klikt u vervolgens op **Overschakelen naar tekstmodus** in de rechterbovenhoek van de builder.

   >[!TIP]
   U kunt maximaal drie groepen toevoegen in de standaardinterface. U kunt een vierde groep alleen met behulp van de tekstmodus toevoegen en u kunt in Workfront niet meer dan vier niveaus groeperen.

1. Typ de naam van een veld waarop u wilt groeperen.

   Selecteer de naam van het veld wanneer dit wordt weergegeven in de lijst.

1. Klikken **Overschakelen naar tekstmodus** in de rechterbovenhoek van de builder.

   De groepering wordt dan getoond op tekstwijze.

   Als u een groep bewerkt in de tekstmodus, voegt Workfront de opdracht

   ```
   textmode=true
   ```

   coderegel naar de groepering. Dit geeft aan dat de groepering wordt gewijzigd in de tekstmodus.

   **Voorbeeld:** Om een lijst van taken door de Naam van het Project en dan door de naam van de Primaire Ontvanger te groeperen, zou uw groepering als het volgende, op tekstwijze moeten kijken.

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   De vetgedrukte regels zijn verplicht.

   <!--
   <div class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <span class="autonumber"><span><b>Example: </b></span></span>
   <p>To group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode:</p>
   <p><code>textmode=true</code> </p>
   <p><code>group.0.linkedname=project</code> </p>
   <p><code>group.0.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.0.valuefield=project:name</code> </p>
   <p><code>group.0.namekeyargkey.0=project</code> </p>
   <p><code>group.0.namekeyargkey.1=name</code> </p>
   <p><code style="font-weight: bold;">group.0.valueformat=string</code> </p>
   <p><code>group.1.linkedname=assignedTo</code> </p>
   <p><code>group.1.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.1.valuefield=assignedTo:name</code> </p>
   <p><code>group.1.namekeyargkey.0=assignedTo</code> </p>
   <p><code>group.1.namekeyargkey.1=nam</code>e</p>
   <p><code style="font-weight: bold;">group.1.valueformat=string</code> </p> <note type="important">
   The lines in bold are mandatory.
   </note>
   </div>
   -->

   Elk veld in de groep bevat verschillende coderegels die naar dat veld verwijzen.

   In de onderstaande tabel worden de hoofdlijnen in een groep tekstmodi weergegeven.

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   De belangrijkste lijnen in een tekstwijze groeperen zijn gelijkaardig aan de lijnen die worden vereist om tekst-wijze meningen te bouwen.

   <!--
   <note type="tip">  
   <p>The key lines in a text mode grouping are similar to the lines required to build text-mode views.</p>
   </note>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th><strong>Voorbeeldregel</strong> </th> 
      <th><strong>Beschrijving</strong> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td><strong>groep.&lt;number&gt;.</strong> </td> 
      <td> <p>Elke coderegel wordt voorafgegaan door deze tekst. De coderegels die naar hetzelfde veld verwijzen dat in de groep is geselecteerd, worden als volgt genummerd met hetzelfde nummer:</p> 
       <ul> 
        <li>De eerste groepering van het rapport heeft een groepsaantal van 0. Alle regels die verwijzen naar de eerste groep beginnen met <code>group.0</code>.</li> 
        <li>De tweede groep van het rapport heeft een groepnummer van 1. Alle regels die verwijzen naar de tweede groep beginnen met <em><code>group.1</code></em>.</li> 
        <li>De derde groep van het rapport heeft een groepnummer van 2. Alle regels die verwijzen naar de derde groep beginnen met <em><code>group.2</code></em>.</li> 
        <li>Alleen in de tekstmodus kunt u een groepnummer van 3 toevoegen voor een vierde groep. Alle regels die verwijzen naar de vierde groep beginnen met <em><code>group.3</code></em>.</li> 
       </ul> <p>Opmerking: 4 groepen worden niet ondersteund in de builder. Ze worden alleen ondersteund bij gebruik van de tekstmodus. Workfront biedt geen ondersteuning voor meer dan vier niveaus van groepen.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>taxiveld</strong>=</p> </td> 
      <td> <p>Dit is de naam van het object of van het veld zoals deze wordt weergegeven in de database. Voor meer informatie over hoe objecten en velden in de database worden weergegeven, raadpleegt u <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>De volgende scenario's bestaan:</p> 
       <ol> 
        <li value="1"> <p> Als de naam van het veld dat u weergeeft een woordgroep is in plaats van een enkel zelfstandig naamwoord, moet u de syntaxis van het hoofdlettergebruik gebruiken voor het <code>valuefield</code>. Voor de geplande begindatum van een taak is de code bijvoorbeeld:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Als u een aangepast veld wilt weergeven, <code>valuefield</code> waarde is de daadwerkelijke naam van het gebied, zoals u het in de interface ziet. Voor een aangepast veld met de naam "Meer informatie" is de code bijvoorbeeld:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Als u door voorwerpen wilt groeperen die met andere voorwerpen verwant zijn gebruikend <code>valuefield</code> coderegel de objectnamen en -kenmerken worden gescheiden door dubbele punten.</p> <p>Een groepering op naam Portfolio voor een takenlijst heeft bijvoorbeeld de volgende waarde voor de regel valueField:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>Dit wijst erop dat van het voorwerp van het rapport (taak), u tot het volgende verwante voorwerp (project) kunt toegang hebben; vanaf dat punt hebt u toegang tot het volgende gerelateerde object van het project (portfolio); dan de naam van het portfolio (naam).</p> </li> 
       </ol> <p>Zie de sectie voor informatie over hoe objecten met elkaar verbinden <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependentie en hiërarchie van objecten</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Objecten in Adobe Workfront begrijpen</a>.</p> <p>Opmerking: Als u een veld kiest in de tekstmodus dat niet geldig is in de standaardinterface en u overschakelt naar de standaardinterface, wordt de groepering verwijderd.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>Deze lijn vertegenwoordigt het formaat dat wordt gebruikt om te tonen <code>valuefield</code>. De <code>valueformat</code> Hiermee geeft u aan of een object of veld wordt weergegeven als tekst, getal, percentage of datum.</p> <p>We raden u aan <code>HTML</code> voor uw <code>valueformat</code>, vooral bij gebruik <code>valueexpression</code>, zodat uw gegevens zo accuraat mogelijk worden weergegeven.</p> <p>Voor informatie over extra waarden voor deze lijn raadpleegt u <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Voorwaardelijke opmaak gebruiken in tekstmodus</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valueexpression=</strong> </p> </td> 
      <td> <p>U kunt deze regel toevoegen ter vervanging <code>valuefield</code>, als u de lijst wilt groeperen met een berekening tussen verschillende velden.</p> <p>U moet de <code>valuefield</code> van de objecten tussen accolades telkens wanneer u deze gebruikt in een <code>valueexpression</code>.</p> <p>De volgende scenario's bestaan:</p> 
       <ol> 
        <li value="1"> <p>Als u de naam van een groep in hoofdletters wilt weergeven, gebruikt u:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>De <code>valuefield</code> van het object wordt gespeld zoals het wordt weergegeven in de API Explorer.</p> </li> 
        <li value="2">Als u meerdere items wilt toevoegen <code>valuefields</code> door ze in een <code>valueexpression </code>regel, moet u ze met een punt scheiden.<p>Als u bijvoorbeeld de naam van het portfolio in hoofdletters wilt weergeven in een takenlijst, gebruikt u de volgende code in het dialoogvenster <code>valueexpression</code> regel:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>Als u een aangepast veld wilt gebruiken in een <code>valueexpression</code> regel die u voor de naam van het veld moet opgeven <code>DE:</code> om aan te geven dat het een aangepast veld is. De naam van het veld wordt gespeld zoals deze wordt weergegeven in de interface.</p><p>Belangrijk: <span>Wanneer u een aangepast veld gebruikt dat is geplaatst in een aangepaste formuliersectie waarvoor bepaalde gebruikers beperkte machtigingen hebben, wordt de berekening van de waarde <code>valueexpression </code>is leeg wanneer deze gebruikers deze berekening in een rapport bekijken. Voor informatie over het aanpassen van machtigingen voor aangepaste formuliersecties raadpleegt u</span> <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Een aangepast formulier maken of bewerken</a></span>.</p><p>Als u bijvoorbeeld een aangepast veld hebt met de naam "Naam ontwikkelaar" en u dit veld door dit veld wilt groeperen en in hoofdletters wilt weergeven, kunt u het volgende gebruiken <code>valueexpression</code> dit aan te geven:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>Wanneer u naar een aangepast Typeahead-tekstveld verwijst, gebruikt u de volgende expressie om naar de naam van het object te verwijzen dat is geselecteerd in een veld met de naam "Naam ontwikkelaar":</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>Deze regel definieert het groeperingslabel. In dit geval wordt de verkorte waarde op basis van de sleutel gebruikt.</p> <p>Als u de naam van de groep wilt wijzigen, kunt u deze waarde als volgt wijzigen:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> kunt u elke gewenste tekst voor de naam van de groep invoeren, terwijl <code>namekey</code> moet u een sleutel invoeren die wordt gebruikt om de naam van een groep te vertalen.</p> <p>Als u de naam van de groep wilt wijzigen, kunt u ook de opdracht <code>displayname </code>regel, als er geen regel is.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>U kunt de volgende regel toevoegen om de naam van een kolom te wijzigen, waardoor de <code>namekey/name</code> waarde:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>We raden u aan alle regels die <code>name </code>wanneer u de naam van een groep wijzigt.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Voeg een van de volgende coderegels toe aan een willekeurige groep om aan te geven of de resultaten in de groep moeten worden weergegeven in een uitgevouwen of samengevouwen lijst. Standaard worden groepen weergegeven als uitgevouwen:


   ```
   group.0.iscollapsed=true
   ```

   als u wilt dat de groep wordt weergegeven met de resultaten samengevouwen

   ```
   group.0.iscollapsed=false
   ```

   als u wilt dat de groep wordt weergegeven met de resultaten uitgevouwen

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   * Wanneer u groepen handmatig aanpast wanneer u een lijst weergeeft, onthoudt Workfront uw handmatige voorkeur totdat u zich afmeldt. Wanneer u zich weer aanmeldt, wordt de lijst weergegeven volgens deze instelling.
   * De resultaten van een groepering tonen altijd uitgevouwen na de toegang tot hen van een grafiekelement.


1. Klikken **Gereed** als u de wijzigingen wilt opslaan en de groepering of het rapport wilt blijven bewerken.
1. Klikken **Groepering opslaan** in een lijst of **Opslaan + Sluiten** om uw rapport op te slaan.
