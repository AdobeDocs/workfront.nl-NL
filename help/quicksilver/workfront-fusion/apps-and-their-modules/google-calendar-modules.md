---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: connector
navigation-topic: apps-and-their-modules
title: Google-kalendermodules
description: In een [!DNL Adobe Workfront Fusion] scenario's, kunt u werkschema's automatiseren die Google Kalender gebruiken, evenals het verbinden met veelvoudige derdetoepassingen en de diensten.
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '3287'
ht-degree: 0%

---

# [!DNL Google Calendar] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!UICONTROL Google Calendar]en deze verbinding maken met meerdere toepassingen en services van derden.

Als u instructies bij het creëren van een scenario nodig hebt, zie [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Voor informatie over modules, zie [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] of hoger</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereisten: Als u de [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Oudere productvereisten: Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Te gebruiken [!DNL Google Calendar] modules, moet u een [!DNL Google] account.

## [!DNL Google Calendar] modules en hun velden

Wanneer u [!DNL Google Calendar] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Google Calendar] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Gebeurtenissen](#events)
* [Kalenders](#calendars)
* [Toegangscontrolevoorschriften](#access-control-rules)
* [Iteratoren (afgekeurd)](#iterators-deprecated)
* [Overige](#other)

### Gebeurtenissen

* [[!UICONTROL Watch events]](#watch-events)
* [[!UICONTROL Search events]](#search-events)
* [[!UICONTROL Get an event]](#get-an-event)
* [[!UICONTROL Create an event]](#create-an-event)
* [[!UICONTROL Update an event]](#update-an-event)
* [[!UICONTROL Delete an event]](#delete-an-event)


#### [!UICONTROL Watch events]

Deze triggermodule voert een scenario uit wanneer een nieuwe gebeurtenis wordt toegevoegd, bijgewerkt, verwijderd, gestart of beëindigd in de kalender die u opgeeft. De module retourneert alle standaardvelden die zijn gekoppeld aan de record of records, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar] </td> 
   <td> <p>Selecteer de kalender waarmee de module moet werken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch Events]</td> 
   <td> <p>Kies of u gebeurtenissen wilt bekijken op Aanmaakdatum, Bijgewerkte datum, Begindatum of Einddatum.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show deleted events]</td> 
   <td> <p>Schakel deze optie in om gebeurtenissen op te nemen die zijn verwijderd.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query] </td> 
   <td> <p>Voer de tekst in waarnaar u wilt zoeken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p> Het maximum aantal gebeurtenissen instellen dat [!DNL Workfront Fusion] werkt met tijdens één cyclus (het aantal herhalingen per scenario looppas). Als de waarde te hoog is ingesteld, kan de verbinding aan de kant van de opgegeven service van derden (timeout) worden onderbroken. [!DNL Workfront Fusion] heeft daar geen invloed op. Wij adviseren dat u een lagere waarde plaatst en of een hogere waarde voor het maximumaantal cycli bepaalt of het scenario vaker in werking stelt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search events]

Deze actiemodule zoekt naar een gebeurtenis in de geselecteerde kalender.

U geeft de kalender en de parameters van de zoekopdracht op.

De module retourneert de id van de gebeurtenis en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan Workfront Fusion, zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe Workfront Fusion - Basisinstructies</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Selecteer de kalender die u wilt doorzoeken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Start date]</td> 
   <td> <p> Voer de datum in waarop de gebeurtenis begint of wijs de datum toe. Deze module wint ook gebeurtenissen terug die vóór deze datum beginnen, die nog op de ingegaan begindatum voorkomen. </p> <p>Voor een lijst met ondersteunde datum- en tijdnotaties raadpleegt u <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Afgedwongen typegebruik in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL End date]</td> 
   <td> <p> Voer de datum in of wijs de datum toe waarop de gebeurtenis eindigt. </p> <p> Voor een lijst met ondersteunde datum- en tijdnotaties raadpleegt u <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Afgedwongen typegebruik in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Single events]</td> 
   <td> <p> Schakel deze optie in om terugkerende gebeurtenissen als één instantie te behandelen. Als u bijvoorbeeld een wekelijkse vergadering hebt en deze optie is ingeschakeld, retourneert de module de vergadering van elke week als een aparte gebeurtenis.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query]</td> 
   <td> <p>Voer de zoekterm in of wijs deze toe waarop u wilt zoeken. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Order by]</td> 
   <td> <p>Selecteer de volgorde van de gebeurtenissen die in het resultaat worden geretourneerd.</p> 
    <ul> 
     <li><strong>[!UICONTROL Start Time]</strong>: Volgorde op de begindatum en -tijd (oplopend). Dit is alleen beschikbaar bij het opvragen van afzonderlijke gebeurtenissen.</li> 
     <li><strong>[!UICONTROL Updated Time]</strong>: Volgorde bij laatste wijzigingstijd (oplopend).</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Het maximum aantal gebeurtenissen instellen [!DNL Workfront Fusion] retourneert tijdens één uitvoeringscyclus.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get an event]

