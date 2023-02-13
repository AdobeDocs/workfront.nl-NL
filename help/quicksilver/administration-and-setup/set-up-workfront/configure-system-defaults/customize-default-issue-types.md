---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Standaardtypen voor problemen aanpassen
description: U kunt de labels voor elk standaarduitgavetype aanpassen zodat deze beter overeenkomen met de terminologie die in uw organisatie wordt gebruikt. De types van kwestie zijn nuttig om uitgavestatus aan te passen en verzoekrijen te creëren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Standaardtypen voor problemen aanpassen

Typen problemen zijn handig in de volgende omstandigheden:

* Bij het aanpassen van uitgiftestatussen, zoals beschreven in [Een status maken of bewerken](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
* Bij het maken van een aanvraagwachtrij, zoals beschreven in [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

U kunt de labels voor elk standaarduitgavetype aanpassen zodat deze beter overeenkomen met de terminologie die in uw organisatie wordt gebruikt.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Standaardtypen problemen

Als u [!DNL Adobe Workfront] [!UICONTROL administrator] toegang, zijn er vier standaardtypes van kwesties die u kunt vormen en anders noemen:

* **[!UICONTROL Bug Report]** Wordt gebruikt om gemelde fouten in het systeem bij te houden.
* **[!UICONTROL Change Order]** Wordt gebruikt om problemen bij te houden die moeten worden bijgewerkt of herzien.
* **[!UICONTROL Issue]** Een object in [!DNL Workfront] die ongeplande werkzaamheden, een probleem dat zich voordoet of iets dat moet worden opgelost om een taak voort te zetten, aan het licht brengt.
* **[!UICONTROL Request]** Een type kwestie dat op een verzoekrij van toepassing is waar de gebruikers verzoeken in Workfront indienen.

![](assets/default-issue-types.png)

## Een type uitgave aanpassen

Overweeg het volgende over het aanpassen van types van kwesties:

* U kunt het label voor een type uitgave wijzigen, maar u kunt de functie ervan niet wijzigen.
* U kunt geen extra typen uitgaven maken.
* U kunt de filterwaarden voor de naam van een type uitgave niet wijzigen. Als u dus een filter maakt op een issue report, geeft de waarde van het filter (key) niet de aangepaste naam van het type uitgave weer.
* Er zijn drie standaardstatussen gekoppeld aan elk type uitgave: [!UICONTROL New], [!UICONTROL In Progress], en [!UICONTROL Closed]. U kunt deze statussen niet verwijderen of ze uit een type uitgave verwijderen, maar u kunt ze wel een andere naam geven.
* U kunt de volgorde van de opties in het vervolgkeuzemenu voor elk type uitgave wijzigen.

Een type uitgave aanpassen:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik op **[!UICONTROL Project Preferences]** > **[!UICONTROL Statuses]**.

1. Klik op de knop **[!UICONTROL Issues]** tab.
1. Voer een van de volgende handelingen uit:

   * Houd de muisaanwijzer boven het type uitgave dat u wilt aanpassen en klik op de knop [!UICONTROL Edit] pictogram ![](assets/edit-icon.png) helemaal rechts, typt u een nieuwe naam voor het type uitgave.

      ![](assets/customize-issue-type.png)

   * Klik op een [!UICONTROL issue type] om de bijbehorende statussen weer te geven, sleept u de handgrepen die worden weergegeven wanneer u de muisaanwijzer op de statussen plaatst en zet u deze neer in de volgorde waarin u ze wilt weergeven in de gebruikerskwestie **[!UICONTROL Status]** vervolgkeuzemenu.
