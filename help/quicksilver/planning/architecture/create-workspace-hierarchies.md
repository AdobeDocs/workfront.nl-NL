---
title: Workspace-hiërarchieën maken
description: Als werkruimtemanager kunt u meerdere werkruimtemhiërarchieën maken tussen de recordtypen in Adobe Workfront Planning. Nadat u recordtypes in een werkruimte verbindt en een hiërarchie creeert, worden de verslagtypes verbonden met elkaar, met één verslagtype dat als ouder en tot 3 andere verslagtypes wordt aangewezen die als kinderen worden gevormd.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 34921b12ad902ba7390e4ea34825331280e7a8d6
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---


# Hiërarchieën voor werkruimten maken

<span class="preview"> de informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [&#x200B; snelle versies voor uw organisatie &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

Als werkruimtemanager kunt u veelvoudige werkruimtehiërarchieën tussen verslagtypes in de Planning van Adobe Workfront tot stand brengen.

Nadat recordtypen in een werkruimte zijn verbonden, kunt u een hiërarchie maken die deze verbindingen ordent. In hiërarchieën worden record- en objecttypen geordend in relatie bovenliggend-onderliggend en kunnen maximaal vier niveaus van objecttypen worden opgenomen.

Als er nog geen verbinding tussen twee recordtypen bestaat, kan deze worden gemaakt terwijl u de hiërarchie instelt. Zodra bepaald, vestigt de hiërarchie een gestructureerd weg over verwante verslagtypes binnen de werkruimte.

De hiërarchie produceert broodkruimels voor hun respectieve verslagen die in hun kopballen tonen. Op deze manier weten gebruikers waar ze zich in de hiërarchie bevinden in elk stadium van hun workflow.

Voor algemene informatie over hiërarchieën en broodkruimels, zie [&#x200B; Hiërarchie en breadcrumb overzicht &#x200B;](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Toegangsvereisten

+++ Breid uit om de toegangsvereisten te bekijken om de stappen in dit artikel uit te voeren:  

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
<ul> 
<li><p>Alle Workfront en alle planningspakketten</p></li>
of
<li><p>Willekeurige workflow en planningspakket</p></li></ul>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
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

## Een werkruimtehiërarchie maken

U kunt maximaal vijf hiërarchieën maken in één werkruimte.

{#step1-to-planning}

1. Klik op een werkruimtekaart.
1. Klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png) rechts van de werkruimtenaam, dan klik **Montages**.
De **sectie van Hiërarchieën** opent door gebrek.
1. Klik **Nieuwe hiërarchie** in de hoger-juiste hoek van de **pagina van Hiërarchieën**.
1. Klik **toevoegen voorwerp** en selecteer een objecten type van het dropdown menu. Dit wordt het eerste objecttype in uw hiërarchie. <!--logged bug to correct to "Add object type"-->

   Het eerste objecttype kan alleen een Planningsrecordtype zijn.

   Workfront-projecten kunnen niet worden geselecteerd als bovenliggende items van andere objecttypen in een hiërarchie.

1. Klik **toevoegen voorwerp** om een tweede objecten type toe te voegen dat het eerste kind in uw hiërarchie is, dan een ander objecten type in het dropdown menu selecteren.
Elke extra objecttype wordt een onderliggend object van de vorige objecttypen.

   ![&#x200B; Nieuwe hiërarchiedoos zonder gebied selecteerde &#x200B;](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)

1. Klik **Uitgezochte verbonden gebied** om erop te wijzen welk gebied de twee voorwerpen verbindt.
1. (Voorwaardelijk) Als er meerdere verbindingsvelden zijn, selecteert u een veld in de lijst.

   of

   Klik **toevoegen nieuwe verbinding** om een nieuw verbindingsgebied toe te voegen.

   Hiermee maakt u een verbindingsveld van het recordtype dat u als bovenliggend element gebruikt en een overeenkomstig verbindingsveld van het recordtype dat u als onderliggend element gebruikt.

   Als u een verbinding met Workfront-projecten maakt, wordt er geen veld voor het project gemaakt.

1. (Voorwaardelijk) als er geen verbonden beschikbare gebieden zijn, klik **creeer verbinding** en voeg een nieuwe verbinding toe, dan klik **sparen**.

1. (Voorwaardelijk) Als u een nieuwe verbinding toevoegt, doe het volgende:

   1. Voeg een naam voor uw verbonden gebied in de **doos van de Naam** toe.
   1. Selecteer een van de volgende verbindingstypen:

      * **Velen aan velen**
      * **Één aan vele**
      * **Velen aan één**
      * **Één aan één**

   1. Selecteer een van de volgende typen opnamen:

      * **Naam en beeld**
      * **Naam**
      * **Beeld**

      Voor meer informatie, zie [&#x200B; Connect verslagtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md).

   1. Klik **sparen**.

1. (Voorwaardelijk) als **creeer het overeenkomstige gebied op verbonden verslagtype** niet werd geselecteerd toen het verbonden gebied werd gecreeerd, krijgt u een fout en moet het volgende eerst doen: <!--check back on these steps; this is supposed to be seamless, but now you have to abandon creating a hierarchy to do this-->

   1. Klik **annuleren** in de **Nieuwe hiërarchie** doos.
   1. Klik op de pijl Vorige links van de naam van de werkruimte en klik vervolgens op de kaart van het recordtype dat u als bovenliggend element wilt kiezen.
   1. Open de lijstmening van het verslagtype u in de stap hierboven selecteerde, dan ga naar het verbindingsgebied met het objecten type u als kind wilt gebruiken, over de kolomkopbal, dan klik **uitgeven** gebied.
   1. Zet **aan creeer het corresponderende gebied op verbonden verslagtype** plaatsen, dan klik **sparen**.
   1. Terugkeer aan het gebied van de Montages van de werkruimte **&#x200B;**&#x200B;en klik **Nieuwe hiërarchie** opnieuw, dan volg de stappen om een hiërarchie tot stand te brengen.

1. (Optioneel) Voeg na de bovenstaande stappen maximaal vier objecttypen toe aan uw hiërarchieën. U kunt eerst alle objecttypen toevoegen en vervolgens de verbindingsvelden tussen de objecttypen toevoegen.
1. (Facultatief) klik **verwijder** pictogram ![&#x200B; verwijderen pictogram &#x200B;](assets/minus-icon.png) om een verbinding te verwijderen.
1. Klik **sparen** om uw hiërarchie te bewaren.

   >[!TIP]
   >
   >**sparen** knoop wordt gedimd als u niet alle verbonden gebieden op zijn plaats hebt.

   De volgende dingen doen zich voor:

   * De hiërarchie wordt toegevoegd aan de **sectie van Hiërarchieën** van de werkruimte.
   * De verslagen die de verbindingsgebieden bevolken tonen alle verbindingen in hun broodkruimels, wanneer u naar de pagina van een verslag gaat.

   >[!NOTE]
   >
   >U kunt één record van een onderliggend recordtype verbinden met maximaal 10 records van een bovenliggend recordtype.
   >
   >Voor meer informatie, zie [&#x200B; Hiërarchie en breadcrumb overzicht &#x200B;](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

1. (Optioneel) Houd de muis boven een hiërarchie en klik vervolgens op het menu **Meer** .

   ![&#x200B; Hiërarchie Meer uitgevouwen menu &#x200B;](assets/hierarchy-more-menu-expanded.png)

1. Klik op een van de volgende opties:

   * **geeft** uit: Dit opent **uitgeeft hiërarchie** doos waar u veranderingen kunt aanbrengen.
   * **Schrapping**: Dit schrapt permanent de hiërarchie. Verwijderde hiërarchieën kunnen niet worden hersteld. Verbindingsvelden worden niet verwijderd.





