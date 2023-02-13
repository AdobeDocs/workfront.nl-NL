---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: De knop Aan de werkbalk vervangen door de knop Start
description: De standaardconfiguratie van Adobe Workfront omvat het Werk aan het knoop voor taken en kwesties die voor punten tonen die u aan bent toegewezen.
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# Vervang de [!UICONTROL Work On It] met een [!UICONTROL Start] knop

[!DNL Adobe Workfront]De standaardconfiguratie van [!UICONTROL Work On It] knop voor taken en problemen die worden weergegeven voor items waaraan u bent toegewezen. Wanneer u op [!UICONTROL Work On It] op punten die aan u worden toegewezen, geeft u aan andere gebruikers aan dat u het werk hebt ontvangen en bevestigt dat u aan het zult werken. De [!DNL Work On It] de knoop werkt niet de taak of uitgeverstatus bij om te signaleren dat het werk eigenlijk is begonnen.

U kunt de [!DNL Work On It] met een [!UICONTROL Start] voor een team u tot behoort. In dit geval klikt u op de knop [!UICONTROL Start] in plaats van [!UICONTROL Work On It], die automatisch de status en de [!UICONTROL Actual Start Date] van het het werkpunt, signalerend dat u begon te werken. Voor informatie over het plaatsen van welk team uw veranderingen in zou kunnen beïnvloeden [!UICONTROL Work On It] knop, zie de sectie [Configureer de [!UICONTROL Start] knop](#configure-the-uicontrol-start-button) in dit artikel.

>[!IMPORTANT]
>
>Klik op de knop [!UICONTROL Start] wijzigt de status van het item en [!UICONTROL Actual Start Date]. Als iemand anders aan een taak of kwestie (die de status in [!UICONTROL In Progress] en de [!UICONTROL Actual Start Date]), wordt de knop voor het item weergegeven als [!UICONTROL Work On It] zelfs wanneer een team u tot behoort heeft de knoop vervangen met een [!UICONTROL Start] knop.

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
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Configureer de [!UICONTROL Start] knop

Als u een [!UICONTROL Plan] licentie, kunt u de [!UICONTROL Start] voor een team in het [!UICONTROL Edit] teamvenster. Hieronder wordt beschreven hoe de knop werkt nadat deze is ingeschakeld voor een team:

* **Het team wordt toegewezen aan een werkitem**: Als een team aan het het werkpunt wordt toegewezen, zien de leden op dat team het [!UICONTROL Start] en de statussen die voor dat team worden geconfigureerd.
* **De gebruiker behoort tot een Home Team**: Als geen team aan het het werkpunt maar de gebruiker wordt toegewezen aan een Team van het Huis in hun profiel wordt toegewezen, dan ziet de gebruiker [!UICONTROL Start] en de statussen die voor dat team worden geconfigureerd. Dit is het scenario wij adviseren als u gebruikers wilt gebruiken [!UICONTROL Start] vaak.
* **De gebruiker wordt toegewezen aan een werkitem**: Als er geen team aan het het werkpunt wordt toegewezen en geen Team van het Huis dat aan de gebruiker wordt toegewezen maar de gebruiker wordt toegewezen aan het het werkpunt, dan ziet de gebruiker het [!UICONTROL Start] knoop en de gecombineerde statussen die voor dat alle teams worden gevormd zij worden toegewezen aan.
* **De gebruiker wordt niet toegewezen aan om het even welke teams:** Als er geen team aan het het werkpunt en geen team voor de gebruiker, met inbegrip van het Team van het Huis wordt toegewezen, en het punt wordt toegewezen aan de gebruiker, dan lijkt de gebruiker [!UICONTROL Work On It] knop.

>[!NOTE]
>
>Deze functie is momenteel niet beschikbaar in
>
>* De [!DNL Workfront] mobiele app
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] e-mailberichten
>


De knop Start configureren:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **[!UICONTROL Teams]**.

1. In de **[!UICONTROL Teams]** selecteert u een team.\
   of\
   Klik op **[!UICONTROL Create Team]**.

1. Klik op de knop **[!UICONTROL More]** pictogram ![](assets/more-icon.png)en klik vervolgens op **[!UICONTROL Edit]**.

1. Zoek de **[!UICONTROL Work On It]** knopsectie bij de onderkant van de [!UICONTROL Edit Teams] pagina.
1. Selecteer **[!UICONTROL Change the Work On It button to a Start button to automatically update the status of an item]** selectievakje.
1. Selecteer een of meer statussen voor elk type werkitem. Als u meerdere statussen selecteert, wordt een vervolgkeuzemenu weergegeven wanneer u op [!UICONTROL Start] waar u de gewenste status kunt kiezen.
1. Klik op **[!UICONTROL Save changes]**. Gebruikers zien nu een [!UICONTROL Start Task] of [!UICONTROL Start Issue] in plaats van de [!UICONTROL Work On It] als aan hen een tijdelijk onderdeel is toegewezen.

   >[!NOTE]
   >
   >Wij adviseren plaatsend het team als Team van het Huis van de gebruiker zodat verschijnt de beginknoop op elk van hun toegewezen het werkpunten. Zie [Gebruikers koppelen aan een Home Team](#associate-users-with-a-home-team) hieronder.

## Gebruikers koppelen aan een Home Team

Om gebruikers met een Team van het Huis te associëren:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront].

1. Klikken **[!UICONTROL Users]** en selecteert u vervolgens de gebruiker of gebruikers die u aan een Home Team wilt koppelen.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **[!UICONTROL Edit]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. In de **[!UICONTROL Organization]** selecteert u de **[!UICONTROL Home Team]** veld. Begin de naam van het team te typen waarvan montages u met de gebruikers wilt associëren. Klik op de naam van het team wanneer deze wordt weergegeven in de lijst.

1. Klik op **[!UICONTROL Save Changes]**.\
   De gebruikers u selecteerde worden nu geassocieerd met een Team van het Huis.

   Om het even welke teammontages, met inbegrip van de statussen verbonden aan [!UICONTROL Done] deze gebruikers kunnen de knop nu zien.

