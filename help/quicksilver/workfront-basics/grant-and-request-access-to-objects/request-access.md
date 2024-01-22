---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Toegang tot objecten aanvragen
description: De zichtbaarheid van objecten in Adobe Workfront is afhankelijk van de toegang tot dat type object en van de machtigingen die u voor een afzonderlijk object hebt.
author: Alina
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 0%

---

# Toegang tot objecten aanvragen

De zichtbaarheid van objecten in Adobe Workfront is afhankelijk van de toegang tot dat type object en van de machtigingen die u voor een afzonderlijk object hebt.

>[!NOTE]
>
>In dit artikel wordt beschreven hoe u machtigingen kunt aanvragen voor alle objecten, behalve voor plannen in de Adobe Workfront Scenario Planner. Voor informatie over het vragen van toegang tot plannen, zie [Toegang tot een abonnement aanvragen in de Scenario Planner](../../scenario-planner/request-access-to-plan.md). Hiervoor is een aanvullende licentie vereist.

Uw Workfront-beheerder configureert uw toegang tot een type object op uw toegangsniveau. Zie voor meer informatie [Hoe de toegangsniveaus en de toestemmingen samenwerken](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Als u machtigingen nodig hebt voor specifieke objecten in Workfront, kunt u deze objecten aanvragen. In plaats van e-mail naar de Workfront-beheerder of objecteigenaar te verzenden om uw behoeften uit te leggen, kunt u aanvullende toegang (of machtigingen) aanvragen in Workfront.

U kunt een eerste toegang tot objecten aanvragen als iemand een koppeling naar het object met u deelt of als u aanvullende toegang tot objecten wilt vragen die u tenminste wilt bekijken.

Bijvoorbeeld, zou u de toestemmingen van de Mening aan een project kunnen hebben, maar u moet taken aan dat project toevoegen. In dit geval kunt u Contribute-machtigingen voor het project aanvragen.

## Toegangsvereisten

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you request permissions to</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

U moet het volgende hebben om objecten te delen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot of hoger weergeven voor objecten waarvoor u machtigingen aanvraagt</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Standaarden voor delen begrijpen

De volgende standaard regels voor delen worden automatisch van kracht, omdat deze als standaardopties in uw Workfront-systeem zijn ingesteld.

* Gebruikers die zijn toegewezen aan een taak of een uitgave, hebben Contribute-toegang hierop.
* Project-, Portfolio- en programmamanagers hebben toegang tot de objecten die zij bezitten.
* De gebruikers inbegrepen in een gesprek hebben de toegang van de Mening over het voorwerp waar het gesprek gebeurt.
* Gebruikers die als fiatteurs zijn toegewezen, hebben toegang tot de weergave op het object dat wacht op goedkeuring.
* Wanneer u een dashboard deelt, worden alle rapporten op het dashboard ook gedeeld met dezelfde toegang tot dezelfde gebruikers.
* Objecteigenaars kunnen de toegang tot een object niet uitbreiden tot buiten hun toegang tot dat object, zoals gedefinieerd door de beheerder.

## Toegang aanvragen

U kunt een eerste toegang aanvragen tot objecten waartoe u momenteel geen toegang hebt, of u kunt aanvullende toegang aanvragen tot objecten waartoe u slechts beperkte toegang hebt.

* [Aanvankelijke toegang aanvragen](#request-initial-access)
* [Aanvullende toegang aanvragen](#request-additional-access)

### Aanvankelijke toegang aanvragen  {#request-initial-access}

Als u nog geen toegang hebt tot een object en u vanuit een koppeling naar dat object navigeert, wordt een scherm weergegeven met de mededeling dat u geen toegang hebt om de informatie te bekijken.

Aanvankelijke toegang tot een object aanvragen:

1. Klikken **Toegang aanvragen**.\
   De **Toegang aanvragen** wordt weergegeven.

1. (Voorwaardelijk) als meer dan één gebruiker de aangewezen toegang heeft om u extra toegang te verlenen, wordt een drop-down pijl getoond naast de naam van de gebruiker.
1. Selecteer in de vervolgkeuzelijst de gebruiker die u uw toegangsverzoek wilt ontvangen.\
   In de vervolgkeuzelijst worden slechts tien gebruikers weergegeven. De lijst wordt alfabetisch gesorteerd.\
   Voor meer informatie over de orde van de gebruikers die in dit drop-down menu worden vermeld, zie  [Hiërarchie van de vervolgkeuzemenu&#39;s &quot;Toegang aanvragen&quot; en &quot;Meer toegang aanvragen&quot;](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Selecteer in de vervolgkeuzelijst het type toegang dat u aanvraagt.
1. (Optioneel) In het dialoogvenster **P.S.** geeft u de gebruiker een opmerking met betrekking tot waarom u aanvullende toegang nodig hebt.

   ![](assets/request-access-dialog-350x314.png)

Als u geen toegangsniveaurechten voor een voorwerp hebt en u probeert om tot dat voorwerp van een verbinding toegang te hebben, wordt een scherm getoond informerend u om de beheerder van Workfront te contacteren.

Als u bijvoorbeeld geen portfoliotoegang hebt, maar u een koppeling naar een portfolio hebt gekregen, wordt het volgende bericht weergegeven:\
![](assets/permission-request-initial2-350x96.png)

### Aanvullende toegang aanvragen {#request-additional-access}

Aanvullende toegang aanvragen tot een object waartoe u al beperkte toegang hebt:

1. Ga naar het object waarvoor u aanvullende toegang wilt aanvragen.

1. Klik op de knop **Meer** rechts van de projectnaam klikt u op **Meer toegang aanvragen**.

   ![](assets/request-access-in-project-350x201.png)

1. (Voorwaardelijk) als meer dan één gebruiker de aangewezen toegang heeft om u extra toegang te verlenen, wordt een drop-down pijl getoond naast de naam van de gebruiker.
1. Selecteer in de vervolgkeuzelijst de gebruiker die u uw toegangsverzoek wilt ontvangen.\
   In de vervolgkeuzelijst worden slechts tien gebruikers weergegeven. De lijst wordt alfabetisch gesorteerd.\
   Voor meer informatie over de orde van de gebruikers die in dit drop-down menu worden vermeld, zie  [Hiërarchie van de vervolgkeuzemenu&#39;s &quot;Toegang aanvragen&quot; en &quot;Meer toegang aanvragen&quot;](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Selecteer in de vervolgkeuzelijst het toegangsniveau dat u aanvraagt.
1. (Optioneel) In het dialoogvenster **P.S.** veld, geeft u een notitie op met betrekking tot de vraag waarom u aanvullende toegang nodig hebt.
1. Klikken **Toegang aanvragen**.\
   ![](assets/request-access-dialog-350x314.png)

## Hiërarchie van de vervolgkeuzemenu&#39;s &quot;Toegang aanvragen&quot; en &quot;Meer toegang aanvragen&quot; {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [Begrijp de hiërarchie van gebruikers die in de drop-down menu&#39;s van de Toegang van het Verzoek en van het Verzoek Meer Toegang worden vermeld](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [De eigenaar van een object begrijpen](#understand-the-owner-of-an-object)

### Begrijp de hiërarchie van gebruikers die in de drop-down menu&#39;s van de Toegang van het Verzoek en van het Verzoek Meer Toegang worden vermeld {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

Wanneer Workfront de lijsten &quot;Request Access&quot; of &quot;Request More Access&quot; op objecten vult, selecteert het een lijst met maximaal tien gebruikers die verschillende rollen vervullen bij het delen van het object, zoals hieronder wordt beschreven. Deze gebruikers kunnen toegang tot het object verlenen aan de gebruiker die het aanvraagt.\
De resulterende lijst wordt dan gesorteerd op hun naam in oplopende alfabetische volgorde.\
Workfront geeft maximaal 10 gebruikers weer in de lijsten &quot;Toegang aanvragen&quot; en &quot;Meer toegang aanvragen&quot;.

De volgorde van de gebruikers in de vervolgkeuzemenu&#39;s &#39;Toegang aanvragen&#39; of &#39;Meer toegang aanvragen&#39; wordt bepaald door de volgende regels:

* De eerste gebruiker in de lijst is het object &quot;owner&quot;, zoals beschreven in [De eigenaar van een object begrijpen](#understand-the-owner-of-an-object).
* Vervolgens wordt de lijst gevuld met gebruikers met wie het object afzonderlijk wordt gedeeld. Ze worden in alfabetische volgorde weergegeven.
* Dan is de lijst verder bevolkt met gebruikers die de vereiste toegang door het delen met hun teams, groepen, of bedrijven krijgen. Ze worden in alfabetische volgorde weergegeven.
* Als de lijst leeg is, worden de beheerders van Workfront toegevoegd zodat er altijd iemand is om toegang van te vragen. Ze worden in alfabetische volgorde weergegeven.
* Elk van de gebruikers in de lijst moet de gevraagde toegang tot het voorwerp en de toegang hebben om het voorwerp te delen.

### De eigenaar van een object begrijpen {#understand-the-owner-of-an-object}

De eigenaar van een object wordt als volgt gedefinieerd:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Object</strong> </th> 
   <th><strong>Definitie van de eigenaar van het object</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projecten</td> 
   <td>De eigenaar is de eigenaar van het project of, als deze ontbreekt of niet over de benodigde toegang beschikt, de eigenaar van het bovenliggende portfolio. <p>Zij zouden niet de zelfde persoon kunnen zijn zoals de projectschepper. </p></td> 
  </tr> 
  <tr> 
   <td>Taken</td> 
   <td>De eigenaar is de Primaire Ontvanger of, als het ontbreekt of zij hebben niet de noodzakelijke toegang, de eigenaar van project waarop de taak, zoals hierboven bepaald verblijft. <p>Zij zouden niet de zelfde persoon kunnen zijn zoals de taakschepper. </p></td> 
  </tr> 
  <tr> 
   <td>Problemen</td> 
   <td> <p>De eigenaar is de primaire contactpersoon van de uitgave of, als deze ontbreekt of niet over de benodigde toegang beschikt, de eigenaar van het project waarop de uitgave zich bevindt, zoals hierboven gedefinieerd. </p> <p>Ze zijn mogelijk niet dezelfde persoon als de maker van de uitgave. </p> </td> 
  </tr> 
  <tr> 
   <td>Portfolio's</td> 
   <td>De eigenaar is de eigenaar van het Portfolio. <p>Ze zijn mogelijk niet dezelfde persoon als de maker van de portefeuille. </p></td> 
  </tr> 
  <tr> 
   <td>Documenten</td> 
   <td>De eigenaar is de eigenaar van het document (de gebruiker die het document heeft geüpload) of, als het document ontbreekt of niet de benodigde toegang heeft, de eigenaar van het object waarop het document zich bevindt.</td> 
  </tr> 
  <tr> 
   <td>Rapporten en dashboards</td> 
   <td>De eigenaar is de maker van het rapport of het dashboard. </td> 
  </tr> 
  <tr> 
   <td>Kalenders</td> 
   <td>De eigenaar is de maker van de kalender. Aan alle gebruikers is standaard een kalender toegewezen. Zij worden beschouwd als de eigenaar van die kalender. </td> 
  </tr> 
  <tr> 
   <td>Filters, weergaven en groepen</td> 
   <td>De eigenaar van een filter, weergave of groep is de maker. </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Abonnementen</span> </td> 
   <td> <p><span>De eigenaar is de maker van de regeling.</span> </p> <p>Hiervoor is een aanvullende licentie vereist. </p> <p><span>Voor informatie over de Workfront Scenario Planner raadpleegt u</span> <a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Overzicht van de functie Scenario Planner</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Doelen</td> 
   <td> <p>De eigenaar is de gebruiker die als eigenaar is aangewezen. Ze zijn misschien niet dezelfde persoon als de maker van het doel. </p> <p>Hiervoor is een aanvullende licentie vereist. </p> <p>Voor informatie over Workfront Goals raadpleegt u <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Overzicht van Adobe Workfront-doelen</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


