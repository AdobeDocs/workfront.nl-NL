---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Factureringstarieven voor de rol van de werknemer op bedrijfsniveau overschrijven
description: Wanneer een baanrol wordt gecreeerd, hebt u de optie om een uurtarief voor die rol te selecteren. U kunt een factureringstarief per uur tot stand brengen dat voor een bedrijf specifiek is.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# Factureringstarieven voor de rol van de werknemer op bedrijfsniveau overschrijven

Wanneer een baanrol wordt gecreeerd, hebt u de optie om een uurtarief voor die rol te selecteren. U kunt een factureringstarief per uur tot stand brengen dat voor een bedrijf specifiek is.

Op het projectniveau, kunt u een optie toelaten om bedrijf-vlakke het factureringspercentages toe te staan om tarief op projectniveau met voeten te treden. Zie voor meer informatie [Override project-Level het Factureren Tarieven met het bedrijf-Vlakke FactureringsTarieven](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Administratieve toegang tot Bedrijven als u geen Beheerder van het Systeem bent</p> <p>[!UICONTROL Edit] toegang tot financiële gegevens</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Een vastgestelde factureringssnelheid overschrijven of wijzigen die wordt gebruikt voor een specifieke taakrol

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe] Workfront, klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik op **[!UICONTROL Companies]**.
1. Zoek het bedrijf waaraan de functie is toegewezen.
1. Klikken **[!UICONTROL Edit Company]** in de rechterbovenhoek.
1. In de **[!UICONTROL Billing Rates]** selecteert u de taakrol die u wilt bewerken en voert u de nieuwe factureringsfrequentie voor die taakrol in de **[!UICONTROL Company Billing Rate]** doos.

   >[!NOTE]
   >
   >Veranderde roltarieven op het project hebben alleen invloed op dat project. De op bedrijfsniveau gewijzigde tarieven zullen gevolgen hebben voor alle projecten. Zie voor meer informatie [Overzicht van het overschrijven van de Billing Rates van de Rol en het berekenen van Inkomsten op een project](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
