---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Een bestaand object bijwerken vanuit een Outlook-e-mail
description: U kunt een bestaand project, een taak, of een kwestie met informatie van een e-mail van Vooruitzichten bijwerken.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 297eb1c4-ee9f-4bb3-a412-18f23c74b0eb
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# Een bestaand object bijwerken via een e-mailbericht van [!DNL Outlook]

>[!IMPORTANT]
>
>[ Microsoft is in het proces om steun voor de online tokens van de erfenisUitwisseling ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) onbruikbaar te maken, die momenteel door de toe:voegen-binnen van Workfront Vooruitzichten voor authentificatie worden gebruikt. Deze verandering door Microsoft is al begonnen met gevolgen voor de klanten en zal tot oktober 2025 in fasen blijven doorlopen.
>
>* **nadat Microsoft volledig deze tokens onbruikbaar maakt, zal Workfront voor de integratie van Microsoft Outlook niet meer functioneren.**
>
>Als onderdeel van deze wijziging heeft Microsoft besloten om de manier te wijzigen waarop tokens opnieuw worden ingeschakeld. Na **Juni 30, 2025**, zullen de beheerders niet meer tokens kunnen re-toelaten zelf-slechts de Steun van Microsoft kan uitzonderingen verlenen. **Op 1 Oktober, 2025, zullen de erfenistokens voor alle huurders worden uitgezet. Er worden geen uitzonderingen toegestaan.**

U kunt een bestaand project, een bestaande taak of een bestaand probleem bijwerken met informatie uit een [!DNL Outlook] -e-mail.

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

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## Vereisten

Uw [!DNL Workfront] beheerder moet [!DNL Outlook for Office] with [!DNL Workfront] inschakelen voordat u deze integratie kunt gebruiken.

## Een bestaand object bijwerken via een e-mailbericht van [!DNL Outlook]

1. Selecteer in [!DNL Outlook] het e-mailbericht dat de gegevens bevat die u in een [!DNL Adobe Workfront update] wilt opnemen.
1. Klik op het pictogram **[!DNL Workfront]** rechtsboven in het e-mailbericht om de invoegtoepassing Workfront weer te geven.\
   Mogelijk moet u op de pijl omlaag in de rechterbovenhoek van uw e-mail klikken om het pictogram [!DNL Workfront] te openen.

1. Klik het **[!UICONTROL Menu]** pictogram ![ o365_addin_menu_icon.png ](assets/o365-addin-menu2-icon.png) om de lijst van beschikbare [!DNL Workfront] opties te tonen.\


1. Klik **[!UICONTROL Update]in Workfront**.\
   U kunt de volgende gegevens uit de e-mail bijwerken voordat u deze als taak opslaat:

   * **[!UICONTROL Type]**: selecteer het type object dat u wilt bijwerken. U kunt **[!UICONTROL Project]**, **[!UICONTROL Task]** of **[!UICONTROL Issue]** selecteren. Het object dat u selecteert, bepaalt de resultaten die in het onderstaande veld **[!UICONTROL Name]** worden weergegeven. Als u niet zeker bent van het type object, selecteert u **[!UICONTROL All]** om te zoeken naar projecten, taken en problemen tegelijk.

   * **[!UICONTROL Name]**: typ de naam van het project, de taak of de uitgave die u wilt bijwerken. Klik op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.
   * **[!UICONTROL Update]**: De update is standaard hetzelfde als de e-mailtekst. U kunt de update naar wens wijzigen.\

     Dit [!UICONTROL update] wordt weergegeven als de updatestatus in Workfront.

   * **[!UICONTROL Attachments]**: alle e-mailbijlagen worden opgeslagen in het gedeelte [!UICONTROL Documents] van de taak. U kunt alle bijlagen verwijderen voordat u de update verzendt.

1. (Optioneel) Klik op **[!UICONTROL Include Others]**, typ de naam van de gebruikers die u in de update wilt opnemen en klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.\
   Herhaal dit proces om extra gebruikers op te nemen en klik vervolgens op **[!UICONTROL Done]** .\
   Standaard ontvangt de gebruiker waarop u antwoordt een melding, ongeacht of u deze opneemt.\

1. (Optioneel) Klik op het pictogram **[!UICONTROL Lock]** om deze update te beperken tot gebruikers binnen uw bedrijf. Wanneer de update is vergrendeld, kunnen gebruikers buiten uw bedrijf de update niet zien.

   * **[!UICONTROL Unlocked]:** Elke gebruiker met toegang tot het project, de taak of het probleem waar de update zich bevindt, kan de update weergeven.\

     De update is standaard ontgrendeld.\
      ![ o365_addin_unlock.png ](assets/o365-addin-unlock.png)

   * **[!UICONTROL Locked]:** alleen gebruikers binnen uw bedrijf kunnen de update weergeven.\

     ![ o365_addin_lock.png ](assets/o365-addin-lock.png)

1. Klik op **[!UICONTROL Update]**.
1. (Optioneel) Klik op **[!UICONTROL View in Workfront]** om het bijgewerkte item weer te geven met de [!DNL Workfront] integratie in [!UICONTROL Outlook] .
