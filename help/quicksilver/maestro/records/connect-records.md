---
title: Connect-records
description: Nadat u verbindingen tussen recordtypen hebt gemaakt, kunt u afzonderlijke records met elkaar verbinden.
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '1804'
ht-degree: 0%

---


<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# Connect-records

>[!IMPORTANT]
>
>Adobe Maestro maakt momenteel deel uit van een gesloten bètaprogramma dat voor een beperkt aantal klanten toegankelijk is.
>
>Neem contact op met uw accountvertegenwoordiger voor meer informatie over deelname aan het bètaprogramma voor Maestro.
>
>Zie voor meer informatie [Overzicht van Adobe Maestro](../maestro-overview.md).

U kunt Adobe Maestro-records met elkaar of met objecten van andere toepassingen verbinden.

U moet eerst twee recordtypen met elkaar verbinden of een recordtype verbinden met een objecttype vanuit een andere toepassing. Vervolgens kunt u de tabelweergave van het recordtype gebruiken om records met elkaar te verbinden of records met andere objecten te verbinden.

Voor informatie over het verbinden van verslagtypes met elkaar of aan objecten types van andere toepassingen, zie [Verbind recordtypen](../architecture-and-fields/connect-record-types.md).

Zie voor een voorbeeld van het verbinden van recordtypen [Voorbeeld van het verbinden van recordtypen en records](../architecture-and-fields/example-connect-record-types-and-records.md).

U kunt het volgende verbinden:

* Operationele Maestro-gegevens
* Operationele gegevens van Maestro naar taxonomische gegevens
* Operationele Maestro-records en objecten van andere toepassingen.

  De volgende toepassingen en objecttypen worden momenteel ondersteund:

   * Adobe Workfront

      * Projecten
      * Portfolio&#39;s
      * Programma&#39;s
      * Bedrijf
      * Groep

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

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
   <td><p>Willekeurig, om Maestro-records te maken</p> 
<p>Werk of hoger om projecten in Workfront weer te geven</p>
  <p>Zie voor meer informatie <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Overzicht van Adobe Workfront-licenties</a>.</p> 
  </td>
  </tr>
  <tr>
   <td role="rowheader">Toegangsniveau</td>
   <td> <p>Willekeurig, om Maestro-records te maken</p>
<p>De mening of hogere toegang tot Projecten, Portfolio's, Programma's</p> 
<p>Extra toegang tot Groepen en Bedrijven, wanneer het bekijken van groepen of bedrijven de gebruikers behoren niet tot</p>   
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objectmachtigingen</p></td>
   <td> <p>Machtigingen weergeven voor de objecten die u wilt koppelen aan Maestro-records  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw systeembeheerder moet het gebied Maestro in uw lay-outmalplaatje toevoegen. Zie voor meer informatie <a href="../access/grant-access.md">Toegang verlenen tot Adobe Maestro</a>. </p></td>
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

## Connect-records

### Overwegingen bij het verbinden van records

* Nadat de verbinding tussen recordtypen tot stand is gebracht, worden de verbonden recordtypen weergegeven als gekoppelde recordvelden in de tabel met de recordtypen waarvan ze gekoppeld zijn.
* U kunt records en objecten van de gekoppelde record- en objecttypen bladeren en deze toevoegen vanuit de gekoppelde recordvelden.
* U kunt velden van de gekoppelde recordtypen toevoegen aan de tabel van het recordtype waarvan u een koppeling maakt.
* U kunt de waarden van gekoppelde velden niet handmatig bijwerken in de records waarvan u een koppeling maakt.

  De waarden van de gekoppelde velden uit de gekoppelde records vullen de Maestro-record die u automatisch koppelt.

* Iedereen met toegang tot Maestro kan de verbindingen zien die u maakt tussen Maestro records of tussen Maestro records en Workfront objecten. U kunt ook de verbindingen van alle anderen weergeven en bewerken. <!--add that this is based on your permissions in both Maestro and Workfront (or, later, any other application)-->
* U kunt één Maestro-record verbinden met een of meerdere objecten vanuit een andere toepassing.
* U kunt taxonomieën niet verbinden met recordtypen of met objecten uit een andere toepassing. <!-- this is temporary; there will be certain objects (teams, etc) that will be linked to taxonomies, per Lilit-->
* U kunt Maestro-records momenteel alleen koppelen aan Workfront-objecten. Als u Maestro-records wilt koppelen aan Workfront-objecten, moet u over het volgende beschikken:

   * Workfront-objecten. U moet bijvoorbeeld eerst projecten, portfolio&#39;s, programma&#39;s, bedrijven of groepen maken in Workfront.
   * Maestro-werkruimten, recordtypen en records. Raadpleeg de volgende artikelen voor meer informatie:

      * [Werkruimten maken](../architecture-and-fields/create-workspaces.md)
      * [Recordtypen maken](../architecture-and-fields/create-record-types.md)
      * [Records maken](../records/create-records.md)

   * Verbindingen tussen recordtypen of tussen recordtypen en objecten uit andere toepassingen. Zie voor meer informatie [Verbind recordtypen](../architecture-and-fields/connect-record-types.md).

