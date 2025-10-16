---
title: Goedkeuring toevoegen aan een aanvraagformulier in Adobe Workfront-planning
description: U kunt een goedkeuringsproces aan een formulier van het de planningsverzoek van Adobe Workfront toevoegen, om een goedkeuring voor elk voorgelegd verzoek in werking te stellen, alvorens het tot een verslag leidt.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: 1a56846647e443cf3f5f09eed8c3084434de5ddb
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# Goedkeuring toevoegen aan een aanvraagformulier in Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt een goedkeuringsproces aan een formulier van het de planningsverzoek van Adobe Workfront toevoegen, om een goedkeuring voor elk voorgelegd verzoek in werking te stellen, alvorens het tot een verslag leidt.

In dit artikel wordt beschreven hoe een werkruimtebeheerder een goedkeuring kan toevoegen aan een aanvraagformulier dat is gekoppeld aan een recordtype.

Voor informatie over het creëren van een verzoekvorm in de Planning van Workfront, zie [ een verzoekvorm in de Planning van Adobe Workfront creëren en beheren ](/help/quicksilver/planning/requests/create-request-form.md).

Voor informatie over het voorleggen van een verzoek aan een verslagtype om een verslag tot stand te brengen, zie [ de Verzoeken van de Planning van Adobe Workfront voorleggen om verslagen ](/help/quicksilver/planning/requests/submit-requests.md) tot stand te brengen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakketten</p></td> 
   <td> 
<ul><li><p>Willekeurig Workfront-pakket</p></li>
en
<li><p>Willekeurig planningspakket</p></li></ul>
of
<ul><li><p>Willekeurig workflowpakket</p></li>
en
<li><p>Willekeurig planningspakket</p></li></ul>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Machtigingen beheren voor een werkruimte en recordtype </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr>  
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het toevoegen van goedkeuringen aan een aanvraagformulier

* U kunt een of meerdere fiatteurs toevoegen aan een aanvraagformulier. U kunt alleen gebruikers toevoegen als fiatteurs.
* <span class="preview"> u kunt goedkeuringsinformatie over een verslag tonen dat door een verzoekvorm in Goedgekeurd door en Goedgekeurde datumgebieden wordt gecreeerd voor te leggen. Voor informatie, zie [ gebieden ](/help/quicksilver/planning/fields/create-fields.md) creëren.</span>
* Wanneer u meerdere fiatteurs toevoegt aan een aanvraagformulier, moeten alle fiatteurs het verzoek accepteren voordat een record wordt gemaakt in Workfront Planning.
* Als alle fiatteurs het verzoek goedkeuren, wordt een verslag gecreeerd voor het verslagtype verbonden aan het verzoekformulier.
* Als minstens één fiatteur het verzoek verwerpt, en alle anderen het goedkeuren, wordt een verzoek gecreeerd voor het gebied van Verzoeken in Workfront, maar geen verslag wordt gecreeerd voor het verslagtype verbonden aan het verzoekformulier.
* Het toevoegen van goedkeuringen aan een aanvraagformulier is optioneel. Workfront Planning maakt onmiddellijk een record wanneer een aanvraag wordt ingediend, als het aanvraagformulier niet aan een goedkeuring is gekoppeld.

## Een goedkeuring toevoegen aan een aanvraagformulier

1. Begin creërend een verzoekvorm voor een verslagtype, zoals die in [ wordt beschreven creeer en beheer een verzoekvorm in de Planning van Adobe Workfront ](/help/quicksilver/planning/requests/create-request-form.md).
1. Klik **Configuratie**.

   De **vertoningen van het het gebiedsgebied van de Configuratie**.

   ![ het lusje van de Configuratie ](assets/configuration-tab.png)
1. In het **Approvers** gebied, klik het drop-down pictogram en selecteer één of verscheidene gebruikers of teams in de lijst

   of

   Typ de naam van een gebruiker of team die u als fiatteur wilt instellen en selecteer deze vervolgens wanneer deze in de lijst wordt weergegeven.

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* U kunt een of meer fiatteurs toevoegen aan een aanvraagformulier.
   >
   >* Als u meerdere fiatteurs toevoegt, moeten alle fiatteurs het verzoek goedkeuren voordat Workfront Planning een record maakt.
   >
   >* Als ten minste één fiatteur het verzoek afwijst, wordt het verzoek afgewezen en wordt de record niet gemaakt. Het verzoek blijft op het lusje van de Planning van de Verzendende sectie in het gebied van Verzoeken van Workfront.
   >
   >* Elke fiatteur moet een beslissing nemen voordat een verzoek wordt goedgekeurd of afgewezen.
   >
   >* Als een team als fiatteur wordt geplaatst, wordt slechts één besluit vereist van het team.


1. (Facultatief) klik **publiceren** als u nooit de verzoekvorm vóór hebt gedeeld

   of

   Klik **Aandeel** om de vorm te delen, toen **verbinding van het Exemplaar**.
1. (Optioneel) Nadat een gebruiker de koppeling gebruikt die u deelt en een aanvraag verzendt, verzendt Workfront Planning een melding voor goedkeuring in de app en een e-mail naar de fiatteurs.

   >[!NOTE]
   >
   >   Het exemplaar van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden ingezien zodat de gebruikers e-mail en in-app berichten kunnen ontvangen.


   Voor informatie over het goedkeuren van verzoeken, zie [ een verzoek ](/help/quicksilver/planning/requests/approve-request.md) goedkeuren.
