---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Taakrollen maken en beheren
description: Als  [!DNL Adobe Workfront]  beheerder of een gebruiker met administratieve toegang tot de Rollen van de Baan, kunt u baanrollen creëren die aan gebruikers kunnen worden toegewezen en standaardbaanrollen schrappen die niet relevant voor uw organisatie zijn.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: cada5387ddfb710029d06cd38841ecb9c8a6484b
workflow-type: tm+mt
source-wordcount: '1689'
ht-degree: 0%

---

# Taakrollen maken en beheren

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

{{highlighted-preview}}

>[!IMPORTANT]
>
>Met de versie 25.11 is de valuta van de Overschrijving voor baanrollen afgekeurd in Productie. (De veroudering vond plaats op 30 oktober in de voorvertoningsomgeving.) In plaats van een basisvaluta te hebben en valuta&#39;s te overschrijven, is er nu één valuta beschikbaar voor functies, en de kosten en factureringstarieven worden bepaald met behulp van die valuta.

Als [!DNL Adobe Workfront] beheerder of een gebruiker met administratieve toegang tot de Rollen van de Baan, kunt u baanrollen tot stand brengen die aan gebruikers kunnen worden toegewezen en standaardbaanrollen schrappen die niet relevant voor uw organisatie zijn. Voor informatie over administratieve toegang in [!DNL Workfront], zie [&#x200B; gebruikers administratieve toegang van de Verlening tot bepaalde gebieden &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!TIP]
>
>De rollen van de baan zijn een integraal deel van het beheren van middelen. Om de middelen planningshulpmiddelen te gebruiken, hebben de baanrollen een kosten en het facturerings tarief verbonden aan hen nodig. Voor informatie, zie [&#x200B; begonnen worden met het Beheer van het Middel &#x200B;](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Om een taakrol te maken of te bewerken: een Workfront- of workflowpakket</p>
   <p>Om tariefattributen toe te passen en douaneformulieren toe te voegen aan de baanrol: Workflow Ultimate</p></td> 
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

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een taakrol maken

Een taakrol maken:

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **[!UICONTROL Job Roles]** .
1. Klik op **[!UICONTROL New Job Role]<span class="preview"> > Nieuwe taakrol maken** . </span>
1. Voer in de volgende velden gegevens in:

   * **Naam**: Verwijs op een naam voor de baanrol. Dit is de naam die overal in Workfront wordt weergegeven waar het veld Functie wordt weergegeven.

     >[!TIP]
     >
     >De naam van een taakrol kan maximaal 255 tekens bevatten. Langere namen kunnen echter in bepaalde gebieden van Workfront worden afgebroken.

   * **Beschrijving**: Ga een beschrijving voor de rol in die erop wijst wat over het uniek is.
   * **is Actief**: Selecteer **ja** als u de rol actief en beschikbaar overal in Workfront wilt zijn om met gebruikers, het werkpunten, enz. worden geassocieerd. Selecteer **Nr** als u de rol wilt worden gedeactiveerd en niet beschikbaar aan gebruikers, het werkpunten, enz. toewijzen.

     Voor informatie over het deactiveren van baanrollen, zie [&#x200B; werkrollen &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md) deactiveren.

   * **Valuta**: De Valuta van de Basis wordt getoond door gebrek. De beheerder van Workfront voegt de Valuta van de Basis in het gebied van de Opstelling toe. U kunt de selectie wijzigen in een andere beschikbare valuta en u kunt de valuta wijzigen voor effectieve gedateerde tijdbereiken.

     >[!TIP]
     >
     >Alleen valuta&#39;s die beschikbaar zijn in het gebied Wisselkoersen in uw systeem zijn beschikbaar in dit veld. Als er maar één valuta is ingesteld, is alleen die valuta beschikbaar.

     Voor informatie over vestiging de Valuta van de Basis in Workfront, zie [&#x200B; de wisselkoers van de Opstelling &#x200B;](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

     Voor informatie over het veranderen van de munt van een project, zie [&#x200B; de projectmunt &#x200B;](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md) veranderen.

   * **Tarief van Kosten**: Dit is de kosten per uurtarief van de baanrol. Deze waarde berekent de geplande en de werkelijke kosten van taken en kwesties die verband houden met de rol, en uiteindelijk de geplande en werkelijke kosten van de projecten. Voer de koers in met de geselecteerde valuta.

     Voor datum efficiënte kostentarieven, klik **toevoegen Tarief**. Voer de waarde van de kosten/het uur voor de tijdsperiode in en wijs zo nodig een begindatum en einddatum toe. De eerste kostprijs heeft geen begindatum en de laatste kostprijs heeft geen einddatum.

     Sommige datums worden automatisch toegevoegd. Als de eerste kostenvoet bijvoorbeeld geen einddatum heeft en u een tweede kostenpercentage toevoegt met een begindatum van 1 mei 2025, wordt een einddatum van 30 april 2025 toegevoegd aan de eerste kostenvoet zodat er geen hiaten bestaan.

     Voor informatie over hoe Workfront kosten berekent, zie [&#x200B; Kosten van het Spoor &#x200B;](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >Wanneer u een bestaande taakrol bewerkt, kunt u de lijst sorteren om de meest recente begindatum boven aan de lijst met percentages weer te geven.

   * **het Factureren Tarief**: Dit is het factureren per uurtarief van de baanrol. Deze waarde berekent de geplande en werkelijke inkomsten van de taken en kwesties die verband houden met de rol, en uiteindelijk de geplande en werkelijke inkomsten van de projecten. Voer de koers in met de geselecteerde valuta.

     Voor datum daadwerkelijke het factureren tarieven, klik **voegt Tarief** toe. Voer de waarde van de facturering/het uur voor de tijdsperiode in en wijs zo nodig een begindatum en einddatum toe. Het eerste factuurtarief heeft geen begindatum en het laatste factuurtarief heeft geen einddatum.

     Sommige datums worden automatisch toegevoegd. Als de eerste factureringsfrequentie bijvoorbeeld geen einddatum heeft en u een seconde toevoegt met een begindatum van 1 mei 2025, wordt een einddatum van 30 april 2025 toegevoegd aan de eerste factureringssnelheid zodat er geen hiaten bestaan.

     Voor informatie over hoe Workfront opbrengst berekent, zie [&#x200B; Overzicht van Facturering en Ontvangsten &#x200B;](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >Wanneer u een bestaande taakrol bewerkt, kunt u de lijst sorteren om de meest recente begindatum boven aan de lijst met percentages weer te geven.

<!-- Remove or hide the billing rate and cost rate bullets on April 16 for GA -->

1. Klik op **[!UICONTROL Create Job Role]**. De taakrol is nu beschikbaar om te worden toegewezen aan taken, uitgaven, goedkeuringen of u kunt lay-outsjablonen of andere objecten ermee delen. Voor informatie over al gebruik van baanrollen in [!DNL Workfront], zie [&#x200B; het overzicht van de rol van de Baan &#x200B;](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Voor informatie over het schrappen van een baanrol, zie [&#x200B; baanrollen van de Schrapping &#x200B;](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

<div class="preview">

## Tarieven en kenmerken toevoegen aan een taakrol

Facturerings- en kostenpercentages voor een functie worden in financiële berekeningen gebruikt.

Snelheidskenmerken worden ondersteund in gebieden van Workfront waar tarieven bestaan, zoals taakrollen en gebruikers. Wanneer kenmerken op een taakrol worden toegepast, worden hun toewijzingen automatisch omgezet in de juiste percentages.

Voor meer informatie, zie [&#x200B; tariefattributen &#x200B;](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md) bepalen.

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **[!UICONTROL Job Roles]** .
1. Klik op de naam van een bestaande taakrol om deze te bewerken.
1. Om de details van de baanrol bij te werken, klik **Details** in het linkerpaneel.
1. (Facultatief) om een douaneformulier aan de baanrol vast te maken, klik **voeg douanevorm** gebied in de hoger-juiste hoek van de pagina van Details toe, en selecteer een douaneformulier van de lijst die toont.

   Voor meer informatie bij het vastmaken van een douanevorm, zie [&#x200B; een douanevorm aan een voorwerp &#x200B;](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toevoegen.

1. Klik [!UICONTROL **Tarieven**] in het linkerpaneel.
1. Klik [!UICONTROL **het Factureren**] of [!UICONTROL **Kosten**] om het tarieftype te selecteren.
1. Klik [!UICONTROL **Add Tarieven**] om een nieuw tarief toe te voegen.

   of

   Selecteer een bestaand tarief en klik **uitgeven** pictogram ![&#x200B; pictogram &#x200B;](assets/edit-icon.png) om het bij te werken.

   >[!NOTE]
   >
   >Omdat elke snelheid is gekoppeld aan de combinatie van de rol en kenmerken om een unieke snelheid te maken, kunnen de kenmerken niet worden gewijzigd wanneer u een snelheid bewerkt.

1. Voor het **Nieuwe Tarief** vakje, uitgezochte attributen voor het tarief zoals Agentschap, Plaats, of het Centrum van Kosten.

   >[!NOTE]
   >
   >Deze eigenschappen worden afzonderlijk gedefinieerd en kunnen de opbrengsten- en kostprijsberekeningen beïnvloeden. Voor meer informatie, zie [&#x200B; tariefattributen &#x200B;](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md) bepalen.

1. Selecteer de **Valuta** voor het tarief. De beheerder van Workfront voegt de Valuta van de Basis in het gebied van de Opstelling toe. U kunt de selectie wijzigen in een andere beschikbare valuta en u kunt de valuta wijzigen voor effectieve gedateerde tijdbereiken.

   >[!TIP]
   >
   >Alleen valuta&#39;s die beschikbaar zijn in het gebied Wisselkoersen in uw systeem zijn beschikbaar in dit veld. Als er maar één valuta is ingesteld, is alleen die valuta beschikbaar.

   Voor informatie over vestiging de Valuta van de Basis in Workfront, zie [&#x200B; de wisselkoers van de Opstelling &#x200B;](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   Voor informatie over het veranderen van de munt van een project, zie [&#x200B; de projectmunt &#x200B;](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md) veranderen.

1. (Voorwaardelijk) voor een het factureren tarief, ga het **Facturerings Tarief** voor deze baanrol in.

   Dit is het facturerings per uurtarief van de baanrol. Deze waarde berekent de geplande en werkelijke inkomsten van de taken en kwesties die verband houden met de rol, en uiteindelijk de geplande en werkelijke inkomsten van de projecten. Voer de koers in met de geselecteerde valuta.

   Als u kenmerken gebruikt, vormen de kenmerken en de rol van de taak samen een uniek tarief. Zo kan een Designer-rol in New York voor Agentschap A een afzonderlijk tarief hebben dan een Designer-rol in Parijs voor Agentschap B.

   Voor datum daadwerkelijke het factureren tarieven, klik **voegt Tarief** toe. Voer de waarde van de facturering/het uur voor de tijdsperiode in en wijs zo nodig een begindatum en einddatum toe. Het eerste factuurtarief heeft geen begindatum en het laatste factuurtarief heeft geen einddatum.

   Sommige datums worden automatisch toegevoegd. Als de eerste factureringsfrequentie bijvoorbeeld geen einddatum heeft en u een seconde toevoegt met een begindatum van 1 mei, wordt een einddatum van 30 april toegevoegd aan de eerste factureringssnelheid zodat er geen hiaten bestaan.

   Voor informatie over hoe Workfront opbrengst berekent, zie [&#x200B; Overzicht van Facturering en Ontvangsten &#x200B;](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

   >[!TIP]
   >
   >Wanneer u een bestaande taakrol bewerkt, kunt u de lijst sorteren om de meest recente begindatum boven aan de lijst met percentages weer te geven.

1. (Voorwaardelijk) voor een kostentarief, ga het **Tarief van Kosten** voor deze baanrol in.

   Dit is het kostenpercentage per uur van de functie. Deze waarde berekent de geplande en de werkelijke kosten van taken en kwesties die verband houden met de rol, en uiteindelijk de geplande en werkelijke kosten van de projecten. Voer de koers in met de geselecteerde valuta.

   Als u kenmerken gebruikt, vormen de kenmerken en de rol van de taak samen een uniek tarief. Zo kan een Designer-rol in New York voor Agentschap A een afzonderlijk tarief hebben dan een Designer-rol in Parijs voor Agentschap B.

   Voor datum efficiënte kostentarieven, klik **toevoegen Tarief**. Voer de waarde van de kosten/het uur voor de tijdsperiode in en wijs zo nodig een begindatum en einddatum toe. De eerste kostprijs heeft geen begindatum en de laatste kostprijs heeft geen einddatum.

   Sommige datums worden automatisch toegevoegd. Als de eerste kostenvoet bijvoorbeeld geen einddatum heeft en u een tweede kostenpercentage toevoegt met een begindatum van 1 mei, wordt een einddatum van 30 april toegevoegd aan de eerste kostenvoet zodat er geen hiaten bestaan.

   Voor informatie over hoe Workfront kosten berekent, zie [&#x200B; Kosten van het Spoor &#x200B;](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

   >[!TIP]
   >
   >Wanneer u een bestaande taakrol bewerkt, kunt u de lijst sorteren om de meest recente begindatum boven aan de lijst met percentages weer te geven.

1. Klik [!UICONTROL **sparen**].

</div>

<!--
   * **Override Currency Cost Rate**: This is the cost per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role.

     Enter the rate in the Override Currency specified above. This also updates the Cost Rate for this job role when using the Base Currency.

     For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a cost rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Cost Rate, the cost rate of the job role also updates automatically.

   * **Override Currency Billing Rate**: This is the billing per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role.

      Enter the rate in the Override Currency specified above. This also updates the Billing Rate for this job role when using the Base Currency.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a billing rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the billing rate of the job role also updates automatically.

-->



