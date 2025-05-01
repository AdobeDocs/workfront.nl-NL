---
title: Publiceren van een aanvraagformulier in Adobe Workfront-planning ongedaan maken
description: U kunt de publicatie van een aanvraagformulier ongedaan maken als dit niet meer nodig of relevant is. Als u de publicatie ongedaan maakt, verwijdert u ieders machtigingen om het formulier te openen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 0%

---

# Publiceren van een aanvraagformulier in Adobe Workfront Planning ongedaan maken


<!--take Preview and Production references at Production time-->

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt de publicatie van een aanvraagformulier ongedaan maken als dit niet meer nodig of relevant is. Als u de publicatie ongedaan maakt, verwijdert u ieders machtigingen om het formulier te openen.

U kunt ook de entiteiten wijzigen waarmee u een aanvraagformulier deelt, als u het beschikbaar wilt houden voor een kleinere groep personen.

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

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
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningsplan is opgenomen. </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-platform</p></td>
   <td>
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden bezeten om tot alle mogelijkheden van de Planning van Workfront toegang te hebben.</p>
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td>
   <td>
   <p>Standaard</p>
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
   <td>
   <ul>
   <li><p>Beheer toestemmingen aan een werkruimte <span class="preview"> en verslagtype </span> </p></li>
    <li><p>Systeembeheerders kunnen werkruimten beheren die ze niet hebben gemaakt. </p></li>
    </ul>
   <p>Voor informatie over het delen van machtigingen voor Workfront Planning-objecten raadpleegt u  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md"> Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront </a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>In het milieu van de Productie, moeten alle gebruikers met inbegrip van de Beheerders van het Systeem aan een lay-outmalplaatje worden toegewezen dat Planning omvat.</p>
<p><span class="preview">In het milieu van de Voorproef, hebben de Standaardgebruikers en de Beheerders van het Systeem Planning die door gebrek wordt toegelaten.</span></p>  
</td>
  </tr>
 </tbody>
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Het delen van een aanvraagformulier wijzigen

Als u een verzoek voor openbaar deelt, met iedereen met inbegrip van gebruikers van buiten uw organisatie, zou u kunnen overwegen om deze toegang tot bepaalde gebruikers te beperken die of de werkruimte bekijken of beheren het formulier wordt geassocieerd met.

Zo wijzigt u het delen van een aanvraagformulier:

{{step1-to-planning}}

1. Klik op de werkruimte waar u records wilt toevoegen.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype. Voor informatie over het creëren van een verslagtype, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

   De pagina met recordtypen wordt geopend in de weergave die u het laatst hebt geopend. Standaard wordt een pagina met recordtypen geopend in de tabelweergave.

1. Klik **Meer** menu ![ Meer menu ](assets/more-menu.png) aan het recht van de naam van het verslagtype in de paginakop, dan klik **leidt verzoekvormen**.

   Alle aanvraagformulieren die aan het recordtype zijn gekoppeld, worden in een tabelweergave weergegeven.
1. Beweeg over de naam van een verzoekvorm, dan klik **Meer** menu ![ Meer menu ](assets/more-menu.png) aan het recht van zijn naam, dan klik **Aandeel**.
1. Werk de opties voor delen bij door een van de volgende opties te selecteren:

   * Iedereen met weergave of hogere toegang tot de werkruimte
   * Iedereen met een hogere of hogere toegang tot de werkruimte
   * Iedereen met de koppeling

   Voor meer informatie, zie [ creeer en beheer een verzoekvorm in de Planning van Adobe Workfront ](/help/quicksilver/planning/requests/create-request-form.md).
1. (Facultatief) klik **verbinding van het Exemplaar**, als u het delen van de verzoekvorm veranderde en u het aan de nieuwe groep mensen met een nieuwe verbinding wilt delen.

## Publiceren van een aanvraagformulier voor een recordtype ongedaan maken

Wanneer een aanvraagformulier irrelevant wordt en u wilt dat niemand er langer toegang toe heeft, kunt u de publicatie ervan ongedaan maken.

{{step1-to-planning}}

1. Klik op de werkruimte waar u records wilt toevoegen.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype. Voor informatie over het creëren van een verslagtype, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

   De pagina met recordtypen wordt geopend in de weergave die u het laatst hebt geopend. Standaard wordt een pagina met recordtypen geopend in de tabelweergave.

1. Klik **Meer** menu ![ Meer menu ](assets/more-menu.png) aan het recht van de naam van het verslagtype in de paginakop, dan klik **leidt verzoekvormen**.

   Alle aanvraagformulieren die aan het recordtype zijn gekoppeld, worden in een tabelweergave weergegeven.
1. Beweeg over de naam van een verzoekvorm, dan klik **Meer** menu ![ Meer menu ](assets/more-menu.png) aan het recht van zijn naam, dan klik **unpublish**

of

Klik de naam van de verzoekvorm om het te openen, dan klik **unpublish** in de hoger-juiste hoek van de verzoekvorm.

![ Unpublish benadrukte knoop ](assets/unpublish-button-highlighted.png)

Onder aan het scherm verschijnt een bevestiging met de mededeling dat het formulier niet is gepubliceerd.

De **unpublish** verbinding of de knoopveranderingen in **publiceren**.

1. (Voorwaardelijk) klik **sparen**, als u de vorm na het openen van het unpublished.

   Gebruikers hebben geen toegang meer tot het aanvraagformulier via een koppeling of vanuit de wachtrij met aanvragen in het gedeelte Aanvragen van Workfront.

   Alle records die u eerder met het aanvraagformulier hebt toegevoegd, blijven op de recordtypepagina staan.

   Alle eerder toegevoegde verzoeken blijven op het tabblad Planning in het gebied Verzoeken van Workfront.
