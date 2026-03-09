---
title: Overzicht van bedrijfsprofielen
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: add-users-to-workfront
description: De bedrijfsprofielen zijn een verbeterd toestemmingsmodel dat klanten zoals agentschappen toestaat om gebruikerstoegang efficiënt te beheren en nauwkeurige controle over toestemmingen op groepsniveau te verzekeren. In een bedrijfsprofiel, hebben de gebruikers duidelijke toestemmingen aan groep-specifieke voorwerpen. Aanvullende objecten kunnen ook rechtstreeks met het bedrijfsprofiel worden gedeeld.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
exl-id: 7f62de33-e544-4be9-8dcf-03a2e09e8a05
source-git-commit: 1389c6a1f41a14bafd6b70e2e079e40d22d47b07
workflow-type: tm+mt
source-wordcount: '1466'
ht-degree: 0%

---

# Overzicht van bedrijfsprofielen

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Het is beschikbaar slechts in het milieu van de Voorproef voor specifieke klanten.</span>

De bedrijfsprofielen zijn een verbeterd toestemmingsmodel dat klanten zoals agentschappen toestaat om gebruikerstoegang efficiënt te beheren en nauwkeurige controle over toestemmingen op groepsniveau te verzekeren. In een bedrijfsprofiel, hebben de gebruikers duidelijke toestemmingen aan groep-specifieke voorwerpen. Aanvullende objecten kunnen ook rechtstreeks met het bedrijfsprofiel worden gedeeld.

Een bedrijfsprofiel voor een gebruiker is gelijkaardig aan die gebruiker die een specifieke rol in een groep, zoals een financieel controlemechanisme of een projectmanager heeft, en het ontvangen van de toestemmingen die samen met die rol voor de gespecificeerde groep gaan. Het bedrijfsprofiel kan tijdelijk zijn, die de toestemmingen voor een periode toestaat die wordt geplaatst om te verlopen, en het handhaven van gegevensbeperkingen voor de groep of de instantie.

De Workfront-systeembeheerder:

* Maakt de toegangsniveaus en definieert zo nodig beperkte velden
* Werkt het gebruikersprofiel met de groep en het toegangsniveau voor die groep bij (dit is het bedrijfsprofiel)
* Definieert zo nodig effectieve datums voor het bedrijfsprofiel
* Wijst lay-outmalplaatjes aan de toegangsniveaus toe

Elke gebruiker die toegang heeft tot gezamenlijke objecten, kan deze delen met het bedrijfsprofiel. Alle gebruikers met het profiel zien het object.

## Voorbeeld van bedrijfsprofiel

>[!BEGINSHADEBOX]

Sam heeft verschillende toegang tot projecten nodig voor Agentschap A en Agentschap B. Beide agentschappen zijn opgericht als groepen in Workfront. (Zie Overzicht van groepen voor informatie over groepen.)

Voor Agentschap A treedt Sam op als financieel controleur en heeft hij toegang nodig om alle financiële gebieden van zijn projecten te zien. Voor Agentschap B treedt Sam op als projectmanager en moet hij de taken en kwesties beheren, maar mag hij de financiële informatie niet kunnen bekijken.

De het systeembeheerder van Workfront leidt tot nieuwe toegangsniveaus genoemd Financieel Controlemechanisme en de Manager van het Project. Deze toegangsniveaus krijgen de juiste toegang tot financiële gegevens. Dan opent de beheerder het gebruikersprofiel van Sam en selecteert &quot;Agentschap A&quot;als groep met het toegangsniveau &quot;Financiële Controlemechanisme&quot;om het eerste bedrijfsprofiel tot stand te brengen, en &quot;Agentschap B&quot;als groep met het toegangsniveau &quot;de Manager van het Project&quot;om het tweede bedrijfsprofiel tot stand te brengen.

Zodra de bedrijfsprofielen opstelling zijn, wanneer Sam naar de lijst van projecten gaat, zullen alle projecten voor Agentschap A en Agentschap B verschijnen (samen met andere projecten die Sam heeft gecreeerd of toestemmingen aan gekregen). De financiële gebieden van de projecten van Agentschap A zijn voor Sam zichtbaar in zowel de lijstweergave als de projectdetails, maar de financiële gebieden van de projecten van Agentschap B zijn verborgen. De veldnamen worden weergegeven, maar de veldgegevens zijn leeg.

