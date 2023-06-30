---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: De knop Gereed configureren voor taken
description: Met de knop Gereed kunt u automatisch de status van een taak of een uitgave instellen. Standaard markeert Adobe Workfront een taak als Voltooid wanneer een toegewezen persoon op Gereed klikt voor het betreffende werkitem.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 62db557f6347004836fac1ea37e55d557dcc6b87
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---

# Configureer de [!UICONTROL Done] knop voor taken

De [!UICONTROL Done] kan de status van een taak of een uitgave automatisch instellen. Standaard, [!UICONTROL Adobe Workfront] markeert een taak als [!UICONTROL Completed] wanneer een ontvanger op hun werkitem klikt.

## Overzicht

Gebruikers met bepaalde machtigingen kunnen de [!UICONTROL Done] om bepaalde statussen in het systeem te weerspiegelen. Er zijn twee verschillende manieren om [!UICONTROL Done] de knop werkt voor taken in [!UICONTROL Workfront]:

* Als de gebruiker een toegewezen Team van het Huis heeft, a [!DNL Workfront] beheerder of een gebruiker met een [!UICONTROL Plan] licentie kan de [!UICONTROL Done] om bepaalde statussen voor teamleden te weerspiegelen. Zie [Configureer de [!UICONTROL Done] knoop voor een Team](#configure-the-uicontrol-done-button-for-a-team) in dit artikel.
* Als de gebruiker geen [!UICONTROL Home Team], maar ze hebben [!UICONTROL Other Teams] in hun profiel, zoekt Workfront naar de instelling van de [!UICONTROL Done] op om het even welke teams verbonden aan de gebruiker. De selectie is willekeurig en de status verbonden aan om het even welke teams wordt gebruikt voor de taak.
* Als de gebruiker geen toegewezen Team van het Huis heeft, [!UICONTROL Done] knop voor taken is gekoppeld aan een volledige status. Er zijn geen configuratieopties beschikbaar in dit scenario. De [!UICONTROL Done] automatisch wordt deze status ingesteld.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] plan*</strong></p></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] licentie*</strong></p></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Configureer de [!UICONTROL Done] knoop voor een Team

U kunt wijzigen welke status op het werkitem is toegepast met de opdracht [!UICONTROL Done] knop. U kunt ook meerdere statussen instellen en de gebruiker de mogelijkheid geven om te kiezen welke status geschikt is.

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **[!UICONTROL Teams]**.

1. Klik op de knop **[!UICONTROL Switch team]** selecteert u vervolgens een nieuw team in het keuzemenu of zoekt u naar een team in de zoekbalk.
1. Klik op de knop **[!UICONTROL More]** en klik vervolgens op **[!UICONTROL Edit]**.
1. Zoek de **[!UICONTROL Done Button]** onderaan in het gedeelte **[!UICONTROL Team Settings]** pagina.

1. Selecteer één status of meer dan één status voor elk type werkitem.

   >[!NOTE]
   >
   >Houd rekening met het volgende wanneer u statussen selecteert voor taken of problemen:
   >
   >* Wanneer u één status selecteert voor elk type werkitem, wordt de taak- of uitgiftestatus ingesteld op die status wanneer een gebruiker klikt [!UICONTROL Done] op hun object. Als u meerdere statussen instelt voor elk type werkitem, wordt een vervolgkeuzemenu toegevoegd aan het dialoogvenster [!UICONTROL Done] en de gebruiker moet een status selecteren om de status van het werkitem te wijzigen.
   >* U kunt alleen statussen op systeemniveau koppelen aan de [!UICONTROL Done] knop. U kunt geen groepsspecifieke statussen koppelen aan de status van het werkitem.
   >* Wanneer een gebruiker die aan het item is toegewezen het item in de status plaatst die aan het [!UICONTROL Done] knop, het item wordt weergegeven als [!UICONTROL Done] voor die gebruiker, ongeacht of de status die u selecteert een [!UICONTROL Completed] of [!UICONTROL Closed] status of een werkstatus.
   >   
   >   
   >  Bijvoorbeeld, associating [!UICONTROL Done] knop met [!UICONTROL In Progress] zorgt ervoor dat het werkitem wordt weergegeven als [!UICONTROL Done] voor de gebruiker die de status wijzigt van [!UICONTROL New] tot [!UICONTROL In progress].
   >   
   >* De types van kwestie zijn aanpasbaar en zij zouden verschillende namen kunnen hebben dan hieronder vermeld in uw milieu.\
   >  Hier volgen de standaardtaken en -typen:
   >     
   >   * [!UICONTROL Tasks]
   >   * [!UICONTROL Issue]
   >   * [!UICONTROL Request]
   >   * [!UICONTROL Change Order]
   >   * [!UICONTROL Bug Report]

   Als de taak of kwestie aan veelvoudige gebruikers wordt toegewezen, ziet u &quot;[!UICONTROL Done with my part]&quot; in het keuzemenu, naast de meerdere statussen die voor uw team zijn gekozen.

1. Klik op **[!UICONTROL Save Changes]**.

## Gebruikers koppelen aan een Home Team

Als u de wijzigingen wilt aanbrengen in het dialoogvenster [!UICONTROL Done] de knoopfunctionaliteit zichtbaar aan gebruikers, kunt u het team maken waarvan montages u het Team van het Huis van de gebruikers veranderde.

Om gebruikers met een Team van het Huis te associëren:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront].

1. Klikken **[!UICONTROL Users]** en selecteert u vervolgens de gebruiker of gebruikers die u aan een Home Team wilt koppelen.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **[!UICONTROL Edit]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. In de **[!UICONTROL Organization]** selecteert u de **[!UICONTROL Home Team]** veld. Begin de naam van het team te typen waarvan montages u met de gebruikers wilt associëren. Klik op de naam van het team wanneer deze wordt weergegeven in de lijst.

1. Klik op **[!UICONTROL Save Changes]**.\
   De gebruikers u selecteerde worden nu geassocieerd met een Team van het Huis.
Om het even welke teammontages, met inbegrip van de statussen verbonden aan [!UICONTROL Done] deze gebruikers kunnen de knop nu zien.
