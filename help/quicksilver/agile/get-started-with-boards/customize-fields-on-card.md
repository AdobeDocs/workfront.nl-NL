---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Aanpassen welke velden worden weergegeven op een kaart
description: U kunt aanpassen welke velden op een kaart worden weergegeven door een veld uit te schakelen zodat het niet wordt weergegeven op de volledige kaart of in de verkorte weergave, of door een veld te verbergen in de weergave van de verkorte kaart.
author: Lisa
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: 0beb96dc3869e6f913d87f699aa9a51c5aaa8f79
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Aanpassen welke velden worden weergegeven op een kaart

Standaard worden alle beschikbare velden op een kaart weergegeven, zowel in de volledige weergave wanneer de kaart is geopend als in de weergave Versmalde kaart op het bord. U kunt aanpassen welke velden worden weergegeven door:

* Een veld uitschakelen zodat het niet wordt weergegeven in een van beide weergaven
* Een veld verbergen in de weergave Versmalde kaart

Als een veld een waarde bevat en u het veld uitschakelt, blijft de waarde behouden als u het veld later weer inschakelt.

Secties (die worden weergegeven als de linkernavigatieopties op de kaartdetails) zijn ook beschikbaar voor weergave en verbergen.

U kunt ook aangepaste velden weergeven die eerder zijn gemaakt. U kunt geen nieuwe aangepaste velden in een board ontwerpen en maken.

>[!NOTE]
>
>Aanpassingen in velden die u aanbrengt, zijn alleen van toepassing op de kaart waarin u werkt.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Request] of hoger</p> </td> 
  </tr>
   </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Kaarten configureren {#configure-cards}

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Boards]**.
1. Toegang tot een bord. Zie voor meer informatie [Een board maken of bewerken](../../agile/get-started-with-boards/create-edit-board.md).
1. Klikken [!UICONTROL **Configureren**] rechts van de board om het Configure paneel te openen.
1. Uitbreiden [!UICONTROL **Kaarten**].

   De meeste velden en secties zijn standaard ingeschakeld.

1. Schakel een veld of sectie uit om het in beide kaartweergaven uit te schakelen.
1. Klik op het pictogram Verbergen ![Pictogram verbergen](assets/eye-hide-icon.png) naast een veld of sectie om deze in de versmalde weergave te verbergen.
1. Klik op [!UICONTROL **Standaardwaarden van alle velden herstellen**].
1. Klikken [!UICONTROL **Configureren verbergen**] om het Configure paneel te sluiten.

## Aangepaste velden toevoegen aan kaarten

Aangepaste velden zijn beschikbaar op verbonden kaarten. Ze zijn alleen zichtbaar in de volledige kaartweergave, niet in de versmalde weergave op het bord.

>[!NOTE]
>
>Wanneer u een aangepast veld aan uw kaarten toevoegt, zijn de gegevens op de kaart alleen-lezen.

1. Een board openen en klikken [!UICONTROL **Configureren**] om het Configure paneel te openen.
1. Uitbreiden [!UICONTROL **Kaarten**].
1. Onder [!UICONTROL Card Fields], klikt u op [!UICONTROL **Aangepast veld toevoegen**].
1. Selecteren [!UICONTROL **Taak**] of [!UICONTROL **Probleem**].

   De categorieën van beschikbare gebieden voor taken of kwesties verschijnen. Vouw een categorie uit om alle velden weer te geven. U kunt ook naar een veld zoeken.

   ![Zoeken naar aangepast veld](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >De volgende veldtypen kunnen niet aan kaarten worden toegevoegd: Adobe XD, Image, PDF, Video.

1. Selecteer de veldnaam.
1. (Optioneel) Klik in het dialoogvenster **[!UICONTROL Field value]** om dit aangepaste veld te wijzigen in een ander veld.
1. (Optioneel) Wijzig de instelling **[!UICONTROL Field label]** aan de veldnaam die u op kaarten wilt weergeven.
1. Als u alle gewenste wijzigingen hebt aangebracht, klikt u op [!UICONTROL **Veld opslaan**].

   ![Waarde en label van aangepast veld](assets/save-custom-field-value-label.png)

   Het aangepaste veld wordt toegevoegd aan de lijst met beschikbare velden en is standaard ingeschakeld. U kunt het aangepaste veld uitschakelen in het kader van de stappen in het dialoogvenster [Kaarten configureren](customize-fields-on-card.md#configure-cards) van alle kaarten te verwijderen.

>[!NOTE]
>
>Als u het aangepaste veld later in Workfront een andere naam geeft, moet u het veldlabel in het deelvenster Configureren bewerken, anders wordt het veld niet op de kaarten weergegeven.