Deze actiemodule retourneert de metagegevens voor één gebeurtenis in de opgegeven kalender.

U geeft de kalender en de gebeurtenis op.

De module retourneert de id van de gebeurtenis en alle bijbehorende velden, samen met eventuele aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Voer de id in of wijs deze toe aan de kalender met de gebeurtenis die u wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID] </td> 
   <td> <p>Voer de gebeurtenis-id van het bestaande [!DNL Google Calendar] -gebeurtenis die u wilt ophalen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create an event]

Deze actiemodule maakt een gebeurtenis.

U geeft de kalender en de parameters voor de gebeurtenis op.

De module retourneert de id van de gebeurtenis en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan Workfront Fusion, zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe Workfront Fusion - Basisinstructies</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Create an Event]</td> 
   <td> <p>Selecteer hoe u de gebeurtenis wilt maken.</p> 
    <ul> 
     <li><b>[!UICONTROL In Detail]</b><p>Met deze optie kunt u meer details over de gebeurtenis geven.<br></p></li> 
     <li><b>[!UICONTROL Quickly]</b><p>U hoeft alleen de kalender te selecteren en een naam voor de gebeurtenis in te voeren. U kunt tijd opnemen en details in de naam plaatsen, en [!DNL Google Calendar] de gebeurtenis voor die plaats en tijd plannen.</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Selecteer de kalender waarin u de gebeurtenis wilt weergeven.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Color]</td> 
   <td>Selecteer de kleur die de gebeurtenis in de kalender weergeeft.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event name]</td> 
   <td> <p> Voer een naam voor de gebeurtenis in of wijs een naam toe. </p> <p>Opmerking: Als u [!UICONTROL Quick add] in de [!UICONTROL Create an event] in het veld kunt u de datum en tijd van de gebeurtenis opnemen, en [!DNL Workfront Fusion] maakt de gebeurtenis voor die datum en tijd. Voorbeeld: <code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>. Als u [!UICONTROL Quick add] maar zonder datum en tijd in de naam van de gebeurtenis, wordt de gebeurtenis gemaakt op basis van de huidige tijd en duurt deze een uur.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL All day event]</td> 
   <td>Schakel deze optie in als de gebeurtenis een alledaagse gebeurtenis is (geen begin- en eindtijd nodig).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Start date]</td> 
   <td> <p>Als dit een alledaagse gebeurtenis is, voert u de begindatum van de gebeurtenis in. </p> <p>Voor een lijst met ondersteunde datumnotaties raadpleegt u <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Afgedwongen typegebruik in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL End date]</td> 
   <td> <p> Als dit een alledaagse gebeurtenis is, voert u de einddatum van de gebeurtenis in. </p> <p>Voor een lijst met ondersteunde datumnotaties raadpleegt u <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Afgedwongen typegebruik in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Description]</td> 
   <td>Voer een beschrijving van de gebeurtenis in of wijs deze toe. Dit veld ondersteunt HTML.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Location]</td> 
   <td>Voer een locatie voor de gebeurtenis in het tekstformulier in.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Use the default reminder settings for this event]</td> 
   <td>Schakel deze optie in als u de standaardinstellingen voor herinneringen wilt gebruiken. Als u een aangepaste herinnering instelt in het dialoogvenster [!UICONTROL Reminder] wordt deze waarde ingesteld op Nee.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reminder] </td> 
   <td> <p>Herinnering toevoegen voor de gebeurtenis. Voor elke herinnering, selecteer de methode u met moet worden herinnerd en bepaalt hoe lang (in notulen) vóór de gebeurtenis u wilt worden herinnerd.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attendees]</td> 
   <td>Voeg de deelnemers aan de gebeurtenis toe. Voer voor elke deelnemer de naam en het e-mailadres van de deelnemer in of wijs deze toe.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show me as]</td> 
   <td>Selecteer of u wilt dat mensen die uw kalender bekijken u als Bezig of Beschikbaar tijdens deze gebeurtenis zien.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Visibility] </td> 
   <td> <p>Selecteer de zichtbaarheid van deze gebeurtenis. </p> 
    <ul> 
     <li> <p><b>[!UICONTROL Default]</b></p> <p>De gebeurtenis heeft de zichtbaarheid die u hebt ingesteld in uw kalenderinstellingen.</p> </li> 
     <li> <p><b>[!UICONTROL Public]</b></p> <p>Iedereen met wie de kalender wordt gedeeld kan deze gebeurtenis zien.</p> </li> 
     <li> <p><b>[!UICONTROL Private]</b></p> <p>Alleen deelnemers kunnen deze gebeurtenis zien.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Send notification about the event creation]</td> 
   <td> <p>Geef op of u meldingen over het maken van een nieuwe gebeurtenis wilt verzenden naar alle gasten en naar niet-[!DNL Google Calendar] gasten, of niemand.</p> <p>Tip: We raden u aan de [!UICONTROL None] alleen voor migratiegebruik.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Guests can modify the event]</td> 
   <td> <p>Schakel deze optie in als u gasten in staat wilt stellen deze gebeurtenis te wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recurrence]</td> 
   <td>Voeg terugkerende regels toe die u op deze gebeurtenis wilt toepassen. Elke regel vereist een lijst van [!UICONTROL RRULE], [!UICONTROL EXRULE], [!UICONTROL RDATE], en [!UICONTROL EXDATE] regels voor een terugkerende gebeurtenis. Let op: [!UICONTROL DTSTART] en [!UICONTROL DTEND] lijnen zijn niet toegestaan in dit veld; De begin- en eindtijd van de gebeurtenis worden opgegeven in de begin- en eindvelden. Dit veld wordt weggelaten voor enkele gebeurtenissen of voor terugkerende gebeurtenissen. Zie voor meer informatie <a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a>.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update an event]