### Connect Maestro-records

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-workfront.png) in de rechterbovenhoek van Workfront <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> klik vervolgens op **Maestro** ![](assets/maestro-icon.png).

   De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Vouw de pijl omlaag naar rechts uit van de naam van een bestaande werkruimte en selecteer de werkruimte waaruit u records wilt verbinden.
1. Klik op de kaart van een recordtype om de pagina met recordtypen te openen.
1. Selecteer een tabelweergave in het menu **Weergave** in de rechterbovenhoek van de pagina met recordtypen.
1. Voeg een verbinding aan een ander verslag of objecten type van het geselecteerde verslagtype toe. Zie voor meer informatie [Verbind recordtypen](../architecture-and-fields/connect-record-types.md).

Er wordt een nieuwe kolom aan de tabel toegevoegd om het gekoppelde recordtype weer te geven.

1. Voeg records toe aan het recordtype dat u hebt geselecteerd door een nieuwe rij aan de tabel toe te voegen. Zie voor meer informatie [Records maken](../../maestro/records/create-records.md).
1. Ga in een record in de tabelweergave naar de gekoppelde recordkolom en houd de cursor boven de cel die overeenkomt met de record die u wilt koppelen aan andere Maestro-records, en klik vervolgens op de knop **+** pictogram.

   De **Objecten verbinden** wordt weergegeven.

   ![](assets/connected-objects-table-for-records.png)

1. Typ de naam van een record in het zoekvak en selecteer de naam wanneer de record in de lijst wordt weergegeven

   of

   Selecteer de naam van een of meerdere records in het vak en klik op **Objecten verbinden** in de rechterbovenhoek van het vak Connect-objecten.

   Het volgende wordt toegevoegd:

   * De gekoppelde records worden weergegeven in het gekoppelde recordveld van de record die u in stap 3 hebt geselecteerd. Wanneer u de gekoppelde records bijwerkt, worden de gekoppelde recordvelden automatisch bijgewerkt voor de records die u koppelt. <!--ensure the number of the step stays accurate-->
   * De gekoppelde velden die bij de gekoppelde records horen, worden automatisch gevuld met de gegevens van de oorspronkelijke gekoppelde records. U kunt gekoppelde velden niet handmatig bewerken.

     >[!TIP]
     >
     >* We gebruiken onderling gekoppelde velden en opzoekvelden.
     >
     >* Als u de instelling Meerdere records toestaan hebt ingeschakeld toen u de recordtypen aansloot, worden de waarden van velden voor de meerdere geselecteerde objecten weergegeven met komma&#39;s van elkaar gescheiden of samengevoegd op basis van de gekozen aggregator.

1. (Optioneel) Sluit de pagina Type Maestro-record en ga naar de geselecteerde werkruimte.
1. Klik op de kaart voor het recordtype waarmee u een koppeling hebt gemaakt.

   Als u bijvoorbeeld de campagnerecord hebt verbonden met de productrecord, klikt u op de knop **Product** kaart.

   Het recordtype moet worden geopend in de tabelweergave.

   Het veld Campagne gekoppeld record bevat de namen van de campagnes die u aan producten hebt gekoppeld op de pagina Type productrecord. Wanneer u de Campagnegegevens bijwerkt, wordt het aan Campagne gekoppelde recordveld voor het type productrecord automatisch bijgewerkt.

### Connect Maestro-records verbinden met Workfront-objecten

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

Nadat u een verbinding hebt gemaakt tussen een Maestro-recordtype en een Workfront-objecttype, kunt u afzonderlijke Maestro-records verbinden met objecten in Workfront. U kunt ook velden van het Workfront-object verbinden met het Maestro-recordtype.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-workfront.png) in de rechterbovenhoek van Workfront <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> klik vervolgens op **Maestro** ![](assets/maestro-icon.png).

   De laatst geopende werkruimte moet standaard worden geopend.

1. (Optioneel) Vouw de pijl omlaag naar rechts uit van de naam van een bestaande werkruimte en selecteer de werkruimte waaruit u records wilt verbinden.
1. Klik op de kaart van een recordtype om de pagina met recordtypen te openen.
1. Selecteer een tabelweergave in het menu **Weergave** in de rechterbovenhoek van de pagina met recordtypen.
1. Voeg een nieuwe verbinding aan een objecten type van Workfront het geselecteerde verslagtype toe. Selecteer een van de volgende objecten onder de sectie Workfront:

   * Project
   * Portfolio
   * Programma
   * Bedrijf
   * Groep

   Zie voor meer informatie [Verbind recordtypen](../architecture-and-fields/connect-record-types.md).

   Er wordt een nieuwe kolom toegevoegd aan de tabel om het gekoppelde objecttype weer te geven.

