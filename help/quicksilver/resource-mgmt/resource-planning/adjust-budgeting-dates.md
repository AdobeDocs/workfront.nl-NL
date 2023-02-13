---
product-area: resource-management
navigation-topic: resource-planning
title: Datums voor budgettering aanpassen in de functie voor middelenplanning
description: Als u vindt dat er overtoewijzingen van uw middelen zijn nadat u hen in de Planner van het Middel hebt begroot, kunt u onderzoeken wat-als scenario's door de Begrotende Uren, FTE, of Kosten naar een ander tijdkader te verplaatsen. Op basis van de bevindingen in deze scenario's kunt u uw begrote uren uren, VTE, of Kosten dan aanpassen.
author: Alina
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 0%

---

# Datums voor budgettering aanpassen in de functie voor middelenplanning

Als u vindt dat er overtoewijzingen van uw middelen zijn nadat u hen in de Planner van het Middel hebt begroot, kunt u onderzoeken wat-als scenario&#39;s door de Begrotende Uren, FTE, of Kosten naar een ander tijdkader te verplaatsen. Op basis van de bevindingen in deze scenario&#39;s kunt u uw begrote uren uren, VTE, of Kosten dan aanpassen.

Overtoewijzingen kunnen verschijnen wanneer de begrote Uren, FTE, of Kosten van uw middelen hoger dan hun Beschikbare Uren, VTE, of Kosten zijn. Hierdoor wordt een negatieve nettowaarde gegenereerd.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Pro en hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot resourcebeheer bewerken, inclusief toegang tot bewerkingsprioriteiten en begrotingstijden in de bronnenplanner</p> <p>Toegang tot financiële gegevens, projecten en gebruikers bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Beheer machtigingen voor de projecten waarvoor u begrotingsgegevens wilt maken met de mogelijkheid om financiën te beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Bochtingsdatums aanpassen

1. Ga naar de bronnenplanner en selecteer **Weergeven op project**.

   >[!NOTE]
   >
   >U kunt de Adjust Gefabriceerde optie van Datums gebruiken slechts wanneer u de Planner van het Middel door project bekijkt.

1. Houd de muisaanwijzer boven de naam van een project en klik vervolgens op de knop **Meer** -menu.
1. Klikken **Bochtingsdatums aanpassen**.\
   De tijdlijn voor projecttoewijzing wordt weergegeven.\
   Het tijdsbestek waarin de uren momenteel in de begroting zijn opgenomen, wordt oranje gemarkeerd als er sprake is van een begrotingsconflict en blauw als er geen conflicten zijn.

   ![](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. Sleep het gemarkeerde tijdframe naar een ander tijdstip om te begrijpen waar er geen begrotingsconflicten zijn voor het geselecteerde project. Wanneer u een tijdkader vindt waar de Netto waarde positief is, verandert het benadrukte tijdkader in blauw.
1. Klik op de &#39;x&#39; in de rechterbovenhoek van de tijdlijn van de projecttoewijzing om deze te sluiten.
1. Verwijder de begrote uren uren uit de bestaande chronologie van het project en voeg hen aan de chronologie toe die de meeste beschikbaarheid toont.
1. Klikken **Opslaan**.
1. (Voorwaardelijk en optioneel) Als de tijdframes zonder budgetconflicten zich buiten de tijdlijn van het project bevinden, klikt u op de naam van het project om het project te openen.
1. (Voorwaardelijk en optioneel) Klik op **Project bewerken** en bewerkt u vervolgens de **Geplande begindatum** of de **Geplande afsluitdatum** om de tijdlijn van het project te wijzigen voor het tijdsbestek zonder begrotingsconflicten.\
   Raadpleeg het artikel voor meer informatie over het bewerken van projecten [Projecten bewerken](../../manage-work/projects/manage-projects/edit-projects.md).

1. (Voorwaardelijk en optioneel) Klik op **Wijzigingen opslaan**.
1. Keer terug naar de Planner van het Middel en neem de Begrotingspunten, FTEs, of Kosten in het tijdkader opnieuw op zonder in de begroting op te nemen conflicten.
1. Klikken **Opslaan**.