Deze actiemodule wijzigt een bestaande gebeurtenis.

U geeft de kalender en gebeurtenis-id op.

De module retourneert de id van de gebeurtenis en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar] </td> 
   <td> <p>Selecteer de kalender waarmee u wilt werken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID] </td> 
   <td> <p>Voer de gebeurtenis-id in van de eerder gemaakte [!DNL Google Calendar] -gebeurtenis die u wilt bijwerken.</p> </td> 
  </tr> 
 </tbody> 
</table>

U kunt de gebeurtenisinformatie bijwerken door nieuwe waarden in te voeren in het gewenste veld. Zie voor meer informatie over de afzonderlijke velden [[!UICONTROL Create an event]](#create-an-event).

#### [!UICONTROL Delete an event]

Deze actiemodule verwijdert een gebeurtenis.

U geeft de kalender en gebeurtenis-id op.

De module retourneert de id van de gebeurtenis en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Selecteer de kalender die de gebeurtenis bevat die u wilt verwijderen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event ID]</td> 
   <td> <p> Voer de gebeurtenis-id in vanuit een eerder gemaakt [!DNL Google Calendar] -gebeurtenis die u wilt verwijderen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Send notification about the event deletion]</td> 
   <td>Geef op of u meldingen over het verwijderen van gebeurtenissen wilt verzenden naar alle gasten en gasten die deze functie niet gebruiken [!DNL Google Calendar], of niemand.</td> 
  </tr> 
 </tbody> 
</table>

### Kalenders

