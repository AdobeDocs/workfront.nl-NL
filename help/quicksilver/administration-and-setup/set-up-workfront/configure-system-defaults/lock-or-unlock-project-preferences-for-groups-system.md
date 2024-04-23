---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Projectvoorkeuren voor alle groepen in het systeem vergrendelen of ontgrendelen
description: De groepen in uw organisatie zouden een projectvoorkeur kunnen nodig hebben die verschillend voor hun unieke werkschema's wordt gevormd. U kunt de voorkeur voor alle groepen door de organisatie ontgrendelen zodat zij het op hun kunnen vormen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 3e97df265df83965d094d8723fe76043ff4af80e
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# Projectvoorkeuren voor alle groepen in het systeem vergrendelen of ontgrendelen

De groepen in uw organisatie zouden een projectvoorkeur kunnen nodig hebben die verschillend voor hun unieke werkschema&#39;s wordt gevormd. U kunt de voorkeur voor alle groepen door de organisatie ontgrendelen zodat zij het op hun kunnen vormen.

Wanneer een voorkeur wordt ontgrendeld en de groepsbeheerder het wijzigt, verwerven de projecten verbonden aan de groep de configuratie voor die voorkeur van groep-niveau het plaatsen in plaats van van van systeem-niveau het plaatsen.

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

## Over vergrendelde en ontgrendelde voorkeuren

Door een project, taak of uitgiftevoorkeur te vergrendelen die u op systeemniveau hebt geconfigureerd, zorgt u ervoor dat iedereen dezelfde instelling gebruikt voor die voorkeur. Hoewel u een voorkeur kunt nog aanpassen die u sluit, kunnen de groepsbeheerders het voor hun groepen niet aanpassen.

Omgekeerd, staat het ontgrendelen van een project, een taak, of een uitgiftevoorkeur groepsbeheerders meer flexibiliteit toe om de manier te beheren hun groepen met die punten werken. Wanneer een voorkeur wordt ontgrendeld, kunnen groepsbeheerders deze opnieuw configureren voor hun groepen.

Als een veld geen schakelaar voor vergrendelen/ontgrendelen heeft, kan de configuratie van instellingen op groepsniveau niet worden ontgrendeld door groepsbeheerders. Configuratie is alleen beschikbaar op systeemniveau.

Voor instructies over het vergrendelen of ontgrendelen van een project, taak of uitgiftevoorkeur op systeemniveau raadpleegt u [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>Na een [!DNL Workfront] de beheerder ontgrendelt een voorkeur op systeemniveau, kan om het even welke groepsbeheerder het vormen en dan het sluiten om ervoor te zorgen dat iedereen in hun groep en subgroups hieronder de zelfde configuratie gebruikt. Dit is parallel aan de mogelijkheid dat een [!DNL Workfront] de beheerder moet een voorkeur voor iedereen in het systeem vormen en sluiten. Zie voor meer informatie [Projectvoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) en [Een project, taak of uitgave van subgroepen vergrendelen of ontgrendelen](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## Ontgrendel een projectvoorkeur zodat de groepen het kunnen vormen

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klikken **[!UICONTROL Project Preferences]** en klik vervolgens op **[!UICONTROL Projects]**.

1. Voer een van de volgende handelingen uit:

   * Als u wilt dat groepsbeheerders een voorkeur voor hun groepen kunnen vormen, ontgrendel het ![](assets/unlock-toggle-button.png).
   * Als u wilt dat alle groepen uw configuratie voor een voorkeur gebruiken, zorg ervoor dat het gesloten is (dit is het gebrek).

     >[!IMPORTANT]
     >
     >Wij adviseren dat u met de beheerders en de gebruikers in groepen door het systeem communiceert om ervoor te zorgen dat alle behoeften rekenschap worden gegeven op de manier u een gesloten voorkeur vormt. Wanneer u het sluit, wordt uw configuratie voor het geërft door alle groepen in het systeem. En als de voorkeur voor om het even welke periode is ontgrendeld, vervangt uw configuratie die die groepsbeheerders zouden kunnen hebben gemaakt.

1. Klik op **[!UICONTROL Save]**.
