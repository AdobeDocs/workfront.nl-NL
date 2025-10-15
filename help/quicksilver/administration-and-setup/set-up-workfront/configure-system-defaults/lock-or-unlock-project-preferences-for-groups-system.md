---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: De Voorkeur van het Project van het slot of van het Ontgrendelen voor Alle Groepen in het Systeem
description: De groepen in uw organisatie zouden een projectvoorkeur kunnen nodig hebben die verschillend voor hun unieke werkschema's wordt gevormd. U kunt de voorkeur voor alle groepen door de organisatie ontgrendelen zodat zij het op hun kunnen vormen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# Projectvoorkeuren voor alle groepen in het systeem vergrendelen of ontgrendelen

De groepen in uw organisatie zouden een projectvoorkeur kunnen nodig hebben die verschillend voor hun unieke werkschema&#39;s wordt gevormd. U kunt de voorkeur voor alle groepen door de organisatie ontgrendelen zodat zij het op hun kunnen vormen.

Wanneer een voorkeur wordt ontgrendeld en de groepsbeheerder het wijzigt, verwerven de projecten verbonden aan de groep de configuratie voor die voorkeur van groep-niveau het plaatsen in plaats van van van systeem-niveau het plaatsen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licentie</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Over vergrendelde en ontgrendelde voorkeuren

Door een project, taak of uitgiftevoorkeur te vergrendelen die u op systeemniveau hebt geconfigureerd, zorgt u ervoor dat iedereen dezelfde instelling gebruikt voor die voorkeur. Hoewel u een voorkeur kunt nog aanpassen die u sluit, kunnen de groepsbeheerders het voor hun groepen niet aanpassen.

Omgekeerd, staat het ontgrendelen van een project, een taak, of een uitgiftevoorkeur groepsbeheerders meer flexibiliteit toe om de manier te beheren hun groepen met die punten werken. Wanneer een voorkeur wordt ontgrendeld, kunnen groepsbeheerders deze opnieuw configureren voor hun groepen.

Als een veld geen schakelaar voor vergrendelen/ontgrendelen heeft, kan de configuratie van instellingen op groepsniveau niet worden ontgrendeld door groepsbeheerders. Configuratie is alleen beschikbaar op systeemniveau.

Voor instructies bij het sluiten van of het ontgrendelen van een systeem-vlakke project, ziet de taak, of de uitgiftevoorkeur, [&#x200B; taak voor het hele systeem vormen en voorkeur uitgeven &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>Nadat een [!DNL Workfront] beheerder een voorkeur op het systeemniveau ontgrendelt, kan om het even welke groepbeheerder het vormen en dan het sluiten om ervoor te zorgen dat iedereen in hun groep en subgroups hieronder de zelfde configuratie gebruikt. Dit is parallel aan de mogelijkheid dat een [!DNL Workfront] -beheerder een voorkeur voor iedereen in het systeem moet configureren en vergrendelen. Voor meer informatie, zie [&#x200B; projectvoorkeur voor een groep &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) en [&#x200B; Slot of ontgrendel een project, een taak, of een uitgiftevoorkeur voor subgroups &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md) vormen.

## Ontgrendel een projectvoorkeur zodat de groepen het kunnen vormen

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Project Preferences]** en vervolgens op **[!UICONTROL Projects]** .

1. Voer een van de volgende handelingen uit:

   * Als u groepsbeheerders een voorkeur voor hun groepen wilt kunnen vormen, ontgrendel het ![&#x200B; knevel van de Ontgrendeling &#x200B;](assets/unlock-toggle-button.png).
   * Als u wilt dat alle groepen uw configuratie voor een voorkeur gebruiken, zorg ervoor dat het gesloten is (dit is het gebrek).

     >[!IMPORTANT]
     >
     >Wij adviseren dat u met de beheerders en de gebruikers in groepen door het systeem communiceert om ervoor te zorgen dat alle behoeften rekenschap worden gegeven op de manier u een gesloten voorkeur vormt. Wanneer u het sluit, wordt uw configuratie voor het geërft door alle groepen in het systeem. En als de voorkeur voor om het even welke periode is ontgrendeld, vervangt uw configuratie die die groepsbeheerders zouden kunnen hebben gemaakt.

1. Klik op **[!UICONTROL Save]**.
