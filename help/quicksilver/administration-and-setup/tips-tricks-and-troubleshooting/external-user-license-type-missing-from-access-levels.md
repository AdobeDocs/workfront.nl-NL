---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Licentietype voor externe gebruiker ontbreekt in Toegangsniveaus
description: Ik kan het type van vergunning van de Externe Gebruiker niet meer zien onder de Niveaus van de Toegang in Opstelling.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '101'
ht-degree: 1%

---

# Het type externe gebruikerslicentie ontbreekt in toegangsniveaus

## Probleem

Ik kan het type van vergunning van de Externe Gebruiker niet meer zien onder de Niveaus van de Toegang in Opstelling.

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
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Oplossing

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Preferences]** .

1. Controleer in de sectie **[!UICONTROL Security]** of de optie **[!UICONTROL Collaborate with people without Workfront accounts by using their email address]** is ingeschakeld.

   Als deze optie niet wordt toegelaten, verschijnt de externe gebruiker niet in de Opstelling van het Niveau van de Toegang.
