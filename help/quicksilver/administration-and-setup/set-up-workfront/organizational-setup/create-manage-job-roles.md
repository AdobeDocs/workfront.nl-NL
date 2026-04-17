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
source-git-commit: d8a01839b8f1332741f87be766f3ccb7d08cef96
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 0%

---

# Taakrollen maken en beheren

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>Met de versie 25.11 is de valuta van de Overschrijving voor baanrollen afgekeurd in Productie. (De veroudering vond plaats op 30 oktober in de voorvertoningsomgeving.) In plaats van een basisvaluta te hebben en valuta&#39;s te overschrijven, is er nu één valuta beschikbaar voor functies, en de kosten en factureringstarieven worden bepaald met behulp van die valuta.

Als [!DNL Adobe Workfront] beheerder of Standaardgebruiker met Edit toegang tot de Rollen van de Baan, kunt u baanrollen tot stand brengen die aan gebruikers kunnen worden toegewezen en standaardbaanrollen schrappen die niet relevant voor uw organisatie zijn. Voor informatie over administratieve toegang in [!DNL Workfront], zie [ gebruikers administratieve toegang van de Verlening tot bepaalde gebieden ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!TIP]
>
>De rollen van de baan zijn een integraal deel van het beheren van middelen. Om de middelen planningshulpmiddelen te gebruiken, hebben de baanrollen een kosten en het facturerings tarief verbonden aan hen nodig. Voor informatie, zie [ begonnen worden met het Beheer van het Middel ](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

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
   <td>Toegang tot taakrollen bewerken</td>
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een taakrol maken

Een taakrol maken:

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **[!UICONTROL Job Roles]** .
1. Klik op **[!UICONTROL New Job Role]> Nieuwe taakrol maken** .
1. Voer in de volgende velden gegevens in:

   * **Naam**: Verwijs op een naam voor de baanrol. Dit is de naam die overal in Workfront wordt weergegeven waar het veld Functie wordt weergegeven.

     >[!TIP]
     >
     >De naam van een taakrol kan maximaal 255 tekens bevatten. Langere namen kunnen echter in bepaalde gebieden van Workfront worden afgebroken.

   * **Beschrijving**: Ga een beschrijving voor de rol in die erop wijst wat over het uniek is.
   * **is Actief**: Selecteer **ja** als u de rol actief en beschikbaar overal in Workfront wilt zijn om met gebruikers, het werkpunten, enz. worden geassocieerd. Selecteer **Nr** als u de rol wilt worden gedeactiveerd en niet beschikbaar aan gebruikers, het werkpunten, enz. toewijzen.

     Voor informatie over het deactiveren van baanrollen, zie [ werkrollen ](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md) deactiveren.

1. Klik op **[!UICONTROL Create Job Role]**. De taakrol is nu beschikbaar om te worden toegewezen aan taken, uitgaven, goedkeuringen of u kunt lay-outsjablonen of andere objecten ermee delen. Voor informatie over al gebruik van baanrollen in [!DNL Workfront], zie [ het overzicht van de rol van de Baan ](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Voor informatie over het schrappen van een baanrol, zie [ baanrollen van de Schrapping ](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

## Tarieven en kenmerken toevoegen aan een taakrol

Facturerings- en kostenpercentages voor een functie worden in financiële berekeningen gebruikt.

Snelheidskenmerken worden ondersteund in gebieden van Workfront waar tarieven bestaan, zoals taakrollen en gebruikers. Wanneer kenmerken op een taakrol worden toegepast, worden hun toewijzingen automatisch omgezet in de juiste percentages.

Voor meer informatie, zie [ tariefattributen ](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md) bepalen.

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **[!UICONTROL Job Roles]** .
1. Klik op de naam van een bestaande taakrol om deze te bewerken.
1. Om de details van de baanrol bij te werken, klik **Details** in het linkerpaneel.
1. (Facultatief) om een douaneformulier aan de baanrol vast te maken, klik **voeg douanevorm** gebied in de hoger-juiste hoek van de pagina van Details toe, en selecteer een douaneformulier van de lijst die toont.

   Voor meer informatie bij het vastmaken van een douanevorm, zie [ een douanevorm aan een voorwerp ](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toevoegen.

1. Klik [!UICONTROL **Tarieven**] in het linkerpaneel.
1. Klik [!UICONTROL **het Factureren**] of [!UICONTROL **Kosten**] om het tarieftype te selecteren.
1. Klik [!UICONTROL **Add Tarieven**] om een nieuw tarief toe te voegen.

   of

   Selecteer een bestaand tarief en klik **uitgeven** pictogram ![ pictogram ](assets/edit-icon.png) om het bij te werken.

   >[!NOTE]
   >
   >Omdat elke snelheid is gekoppeld aan de combinatie van de rol en kenmerken om een unieke snelheid te maken, kunnen de kenmerken niet worden gewijzigd wanneer u een snelheid bewerkt.

1. Voor het **Nieuwe Tarief** vakje, uitgezochte attributen voor het tarief zoals Agentschap, Plaats, of het Centrum van Kosten.

   >[!NOTE]
   >
   >Deze eigenschappen worden afzonderlijk gedefinieerd en kunnen de opbrengsten- en kostprijsberekeningen beïnvloeden. Voor meer informatie, zie [ tariefattributen ](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md) bepalen.

1. Selecteer de **Valuta** voor het tarief. De beheerder van Workfront voegt de Valuta van de Basis in het gebied van de Opstelling toe. U kunt de selectie wijzigen in een andere beschikbare valuta en u kunt de valuta wijzigen voor effectieve gedateerde tijdbereiken.

   >[!TIP]
   >
   >Alleen valuta&#39;s die beschikbaar zijn in het gebied Wisselkoersen in uw systeem zijn beschikbaar in dit veld. Als er maar één valuta is ingesteld, is alleen die valuta beschikbaar.

   Voor informatie over vestiging de Valuta van de Basis in Workfront, zie [ de wisselkoers van de Opstelling ](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   Voor informatie over het veranderen van de munt van een project, zie [ de projectmunt ](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md) veranderen.

1. (Voorwaardelijk) voor een het factureren tarief, ga het **Facturerings Tarief** voor deze baanrol in.

   Dit is het facturerings per uurtarief van de baanrol. Deze waarde berekent de geplande en werkelijke inkomsten van de taken en kwesties die verband houden met de rol, en uiteindelijk de geplande en werkelijke inkomsten van de projecten. Voer de koers in met de geselecteerde valuta.

   Als u kenmerken gebruikt, vormen de kenmerken en de rol van de taak samen een uniek tarief. Zo kan een Designer-rol in New York voor Agentschap A een afzonderlijk tarief hebben dan een Designer-rol in Parijs voor Agentschap B.

   Voor datum daadwerkelijke het factureren tarieven, klik **voegt Tarief** toe. Voer de waarde van de facturering/het uur voor de tijdsperiode in en wijs zo nodig een begindatum en einddatum toe. Het eerste factuurtarief heeft geen begindatum en het laatste factuurtarief heeft geen einddatum.

   <!-- Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, an end date of April 30 is added to the first billing rate so that no gaps exist.-->

   In Workfront kunt u tussenruimten tussen datumbereiken weglaten, maar u ontvangt een waarschuwing om te bevestigen dat dit opzettelijk is.

   Voor informatie over hoe Workfront opbrengst berekent, zie [ Overzicht van Facturering en Ontvangsten ](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

   >[!TIP]
   >
   >Wanneer u een bestaande taakrol bewerkt, kunt u de lijst sorteren om de meest recente begindatum boven aan de lijst met percentages weer te geven.

1. (Voorwaardelijk) voor een kostentarief, ga het **Tarief van Kosten** voor deze baanrol in.

   Dit is het kostenpercentage per uur van de functie. Deze waarde berekent de geplande en de werkelijke kosten van taken en kwesties die verband houden met de rol, en uiteindelijk de geplande en werkelijke kosten van de projecten. Voer de koers in met de geselecteerde valuta.

   Als u kenmerken gebruikt, vormen de kenmerken en de rol van de taak samen een uniek tarief. Zo kan een Designer-rol in New York voor Agentschap A een afzonderlijk tarief hebben dan een Designer-rol in Parijs voor Agentschap B.

   Voor datum efficiënte kostentarieven, klik **toevoegen Tarief**. Voer de waarde van de kosten/het uur voor de tijdsperiode in en wijs zo nodig een begindatum en einddatum toe. De eerste kostprijs heeft geen begindatum en de laatste kostprijs heeft geen einddatum.

   Sommige datums worden automatisch toegevoegd. Als de eerste kostenvoet bijvoorbeeld geen einddatum heeft en u een tweede kostenpercentage toevoegt met een begindatum van 1 mei, wordt een einddatum van 30 april toegevoegd aan de eerste kostenvoet zodat er geen hiaten bestaan.

   Voor informatie over hoe Workfront kosten berekent, zie [ Kosten van het Spoor ](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

   >[!TIP]
   >
   >Wanneer u een bestaande taakrol bewerkt, kunt u de lijst sorteren om de meest recente begindatum boven aan de lijst met percentages weer te geven.

1. Klik [!UICONTROL **sparen**].

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


<!--

   * **Currency**: The Base Currency is shown by default. The Workfront administrator adds the Base Currency in the Setup area. You can change the selection to another available currency, and you can change the currency on effective dated time ranges.

      >[!TIP]
      >
      >Only currencies available in the Exchange Rates area in your system are available in this field. If you only have one currency set up, only that currency is available.

      For information about setting up the Base Currency in Workfront, see [Set up exchange rates](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

      For information about changing the currency of a project, see [Change the project currency](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).
   
   * **Cost Rate**: This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the selected currency.

      For date effective cost rates, click **Add Rate**. Enter the value of the cost/hour for the time period, and assign a Start Date and End Date as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.

      Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first cost rate so that no gaps exist.

      For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

   * **Billing Rate**: This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the selected currency.

      For date effective billing rates, click **Add Rate**. Enter the value of the billing/hour for the time period, and assign a Start Date and End Date as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.

      Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first billing rate so that no gaps exist.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

-->



