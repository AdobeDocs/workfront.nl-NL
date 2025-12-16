---
title: Workspace-hiërarchieën maken
description: Als werkruimtemanager kunt u meerdere werkruimtemhiërarchieën maken tussen de recordtypen in Adobe Workfront Planning. Nadat u recordtypes in een werkruimte verbindt en een hiërarchie creeert, worden de verslagtypes verbonden met elkaar, met één verslagtype dat als ouder en tot 6 andere verslagtypes wordt aangewezen die als kinderen worden gevormd.
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 6aba4316228a320cf33e419249a64b3cf56e8f39
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Create Workspace Hierarchies
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---

-->

# Hiërarchieën voor werkruimten maken

Als werkruimtemanager kunt u meerdere werkruimtemhiërarchieën maken tussen de recordtypen in Adobe Workfront Planning.


Nadat recordtypen in een werkruimte zijn verbonden, kunt u een hiërarchie maken die deze verbindingen ordent. De hiërarchie organiseert verslagtypes in ouder-kind verhoudingen en kan tot vier niveaus van objecten types bevatten.

Als er nog geen verbinding tussen twee recordtypen bestaat, kan deze worden gemaakt terwijl u de hiërarchie instelt. Zodra bepaald, vestigt de hiërarchie een gestructureerd weg over verwante verslagtypes binnen de werkruimte.

Hierarchieën genereren broodkruimels voor de recordtypen en records <!--ensure this is the case: does the breadcrumb show for both the RT and the record??--> die in de koppen worden weergegeven. Op deze manier weten gebruikers waar ze zich in de hiërarchie bevinden in elk stadium van hun workflow.

Voor algemene informatie over hiërarchieën en broodkruimels, zie [&#x200B; Hiërarchie en breadcrumb overzicht &#x200B;](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Toegangsvereisten

<!--check the access to see if you oversimplified???-->

<!--Update the TOC for this to publish-->

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

{#step1-to-planning}

1. Klik op een werkruimtekaart.
1. Klik **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-menu.png) rechts van de werkruimtenaam, dan klik **Montages**.
De **sectie van Hiërarchieën** opent door gebrek.
1. Klik **Nieuwe hiërarchie** in de hoger-juiste hoek van de **pagina van Hiërarchieën**.
1. Klik **toevoegen voorwerp** en selecteer een voorwerp van het dropdown menu. Dit wordt het eerste bovenliggende object in uw hiërarchie.
De eerste ouder kan slechts een het verslagtype van de Planning zijn. Workfront-projecten kunnen niet worden geselecteerd als bovenliggende items van andere objecttypen in een hiërarchie.
1. Klik **toevoegen voorwerp** om een tweede voorwerp toe te voegen dat het eerste kind in uw hiërarchie is, dan een ander voorwerp in het dropdown menu selecteren.
   ![&#x200B; Nieuwe hiërarchiedoos zonder gebied selecteerde &#x200B;](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)
1. Klik **Uitgezochte verbonden gebied** om erop te wijzen welk gebied de twee voorwerpen verbindt.
1. (Voorwaardelijk) Als een verbonden gebied tussen de twee objecten types bestaat, selecteer het van de lijst. Anders, klik **toevoegen nieuwe verbinding**.

   >[!WARNING]
   >
   >Als **creeer corresponderend gebied op verbonden verslagtype** niet werd geselecteerd toen het verbonden gebied werd gecreeerd, moet u het gebied eerst uitgeven alvorens u kunt verdergaan.

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
1. (Optioneel) Voeg na de bovenstaande stappen maximaal vier objecttypen toe aan uw hiërarchieën. U kunt eerst alle objecttypen toevoegen en vervolgens de verbindingsvelden tussen de objecttypen toevoegen.
1. (Facultatief) klik **verwijder** pictogram ![&#x200B; verwijderen pictogram &#x200B;](assets/minus-icon.png) om een verbinding te verwijderen.
1. Klik **sparen** om uw hiërarchie te bewaren.

   >[!TIP]
   >
   >**sparen** knoop wordt gedimd als u niet alle verbonden gebieden op zijn plaats hebt.

   De volgende dingen doen zich voor:

   * De hiërarchie wordt toegevoegd aan de **sectie van Hiërarchieën** van de werkruimte.
   * De verslagen die de verbindingsgebieden bevolken tonen alle verbindingen in hun broodkruimels, wanneer u naar de pagina van een verslag gaat.
1. (Facultatief) Beweeg over een hiërarchie, dan klik **Meer** menu, dan klik één van het volgende:

   * **geeft** uit: Dit opent **uitgeeft hiërarchie** doos waar u veranderingen kunt aanbrengen.
   * **Schrapping**: Dit schrapt permanent de hiërarchie. Verwijderde hiërarchieën kunnen niet worden hersteld. Verbindingsvelden worden niet verwijderd.





