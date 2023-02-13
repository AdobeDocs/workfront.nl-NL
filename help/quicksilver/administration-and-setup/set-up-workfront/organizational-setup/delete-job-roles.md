---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Taakrollen verwijderen
description: U kunt taakrollen verwijderen die uw organisatie niet meer gebruikt. Wij adviseren dat u baanrollen niet schrapt als zij met het werkpunten in het verleden zijn geassocieerd. Om al uw historische informatie over werktaken te houden, adviseren wij dat u rollen deactiveert, eerder dan hen schrapt wanneer zij verouderd worden. Voor informatie over het deactiveren van rollen, zie baanrollen deactiveren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Taakrollen verwijderen

U kunt taakrollen verwijderen die uw organisatie niet meer gebruikt. Wij adviseren dat u baanrollen niet schrapt als zij met het werkpunten in het verleden zijn geassocieerd.

Om al uw historische informatie over werktaken te houden, adviseren wij dat u rollen deactiveert, eerder dan hen schrapt wanneer zij verouderd worden. Voor informatie over het deactiveren van rollen, zie [Taakrollen deactiveren](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Administratieve toegang tot functies</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Een taakrol verwijderen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik op **[!UICONTROL Job Roles].**
1. Selecteer de taakrol die u wilt verwijderen en klik vervolgens op **[!UICONTROL Delete].**
1. Voer een van de volgende handelingen uit als er objecten (gebruikers, taken, problemen) zijn toegewezen aan de taakrol:

   * **Vervang de rol van de taak door een andere taakrol:** Selecteer de nieuwe taakrol in de vervolgkeuzelijst.

      Eventuele huidige en eerdere bronnentoewijzingen die aan de verwijderde taakrol zijn gekoppeld, worden overgebracht naar de taakrol die u selecteert.

      Gebruikers die slechts één taakrol aan hen hebben toegewezen, worden opnieuw toegewezen aan de taakrol die u selecteert; gebruikers die een secundaire functie hebben die aan hen wordt toegewezen, worden niet opnieuw toegewezen aan de taakrol die u selecteert.

   * **Verwijder de taakrol en de toewijzing van bronnen:** Selecteren **[!UICONTROL None]** in de vervolgkeuzelijst.

      >[!IMPORTANT]
      >
      >Als u een taakrol verwijdert, worden alle huidige en eerdere toewijzingen van bronnen met betrekking tot die taakrol voor alle projecten verwijderd.

      &#x200B; bijvoorbeeld, als een taak of een kwestie aan slechts die baanrol wordt toegewezen, wordt de taak of de kwestie unassigned nadat de baanrol wordt geschrapt.

1. Klik op  **[!UICONTROL Yes, Delete It]**.
