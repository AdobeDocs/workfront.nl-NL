---
title: Goedkeuring toevoegen aan een aanvraagformulier in Adobe Workfront-planning
description: U kunt een goedkeuringsproces aan een formulier van het de planningsverzoek van Adobe Workfront toevoegen, om een goedkeuring voor elk voorgelegd verzoek in werking te stellen, alvorens het tot een verslag leidt.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: 2ffd06f2f50d14b6d33bc79c92616ebed1d58fed
workflow-type: tm+mt
source-wordcount: '1195'
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
<p>Alle Workfront-pakketten en alle planningspakketten</p>
of
<p>Willekeurig workflowpakket en elk planningspakket</p>

<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger.</p>
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
* U kunt goedkeuringsgegevens weergeven in een record die is gemaakt door een aanvraagformulier in te dienen in de velden Goedgekeurd door en Goedgekeurd. Voor informatie, zie [ gebieden ](/help/quicksilver/planning/fields/create-fields.md) creëren.
* Wanneer u meerdere fiatteurs toevoegt aan een aanvraagformulier, moeten alle fiatteurs het verzoek accepteren voordat een record wordt gemaakt in Workfront Planning.
* Als alle fiatteurs het verzoek goedkeuren, wordt een verslag gecreeerd voor het verslagtype verbonden aan het verzoekformulier.
* Als minstens één fiatteur het verzoek verwerpt, en alle anderen het goedkeuren, wordt een verzoek gecreeerd voor het gebied van Verzoeken in Workfront, maar geen verslag wordt gecreeerd voor het verslagtype verbonden aan het verzoekformulier.
* Het toevoegen van goedkeuringen aan een aanvraagformulier is optioneel. Workfront Planning maakt onmiddellijk een record wanneer een aanvraag wordt ingediend, als het aanvraagformulier niet aan een goedkeuring is gekoppeld.

## Een goedkeuring toevoegen aan een aanvraagformulier in de productieomgeving

1. Begin creërend een verzoekvorm voor een verslagtype, zoals die in [ wordt beschreven creeer en beheer een verzoekvorm in de Planning van Adobe Workfront ](/help/quicksilver/planning/requests/create-request-form.md).
1. Klik **Configuratie**.

   De **vertoningen van het het gebiedsgebied van de Configuratie**.

   ![ het lusje van de Configuratie ](assets/configuration-tab.png)
1. Op het **Approvers** gebied, begin de naam van een gebruiker of een team te typen dat u als fiatteur wilt plaatsen, dan het selecteren wanneer het in de lijst toont.
1. (Facultatief en voorwaardelijk) als u meer dan één fiatteur hebt geplaatst, en slechts één fiatteur nodig om een besluit te nemen, laat **slechts één besluit toe wordt vereist** optie.

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* U kunt een of meer fiatteurs toevoegen aan een aanvraagformulier.
   >
   >* Als u meer dan één fiatteur toevoegt, en slechts één besluit wordt vereist optie wordt niet toegelaten, moeten alle fiatteurs het verzoek goedkeuren alvorens de Planning van Workfront tot een verslag leidt.
   >
   >* Als ten minste één fiatteur het verzoek afwijst, wordt het verzoek afgewezen en wordt de record niet gemaakt. Het verzoek blijft op het gebied van verzoeken van Workfront.
   >
   >* Als u meer dan één fiatteur toevoegt en de optie Alleen één beslissing is vereist is niet ingeschakeld, moeten alle fiatteurs een beslissing nemen voordat een aanvraag wordt goedgekeurd of afgewezen.
   >
   >* Als een team als fiatteur wordt geplaatst, wordt slechts één besluit vereist van het team.


1. (Facultatief) klik **publiceren** als u nooit de verzoekvorm eerder hebt gedeeld.

   of

   Klik **Aandeel** om de vorm te delen, toen **verbinding van het Exemplaar**.
1. (Optioneel) Nadat een gebruiker de koppeling gebruikt die u deelt en een aanvraag verzendt, verzendt Workfront Planning een melding voor goedkeuring in de app en een e-mail naar de fiatteurs.

   >[!NOTE]
   >
   >   Het exemplaar van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden ingezien zodat de gebruikers e-mail en in-app berichten kunnen ontvangen.


   Voor informatie over het goedkeuren van verzoeken, zie [ een verzoek ](/help/quicksilver/planning/requests/approve-request.md) goedkeuren.