* [[!UICONTROL List calendars]](#list-calendars)
* [[!UICONTROL Get a calendar]](#get-a-calendar)
* [[!UICONTROL Create a calendar]](#create-a-calendar)
* [[!UICONTROL Update a calendar]](#update-a-calendar)
* [[!UICONTROL Delete a calendar]](#delete-a-calendar)
* [[!UICONTROL Clear a calendar]](#clear-a-calendar)

#### [!UICONTROL List calendars]

Deze actiemodule keert de kalenders op de kalenderlijst van een gebruiker terug.

De module retourneert de id van de kalender en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Minimum access role]</td> 
   <td> <p>Selecteer de minimale toegangsrol voor de gebruiker. De module keert kalenders terug die op deze minimumtoegangsrol worden gebaseerd.</p> 
    <ul> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>: De gebruiker kan vrije/bezige informatie lezen. </li> 
     <li><strong>[!UICONTROL Owner]</strong>: De gebruiker kan gebeurtenissen lezen en wijzigen en heeft toegang tot besturingslijsten. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: De gebruiker kan gebeurtenissen lezen die niet privé zijn. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: De gebruiker kan gebeurtenissen lezen en wijzigen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show hidden calendars]</td> 
   <td>Schakel deze optie in om verborgen kalenders op te nemen in de lijst die de module retourneert.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Het maximumaantal kalenders instellen [!DNL Workfront Fusion] retourneert tijdens één uitvoeringscyclus.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a calendar]

Deze actiemodule haalt een kalender op.

U geeft de id op van de kalender die u wilt ophalen.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>Selecteer de kalender die u wilt ophalen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a calendar]

Deze actiemodule maakt een nieuwe kalender.

U geeft een naam op voor de kalender.

De module retourneert de id van de kalender en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar name]</td> 
   <td> <p> Voer een naam in voor de nieuwe kalender.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a calendar]

Deze actiemodule werkt een kalender bij.

U geeft de id op van de kalender die u wilt bijwerken.

De module retourneert de id van de kalender en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Selecteer de kalender die u wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar name]</td> 
   <td> <p> Voer een nieuwe naam in voor de kalender.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a calendar]

Met deze actiemodule verwijdert u een kalender.

U geeft de id op van de kalender die u wilt verwijderen.

De module retourneert de id van de kalender en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>Voer de id in van de kalender die u wilt verwijderen of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Clear a calendar]

Deze actiemodule verwijdert alle gebeurtenissen uit de primaire kalender van een account.

U geeft de verbinding op die verbinding maakt met de account die de kalender bevat die u wilt wissen.

De module retourneert de id van de kalender en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
 </tbody> 
</table>

### Toegangscontrolevoorschriften

* [[!UICONTROL List access control rules]](#list-access-control-rules)
* [[!UICONTROL Get an access control rule]](#get-an-access-control-rule)
* [[!UICONTROL Create an access control rule]](#create-an-access-control-rule)
* [[!UICONTROL Update an access control rule]](#update-an-access-control-rule)
* [[!UICONTROL Delete an access control rule]](#delete-an-access-control-rule)

#### [!UICONTROL List access control rules]

Deze actiemodule keert de regels in de toegangsbeheerlijst op een kalender terug.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>Selecteer de kalender die de toegangsbeheerregels bevat die u wilt terugwinnen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Het maximale aantal resultaten instellen [!DNL Workfront Fusion] retourneert tijdens één uitvoeringscyclus.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get an access control rule]

Deze actiemodule keert de meta-gegevens van een toegangsbeheerregel terug.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>Selecteer de kalender die de toegangsbeheerregel bevat die u wilt terugwinnen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Access control rule ID]</td> 
   <td>Selecteer de toegangsbeheerregel u wilt terugwinnen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create an access control rule]

Deze actiemodule leidt tot een nieuwe toegangsbeheerregel.

U geeft een naam op voor de kalender.

De module keert identiteitskaart van de toegangsbeheerregel en om het even welke bijbehorende gebieden, samen met om het even welke douanegebieden en waarden terug die de verbinding toegang heeft. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Selecteer de kalender waar u een toegangsbeheerregel wilt tot stand brengen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td> <p>Selecteer de rol om aan de toegangsregel toe te wijzen. </p> 
    <ul> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>: De gebruiker kan vrije/bezige informatie lezen. </li> 
     <li><strong>[!UICONTROL Owner]</strong>: De gebruiker kan gebeurtenissen lezen en wijzigen en heeft toegang tot besturingslijsten. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: De gebruiker kan gebeurtenissen lezen die niet privé zijn. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: De gebruiker kan gebeurtenissen lezen en wijzigen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type]</td> 
   <td> <p>Selecteer het type bereik. </p> 
    <ul> 
     <li><strong>[!UICONTROL Default]</strong>: De publieke reikwijdte. Dit is de standaardwaarde. </li> 
     <li><strong>[!UICONTROL User]</strong>: Beperkt het bereik tot één gebruiker. </li> 
     <li><strong>[!UICONTROL Group]</strong>: Beperkt het bereik tot een groep. </li> 
     <li><strong>[!UICONTROL Domain]</strong>: Beperkt het bereik tot een domein. </li> 
    </ul> <p>Opmerking: De aan de [!UICONTROL Default], of het publiek, is het bereik van toepassing op alle gebruikers, al dan niet geverifieerd.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value]</td> 
   <td>Voer het e-mailadres van een gebruiker of groep in of de naam van een domein, afhankelijk van het bereiktype.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Send notifications]</td> 
   <td> <p>Schakel deze optie in om meldingen over de toegangswijziging te verzenden. </p> <p>Opmerking: Er zijn geen meldingen over het verwijderen van toegang. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update an access control rule]

