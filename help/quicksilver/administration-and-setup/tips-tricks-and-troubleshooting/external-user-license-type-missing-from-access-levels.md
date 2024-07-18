---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Het type externe gebruikerslicentie ontbreekt in toegangsniveaus
description: Ik kan het type van vergunning van de Externe Gebruiker niet meer zien onder de Niveaus van de Toegang in Opstelling.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 0%

---

# Het type externe gebruikerslicentie ontbreekt in toegangsniveaus

## Probleem

Ik kan het type van vergunning van de Externe Gebruiker niet meer zien onder de Niveaus van de Toegang in Opstelling.

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder zijn. Voor meer informatie, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> een gebruiker volledige administratieve toegang verlenen </a>.</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Oplossing

1. Ga naar **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Preferences]** .

1. Controleer in de sectie **[!UICONTROL Security]** of de optie **[!UICONTROL Collaborate with people without Workfront accounts by using their email address]** is ingeschakeld.

   Als deze optie niet wordt toegelaten, verschijnt de externe gebruiker niet in de Opstelling van het Niveau van de Toegang.
