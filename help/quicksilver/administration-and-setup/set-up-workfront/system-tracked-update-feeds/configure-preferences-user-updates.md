---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Voorkeuren voor gebruikersupdates configureren
description: U kunt voorkeuren configureren die toegang geven tot bepaalde functies wanneer gebruikers opmerkingen toevoegen in het gebied [!UICONTROL Updates] van een object.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Voorkeuren voor gebruikersupdates configureren

U kunt voorkeuren configureren die gebruikers toegang geven tot bepaalde functies wanneer ze opmerkingen toevoegen in het gebied [!UICONTROL Updates] van een object.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td><p>Nieuw: [!UICONTROL Standard]</p>
   of
   <p>Huidige: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td><p>U hebt het toegangsniveau [!UICONTROL System Administrator] nodig om deze stappen op systeemniveau uit te voeren.</p><p>Om hen voor een groep uit te voeren, moet u een manager van die groep zijn.</p></td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gebruikers toestaan afbeeldingen toe te voegen in updates

Standaard kunnen gebruikers geen afbeeldingen in updates toevoegen. Wanneer u deze voorkeur inschakelt, kunnen gebruikers afbeeldingen bijvoegen in updates. De voorkeur geldt voor alle updates in alle gebieden van de [!DNL Workfront] -instantie.

>[!NOTE]
>
>* Afbeeldingen die zijn opgeslagen in updates tellen mee voor de opslaglimiet van het document. Voor informatie, zie [ de grenzen van de documentopslag van de Controle ](../../../documents/managing-documents/check-document-storage.md).
>* Afbeeldingen zijn toegankelijk via het tabblad [!UICONTROL Updates] op een object en zijn ook beschikbaar in het [!UICONTROL Documents] -gebied onder [!UICONTROL Main Menu] .
>

1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in [!DNL Adobe Workfront] en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png) .
1. Selecteer **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]** in het linkerdeelvenster.
1. Selecteer de tab **[!UICONTROL Preferences]** .

   ![ de voorkeur van de Gebruiker voor updatevoer ](assets/updatefeeds-preferences-350x137.png)

1. Schakel het selectievakje **[!UICONTROL Allow users to add images in updates]** in.
1. Selecteer **[!UICONTROL Save]** .

   Wanneer deze voorkeur wordt toegelaten, kunt u het op elk ogenblik onbruikbaar maken. Alle afbeeldingen die al in updates zijn geplaatst, blijven in het [!UICONTROL Updates] -gebied van het object.