Deze actiemodule werkt een toegangsbeheerregel bij.

U geeft een naam op voor de kalender.

De module keert identiteitskaart van de toegangsbeheerregel en om het even welke bijbehorende gebieden, samen met om het even welke douanegebieden en waarden terug die de verbinding toegang heeft. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Selecteer de kalender die de toegangsbeheerregel bevat u wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Access control rule ID]</td> 
   <td>Selecteer de toegangsbeheerregel u wilt bijwerken.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td> <p>Selecteer de rol om aan de toegangsregel toe te wijzen. </p> 
    <ul> 
     <li><strong>[!UICONTROL None]</strong>: Deze rol biedt geen toegang.</li> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>: De gebruiker kan vrije/bezige informatie lezen. </li> 
     <li><strong>[!UICONTROL Owner]</strong>: De gebruiker kan gebeurtenissen lezen en wijzigen en heeft toegang tot besturingslijsten. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: De gebruiker kan gebeurtenissen lezen die niet privé zijn. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: De gebruiker kan gebeurtenissen lezen en wijzigen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Send notifications]</td> 
   <td> <p>Schakel deze optie in om meldingen over de toegangswijziging te verzenden. </p> <p>Opmerking: Er zijn geen meldingen over het verwijderen van toegang. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete an access control rule]

Deze actiemodule schrapt een toegangsbeheerregel.

U geeft een naam op voor de kalender.

De module keert identiteitskaart van de toegangsbeheerregel en om het even welke bijbehorende gebieden, samen met om het even welke douanegebieden en waarden terug die de verbinding toegang heeft. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar ID]</td> 
   <td> <p>Selecteer of wijs identiteitskaart van de kalender toe die de toegangsbeheerregel bevat u wilt schrappen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Access control rule ID]</td> 
   <td>Selecteer of wijs identiteitskaart van de toegangsbeheerregel toe u wilt schrappen.</td> 
  </tr> 
 </tbody> 
</table>

### Iteratoren (afgekeurd)

De [!UICONTROL iterate attachments] en [!UICONTROL iterate attendees] modules zijn afgekeurd. Als u bijlagen of deelnemers wilt doorlopen, gebruikt u de opdracht [!UICONTROL Flow Control] > [!UICONTROL Iterator] module. Zie voor meer informatie [Interventiemodule in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)

### Overige

