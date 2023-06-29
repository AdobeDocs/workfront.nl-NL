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
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# Factureringstarieven voor de rol van de werknemer op bedrijfsniveau overschrijven

{{highlighted-preview}}

Wanneer een baanrol wordt gecreeerd, hebt u de optie om een uurtarief voor die rol te selecteren. <span class="preview">U kunt meerdere factureringssnelheden per uur maken die specifiek zijn voor een bedrijf. Elk factureringstarief is effectief voor een specifieke datumwaaier.</span>

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
1. <span class="preview">Klik op de bedrijfsnaam in de lijst.</span>
1. <span class="preview">Klikken **[!UICONTROL Billing Rates]** in het linkerdeelvenster.</span>
1. <span class="preview">Klikken **[!UICONTROL Add Billing Rate]>[!UICONTROL New Billing Rate]** of kies een bestaande snelheid om te bewerken.</span>
1. <span class="preview">In de [!UICONTROL New Billing Rate] selecteert u een [!UICONTROL **Functie**] om de factureringssnelheid voor te bepalen.</span>

   <span class="preview">De [!UICONTROL **Standaardfactureringsfrequentie**] toont het systeem-vlakke tarief voor deze baanrol.</span>

   <span class="preview">![Het dialoogvenster Nieuwe factureringsfrequentie](assets/date-effective-billing-rates-for-company.png)</span>

1. <span class="preview">In de [!DNL **Factureringstarieven 1**] voert u de factureringssnelheid in. Klik vervolgens op [!UICONTROL **Opslaan**] om de factureringssnelheid één keer te overschrijven.</span>

   <span class="preview">of</span>

   <span class="preview">Klikken [!UICONTROL **Snelheid toevoegen**] meer factureringssnelheden met effectieve datums toe te voegen.</span>

1. <span class="preview">(Voorwaardelijk) Als u meer dan één factureringstarief toevoegt, ga de volgende informatie in:</span>

   * <span class="preview">**[!UICONTROL Billing Rates 1], 2, enz.**: De waarde van de factureringssnelheid voor de tijdsperiode.</span>
   * <span class="preview">**[!UICONTROL Start Date]**: De datum waarop de rentevoet van kracht wordt.</span>
   * <span class="preview">**[!UICONTROL End Date]**: De datum waarop de rentevoet eindigt.</span>

     <span class="preview">Factureringsgraad 1 zal geen begindatum hebben en het laatste factureringstarief zal geen einddatum hebben. Sommige datums worden automatisch toegevoegd. Bijvoorbeeld, als het Facturerings Tarief 1 geen einddatum heeft, en u het Facturerings Tarief 2 met een begindatum van 1 mei 2023 toevoegt, wordt een einddatum van 30 april, 2023 toegevoegd aan het Facturerings Tarief 1 zodat geen hiaten bestaan.</span>

1. <span class="preview">Klikken [!UICONTROL **Opslaan**].</span>

   >[!NOTE]
   >
   >Veranderde roltarieven op het project hebben alleen invloed op dat project. De op bedrijfsniveau gewijzigde tarieven zullen gevolgen hebben voor alle projecten. Zie voor meer informatie [Overzicht van het overschrijven van de Billing Rates van de Rol en het berekenen van Inkomsten op een project](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
