---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Een bestaand object bijwerken vanuit een Outlook-e-mail
description: U kunt een bestaand project, een taak, of een kwestie met informatie van een e-mail van Vooruitzichten bijwerken.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 297eb1c4-ee9f-4bb3-a412-18f23c74b0eb
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Een bestaand object bijwerken vanuit een [!DNL Outlook] email

U kunt een bestaand project, een bestaande taak of een bestaande uitgave bijwerken met informatie van een [!DNL Outlook] e-mail.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Vereisten

Uw [!DNL Workfront] de beheerder moet toelaten [!DNL Outlook for Office] with [!DNL Workfront] voordat u deze integratie kunt gebruiken.

## Een bestaand object bijwerken vanuit een [!DNL Outlook] email

1. In [!DNL Outlook]selecteert u het e-mailbericht met de gegevens die u in een [!DNL Adobe Workfront update].
1. Klik op de knop **[!DNL Workfront]** in de rechterbovenhoek van het e-mailbericht om de invoegtoepassing Workfront weer te geven.\
   Mogelijk moet u op de pijl omlaag in de rechterbovenhoek van uw e-mail klikken om het dialoogvenster [!DNL Workfront] pictogram.

1. Klik op de knop **[!UICONTROL Menu]** pictogram om de lijst met beschikbare [!DNL Workfront] opties.\
   ![o365_addin_menu_icon.png](assets/o365-addin-menu-icon.png)

1. Klikken **[!UICONTROL Update]in Workfront**.\
   ![outlook_Update_in_workfront_menu.png](assets/outlook-update-in-workfront-menu-253x345.png)\
   U kunt de volgende gegevens uit de e-mail bijwerken voordat u deze als taak opslaat:

   * **[!UICONTROL Type]**: Selecteer het type object dat u wilt bijwerken. U kunt **[!UICONTROL Project]**, **[!UICONTROL Task]**, of **[!UICONTROL Issue]**. Het object dat u selecteert, bepaalt de resultaten die worden weergegeven in het dialoogvenster **[!UICONTROL Name]** veld hieronder. Als u niet zeker bent van het type object, selecteert u **[!UICONTROL All]** om projecten, taken, en kwesties gelijktijdig te zoeken.

   * **[!UICONTROL Name]**: Typ de naam van het project, de taak of de uitgave die u wilt bijwerken. Klik op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.
   * **[!UICONTROL Update]**: Standaard is de update hetzelfde als de e-mailtekst. U kunt de update naar wens wijzigen.\

      Dit [!UICONTROL update] wordt weergegeven als de updatestatus in Workfront.

   * **[!UICONTROL Attachments]**: Alle e-mailbijlagen worden opgeslagen in de [!UICONTROL Documents] taakgebied. U kunt alle bijlagen verwijderen voordat u de update verzendt.

1. (Optioneel) Klik op **[!UICONTROL Include Others]** typt u eerst de naam van de gebruikers die u in de update wilt opnemen. Klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.\
   Herhaal dit proces om extra gebruikers op te nemen, en klik dan **[!UICONTROL Done]**.\
   Standaard ontvangt de gebruiker waarop u antwoordt een melding, ongeacht of u deze opneemt.\
   ![o365_addin_include_other.png](assets/o365-addin-includeothers.png)

1. (Optioneel) Klik op de knop **[!UICONTROL Lock]** pictogram om deze update te beperken tot gebruikers binnen uw bedrijf. Wanneer de update is vergrendeld, kunnen gebruikers buiten uw bedrijf de update niet zien.

   * **[!UICONTROL Unlocked]:** Elke gebruiker met toegang tot het project, de taak of het probleem waar de update zich bevindt, kan de update weergeven.\

      De update is standaard ontgrendeld.\
      ![o365_addin_unlock.png](assets/o365-addin-unlock.png)

   * **[!UICONTROL Locked]:** Alleen gebruikers binnen uw bedrijf kunnen de update weergeven.\

      ![o365_addin_lock.png](assets/o365-addin-lock.png)

1. Klik op **[!UICONTROL Update]**.
1. (Optioneel) Klik op **[!UICONTROL View in Workfront]** om het bijgewerkte item weer te geven met de [!DNL Workfront] integratie binnen [!UICONTROL Outlook].