* [[!UICONTROL Make an API Call]](#make-an-api-call)
* [[!UICONTROL Get Free/Busy Information]](#get-freebusy-information)

#### [!UICONTROL Make an API Call]

In deze module kunt u een aangepaste API-aanroep uitvoeren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe [!DNL Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Een pad invoeren ten opzichte van <code>https://www.googleapis.com/calendar</code>. Voorbeeld: <code>/v3/users/me/calendarList</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van de aanvraag toe in de vorm van een standaard JSON-object. Bijvoorbeeld: <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] Hiermee voegt u de machtigingsheaders voor u toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Voeg de query voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:   <p>Bij het gebruik van voorwaardelijke instructies zoals <code>if</code> in uw JSON, plaats de aanhalingstekens buiten de voorwaardelijke verklaring.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Free/Busy Information]

Deze actiemodule keert vrije en bezige informatie voor een reeks kalenders terug.

De module retourneert de id van de kalender en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Voor instructies over het aansluiten van uw [!DNL Google Calendar] account aan Workfront Fusion, zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met Adobe Workfront Fusion - Basisinstructies</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Minimum time]</td> 
   <td> <p> Ga het begin van het interval in dat u informatie voor wilt terugwinnen.</p> <p> Voor een lijst met ondersteunde datum- en tijdnotaties raadpleegt u <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Afgedwongen typegebruik in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum time]</td> 
   <td> <p> Ga het eind van het interval in dat u informatie voor wilt terugwinnen. </p> <p>Voor een lijst met ondersteunde datum- en tijdnotaties raadpleegt u <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Afgedwongen typegebruik in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendars]</td> 
   <td> <p>Voor elke kalender waarvan u de gegevens wilt ophalen, klikt u op <strong>Toevoegen</strong> en voer de kalender-id in of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Een scenario activeren vóór een gebeurtenis

U kunt een scenario een bepaalde tijd vóór een gebeurtenis met behulp van standaard activeren [!DNL Google Calendar] e-mailherinneringen en de [!UICONTROL Webhooks] >[!UICONTROL Custom mailhook] module.

1. Gebruik de [!UICONTROL Google Calendar] >[!UICONTROL Update an event] om een e-mailherinnering aan uw gebeurtenis toe te voegen:

   ![](assets/trigger-scen-before-event-350x209.png)

1. Maak een nieuw scenario dat begint met de [!UICONTROL Webhooks] >[!UICONTROL Custom mailhook] module.

   1. Kopieer het e-mailadres van de mailhaak.
   1. Sla het scenario op en voer het uit.

1. In [!DNL Gmail]de [!DNL Google Calendar] e-mailherinneringen aan het e-mailadres van de mailhaak:

   1. Open uw **[!UICONTROL [!DNL Gmail] settings]**.
   1. Open de **[!UICONTROL Forwarding and POP/IMAP]** tab.
   1. Klik op **[!UICONTROL Add a forwarding address].**
   1. Plak het e-mailadres van de gekopieerde e-mail, klik op &#x200B;**[!UICONTROL Next]**, bevestigen door te drukken **[!UICONTROL Proceed]** in het pop-upvenster klikt u op **[!UICONTROL OK]**.

   1. In [!DNL Workfront Fusion]Schakel over naar het nieuwe scenario dat de uitvoering moet voltooien door de bevestigingsmail te ontvangen.
   1. Klik de bel boven de module om de output van de module te inspecteren.
   1. Breid uit `Text` item en kopieer de bevestigingscode:

      ![](assets/confirmation-code-350x252.png)

   1. Plak in Gmail de bevestigingscode in het bewerkingsvak en klik op &#x200B;**[!UICONTROL Verify]**:

      ![](assets/paste-code-350x46.png)

   1. Open de **[!UICONTROL Filters and Blocked Addresses]** tab.
   1. Klik op **[!UICONTROL Create a new filter]**.
   1. Een filter instellen voor alle e-mails die afkomstig zijn van `     calendar-notification@google.com` en klik op &#x200B;**[!UICONTROL Create a filter]**:
   1. Selecteren **[!UICONTROL Forward it to]** en kiest u het e-mailadres van de mailhooks in de lijst.
   1. Klikken **[!UICONTROL Create filter]** om het filter te maken.

1. (Optioneel) In [!DNL Workfront Fusion], voegt u de [!UICONTROL Text parser] > [!UICONTROL Match pattern] module na de [!UICONTROL Webhooks] >[!UICONTROL Custom mailhook] om de HTML-code van de e-mail te parseren voor alle informatie die u nodig hebt.

   U kunt de module bijvoorbeeld als volgt configureren om de id van de gebeurtenis op te halen:

   *Patroon*: `<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *Tekst*: De `HTML content` uit het [!UICONTROL Webhooks] >[!UICONTROL Custom mailhook] module.