1. Voeg afzonderlijke records toe aan het recordtype dat u hebt geselecteerd door een nieuwe rij aan de tabel toe te voegen. Zie voor meer informatie [Records maken](../../maestro/records/create-records.md).
1. Ga in een record in de tabelweergave naar de kolom met het gekoppelde object en houd de cursor boven de cel die overeenkomt met de record die u wilt koppelen aan andere objecten uit Workfront. Klik vervolgens op de knop **+** pictogram. <!--change Workfront to other applications, when this will be possible-->

   De **Objecten verbinden** wordt weergegeven.

   ![](assets/connect-objects-box-to-select-projects.png)

1. Typ de naam van een Workfront-object in het zoekvak en selecteer het vervolgens wanneer het in de lijst wordt weergegeven

   of

   Selecteer de naam van een of meerdere objecten in het vak en klik op **Objecten verbinden** in de rechterbovenhoek van het vak Connect-objecten.

   Aan Maestro wordt het volgende toegevoegd:

   * De geselecteerde Workfront-objecten worden toegevoegd aan het gekoppelde recordveld.
   * Er wordt een nieuw gekoppeld veld (of een opzoekveld) gemaakt voor elk gekoppeld veld dat u hebt geselecteerd bij het toevoegen van de velden aan de gekoppelde record.
   * Een nieuw recordtype met de naam &quot;Workfront-object&quot; wordt gemaakt in dezelfde werkruimte als de Maestro-record waaruit u een koppeling maakt. De naam van het object maakt deel uit van de naam van dit recordtype. Als u bijvoorbeeld een koppeling naar Workfront-projecten maakt, maakt u het Workfront-projectrecordtype in Maestro.

     Dit is een alleen-lezen recordtype en er worden Workfront-objecten weergegeven die zijn geselecteerd in het nieuwe gekoppelde objectveld dat u hebt gemaakt van de Maestro-record. De gekoppelde velden van het gekoppelde object worden ook weergegeven op de alleen-lezen gekoppelde Workfront-records.

     >[!IMPORTANT]
     >
     > Het alleen-lezen Workfront-objectrecordtype wordt alleen gemaakt wanneer afzonderlijke projecten aan Maestro-records worden toegevoegd. Het maken van een verbinding tussen een Maestro-recordtype en een Workfront-objecttype leidt niet tot het Workfront-recordtype.

     Eventuele bestaande informatie uit de velden van de Workfront-objecten wordt weergegeven in de gekoppelde of opzoekvelden.

     >[!TIP]
     >
     >
     >* Als u de instelling Meerdere records toestaan hebt ingeschakeld, worden de waarden van de meerdere objecten gescheiden door komma&#39;s weergegeven of worden ze samengevoegd volgens de gekozen aggregator.
     >
     >* Er wordt geen gekoppeld recordveld naar de gekoppelde Maestro-records gemaakt voor de gekoppelde Workfront-objecten.


1. (Optioneel) Sluit de pagina Type Maestro-record en ga naar de geselecteerde werkruimte.
1. Klik op de kaart voor het recordtype van het Workfront-object. Klik bijvoorbeeld op de knop **Workfront-project** als u een koppeling hebt gemaakt naar Workfront-projecten. Het Workfront-recordtype alleen-lezen moet worden geopend in de tabelweergave.

   >[!NOTE]
   >
   >    * De records in de Workfront-recordtypepagina zijn alleen-lezen Workfront-objecten. De velden die zijn gekoppeld via het Workfront-recordtype, worden ook weergegeven als alleen-lezen kolommen en worden automatisch ingevuld wanneer ze in Workfront worden ingevuld.
   >    * U kunt Workfront-velden niet handmatig bijwerken in Maestro. Workfront-objectvelden moeten in Workfront worden ingevuld en de veldwaarden worden automatisch weergegeven in de Workfront-record in Maestro.
   >
   >    * Als u het type Workfront-objectrecord wilt weergeven in de tijdlijnweergave, moet u ten minste twee datumvelden weergeven in de tabelweergave van de alleen-lezen Workfront-recordtype.

1. (Optioneel) Klik op de knop **Meer** menu ![](assets/more-menu.png) naast de naam van het Workfront-objectrecordtype in de koptekst van de pagina klikt u op **Naam wijzigen** om de naam van de record te bewerken.

   >[!NOTE]
   >
   >    U kunt een gekoppeld Workfront-recordtype of objecten niet verwijderen van de Workfront-recordtype pagina.

1. (Optioneel) Klik op de knop **Velden toevoegen** pictogram ![](assets/add-fields-icon.png) in de rechterbovenhoek van de tabelweergave op de Workfront-pagina met recordtypen om Workfront-velden toe te voegen aan of te verwijderen uit het Workfront-recordtype.

   >[!NOTE]
   >
   >  De velden die u toevoegt of verwijdert op de pagina met Workfront-objectrecordtypen, worden niet toegevoegd aan of verwijderd uit het Maestro-recordtype dat is gekoppeld aan het Workfront-objecttype. De velden zijn alleen zichtbaar op de pagina met alleen-lezen Workfront-recordtypen, zodat u ze in Maestro kunt bekijken.

1. (Optioneel) Kies in het vervolgkeuzemenu Weergave op de pagina Type Workfront-objectrecord de tijdlijnweergave om de Workfront-gekoppelde objecten weer te geven in de tijdlijnweergave.












