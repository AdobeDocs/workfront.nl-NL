---
title: Goedkeuring toevoegen aan een aanvraagformulier in Adobe Workfront-planning
description: U kunt een goedkeuringsproces aan een formulier van het de planningsverzoek van Adobe Workfront toevoegen, om een goedkeuring voor elk voorgelegd verzoek in werking te stellen, alvorens het tot een verslag leidt.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: 83b3bd73fd30b5fba931e64783dee67485d98fe9
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 0%

---

# Goedkeuring toevoegen aan een aanvraagformulier in Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [&#x200B; snelle versies voor uw organisatie &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

U kunt een goedkeuringsproces aan een formulier van het de planningsverzoek van Adobe Workfront toevoegen, om een goedkeuring voor elk voorgelegd verzoek in werking te stellen, alvorens het tot een verslag leidt.

In dit artikel wordt beschreven hoe een werkruimtebeheerder een goedkeuring kan toevoegen aan een aanvraagformulier dat is gekoppeld aan een recordtype.

Voor informatie over het creëren van een verzoekvorm in de Planning van Workfront, zie [&#x200B; een verzoekvorm in de Planning van Adobe Workfront creëren en beheren &#x200B;](/help/quicksilver/planning/requests/create-request-form.md).

Voor informatie over het voorleggen van een verzoek aan een verslagtype om een verslag tot stand te brengen, zie [&#x200B; de Verzoeken van de Planning van Adobe Workfront voorleggen om verslagen &#x200B;](/help/quicksilver/planning/requests/submit-requests.md) tot stand te brengen.

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
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningsplan is opgenomen. </td>

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
   <li><p>Machtigingen beheren in een werkruimte en recordtype</p></li>
    <li><p>Systeembeheerders kunnen werkruimten beheren die ze niet hebben gemaakt. </p></li>
    </ul>
   <p>Voor informatie over het delen van machtigingen voor Workfront Planning-objecten raadpleegt u  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md"> Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront </a> 
  </td>
  </tr>

</tbody>
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het toevoegen van goedkeuringen aan een aanvraagformulier

* U kunt een of meerdere fiatteurs toevoegen aan een aanvraagformulier. U kunt alleen gebruikers toevoegen als fiatteurs.
* <span class="preview"> u kunt goedkeuringsinformatie over een verslag tonen dat door een verzoekvorm in Goedgekeurd door en Goedgekeurde datumgebieden wordt gecreeerd voor te leggen. Voor informatie, zie [&#x200B; gebieden &#x200B;](/help/quicksilver/planning/fields/create-fields.md) creëren.</span>
* Wanneer u meerdere fiatteurs toevoegt aan een aanvraagformulier, moeten alle fiatteurs het verzoek accepteren voordat een record wordt gemaakt in Workfront Planning.
* Als alle fiatteurs het verzoek goedkeuren, wordt een verslag gecreeerd voor het verslagtype verbonden aan het verzoekformulier.
* Als minstens één fiatteur het verzoek verwerpt, en alle anderen het goedkeuren, wordt een verzoek gecreeerd voor het gebied van Verzoeken in Workfront, maar geen verslag wordt gecreeerd voor het verslagtype verbonden aan het verzoekformulier.
* Het toevoegen van goedkeuringen aan een aanvraagformulier is optioneel. Workfront Planning maakt onmiddellijk een record wanneer een aanvraag wordt ingediend, als het aanvraagformulier niet aan een goedkeuring is gekoppeld.

## Een goedkeuring toevoegen aan een aanvraagformulier

1. Begin creërend een verzoekvorm voor een verslagtype, zoals die in [&#x200B; wordt beschreven creeer en beheer een verzoekvorm in de Planning van Adobe Workfront &#x200B;](/help/quicksilver/planning/requests/create-request-form.md).
1. Klik **Configuratie**.

   De **vertoningen van het het gebiedsgebied van de Configuratie**.

   ![&#x200B; het lusje van de Configuratie &#x200B;](assets/configuration-tab.png)
1. In het **Approvers** gebied, klik het drop-down pictogram en selecteer één of verscheidene gebruikers <span class="preview"> of teams </span> in de lijst

   of

   Begin de naam van een gebruiker <span class="preview"> of team </span> te typen die u als fiatteur wilt plaatsen, dan het selecteren wanneer het in de lijst toont.

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
   >* <span class="preview"> als een team als fiatteur wordt geplaatst, slechts wordt één besluit vereist van het team.</span>


1. (Facultatief) klik **publiceren** als u nooit de verzoekvorm vóór hebt gedeeld

   of

   Klik **Aandeel** om de vorm te delen, toen **verbinding van het Exemplaar**.
1. (Optioneel) Nadat een gebruiker de koppeling gebruikt die u deelt en een aanvraag verzendt, verzendt Workfront Planning een melding voor goedkeuring in de app en een e-mail naar de fiatteurs.

   >[!NOTE]
   >
   >   Het exemplaar van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden ingezien zodat de gebruikers e-mail en in-app berichten kunnen ontvangen.


   Voor informatie over het goedkeuren van verzoeken, zie [&#x200B; een verzoek &#x200B;](/help/quicksilver/planning/requests/approve-request.md) goedkeuren.
