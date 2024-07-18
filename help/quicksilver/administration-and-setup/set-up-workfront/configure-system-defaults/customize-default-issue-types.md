---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Standaardobjecttypen aanpassen
description: U kunt de labels voor elk standaarduitgavetype aanpassen zodat deze beter overeenkomen met de terminologie die in uw organisatie wordt gebruikt. De types van kwestie zijn nuttig om uitgavestatus aan te passen en verzoekrijen tot stand te brengen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Standaardobjecttypen aanpassen

Typen problemen zijn handig in de volgende omstandigheden:

* Wanneer het aanpassen van uitgiftestatussen, zoals die in [ worden beschreven creeer of geef een status ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) uit.
* Wanneer het creëren van een verzoekrij, zoals die in [ wordt beschreven creeer een Rij van het Verzoek ](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

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
   <td> <p>U moet een [!DNL Workfront] beheerder zijn.</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Standaardtypen problemen

Als u toegang hebt tot [!DNL Adobe Workfront] [!UICONTROL administrator] , zijn er vier standaardtypen voor uitgaven die u kunt configureren en hernoemen:

* **[!UICONTROL Bug Report]** Wordt gebruikt om gerapporteerde fouten in het systeem bij te houden.
* **[!UICONTROL Change Order]** Wordt gebruikt om problemen bij te houden die moeten worden bijgewerkt of herzien.
* **[!UICONTROL Issue]** Een object in [!DNL Workfront] dat ongeplande werkzaamheden communiceert, een probleem dat optreedt of iets dat moet worden opgelost om een taak voort te zetten.
* **[!UICONTROL Request]** Een type uitgave dat van toepassing is op een aanvraagwachtrij waar gebruikers aanvragen indienen in Workfront.

![](assets/default-issue-types.png)

## Een type uitgave aanpassen

Overweeg het volgende over het aanpassen van types van kwesties:

* U kunt het label voor een type uitgave wijzigen, maar u kunt de functie ervan niet wijzigen.
* U kunt geen extra typen uitgaven maken.
* U kunt de filterwaarden voor de naam van een type uitgave niet wijzigen. Als u dus een filter op een uitgiftenrapport maakt, geeft de waarde van het filter (sleutel) niet de aangepaste naam van het type uitgave weer.
* Er zijn drie standaardstatussen gekoppeld aan elk type uitgave: [!UICONTROL New], [!UICONTROL In Progress] en [!UICONTROL Closed] . U kunt deze statussen niet verwijderen of ze uit een type uitgave verwijderen, maar u kunt ze wel een andere naam geven.
* U kunt de volgorde van de opties in het vervolgkeuzemenu voor elk type uitgave wijzigen.

U kunt als volgt een type uitgave aanpassen:

1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in [!DNL Adobe Workfront] en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png) .

1. Klik op **[!UICONTROL Project Preferences]** > **[!UICONTROL Statuses]** .

1. Klik op de tab **[!UICONTROL Issues]** .
1. Voer een van de volgende handelingen uit:

   * Houd de muisaanwijzer boven het type uitgave dat u wilt aanpassen, klik op het [!UICONTROL Edit] pictogram ![](assets/edit-icon.png) dat uiterst rechts wordt weergegeven en typ een nieuwe naam voor het type uitgave.

     ![](assets/customize-issue-type.png)

   * Klik op een [!UICONTROL issue type] om de bijbehorende status weer te geven en sleep vervolgens de grepen die worden weergegeven wanneer u de muisaanwijzer op de status plaatst. Zet deze vervolgens neer in de volgorde waarin u ze wilt weergeven in de vervolgkeuzelijst met uitgaven van uw gebruikers **[!UICONTROL Status]** .
