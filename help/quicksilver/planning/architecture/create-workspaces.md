---
title: Werkruimten maken
description: Een werkruimte is een inzameling van verslagtypes die door een team worden gebruikt en vertegenwoordigt de het werklevenscyclus van het team. U kunt werkruimten volledig aanpassen in Adobe Workfront Planning. Recordtypen worden ingedeeld in secties in een werkruimte.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---


# Werkruimten maken

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->


{{planning-important-intro}}

In de Planning van Adobe Workfront, zijn de werkruimten gecentraliseerde plaatsen voor teams om het werk te plannen.

Een werkruimte is een inzameling van verslagtypes die door een team worden gebruikt en vertegenwoordigt de het werklevenscyclus van het team. U kunt werkruimten volledig aanpassen in Adobe Workfront Planning.

Voor algemene informatie over werkruimten, zie [&#x200B; Overzicht van Werkruimten &#x200B;](/help/quicksilver/planning/architecture/workspaces-overview.md).

## Toegangsvereisten

+++ Breid uit om de toegangsvereisten voor de functionaliteit in dit artikel te bekijken. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Een Workfront- of workflowpakket</p> 
<p>Willekeurig Workfront-planningspakket</p>
<p>Een Workfront Planning Prime of hoger-pakket om meerdere werkruimten tegelijk te maken</p>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
   <p>Systeembeheerder om meerdere werkruimten tegelijk te maken met behulp van de sjabloonbundel met best practices</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Machtigingen beheren in een werkruimte</p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr>  
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--
Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>You receive Manage permissions to the workspaces you create. </p> </td> 
  </tr> 
</tbody> 
</table>
-->

## Een werkruimte maken

U kunt een werkruimte maken en er recordtypen aan toevoegen om uw objecten te ordenen in Workfront Planning.

Voor meer informatie over het uitgeven van een werkruimte, zie [&#x200B; werkruimten &#x200B;](/help/quicksilver/planning/architecture/edit-workspaces.md) uitgeven.

U kunt op de volgende manieren werkruimten maken:

* Een werkruimte maken op basis van een blanco werkruimte of een sjabloon

  Voor informatie, zie de sectie [&#x200B; een werkruimte van kras of van een malplaatje &#x200B;](#create-a-workspace-from-scratch-or-from-a-template) in dit artikel creëren.
* Maak één werkruimte met de door AI aangedreven Planning Designer. Deze functie is momenteel alleen beschikbaar voor een beperkt aantal klanten in een Beta-programma.

  Voor informatie, zie [&#x200B; begonnen worden met de Planning Designer van Adobe Workfront &#x200B;](/help/quicksilver/planning/general/planning-ai-designer.md).

* Meerdere werkruimten maken met behulp van een sjabloonbundel voor aanbevolen werkruimten

  Voor informatie, zie de sectie [&#x200B; veelvoudige werkruimten creëren gebruikend een best-praktijk multi-workspace malplaatjebundel &#x200B;](#create-multiple-workspaces-using-a-best-practice-multi-workspace-template-bundle) in dit artikel

  >[!TIP]
  >
  >U kunt veelvoudige werkruimten in één keer slechts tot stand brengen wanneer u de best-praktijk malplaatjebundel gebruikt.

### Een werkruimte maken op basis van een blanco formulier of een sjabloon

{{step1-to-planning}}

1. Klik **creëren werkruimte**

   Het dialoogvenster Maken wordt weergegeven. U kunt een werkruimte helemaal opnieuw maken of maken met een van de beschikbare sjablonen.

1. (Facultatief en voorwaardelijk) klik **Voorproef** binnen om het even welke volgende vooraf bepaalde werkruimtesjablonen:

   * Basis: Marketing Management
   * Geavanceerd: marketingbeheer
   * Enterprise: Marketing Management
   * Verkoopbeheer
   * Productbeheer

   Het voorbeeldvak voor de sjabloon wordt geopend.

   Er is een indicatie van welke operationele recordtypen, taxonomieën en hoeveel velden aan elke sjabloon zijn gekoppeld.

   ![&#x200B; Previewing een werkruimtemalplaatje &#x200B;](assets/previewing-a-workspace-template.png)

   Voor informatie over de malplaatjes van de werkruimte van de Planning van Workfront, zie [&#x200B; Lijst van werkruimtesjablonen &#x200B;](/help/quicksilver/planning/architecture/workspace-templates.md).

1. Van het vakje van de malplaatjevoorproef, klik **malplaatje van het Gebruik** beginnen de werkruimte van het geselecteerde malplaatje te creëren

   of

   Klik **terug**, dan klik **Nieuwe werkruimte** om een werkruimte van kras tot stand te brengen.

   Er wordt een werkruimte gemaakt voor de volgende typen werkruimten:

   * Een lege werkruimte genoemd **Naamloze Workspace** waar u recordtypes kunt beginnen manueel toe te voegen, wanneer u een werkruimte van kras creeert.
   * Een werkruimte die wordt genoemd naar de geselecteerde sjabloon en die is gevuld met typen voorbeeldrecords. U kunt de recordtypen en de werkruimte verder aanpassen.

   Voor de beheerders van Workfront, de nieuwe werkruimtevertoningen op de **Werkruimten ik op** tabel ben.

   Voor alle andere gebruikers die werkruimten kunnen tot stand brengen, toont de nieuwe werkruimte in het **1&rbrace; gebied van de Werkruimten &lbrace;.**

1. Klik binnen de naam van de werkruimte in de koptekst van de nieuwe werkruimte om de naam ervan te wijzigen en druk vervolgens op Enter.

1. (Facultatief en voorwaardelijk) als u de werkruimte van een malplaatje creeerde, klik binnen de naam van de **Operationele Types van Verslag** of **taxonomieën** secties

   of

   Beweeg de naam van een sectie, dan klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png), dan klik **anders noemen** om de sectie anders te noemen.

   >[!TIP]
   >
   >U kunt de naam van elke sectie vanuit elke werkruimte wijzigen, zelfs als u de sectie niet hebt gemaakt.

   Voor meer informatie over het uitgeven van werkruimten, met inbegrip van het uitgeven van werkruimtesecties, zie [&#x200B; werkruimten &#x200B;](/help/quicksilver/planning/architecture/edit-workspaces.md) uitgeven.

1. (Facultatief) klik **recordtype** toevoegen om verslagtypes aan de werkruimte in om het even welke sectie toe te voegen.

   Voor informatie, zie [&#x200B; recordtypes &#x200B;](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

   Voor meer informatie over het uitgeven van en het schrappen van verslagtypes in een werkruimte, zie [&#x200B; werkruimten &#x200B;](/help/quicksilver/planning/architecture/edit-workspaces.md) uitgeven.

1. (Optioneel) Klik op de pijl Vorige links van de nieuwe werkruimte om de hoofdpagina Planning te openen. Een nieuwe werkruimtekaart wordt gecreeerd voor de nieuwe werkruimte in de **Werkruimten I op** tabel.

   De naam van de gebruiker die de werkruimte heeft gemaakt, wordt als eigenaar opgeslagen op de werkruimtekaart.

   >[!TIP]
   >
   >De werkruimten die door Workfront-slechts gebruikers worden gecreeerd die niet aan de vertoning van Adobe Admin Console zoals gecreeerd door het **Systeem** zijn toegevoegd.
   >

### Meerdere werkruimten maken met behulp van een sjabloonbundel voor aanbevolen werkruimten

>[!IMPORTANT]
>
>Het creëren van veelvoudige werkruimten tegelijkertijd gebruikend de best-praktijkmalplaatjebundel is beschikbaar slechts wanneer de volgende eerste vereisten worden vervuld:
>
>* Uw organisatie heeft een Workfront Planning Prime- of Ultimate-pakket aangeschaft.
>* U bent systeembeheerder

U kunt een sjabloonbundel voor meerdere werkruimten gebruiken om met één klik zes werkruimten te maken.

De malplaatjes inbegrepen in de bundel bevatten werkruimten, verslagtypes, verslagen, meningen, en gebieden om u te helpen met uw implementatie van de Planning beginnen.

>[!IMPORTANT]
>
>De namen van werkruimten en records in de bundel zijn voorbeelden en zijn geen weerspiegeling van uw eigen omgeving.
>
>De namen van de recordtypen en -velden kunnen in elke organisatie worden gebruikt als standaard voor implementatie in elke branche, volgens onze aanbeveling.
>

{{step1-to-planning}}

1. Klik **creëren werkruimte**

   Het dialoogvenster Maken wordt weergegeven. U kunt een werkruimte helemaal opnieuw maken of maken met een van de beschikbare sjablonen.

1. Klik **de werkruimteopstelling van het 0&rbrace; Overzicht in het** Begin hier (Geadviseerd) **gebied.**
1. (Facultatief) klik **Voorproef** binnen om het even welke volgende vooraf bepaalde werkruimtesjablonen om het vakje van de Voorproef voor elk malplaatje te openen:

   * 1.Algemene classificaties en taxonomieën

     Het sjabloon Globale classificaties en taxonomieën bevat alle recordtypen en velden die u in uw omgeving aanbeveelt voor een geslaagde implementatie van Workfront-planning.

     U kunt de recordtypen in deze sjabloon later koppelen of importeren in andere werkruimten die u maakt.
   * 2.Fréscopa Global Marketing
   * 3.Fréscopa Social Marketing
   * 4.Fréscopa Media &amp; PR
   * 5.Fréscopa Global Events
   * 6.Fréscopa Executive Company LeaBladzijde

1. Na het openen van het **vakje van de Voorproef** voor elk werkruimtekalplaatje, klik terug naar **creeer werkruimte** doos, of klik de malplaatjes van het Gebruik met inbegrip van in de bundel gebruiken en creeer werkruimten.

   De werkruimten worden gecreeerd en tonen in de **Werkruimten I** op en **Alle werkruimten** lusjes voor de beheerders van het Systeem. Alle gebruikers met een standaardlicentie zien de werkruimten in hun werkruimte nadat een systeembeheerder deze heeft gemaakt en de nieuwe werkruimten met hen heeft gedeeld.

1. Begin met het bewerken van de werkruimten die u hebt gemaakt en voeg recordtypen, records, weergaven en velden toe die relevant zijn voor uw organisatie.

   Voor meer informatie over beste praktijken om Workfront uit te voeren, zie de artikelen in de [&#x200B; beste praktijken van de Planning van Adobe Workfront: de sectie van de artikelindex &#x200B;](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md).

   Voor informatie over het uitgeven van werkruimten, zie [&#x200B; werkruimten &#x200B;](/help/quicksilver/planning/architecture/edit-workspaces.md) uitgeven.



