---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Taakrollen verwijderen
description: U kunt taakrollen verwijderen die uw organisatie niet meer gebruikt. Wij adviseren dat u baanrollen niet schrapt als zij met het werkpunten in het verleden zijn geassocieerd. Om al uw historische informatie over werktaken te houden, adviseren wij dat u rollen deactiveert, eerder dan hen schrapt wanneer zij verouderd worden. Voor informatie over het deactiveren van rollen, zie baanrollen deactiveren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Taakrollen verwijderen

U kunt taakrollen verwijderen die uw organisatie niet meer gebruikt. Wij adviseren dat u baanrollen niet schrapt als zij met het werkpunten in het verleden zijn geassocieerd.

Om al uw historische informatie over werktaken te houden, adviseren wij dat u rollen deactiveert, eerder dan hen schrapt wanneer zij verouderd worden. Voor informatie over het deactiveren van rollen, zie [ werkrollen ](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md) deactiveren.

## Toegangsvereisten

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
   <td>Administratieve toegang tot taakrollen</td>
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een taakrol verwijderen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Job Roles].**
1. Selecteer de taakrol die u wilt verwijderen en klik op **[!UICONTROL Delete].**
1. Voer een van de volgende handelingen uit als er objecten (gebruikers, taken, problemen) zijn toegewezen aan de taakrol:

   * **vervangt de baanrol met een verschillende baanrol:** selecteer de nieuwe baanrol van de drop-down lijst.

     Eventuele huidige en eerdere bronnentoewijzingen die aan de verwijderde taakrol zijn gekoppeld, worden overgebracht naar de taakrol die u selecteert.

     Gebruikers die slechts één taakrol aan hen hebben toegewezen, worden opnieuw toegewezen aan de taakrol die u selecteert; gebruikers die een secundaire taakrol aan hen hebben toegewezen, worden niet opnieuw toegewezen aan de baanrol die u selecteert.

   * **Schrap de baanrol en zijn middeltoewijzing:** Uitgezocht **[!UICONTROL None]** van de drop-down lijst.

     >[!IMPORTANT]
     >
     >Als u een taakrol verwijdert, worden alle huidige en eerdere toewijzingen van bronnen met betrekking tot die taakrol voor alle projecten verwijderd.

     &#x200B; bijvoorbeeld, als een taak of een kwestie aan slechts die baanrol wordt toegewezen, wordt de taak of de kwestie unassigned nadat de baanrol wordt geschrapt.

1. Klik op **[!UICONTROL Yes, Delete It]** .
