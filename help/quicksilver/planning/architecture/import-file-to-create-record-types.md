---
title: Recordtypen maken door informatie uit een CSV- of Excel-bestand te importeren
description: Recordtypen zijn de objecttypen voor Adobe Workfront Planning. In de Planning van Workfront, kunt u de types van douaneverslag tot stand brengen die de het werkpunten nodig in de levenscyclus van uw organisatie door informatie van een CSV of dossier van Excel te invoeren illustreren.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2afd6d57-d658-4065-86f5-2324d3818d1f
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# Recordtypen maken door gegevens uit een CSV- of Excel-bestand te importeren

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

Recordtypen zijn de objecttypen voor Adobe Workfront Planning. In de Planning van Workfront, kunt u de types van douaneverslag tot stand brengen die de het werkpunten nodig in de levenscyclus van uw organisatie door informatie van een CSV of dossier van Excel te invoeren illustreren.

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Producten</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-abonnement*</p></td> 
   <td> 
<p>Een van de volgende Workfront-plannen:</p> 
<ul><li>Selecteren</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-planningspakket*</p></td> 
   <td> 
<p>Alle </p> 
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningsplan is opgenomen. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-platform</p></td> 
   <td> 
<p>Het geval van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden genegeerd om tot de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td><p> Standaard</p>
   <p>Workfront Planning is niet beschikbaar voor oudere Workfront-licenties</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Rechten beheren in een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr>

</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Overwegingen bij het importeren van recordtypen met een Excel- of CSV-bestand

* Elk blad van het Excel-bestand wordt een recordtype. De naam van het blad wordt de naam van het recordtype.
* Als er slechts één blad is, of als u een Csv- dossier invoert, wordt de naam van het dossier de naam van het verslagtype.
* De kolomkoppen in elk blad worden de velden die zijn gekoppeld aan elk recordtype.
* Velden zijn uniek voor hun respectievelijke recordtypen.
* Elke rij in elk blad wordt een unieke record die is gekoppeld aan het respectievelijke recordtype.
* Elk blad van het Excel-bestand mag het volgende niet overschrijden:
   * 25.000 rijen
   * 500 kolommen
* Het bestand mag niet groter zijn dan 5 MB.
* Lege bladen worden niet ondersteund.
* Velden van de volgende typen worden niet ondersteund en kunnen niet worden toegewezen aan velden op het importblad:

   * Verbind gebieden met Workfront en AEM Assets objecten types.
   * Velden opzoeken van verbonden planningsrecords of Workfront- en AEM Assets-objecten
   * Formuliervelden
   * Gemaakt op
   * Laatst gewijzigd op
   * <span class="preview"> Goedgekeurde datum, die door </span> wordt goedgekeurd
   * Mensen

Recordtypen importeren met een Excel- of CSV-bestand:

{{step1-to-planning}}

1. Klik op de werkruimte waar u recordtypen wilt maken.

   of

   Vouw in een werkruimte de pijl omlaag naar rechts uit, zoek naar een werkruimte en selecteer deze wanneer de werkruimte in de lijst wordt weergegeven.
1. Klik **toevoegen verslagtype**.
1. Klik **uploaden van dossier**.
1. Sleep en laat vallen een Excel of Csv- dossier eerder op uw computer, of klik **Uitgezocht een Csv of dossier van Excel** om voor te doorbladeren, dan het te selecteren.
1. Klik **Voorproef en geef uit**.

   De **Voorproef en geeft** vakvertoningen uit met de volgende informatie:

   * De namen van de bladen of van de toekomstige recordtypen worden weergegeven in het linkerdeelvenster. Workfront Planning selecteert standaard een pictogram en een kleur voor elk nieuw recordtype.
   * Het eerste blad of recordtype wordt geselecteerd en de namen van de bijbehorende velden worden als kolomkoppen weergegeven. Het type van elk gebied wordt geselecteerd door gebrek.
   * Elke rij vertegenwoordigt een nieuwe record. Alleen de eerste 10 records worden weergegeven in het vak Voorbeeld en bewerken.

   ![ Voorproef en geef doos uit ](assets/preview-and-edit-box.png)

1. (Optioneel) Klik op de naam van elk blad in het linkerdeelvenster om de informatie in het blad te bekijken.

   >[!NOTE]
   >
   >Lege bladen worden niet ondersteund en worden grijs weergegeven.

1. (Optioneel) Schakel de bladen uit die u niet vanuit het linkerdeelvenster wilt importeren.

   ![ Uitgezochte bladen om drop-down met unselected in te voeren ](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Bladen die u hebt uitgeschakeld, worden weergegeven met een grijze achtergrond.

1. (Optioneel) Klik op de pijl die omlaag wijst rechts van een kolomkop om een van de volgende handelingen uit te voeren, op het **Veld** -tabblad:

   ![ lusje van het Gebied op de de invoerdoos van het verslagtype ](assets/field-tab-on-record-type-import-mapping-box.png)

   * De naam van een veld wijzigen
   * Verander het **type van Gebied**
   * Werk het gebied **Beschrijving** bij

1. (Facultatief) klik het **lusje van de Verbinding** om de informatie in de kolom aan een verbonden gebied van andere verslagtypes in kaart te brengen.

   ![ het lusje van de Verbinding op de doos van de de invoerafbeelding van het verslagtype ](assets/connection-tab-on-record-type-import-mapping-box.png)

   >[!TIP]
   >
   >U kunt slechts aan gebieden van de Planning van Workfront verbonden verslagen in kaart brengen. U kunt niet toewijzen aan velden via Workfront- of AEM Assets-verbindingen. Voor meer informatie, zie de sectie [ Overwegingen over het invoeren van verslagtypes gebruikend een Excel of Csv- dossier ](#considerations-about-importing-record-types-using-an-excel-or-csv-file) in dit artikel.

1. (Voorwaardelijk) na het bijwerken van informatie over het gebied, klik **sparen**.

1. Klik **Invoer** wanneer u bereid bent om uw dossier in te voeren.

   De volgende informatie wordt geïmporteerd in Workfront Planning:

   * Nieuwe recordtypen
   * Nieuwe velden die zijn gekoppeld aan elk recordtype
   * Nieuwe records gekoppeld aan elk recordtype

   U kunt velden en records op de recordtypepagina&#39;s gaan beheren.

   Iedereen met toegang tot de Planning van Workfront en de werkruimte kan nu de ingevoerde verslagtypes en hun informatie bekijken en uitgeven.
