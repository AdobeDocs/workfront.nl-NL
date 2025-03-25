---
title: Publiceren van een aanvraagformulier in Adobe Workfront-planning ongedaan maken
description: U kunt de publicatie van een aanvraagformulier ongedaan maken als dit niet meer nodig of relevant is. Als u de publicatie ongedaan maakt, verwijdert u ieders machtigingen om het formulier te openen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 0%

---

# Publiceren van een aanvraagformulier in Adobe Workfront Planning ongedaan maken


<!--take Preview and Production references at Production time-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

U kunt de publicatie van een aanvraagformulier ongedaan maken als dit niet meer nodig of relevant is. Als u de publicatie ongedaan maakt, verwijdert u ieders machtigingen om het formulier te openen.

U kunt ook de entiteiten wijzigen waarmee u een aanvraagformulier deelt, als u het beschikbaar wilt houden voor een kleinere groep personen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <li><p>Machtigingen beheren in een werkruimte <!--<span class="preview">and record type</span>--> </p></li>
    <li><p>Systeembeheerders kunnen werkruimten beheren die ze niet hebben gemaakt. </p></li>
    </ul>
   <p>Voor informatie over het delen van machtigingen voor Workfront Planning-objecten raadpleegt u  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md"> Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront </a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat. </p>  
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

1. Klik **Meer** menu ![ meer menu ](assets/more-menu.png) rechts van de naam van het verslagtype in de paginakop, dan klik **de verzoekvorm van de Update**.
1. Klik **Aandeel** in de hoger-juiste hoek van het scherm, dan werk de het delen keuzen bij. Voor meer informatie, zie [ creeer en beheer een verzoekvorm in de Planning van Adobe Workfront ](/help/quicksilver/planning/requests/create-request-form.md).
1. (Facultatief) klik **verbinding van het Exemplaar**, als u het delen van de verzoekvorm veranderde en u het aan de nieuwe groep mensen met een nieuwe verbinding wilt delen.

## Publiceren van een aanvraagformulier voor een recordtype ongedaan maken

Wanneer een aanvraagformulier irrelevant wordt en u wilt dat niemand er langer toegang toe heeft, kunt u de publicatie ervan ongedaan maken.

{{step1-to-planning}}

1. Klik op de werkruimte waar u records wilt toevoegen.

   De werkruimte wordt geopend en de recordtypen worden als kaarten weergegeven.

1. Klik op een opnametype. Voor informatie over het creëren van een verslagtype, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

   De pagina met recordtypen wordt geopend in de weergave die u het laatst hebt geopend. Standaard wordt een pagina met recordtypen geopend in de tabelweergave.

1. Klik **Meer** menu ![ Meer menu ](assets/more-menu.png) aan het recht van de naam van het verslagtype in de paginakop, dan klik **de verzoekvorm van de Update**.
1. Klik **unpublish** in de hoger-juiste hoek.

   ![ Unpublish benadrukte knoop ](assets/unpublish-button-highlighted.png)

   Onder aan het scherm verschijnt een bevestiging met de mededeling dat het formulier niet is gepubliceerd.

   De **unpublish** knoop verandert in **publiceren**.

1. Klik **sparen**.

   Het formulier kan niet langer worden geopend via een koppeling <!--or from the request queue in the Requests area of Workfront--> .

   Alle records die u eerder met het aanvraagformulier hebt toegevoegd, blijven op de recordtypepagina staan.

   Alle eerder toegevoegde verzoeken blijven op het tabblad Planning in het gebied Verzoeken van Workfront.