Als andere gebruikers bij een van beide agentschappen projecten delen met de bedrijfsprofielen &quot;Financieel controleur - Agentschap A&quot; of &quot;Projectbeheerder - Agentschap B&quot;, zijn die projecten zichtbaar voor Sam. De financiële gebieden van de projecten van het Agentschap B zullen altijd verborgen blijven, omdat dat in het toegangsniveau wordt gedefinieerd.

>[!ENDSHADEBOX]

## Hoe bedrijfsprofielen worden gedefinieerd

De systeembeheerder van Adobe Workfront is verantwoordelijk voor het bepalen van alle gebieden van een bedrijfsprofiel.

### Toegangsniveau maken

De systeembeheerder van Workfront leidt tot het toegangsniveau met de noodzakelijke toegang en bepaalt om het even welke beperkte gebieden zoals nodig.

Voor meer informatie, zie [ douanetoegangsniveaus ](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) creëren en wijzigen.

### Bedrijfsprofiel aan gebruiker toevoegen

De systeembeheerder van Workfront voegt het bedrijfsprofiel aan een gebruikersprofiel toe door een groep en een toegangsniveau te selecteren. De combinatie van beide leidt tot het bedrijfsprofiel. Elke groep kan slechts in één bedrijfsprofiel per gebruiker worden gebruikt. <!--how does this combine with more than one access level per group. As far as I can see a business profile is one level and one group-->

Het bedrijfsprofiel kan meer dan één toegangsniveau per groep hebben. Het niveau met de hoogste toegang neemt belangrijkheid.

De beheerder kan efficiënte datums aan een bedrijfsprofiel toewijzen, zodat de toegang van de gebruiker op een toekomstige datum zal verlopen. De begin- en einddatum geven aan wanneer de gebruiker begint en eindigt met het vasthouden van het profiel in die groep. Als u effectieve datums gebruikt om de toegang te beëindigen in plaats van het profiel te verwijderen, kan het profiel in de toekomst opnieuw worden geactiveerd.

Meerdere bedrijfsprofielen zijn toegestaan voor één gebruiker.

<!--image?-->

