---
title: Een tariefkaart aan een project koppelen
description: Wanneer u een tariefkaart aan een project vastmaakt, worden alle rollen door plaats en hun bijbehorende het factureren tarieven toegevoegd aan het project.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Een tariefkaart aan een project koppelen

De kaarten van het tarief slaan veelvoudige factureringspercentages per baanrol op, die op attributen wordt gebaseerd. U zou bijvoorbeeld een functie van Designer kunnen hebben die in Parijs gevestigd is voor Bureau A, een andere Designer die in Parijs gevestigd is voor Bureau B, en een derde Designer die in New York gevestigd is en niet aan een agentschap toegewezen is, elk met verschillende factureringstarieven. Kenmerken zijn echter niet vereist voor taakrollen op een tariefkaart. De kenmerken dienen als gereedschappen voor het vaststellen van kortere snelheden. Een factureringstarief op een tariefkaart kan ook datatarakter effectief zijn, zodat het tarief begint en op gespecificeerde data eindigt.

Wanneer u een tariefkaart aan een project vastmaakt, worden alle rollen en hun bijbehorende het factureren tarieven toegevoegd aan het project.

>[!NOTE]
>
>Het vastmaken van een tariefkaart treedt om het even welke bestaande tarief kaartfacturerings tarieven op het project met voeten. Overschrijvingen van factureringssnelheden die rechtstreeks aan het project zijn toegevoegd, worden niet verwijderd.

Voor informatie over het creëren van tariefkaarten, zie [&#x200B; tariefkaarten beheren &#x200B;](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

Voor algemene informatie over het met voeten treden van het factureringspercentage van de baanrol voor projecten en het berekenen van projectopbrengst, zie [&#x200B; Overzicht van het met voeten treden van het facturerings tarieven en het berekenen van opbrengst op een project &#x200B;](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>Toegang tot projecten, financiële gegevens en betaalkaarten bewerken</td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td> 
   <td>Rechten voor het project beheren met de machtiging Factureringssnelheden bewerken</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een tariefkaart aan een project koppelen

1. Ga naar het project.
1. Klik **Tarieven** in het linkerpaneel, dan selecteren **Facturering**.
1. Klik **toevoegen het FactureringsTarief > een Kaart van het Tarief vastmaken**.

   **maak een tariefkaart** doos vast opent. U kunt naar een tariefkaart in de lijst zoeken.

   ![&#x200B; maak een doos van de tariefkaart vast &#x200B;](assets/attach-rate-card-dialog.png)

   >[!NOTE]
   >
   >De Groep en het Bedrijf op de tariefkaarten worden gebruikt als filters op deze lijst. Omdat de projecten ook de gebieden van de Groep en van het Bedrijf omvatten, gebruikt Workfront deze waarden om de lijst van beschikbare tariefkaarten aan die relevant voor de context van het project te beperken, en niet alle tariefkaarten over het systeem.
   >
   >De overeenkomst hoeft niet exact te zijn. De kaarten van het tarief met lege Groep en/of de waarden van het Bedrijf kunnen nog afhankelijk van de de Groep/configuratie van het Bedrijf van het project verschijnen. Bijvoorbeeld, als een project een geselecteerde Groep heeft maar het Bedrijf leeg is, kunt u tariefkaarten zien verbonden aan die Groep zelfs als het Bedrijf van de tariefkaart verschillend of leeg is.

1. Selecteer de tariefkaart aan het project toe te voegen, en **te klikken verbindt**.

   De tariefkaart en alle bijbehorende roltarieven worden toegevoegd aan de lijst met factureringssnelheden.

   ![&#x200B; kaart van het Tarief die aan project &#x200B;](assets/rate-card-on-project.png) wordt toegevoegd

## Een tariefkaart uit een project verwijderen

Wanneer u een tariefkaart uit een project verwijdert, worden al zijn banen roltarieven verwijderd. U kunt geen individueel tarief uit het project verwijderen dat uit een tariefkaart komt.

Het tarief van de facturatie treedt voor gebruikers of baanrollen met voeten die rechtstreeks aan het project werden toegevoegd kan worden verwijderd zonder de volledige tariefkaart te verwijderen.

1. Ga naar het project.
1. Klik **Tarieven** in het linkerpaneel, dan selecteren **Facturering**.
1. Klik **verwijderen** pictogram ![&#x200B; verwijderen pictogram &#x200B;](assets/remove-icon.png).
1. Klik **bevestigen** op het bevestigingsbericht om de tariefkaart te verwijderen.

