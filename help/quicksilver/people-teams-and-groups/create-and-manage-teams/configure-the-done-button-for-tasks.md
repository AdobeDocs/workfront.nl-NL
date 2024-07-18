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

# De knop [!UICONTROL Done] voor taken configureren

Met de knop [!UICONTROL Done] kunt u automatisch de status van een taak of een uitgave instellen. Standaard markeert [!UICONTROL Adobe Workfront] een taak als [!UICONTROL Completed] wanneer een toegewezen persoon op Gereed klikt voor het desbetreffende werkitem.

## Overzicht

Gebruikers met bepaalde machtigingen kunnen de knop [!UICONTROL Done] zo configureren dat bepaalde statussen in het systeem worden weerspiegeld. Er zijn twee verschillende manieren waarop de knop [!UICONTROL Done] werkt voor taken in [!UICONTROL Workfront] :

* Als de gebruiker een toegewezen Home Team heeft, kan een [!DNL Workfront] beheerder of een gebruiker met een [!UICONTROL Plan] vergunning de [!UICONTROL Done] knoop vormen om op bepaalde statussen voor teamleden te wijzen. Zie [ de [!UICONTROL Done] knoop voor een Team ](#configure-the-uicontrol-done-button-for-a-team) in dit artikel vormen.
* Als de gebruiker geen [!UICONTROL Home Team] heeft maar [!UICONTROL Other Teams] in zijn profiel, zoekt Workfront naar de instelling van de knop [!UICONTROL Done] in een van de teams die aan de gebruiker zijn gekoppeld. De selectie is willekeurig en de status verbonden aan om het even welke teams wordt gebruikt voor de taak.
* Als aan de gebruiker geen Home Team is toegewezen, is de [!UICONTROL Done] knop voor taken gekoppeld aan een volledige status. Er zijn geen configuratieopties beschikbaar in dit scenario. Deze status wordt automatisch ingesteld op de knop [!UICONTROL Done] .

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

&#42; om te weten te komen welk plan of vergunningstype u hebt, contacteer uw [!DNL Workfront] beheerder.

## De knop [!UICONTROL Done] voor een team configureren

U kunt met de knop [!UICONTROL Done] wijzigen welke status wordt toegepast op het werkitem. U kunt ook meerdere statussen instellen en de gebruiker de mogelijkheid geven om te kiezen welke status geschikt is.

1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in Adobe Workfront en klik vervolgens op **[!UICONTROL Teams]** .

1. Klik op het pictogram **[!UICONTROL Switch team]** en selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.
1. Klik op het menu **[!UICONTROL More]** en klik vervolgens op **[!UICONTROL Edit]** .
1. Zoek de sectie **[!UICONTROL Done Button]** onder aan de pagina van **[!UICONTROL Team Settings]** .

1. Selecteer één status of meer dan één status voor elk type werkitem.

   >[!NOTE]
   >
   >Houd rekening met het volgende wanneer u statussen selecteert voor taken of problemen:
   >
   >* Wanneer u één status voor elk type werkitem selecteert, wordt de taak- of uitgiftestatus ingesteld op die status wanneer een gebruiker op [!UICONTROL Done] op het item klikt. Als u meerdere statussen instelt voor elk type werkitem, wordt een vervolgkeuzemenu toegevoegd aan de knop [!UICONTROL Done] en moet de gebruiker een status kiezen om de status van het werkitem te wijzigen.
   >* U kunt alleen statussen op systeemniveau aan de knop [!UICONTROL Done] koppelen. U kunt geen groepsspecifieke statussen koppelen aan de status van het werkitem.
   >* Wanneer een gebruiker die aan het item is toegewezen het item in de status plaatst die aan de knop [!UICONTROL Done] is gekoppeld, wordt het item weergegeven als [!UICONTROL Done] voor die gebruiker, ongeacht of de status die u selecteert een [!UICONTROL Completed] - of [!UICONTROL Closed] -status of een werkstatus is.
   >   
   >   
   >  Als u bijvoorbeeld de knop [!UICONTROL Done] aan [!UICONTROL In Progress] koppelt, wordt het tijdelijke item weergegeven als [!UICONTROL Done] voor de gebruiker die de status wijzigt van [!UICONTROL New] in [!UICONTROL In progress] .
   >   
   >* De types van kwestie zijn aanpasbaar en zij zouden verschillende namen kunnen hebben dan hieronder vermeld in uw milieu.\
   >  Hier volgen de standaardtaken en -typen:
   >     
   >   * [!UICONTROL Tasks]
   >   * [!UICONTROL Issue]
   >   * [!UICONTROL Request]
   >   * [!UICONTROL Change Order]
   >   * [!UICONTROL Bug Report]

   Als de taak of de kwestie aan veelvoudige gebruikers wordt toegewezen, ziet u een &quot;[!UICONTROL Done with my part]&quot;optie in het drop-down menu, naast de veelvoudige statussen die voor uw team worden gekozen.

1. Klik op **[!UICONTROL Save Changes]**.

## Gebruikers koppelen aan een Home Team

Als u de wijzigingen in de knopfunctionaliteit van [!UICONTROL Done] zichtbaar wilt maken voor gebruikers, kunt u het team maken van wie u de instellingen hebt gewijzigd in het Home Team van de gebruikers.

Om gebruikers met een Team van het Huis te associëren:

1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in [!DNL Adobe Workfront] .

1. Klik op **[!UICONTROL Users]** en selecteer vervolgens de gebruiker of gebruikers die u aan een Home-team wilt koppelen.
1. Klik op het menu **[!UICONTROL More]** en selecteer vervolgens **[!UICONTROL Edit]** .\
   ![](assets/user-settings-nwe-350x291.png)

1. Selecteer in de sectie **[!UICONTROL Organization]** het veld **[!UICONTROL Home Team]** . Begin de naam van het team te typen waarvan montages u met de gebruikers wilt associëren. Klik op de naam van het team wanneer deze wordt weergegeven in de lijst.

1. Klik op **[!UICONTROL Save Changes]**.\
   De gebruikers u selecteerde worden nu geassocieerd met een Team van het Huis.
Alle teaminstellingen, inclusief de statussen die zijn gekoppeld aan de knop [!UICONTROL Done] , zijn nu zichtbaar voor deze gebruikers.