Voor meer informatie, zie [ het profiel van een gebruiker ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven. <!--may be separate article now since it's not in the profile-->

### Lay-outsjablonen toewijzen aan toegangsniveau

De systeembeheerder van Workfront kan naar keuze een lay-outmalplaatje aan het toegangsniveau toewijzen, om ervoor te zorgen dat de gebruikers met het verwante bedrijfsprofiel relevante informatie en acties zien die op hun rol binnen het systeem worden gebaseerd.

Voor meer informatie, zie [ gebruikers aan een lay-outmalplaatje ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md) toewijzen.

## Hoe bedrijfsprofielen werken

Wanneer een bedrijfsprofiel aan een gebruiker wordt toegevoegd, bepalen de toestemmingen in de combinatie van de groep en het toegangsniveau wat de gebruiker in Workfront zal zien.

### Workfront-indeling

Wanneer de groep in het bedrijfsprofiel aan een project wordt geassocieerd, wordt het lay-outmalplaatje voor het toegangsniveau in het bedrijfsprofiel toegepast. Alle gebruikers met het bedrijfsprofiel zien de menu-items, de startpagina en andere lay-outelementen in de sjabloon. De lay-outsjabloon voor bedrijfsprofielen heeft voorrang op een lay-outsjabloon die aan de gebruiker is toegewezen.

Als het bedrijfsprofiel veelvoudige toegangsniveaus met de zelfde groep heeft, worden de lay-outmalplaatjes voor beide toegangsniveaus gecombineerd. Alle beschikbare lay-outelementen worden getoond. Als een menu-item in een sjabloon wordt weergegeven maar in een andere sjabloon verborgen, wordt het weergegeven. Alleen items die in alle sjablonen voor het bedrijfsprofiel verborgen zijn, worden verborgen.

Voor situaties waar de zelfde punten in veelvoudige lay-outmalplaatjes maar de orde van de punten (zoals de linkernavigatie of spelden) worden getoond, dan wordt de orde van het malplaatje van het toegangsniveau dat eerst in het bedrijfsprofiel wordt vermeld gebruikt.

### Projecten en andere gezamenlijke objecten

Wanneer een project aan een groep wordt geassocieerd, kan een gebruiker met een bedrijfsprofiel voor die groep het project bekijken. De zichtbaarheid van velden in het project is gebaseerd op het toegangsniveau in het bedrijfsprofiel. Als de veelvoudige toegangsniveaus aan de groep in het bedrijfsprofiel van de gebruiker worden toegewezen, dan is het niveau met hoogste toestemmingen van toepassing.

Een gebruiker heeft bijvoorbeeld twee bedrijfsprofielen: de eerste geeft toegang aan de financieel controleur voor een groep (om financiële velden te zien) en de tweede geeft toegang aan de projectbeheerder onder een andere groep (waar de financiële gebieden niet moeten worden bekeken).

De gebruiker zou projecten voor beide groepen in de lijst van alle projecten zien. In zowel de lijstmening als de projectdetails, zou de gebruiker financiële gegevens slechts voor de eerste groep zien. De financieringsgebieden van de projecten van de tweede groep zouden leeg zijn.

Elke gebruiker met toegang tot gezamenlijke objecten kan die objecten delen met een bedrijfsprofiel. Alle gebruikers die aan het profiel zijn toegewezen, beschikken over de opgegeven machtigingen voor het object. Nochtans, als de toegang in het toegangsniveau wordt beperkt dat door de beheerder in het bedrijfsprofiel wordt toegewezen, neemt het toegangsniveau belangrijkheid over toestemmingen die in het delen worden gegeven. Bijvoorbeeld, als het toegangsniveau het creëren van taken niet toestaat, dan kan de gebruiker geen taken aan een project toevoegen, zelfs als zij beheertoestemmingen aan een project worden gegeven wanneer het met het bedrijfsprofiel wordt gedeeld.

Als een gebruiker een bedrijfsprofiel krijgt toegewezen nadat een object al met het profiel is gedeeld, ziet de gebruiker het object met de opgegeven toegang.

Wanneer een bedrijfsprofiel veelvoudige toegangsniveaus heeft, neemt het niveau met de hoogste hoeveelheid toegang belangrijkheid.

Voor informatie bij het delen, zie [ een voorwerp ](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md) delen.

Voor informatie over hoe de toegangsniveaus en de toestemmingen samenwerken, zie [ overzicht van de Niveaus van de Toegang ](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

## Overwegingen bij bedrijfsprofielen

* Een gebruiker hoeft geen lid van een groep te zijn om een bedrijfsprofiel voor die groep toe te wijzen.
* Het toegangsniveau op het bedrijfsprofiel kan slechts het &quot;basis&quot;toegangsniveau van een gebruiker bevorderen. Het bedrijfsprofiel kan de bevoegdheden op het niveau van de basistoegang niet verwijderen.
* In objecten lijsten en rapporten, heeft de gebruiker alle toestemmingen die aan hen van al hun toegewezen bedrijfsprofielen over de groepen beschikbaar zijn die met hun basistoegangsniveau worden samengevoegd. Op andere pagina&#39;s heeft de gebruiker de toegangsrechten op het basisniveau.
* Wanneer een groep uit Workfront wordt geschrapt, worden alle toegewezen bedrijfsprofielen voor die groep verwijderd uit de bijbehorende gebruikers.
* Als een toegangsniveau deel van een bedrijfsprofiel uitmaakt en u het toegangsniveau schrapt, wordt u ertoe aangezet om een nieuw toegangsniveau te kiezen in plaats daarvan te gebruiken.
* Updates van bedrijfsprofielen worden bijgehouden in de Workfront-auditlogboeken. Voor meer informatie, zie het overzicht van de Logboeken van de Controle.
