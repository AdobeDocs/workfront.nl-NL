---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Leden toevoegen aan of verwijderen uit een raad
description: Mensen moeten als leden aan de raad van bestuur worden toegevoegd voordat ze de raad kunnen bekijken en aan kaarten kunnen worden toegewezen.
author: Lisa
feature: Agile
exl-id: 8a46846c-f9b8-45cb-9923-e7596854557b
source-git-commit: bf8d566ba9d24310e75d2fbaf523fe5464bb6657
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Leden toevoegen aan of verwijderen uit een board

{{highlighted-preview}}

Personen en teams moeten als leden aan de raad van bestuur worden toegevoegd voordat ze de raad kunnen bekijken.

De maker van een bord is standaard de eigenaar. De eigenaar van het board is de enige persoon die dat bord kan verwijderen of zijn filters in het Configure paneel kan bijwerken. <span class="preview"> slechts kan een systeembeheerder of de huidige boseigenaar de boardeigenaar veranderen.</span>

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> 
   <p>Nieuw: [!UICONTROL Contributor] of hoger</p> 
   <p>of</p>
   <p>Huidig: [!UICONTROL Request] of hoger</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Leden aan een board toevoegen

{{step1-to-boards}}

1. Maak een nieuw bord of bewerk een bestaand bord. Voor informatie, zie [ creeer of geef een raad ](../../agile/get-started-with-boards/create-edit-board.md) uit.
1. Klik het **[!UICONTROL Add member]** pictogram ![ toevoegen leden ](assets/boards-addmember-spectrum-25x25.png).
1. Typ in het vak **[!UICONTROL Add members]** een naam en selecteer deze vervolgens wanneer deze in de lijst wordt weergegeven.

   U kunt een individueel lid of een team selecteren. Als u een team kiest, wordt het team zelf toegevoegd aan het board.

   >[!NOTE]
   >
   >Een individuele gebruiker moet de optie **[!UICONTROL View]** of **[!UICONTROL Edit]** in zijn toegangsniveau voor teams hebben geplaatst, of zij zullen niet de raad kunnen bekijken.


   ![ voegt leden aan raad ](assets/boards-add-members.png) toe

## Leden van een board verwijderen

{{step1-to-boards}}

1. Maak een nieuw bord of bewerk een bestaand bord. Voor informatie, zie [ creeer of geef een raad ](../../agile/get-started-with-boards/create-edit-board.md) uit.
1. Klik het **[!UICONTROL Add member]** pictogram ![ toevoegen leden ](assets/boards-addmember-spectrum-25x25.png).
1. Klik in het vak **[!UICONTROL Add members]** op de X naast de naam van een persoon of team om deze van het bord te verwijderen.

   ![ verwijdert lid uit raad ](assets/boards-remove-member-from-board-350x367.png)

   Wanneer u een lid uit een raad verwijdert, worden zij niet verwijderd uit om het even welke kaarten zij worden toegewezen aan. Voor verbonden kaarten worden de toewijzingen ook bijgewerkt op de taak of uitgave van [!DNL Workfront] .

   Leden worden alleen van dit bestuur verwijderd. Ze worden niet verwijderd uit andere raden van bestuur waartoe ze behoren.

   >[!NOTE]
   >
   >U kunt de eigenaar van het bord niet verwijderen.

<div class="preview">

## De eigenaar van het bord wijzigen

>[!NOTE]
>
>Alleen een systeembeheerder of de huidige eigenaar van de kaart kan de eigenaar van de kaart wijzigen. Een bord kan slechts één eigenaar hebben.
>
>De mogelijkheid om van eigenaar te veranderen is beschikbaar op basis-, retrospectieve en Kanban-borden, maar niet op dynamische borden.

1. Toegang tot het bord.
1. Klik het **[!UICONTROL More]** menu ![ Meer menu ](assets/more-icon-spectrum.png) naast de bordnaam, dan kies **[!UICONTROL Change board owner]**.
1. Zoek en selecteer in het dialoogvenster Eigenaar Wijzigen de gebruiker die u de eigenaar wilt maken.

   U kunt niet zoeken naar gebruikers die al lid zijn van de raad. Als u een bestaand lid de eigenaar wilt maken, moet u deze eerst uit de raad verwijderen. Als u van een gebruiker de eigenaar van de kaart maakt, worden deze aan de kaart toegevoegd.

   Alleen een gebruiker kan de eigenaar van het bord zijn. Een team kan geen eigenaar zijn.

1. Klik [!UICONTROL **Update**].

</div>
