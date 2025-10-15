---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: De Billing van de Rol van de Opheffing van de Opheffing op het Niveau van het Bedrijf
description: Wanneer een baanrol wordt gecreeerd, hebt u de optie om een uurtarief voor die rol te selecteren. U kunt een factureringstarief per uur tot stand brengen dat voor een bedrijf specifiek is.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Factureringstarieven voor de rol van de werknemer op bedrijfsniveau overschrijven

Wanneer een baanrol wordt gecreeerd, hebt u de optie om een uurtarief voor die rol te selecteren. U kunt meerdere factureringssnelheden per uur maken die specifiek zijn voor een bedrijf. Elk factureringstarief is effectief voor een specifieke datumwaaier.

Op het projectniveau, kunt u een optie toelaten om bedrijf-vlakke het factureringspercentages toe te staan om tarief op projectniveau met voeten te treden. Voor meer informatie, zie [ project-Vlakke het Facturerings Tarieven met het bedrijf-Vlakke Facturerings ](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md) met voeten treden.

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
   <td> <p>Administratieve toegang tot Bedrijven als u geen Beheerder van het Systeem bent</p>
   <p>Toegang tot financiële gegevens bewerken</p> </td>
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een vastgestelde factureringssnelheid overschrijven of wijzigen die wordt gebruikt voor een specifieke taakrol

{{step-1-to-setup}}

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