<div class="preview">

## Goedkeuringsregels toevoegen aan een aanvraagformulier

>[!NOTE]
>
>Deze functionaliteit is alleen beschikbaar in de voorvertoningsomgeving.

In de goedkeuringsregels wordt het goedkeuringsproces gedefinieerd op basis van de veldwaarden in de ingediende aanvragen.

Als een aanvraagformulier bijvoorbeeld het veld ‘Campagnertype’ heeft, kan een regel worden gemaakt die de aanvraag naar één persoon verzendt wanneer het veld de waarde ‘Digitaal’ heeft en naar een andere persoon wanneer deze de waarde ‘Afdrukken’ heeft.

Houd rekening met het volgende wanneer u goedkeuringsregels toevoegt:

* U kunt een of meerdere fiatteurs toevoegen aan een goedkeuringsregel.
* Als ten minste één fiatteur het verzoek afwijst, wordt het verzoek afgewezen en wordt de record niet gemaakt. Het verzoek blijft op het gebied van verzoeken van Workfront.
* Als u meer dan één fiatteur toevoegt en de optie Alleen één beslissing is vereist is niet ingeschakeld, moeten alle fiatteurs een beslissing nemen voordat een aanvraag wordt goedgekeurd of afgewezen.
* Als een team als fiatteur wordt geplaatst, wordt slechts één besluit vereist van het team.

Voor meer informatie over het toevoegen van goedkeuringen, zie [ goedkeuring aan een verzoekvorm ](/help/quicksilver/planning/requests/add-approval-to-request-form.md) toevoegen.

Goedkeuringsregels instellen voor een aanvraagformulier:

1. Begin creërend een verzoekvorm voor een verslagtype, zoals die in [ wordt beschreven creeer en beheer een verzoekvorm in de Planning van Adobe Workfront ](/help/quicksilver/planning/requests/create-request-form.md).
1. Klik **Montages**.

   Het tabblad Instellingen wordt weergegeven.

1. Beginnen vormend goedkeuringsregels, klik goedkeurt ![ pictogram ](assets/approvals-icon-on-form.png) in de linkernavigatie.

1. (Facultatief) als u een standaardgoedkeuringsproces wilt plaatsen, voeg minstens één gebruiker of team aan het **Approvers** gebied van het gebied van de Standaard goedkeuringsregel toe, dan klik **slechts één besluit wordt vereist** checkbox als u het verslag wilt worden gecreeerd nadat om het even welke standaard fiatteurs het heeft goedgekeurd.

   ![ gebied van de Standaard goedkeuringsregel ](assets/default-approvers.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

1. (Optioneel) Ga als volgt te werk voor elke aanvullende goedkeuringsregel:

   1. Klik **toevoegen goedkeuringsregel**
   1. Klik op de titel van de tijdelijke aanduiding &quot;Naamloze goedkeuringsregel&quot; en voer een naam in voor de goedkeuringsregel.
   1. Klik **Uitgezocht een gebied** en selecteer het gebied dat de regel activeert.
   1. Selecteer de operator voor de regel. Operatoren variëren afhankelijk van het type veld.
   1. Als de geselecteerde operator een waarde nodig heeft, klikt u op het plusteken en voegt u een of meer waarden toe.
   1. (Optioneel) Voeg meer voorwaarden toe met AND of OR door te klikken op Voorwaarde toevoegen en de aanvullende voorwaarde te configureren, zoals in de stappen C-E.
   1. Op het gebied van Acties van de goedkeuringsregel, op het **Approvers** gebied, voeg bij huur één gebruiker of team toe die bij de fiatteur moet worden geplaatst wanneer de voorwaarde wordt voldaan aan.
   1. 
      1. (Voorwaardelijk) als u het verslag wilt worden gecreeerd nadat om het even welke fiatteurs het heeft goedgekeurd, controleer **slechts één besluit wordt vereist** checkbox.

1. Klik **sparen** om de goedkeuringsregels te bewaren.
1. (Facultatief) klik **publiceren** als u nooit de verzoekvorm eerder hebt gedeeld.

</div>
