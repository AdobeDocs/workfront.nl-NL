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
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---

# Factureringstarieven voor de rol van de werknemer op bedrijfsniveau overschrijven

Wanneer een baanrol wordt gecreeerd, hebt u de optie om een uurtarief voor die rol te selecteren. U kunt meerdere factureringssnelheden per uur maken die specifiek zijn voor een bedrijf. Elk factureringstarief is effectief voor een specifieke datumwaaier.

Op het projectniveau, kunt u een optie toelaten om bedrijf-vlakke het factureringspercentages toe te staan om tarief op projectniveau met voeten te treden. Voor meer informatie, zie [ project-Vlakke het Facturerings Tarieven met het bedrijf-Vlakke Facturerings ](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md) met voeten treden.

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
   <td> <p>Administratieve toegang tot Bedrijven als u geen Beheerder van het Systeem bent</p> <p>[!UICONTROL Edit] toegang tot financiële gegevens</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## Een vastgestelde factureringssnelheid overschrijven of wijzigen die wordt gebruikt voor een specifieke taakrol

1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe] Workfront en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png) .

1. Klik op **[!UICONTROL Companies]**.
1. Zoek het bedrijf waaraan de taakrol is toegewezen.
1. Klik op de bedrijfsnaam in de lijst.
1. Klik op **[!UICONTROL Billing Rates]** in het linkerdeelvenster.
1. Klik op **[!UICONTROL Add Billing Rate]>[!UICONTROL New Billing Rate]** of kies een bestaande frequentie om te bewerken.
1. In de [!UICONTROL New Billing Rate] dialoog, selecteer de Rol van de a [!UICONTROL **Baan**] om het het factureren tarief voor te bepalen.

   Het [!UICONTROL **Standaard het Facturerings Tarief van het Facturerings**] toont het systeem-vlakke tarief voor deze baanrol.

   ![ Nieuwe de dialoog van het Tarief van het Facturerings ](assets/date-effective-billing-rates-for-company.png)

1. Op het [!DNL **Facturerings 1**] gebied van Tarieven 1, ga het factureringstarief in. Dan, klik [!UICONTROL **sparen**] om het het factureren tarief één keer met voeten te treden.

   of

   Klik [!UICONTROL **toevoegen Tarief**] om meer het factureringspercentages met efficiënte data toe te voegen.

1. (Voorwaardelijk) Als u meer dan één factureringstarief toevoegt, ga de volgende informatie in:

   * **[!UICONTROL Billing Rates 1], 2, enzovoort.**: De waarde van de factureringssnelheid voor de tijdsperiode.
   * **[!UICONTROL Start Date]**: De datum waarop de snelheid van kracht wordt.
   * **[!UICONTROL End Date]**: De datum waarop de snelheid eindigt.

     Factureringsgraad 1 zal geen begindatum hebben en het laatste factureringstarief zal geen einddatum hebben. Sommige datums worden automatisch toegevoegd. Bijvoorbeeld, als het Facturerings Tarief 1 geen einddatum heeft, en u het Facturerings Tarief 2 met een begindatum van 1 mei 2023 toevoegt, wordt een einddatum van 30 april, 2023 toegevoegd aan het Facturerings Tarief 1 zodat geen hiaten bestaan.

1. Klik [!UICONTROL **sparen**].

   >[!NOTE]
   >
   >Veranderde roltarieven op het project hebben alleen invloed op dat project. De op bedrijfsniveau gewijzigde tarieven zullen gevolgen hebben voor alle projecten. Voor meer informatie, zie [ Overzicht van het met voeten treden van de FactureringsRates van de Rol van de Baan en het berekenen van Inkomsten op een project ](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
