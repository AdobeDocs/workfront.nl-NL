---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Voorkeuren voor gebruikersupdates configureren
description: U kunt voorkeuren configureren die toegang geven tot bepaalde functies wanneer gebruikers opmerkingen toevoegen in het gebied [!UICONTROL Updates] van een object.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 1%

---

# Voorkeuren voor gebruikersupdates configureren

<!--Audited: 08/2025-->

U kunt voorkeuren configureren die gebruikers toegang geven tot bepaalde functies wanneer ze opmerkingen toevoegen in het gebied [!UICONTROL Updates] van een object.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td><p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td><p>De beheerder van het systeem, om deze stappen op het systeemniveau uit te voeren. </p>
   <p>Planner, om deze stappen voor een groep uit te voeren, naast het zijn van de manager van die groep.</p></td>
  </tr> 
 </tbody> 
</table>

*For meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: [!UICONTROL Standard]</p>
   Or
   <p>Current: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>To perform these steps at the system level, you need the [!UICONTROL System Administrator] access level.</p><p>To perform them for a group, you must be a manager of that group.</p></td>
  </tr> 
 </tbody> 
</table>-->

## Gebruikers toestaan afbeeldingen toe te voegen in updates

Standaard kunnen gebruikers geen afbeeldingen in updates toevoegen. Wanneer u deze voorkeur inschakelt, kunnen gebruikers afbeeldingen bijvoegen in updates. De voorkeur geldt voor alle updates in alle gebieden van de [!DNL Workfront] -instantie.

>[!NOTE]
>
>* Afbeeldingen die zijn opgeslagen in updates tellen mee voor de opslaglimiet van het document. Voor informatie, zie [&#x200B; de grenzen van de documentopslag van de Controle &#x200B;](../../../documents/managing-documents/check-document-storage.md).
>* Afbeeldingen zijn toegankelijk via het tabblad [!UICONTROL Updates] op een object en zijn ook beschikbaar in het [!UICONTROL Documents] -gebied onder [!UICONTROL Main Menu] .
>

1. Klik het **[!UICONTROL Main Menu]** pictogram van het pictogram ![&#x200B; Belangrijkste menupictogram &#x200B;](assets/main-menu-icon.png) in de hoger-juiste hoek van [!DNL Adobe Workfront], dan klik **[!UICONTROL Setup]** ![&#x200B; het montagespictogram van het Gear &#x200B;](assets/gear-icon-settings.png).
1. Selecteer **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]** in het linkerdeelvenster.
1. Selecteer het tabblad **[!UICONTROL Preferences]**. 

   ![&#x200B; de voorkeur van de Gebruiker voor updatevoer &#x200B;](assets/updatefeeds-preferences-350x137.png)

1. Schakel het selectievakje **[!UICONTROL Allow users to add images in updates]** in.
1. Selecteer **[!UICONTROL Save]**.

   Wanneer deze voorkeur wordt toegelaten, kunt u het op elk ogenblik onbruikbaar maken. Alle afbeeldingen die al in updates zijn geplaatst, blijven in het [!UICONTROL Updates] -gebied van het object.
