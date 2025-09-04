---
title: Veldinstellingen bewerken
description: In de Planning van Adobe Workfront, kunt u de gebiedsmontages voor gebieden uitgeven die reeds worden gecreeerd. In dit artikel wordt beschreven hoe u de instellingen voor Workfront-planningsvelden kunt bewerken.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: a00776ecd9f8dc14b9dce14ce9463c2bb709a363
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---


# Veldinstellingen bewerken

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

U kunt de instellingen van bestaande velden bewerken in Adobe Workfront Planning.

Voor informatie over het creëren van de gebieden van de Planning van Adobe Workfront, zie [ gebieden ](/help/quicksilver/planning/fields/create-fields.md) creëren.

In dit artikel wordt beschreven hoe u de instellingen voor Workfront-planningsvelden kunt bewerken. Voor informatie over het uitgeven van gebiedswaarden voor verslagen, zie [ verslagen ](/help/quicksilver/planning/records/edit-records.md) uitgeven.

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
   <td><p> Standard </p>
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
   <td>   <p>Machtigingen beheren voor een werkruimte en recordtype </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p></td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


## Overwegingen bij het bewerken van veldinstellingen

U moet het volgende in overweging nemen voordat u wijzigingen aanbrengt in de configuratie van een veld:

* U kunt de veldinstellingen alleen bewerken vanuit de tabel met recordtypen.
* U kunt de instellingen van een veld niet bewerken op de recordpagina of in een andere weergave, buiten de tabelweergave.
* U kunt het veldtype niet bewerken nadat het veld is opgeslagen.
* U kunt de eerder geselecteerde instelling voor negatieve getallen toestaan niet uitschakelen voor een veld Getal, Percentage of Valuta als er al negatieve waarden zijn opgeslagen in de records waaraan deze is gekoppeld.
* U kunt de configuratie van de volgende veldelementen bewerken nadat u het veld hebt opgeslagen:

   * De naam of beschrijving van een veld
   * De Opties van een Enig-uitgezochte of multi-uitgezochte gebied.
   * De expressie van een veld Formule.

  >[!WARNING]
  >
  >Wanneer formulerendingen veranderen, of de opties van een uitgezocht-type gebied worden toegevoegd of verwijderd, zal er gegevensverlies voor de verslagen zijn die reeds informatie hebben die in de gebieden wordt opgeslagen de waarvan configuratie wordt gewijzigd.
  >
  >Er is geen waarschuwing of indicatie dat dit gegevensverlies kan optreden wanneer u de configuratie van velden wijzigt.
  >
  >Er is geen bericht aan andere gebruikers dat de gebiedsconfiguratie is veranderd.

* U kunt bestaande opzoekvelden van verbonden records bewerken.
* Naast het uitgeven van het gebied zoals die in [ wordt beschreven geef gebiedsmontages ](#edit-field-settings-1) sectie in dit artikel uit, <span class="preview"> kunt u één enkele of multi-uitgezochte keuzen van het gebied uitgeven wanneer u een verslag in de lijstmening uitgeeft, aangezien u de gebiedswaarden bijwerkt. Voor informatie, zie [ nieuwe keuzen aan een bestaand uitgezocht gebied wanneer het uitgeven van verslagen in de 1} sectie van de lijstmening in dit artikel toevoegen.](#add-new-choices-to-an-existing-select-field-when-editing-records-in-the-table-view)</span>

<!--at production - April 10, 2025 - remove the last bullet altogether-->

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

## Veldinstellingen bewerken

{{step1-to-planning}}

1. Klik op de werkruimte waarvan u de recordvelden wilt bewerken.

   De werkruimte wordt geopend en alle recordtypen in de werkruimte worden op kaarten weergegeven.

1. Klik op de kaart van een recordtype.

   Hierdoor wordt de pagina van het recordtype geopend.

1. (Voorwaardelijk) klik het lusje van de mening van de a **Lijst**.

   Alle bestaande records die aan het recordtype zijn gekoppeld, worden in de rijen van de tabelweergave weergegeven.
1. Plaats over de kolomkopbal van een gebied u wilt uitgeven, dan de naar beneden wijzende pijl na de gebiedsnaam klikken, dan **uitgeeft gebied**

   of

   Dubbelklik op de kolomkop voor het veld.

   ![ het menu van de Pijl na naam van gebied in benadrukte lijstkopbal ](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. De informatie van de update over het gebied en klikt **sparen**.

   Voor informatie, zie [ gebieden ](/help/quicksilver/planning/fields/create-fields.md) creëren.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* U kunt het veldtype niet bijwerken nadat het veld is opgeslagen.
   >
   >* Als u veldconfiguraties wijzigt (veldopties of formule-expressies), worden de waarden van records die al informatie in de gewijzigde velden bevatten, in real-time bijgewerkt. Er is geen waarschuwing en geen controlelogboek voor de waardeveranderingen die door de veranderingen van de gebiedsconfiguratie worden teweeggebracht. Alle gebruikers die de velden weergeven, zien de nieuwe waarden direct met de wijzigingen.

   De veldinformatie wordt bijgewerkt voor iedereen die toegang heeft tot de werkruimte.

1. (Voorwaardelijk) voor verbonden verslaggebieden, klik **uitgeeft raadplegingsgebieden** en voeg of verwijder om het even welke raadplegingsgebieden van het verbonden verslagtype toe.

   Voor meer informatie, zie [ Connect verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md).


<div class="preview">

## Nieuwe keuzen toevoegen aan een bestaand selectieveld bij het bewerken van records in de tabelweergave

<!--some of this information is also available in Edit records article - update both when necessary-->

U kunt nieuwe keuzen aan een bestaand enig of multi-uitgezochte gebied toevoegen wanneer het uitgeven van verslagen in de lijstmening.

>[!IMPORTANT]
>
>De in deze sectie beschreven functionaliteit is alleen beschikbaar in de tabelweergave. Deze optie is niet beschikbaar in andere gebieden waar enkelvoudige of meervoudige velden worden weergegeven.

**VOORBEELD**

U hebt mogelijk een veld met de naam Status dat één keuze bevat en de opties Nieuw en Gesloten bevat. U wilt dan een keuze toevoegen voor de status In uitvoering. U kunt de keuze toevoegen door een van de volgende handelingen uit te voeren:

* Het veld bewerken. Voor informatie, zie de sectie [ gebiedsmontages ](#edit-field-settings-1) in dit artikel uitgeven.
* Een nieuwe optie toevoegen tijdens het bewerken van de record in de tabelweergave, zoals hieronder wordt beschreven.

Een nieuwe keuze toevoegen aan een bestaand selectieveld wanneer u een record bewerkt:

1. Ga naar een pagina met recordtypen en open de tabelweergave.
1. Voeg het veld Eén of Meerdere selecties toe waaraan u een keuze wilt toevoegen in de tabelweergave als een nieuwe kolom. Voor informatie, zie [ gebieden ](/help/quicksilver/planning/fields/create-fields.md) creëren.
1. U kunt het veld inline bewerken door te dubbelklikken op de cel voor het veld.
1. Typ de naam van de keus u wilt toevoegen, dan klik **kiezen** toevoegen.

   ![ voeg keus op enig-uitgezocht gebied in lijstmening toe ](assets/add-choice-in-table-view-for-single-select-field.png)

   De nieuwe keuze wordt direct toegevoegd aan het veld Eén keuze.

</div>