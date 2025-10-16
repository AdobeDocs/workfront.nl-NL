---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Een bedrijf deactiveren of opnieuw activeren
description: U kunt een bedrijf deactiveren dat u niet meer gebruikt terwijl het behouden van al zijn bijbehorende historische gegevens. Als u een bedrijf deactiveert dat al ergens in het systeem in gebruik is, blijft het functioneren net als altijd. Het wordt niet verwijderd of geblokkeerd.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: 8fb17d1008b00bc0701ce6e2f06c59d020510e90
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# Een bedrijf deactiveren of opnieuw activeren

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

U kunt een bedrijf deactiveren dat u niet meer gebruikt terwijl het behouden van al zijn bijbehorende historische gegevens. Als u een bedrijf deactiveert dat al ergens in het systeem in gebruik is, blijft het functioneren net als altijd. Het wordt niet verwijderd of geblokkeerd.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] package</p> </td> 
   <td><p>Alle</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licentie</p> </td> 
   <td><p>[!UICONTROL Plan]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
  <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau van [!UICONTROL System Administrator], dat u toestaat om het even welk bedrijf in het systeem uit te geven.</p> </li> 
     <li> <p>Administratieve toegang om bedrijven te beheren, die u toestaat om het even welk bedrijf in het systeem uit te geven.</p> </li> 
    </ul> <p><b> NOTA </b>:
     <ul> 
      <li> <p>U kunt ook bedrijven beheren die zijn gekoppeld aan een groep waaraan u als groepsbeheerder bent toegewezen.</p> </li> 
      <li> <p>Als u gebruikers wilt toevoegen aan en verwijderen uit het [!DNL Workfront] -systeem, moet u over een van de volgende opties beschikken:</p> 
       <ul> 
        <li> <p>Het toegangsniveau van [!UICONTROL System Administrator]. </p> </li> 
        <li> <p><b>[!UICONTROL Users]</b> het instellen in uw toegangsniveau dat is geconfigureerd voor <b>[!UICONTROL Edit]</b> toegang, waarbij <b>[!UICONTROL Create]</b> en ten minste een van de twee <b>[!UICONTROL User Admin]</b> -opties is ingeschakeld onder <b>[!UICONTROL Fine-tune your settings]</b> <img src="assets/gear-icon-in-access-levels.png"> . </p> <p> <img src="assets/access-req-users.png"> </p> <p>Als <b>[!UICONTROL User Admin (Group Users)]</b> is ingeschakeld, moet u een groepbeheerder zijn van een groep waarvan de gebruiker lid is.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td>
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een bedrijf deactiveren of opnieuw activeren

{{step-1-to-setup}}

1. In het linkerpaneel, klik **[!UICONTROL Companies]** ![&#x200B; pictogram van Bedrijven &#x200B;](assets/companies-icon-left-panel.png).

1. Selecteer een of meer bedrijven om te deactiveren of opnieuw te activeren.
1. Klik op **[!UICONTROL Edit]**. <!--MAKE THIS A SEPARATE NUMBERED LINE<span class="preview">In the Preview environment, disable the **[!UICONTROL Is Active]** option to deactivate it, or enable the option to activate it.</span>-->
1. Voor één bedrijf schakelt u de optie **[!UICONTROL Is Active]** uit om het te deactiveren of schakelt u de optie in om het te activeren. <!--ADD TO THE FRONT OF THIS SENTENCE In the Production environment, -->

   of

   Voor meerdere bedrijven selecteert u **[!UICONTROL No]** in de vervolgkeuzelijst **[!UICONTROL Is Active]** om de bedrijven te deactiveren of **[!UICONTROL Yes]** om de bedrijven te activeren.

1. Klik op **[!UICONTROL Save Changes]**.
