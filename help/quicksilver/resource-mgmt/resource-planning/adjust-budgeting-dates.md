---
product-area: resource-management
navigation-topic: resource-planning
title: De begrotingsdatums aanpassen in de bronnenplanner
description: Als u vindt dat er overtoewijzingen van uw middelen zijn nadat u hen in de Planner van het Middel hebt begroot, kunt u onderzoeken wat-als scenario's door de Begrotende Uren, FTE, of Kosten naar een ander tijdkader te verplaatsen. Op basis van de bevindingen in deze scenario's kunt u uw begrote uren uren, VTE, of Kosten dan aanpassen.
author: Lisa
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Datums voor budgettering aanpassen in de functie voor middelenplanning

Als u vindt dat er overtoewijzingen van uw middelen zijn nadat u hen in de Planner van het Middel hebt begroot, kunt u onderzoeken wat-als scenario&#39;s door de Begrotende Uren, FTE, of Kosten naar een ander tijdkader te verplaatsen. Op basis van de bevindingen in deze scenario&#39;s kunt u uw begrote uren uren, VTE, of Kosten dan aanpassen.

Overtoewijzingen kunnen verschijnen wanneer de begrote Uren, FTE, of Kosten van uw middelen hoger dan hun Beschikbare Uren, VTE, of Kosten zijn. Hierdoor wordt een negatieve nettowaarde gegenereerd.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot resourcebeheer bewerken, inclusief toegang tot bewerkingsprioriteiten en begrotingstijden in de bronnenplanner</p> <p>Toegang tot financiële gegevens, projecten en gebruikers bewerken</p></td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td> 
   <td> <p>Beheer machtigingen voor de projecten waarvoor u begrotingsgegevens wilt maken met de mogelijkheid om financiën te beheren</p></td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bochtingsdatums aanpassen

1. Ga naar de Planner van het Middel en selecteer **Mening door Project**.

   >[!NOTE]
   >
   >U kunt de Adjust Gefabriceerde optie van Datums gebruiken slechts wanneer u de Planner van het Middel door project bekijkt.

1. Beweeg over de naam van een project, dan klik **Meer** menu.
1. Klik **aanpassen het Begrotingstermijnen**.\
   De tijdlijn voor projecttoewijzing wordt weergegeven.\
   Het tijdsbestek waarin de uren momenteel in de begroting zijn opgenomen, wordt oranje gemarkeerd als er sprake is van een begrotingsconflict en blauw als er geen conflicten zijn.

   ![&#x200B; Adjust in de begroting stellende data &#x200B;](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. Sleep het gemarkeerde tijdframe naar een ander tijdstip om te begrijpen waar er geen begrotingsconflicten zijn voor het geselecteerde project. Wanneer u een tijdkader vindt waar de Netto waarde positief is, verandert het benadrukte tijdkader in blauw.
1. Klik op de &#39;x&#39; in de rechterbovenhoek van de tijdlijn van de projecttoewijzing om deze te sluiten.
1. Verwijder de begrote uren uren uit de bestaande tijdlijn van het project en voeg hen aan de chronologie toe die de meeste beschikbaarheid toont.
1. Klik **sparen**.
1. (Voorwaardelijk en optioneel) Als de tijdframes zonder budgetconflicten zich buiten de tijdlijn van het project bevinden, klikt u op de naam van het project om het project te openen.
1. (Voorwaardelijk en facultatief) klik **uitgeven Project**, dan geef de **Geplande Datum van het Begin** of de **Geplande Datum van de Voltooiing** uit om de chronologie van het project voor het tijdkader zonder het in de begroting opnemen conflicten te wijzigen.\
   Voor meer informatie over het uitgeven van projecten, zie het artikel [&#x200B; projecten &#x200B;](../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

1. (Voorwaardelijk en facultatief) klik **sparen Veranderingen**.
1. Keer terug naar de Planner van het Middel en neem de Begrotingspunten, FTEs, of Kosten in het tijdkader opnieuw op zonder in de begroting op te nemen conflicten.
1. Klik **sparen**.
