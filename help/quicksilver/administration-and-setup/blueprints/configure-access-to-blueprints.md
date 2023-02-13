---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Toegang tot blauwdrukken configureren
description: Als systeembeheerder, kunt u toegang voor gebruikers toelaten om installatie van blauwdrukken te verzoeken door opstelling een verzoekrij om de verzoeken op te slaan. Hier hebt u één locatie om aanvragen bij te houden en bij te werken.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Toegang tot blauwdrukken configureren

Alles [!DNL Adobe Workfront] gebruikers kunnen door de catalogus met blauwdrukken bladeren.

Als systeembeheerder kunt u:

* Toevoegen [!UICONTROL Blueprints] aan het hoofdmenu in lay-outmalplaatjes en wijs het lay-outmalplaatje aan gebruikers of groepen toe. Zie voor meer informatie [De [!UICONTROL Main Menu] een lay-outsjabloon gebruiken](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) en [Gebruikers toewijzen aan een lay-outsjabloon](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   >[!NOTE]
   >
   >* Gebruikers waaraan geen lay-outsjabloon is toegewezen, zien de [!UICONTROL Blueprints] in het deelvenster [!UICONTROL Main Menu].
   >* Als u een nieuwe lay-outsjabloon maakt, kunt u [!UICONTROL Blueprints] is opgenomen in het dialoogvenster [!UICONTROL Active Items] lijst voor de [!UICONTROL Main Menu] standaard.



* Laat toegang voor gebruikers toe om installatie van blauwdrukken te verzoeken door opstelling een verzoekrij om de verzoeken op te slaan. Hier hebt u één locatie om aanvragen bij te houden en bij te werken. Volg onderstaande procedure voor meer informatie.
* Installeer blauwdrukken. Zie voor meer informatie [Een blauwdruk installeren](../../administration-and-setup/blueprints/blueprints-install.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p> Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licentie</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau</strong></td> 
   <td> <p>[!UICONTROL System Administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Vereisten {#prerequisites}

* U moet een bestaande verzoekrij gebruiken om blauwdrukverzoeken op te slaan. Het project moet als verzoekrij worden bewaard en het moet binnen zijn [!UICONTROL Current] status.
* De verzoekrij moet openbaar zijn. In de details van de verzoekrij, &quot;[!UICONTROL Who can add requests to this queue?]&quot; moet worden ingesteld op **[!UICONTROL Anyone]**.

>[!TIP]
>
>Als u een nieuwe verzoekrij voor blauwdrukverzoeken wilt tot stand brengen, zou u het moeten bouwen alvorens de toegang van blauwdrukken te vormen. Voor informatie over het creëren van een verzoekrij, zie [Een aanvraagwachtrij maken](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Selecteer de aanvraagwachtrij om verzoeken voor afdrukken op te slaan

Voordat gebruikers kunnen aanvragen dat ze blauwdrukken installeren, moet u een aanvraagwachtrij voor deze aanvragen selecteren. Totdat de aanvraagwachtrij is gedefinieerd, kunnen gebruikers alleen door de blauwdrukcatalogus bladeren.

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Blueprints]**.
1. Klikken **[!UICONTROL Configure blueprint requests]** rechtsboven in het catalogusscherm.

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. Op de **[!UICONTROL Configure blueprints]** typt u de naam van een actieve wachtrij en selecteert u deze wanneer deze in de zoekresultaten wordt weergegeven.

   >[!IMPORTANT]
   >
   >Alleen openbare aanvraagrijen worden in deze lijst weergegeven. Om uw verzoekrij openbaar te maken, zie [Vereisten](#prerequisites) hierboven.

   De voorkeur van de verzoekrij wordt geplaatst, en de gebruikers kunnen nu om blauwdrukinstallatie verzoeken.

   ![Aanvraagwachtrij configureren](assets/Blueprints_access_setup_request_queue.png)

1. (Optioneel) Klik op **[!UICONTROL Edit this request queue]**.

   Het project van de verzoekrij opent in een nieuw browser lusje en u kunt het bijwerken zoals nodig.

1. (Facultatief) als de verzoekrij onderwerpgroepen of rijonderwerpen bevat, kunt u hen van de lijst selecteren.
1. Klik op **[!UICONTROL Close]**.

>[!NOTE]
>
>Wanneer u een gewenste blauwdruk installeert, moet u de status van de uitgave wijzigen in **[!UICONTROL Closed]** of **[!UICONTROL Resolved]** in de aanvraagwachtrij zodat de aanvrager op de hoogte wordt gesteld. Voor informatie over het installeren van een blauwdruk raadpleegt u [Een blauwdruk installeren](../../administration-and-setup/blueprints/blueprints-install.md).
