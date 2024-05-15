---
title: Records beheren in het gedeelte Planning van Adobe Workfront-objecten
description: U kunt de records die zijn verbonden met Adobe Workfront-objecten weergeven in het gedeelte Planning van een Workfront-object, in het linkerdeelvenster.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 9b1b8d8661917946230033b661ca652f5edef734
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

<!--add this to the main TOC and the mini TOC-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--add also Group and Company when they are available-->


# Records beheren in het gedeelte Planning van Adobe Workfront-objecten

{{maestro-important-intro}}

U kunt de records die zijn verbonden met Adobe Workfront-objecten weergeven in het gedeelte Planning van een Workfront-object, in het linkerdeelvenster.

Het gedeelte Planning is beschikbaar voor de volgende Workfront-objecten:

* Project
* Portfolio
* Programma
<!--* Group
* Company-->

## Toegangsvereisten

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-overeenkomst</p></td>
   <td>
<p>Uw organisatie moet zijn ingeschreven voor het bètaprogramma Adobe Workfront Planning. Neem contact op met uw accountvertegenwoordiger voor meer informatie over dit nieuwe aanbod. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-plan</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td>
   <td>
   <p>Nieuw: Standaard</p>
   of
   <p>Huidig: Plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td>
   <td> <p>De mening of hogere toegang tot Projecten, Programma's, en Portfolio's</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Machtigingen</p></td>
   <td> <p>In Workfront kunt u de machtiging Weergeven of hoger voor een project, portfolio of programma</a> </p> 
   <p>In Workfront Planning, Mening of hoger toestemmingen aan een werkruimte</a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten voor Workfront Planning, inclusief de werkruimten die ze niet hebben gemaakt</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Uw Workfront of groepsbeheerder moet het gebied van de Planning in het Belangrijkste Menu en de sectie van de Planning in het linkerpaneel aan uw lay-outmalplaatje toevoegen. Zie voor meer informatie <a href="../access/access-overview.md">Overzicht van toegang</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Overwegingen over de sectie Planning van Workfront-objecten

* Eerst moet u recordtypen verbinden met Workfront-objecttypen en records met Workfront-objecten om deze in Workfront te kunnen bekijken.

  Raadpleeg de volgende artikelen voor meer informatie:

   * [Verbind recordtypen](/help/quicksilver/maestro/architecture/connect-record-types.md)
   * [Connect-records](/help/quicksilver/maestro/records/connect-records.md)
* U kunt de sectie Planning weergeven in een Workfront-object, zelfs als er geen records zijn gekoppeld aan het Workfront-object.
* U kunt de verslagen van de Planning met de voorwerpen van Workfront van Workfront, in de sectie van de Planning verbinden.

## Records beheren in de sectie Planning

{{step1-to-maestro}}

De laatst geopende werkruimte wordt standaard geopend.

1. Klik op de kaart van een recordtype die is verbonden met een Workfront-project, -portfolio of -programma.
1. Kies een tabelweergave in het menu **Weergave** vervolgkeuzelijst.
1. (Voorwaardelijk) Ga naar het verbonden verslaggebied in de lijst en voeg een voorwerp van Workfront toe, dan klik de naam van het voorwerp van Workfront in het gebied. Zie voor meer informatie [Connect-records](/help/quicksilver/maestro/records/connect-records.md).
De objectpagina wordt geopend in Workfront Planning.
1. Klikken **Ga naar bron** in de rechterbovenhoek van het scherm.

   De objectpagina wordt geopend in Workfront.
1. Klikken **Planning** in het linkerdeelvenster.

   >[!NOTE]
   >
   >   Uw Workfront of groepsbeheerder moet de sectie Planning toevoegen aan uw lay-outmalplaatje alvorens het voor een project, een portefeuille, of een programma van de Wereld toont.

   Het gedeelte Planning wordt weergegeven met de volgende informatie:

   * De verbonden verslagen tonen op individuele kaarten die de volgende informatie bevatten:
      * Naam van de record
      * De recordminiatuur
      * De naam van het verbonden verslaggebied zoals het in de Planning van Workfront toont.
   * Records worden weergegeven in hun respectievelijke werkruimte.

   ![](assets/planning-section-on-project.png)

1. Klik op een opnamekaart voor meer informatie over de record. Het voorvertoningsvak voor records wordt weergegeven.
1. (Optioneel) Wijzig de velden in het voorvertoningsvak van de record. Uw wijzigingen worden automatisch opgeslagen.
1. (Optioneel) Klik op de knop **Openen in een nieuw tabblad** pictogram ![](assets/open-details-in-a-new-tab-icon.png) in de rechterbovenhoek van het voorvertoningsvak om de detailpagina van de record te openen.
1. Houd de muisaanwijzer boven een opnamekaart en klik vervolgens op het pictogram voor het verbreken van de verbinding **-** en klik vervolgens op **Verbinding verbreken**.
De volgende dingen doen zich voor:
   * De record is niet meer verbonden met het Workfront-object.
   * Het Workfront-object wordt ook verwijderd uit het verbonden veld van de record uit Workfront Planning.
   * De waarden voor de Workfront-velden die zijn verbonden met de planningsrecord, worden ook verwijderd.
1. Klikken **Verbinden** om meer records te verbinden.

   <!--checking with the team on the below note - not sure if if should stay Manage or be changed to Contribute??-->

   >[!NOTE]
   >
   >   De knop Verbinden wordt alleen weergegeven voor de werkruimten waarin u beheermachtigingen hebt.

1. Klik op de records waarmee u verbinding wilt maken. De volgende dingen doen zich voor:

   * De records zijn direct verbonden met het Workfront-object en worden weergegeven in het gedeelte Planning.
   * Het Workfront-object wordt toegevoegd aan het veld voor het maken van een verbinding in het Workfront-planningsrecord.
   * De waarden voor de Workfront-velden die zijn verbonden met de planningsrecord, worden ingevuld in Workfront Planning.

<!--add more steps here for what happens after clicking Connect-->


