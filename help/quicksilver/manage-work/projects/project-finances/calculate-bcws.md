---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Berekenen van de begrote kosten van het Geplande Werk (BCWS)
description: Ook gekend als Geplande Waarde, is de Begrotende Kosten van het Gepland Werk (BCWS) metrische projectprestaties die de hoeveelheid taak vertegenwoordigt die op het tijdstip zou moeten voltooid zijn dat deze metrisch wordt berekend.
author: Alina
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Berekenen van de begrote kosten van het Geplande Werk (BCWS)

## Overzicht van de geplande kosten van het werk (BCWS)

Ook gekend als Geplande Waarde, is de Begrotende Kosten van het Gepland Werk (BCWS) metrische projectprestaties die de hoeveelheid taak vertegenwoordigt die op het tijdstip zou moeten voltooid zijn dat deze metrisch wordt berekend.

Adobe Workfront berekent de begrote kosten van het Geplande Werk (BCWS) voor zowel projecten als taken.

Overweeg het volgende wanneer het herzien van de waarden voor BCWS op een taak of een project:

* Workfront berekent BCWS voor een taak die op uw configuratie voor de Methode van de Index van Prestaties (PIM) van het project wordt gebaseerd.

   U kunt uw project vormen om PIM te berekenen gebruikend uren of kosten en BCWS wordt ook berekend gebruikend de zelfde waarden.

   Voor informatie over het vormen hoe BCWS wordt berekend, zie de sectie [Configureer hoe BCWS wordt berekend](#configure-how-bcws-is-calculated) in dit artikel.

* Workfront berekent BCWS voor een project door alle waarden BCWS van alle oudertaken en individuele taken op het project toe te voegen.

   De waarden van kindtaken worden niet toegevoegd aan BCWS van het project.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten bewerken</p> <p>Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het project beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Configureer hoe BCWS wordt berekend {#configure-how-bcws-is-calculated}

U kunt vormen of BCWS in uren of kosten wordt berekend door te vormen hoe de Methode van de Index van Prestaties (PIM) van het project wordt berekend.

1. Ga naar een project en klik op **Projectdetails** in het linkerdeelvenster.
1. In de **Financiën** gebied, zoek de **Prestatiesindexmethode** en dubbelklik erop om het te bewerken.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. Selecteer een van de volgende opties:

   | Option | Hoe de berekening wordt uitgevoerd |
   |---|---|
   | Op uurbasis | Workfront berekent de BCWS met de geplande uren van de taken. |
   | Op basis van kosten | Workfront berekent de BCWS met de geplande kosten van de taken. |


1. Klikken **Wijzigingen opslaan**.

   Het BCWS van de taken voor het project wordt berekend aan de hand van uren of kosten.

## BCWS berekenen

Workfront berekent de begrote Kosten van Gepland Werk (BCWS) voor taken of projecten door de volgende formules te gebruiken:

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

In deze berekening worden de volgende waarden gebruikt:

| Gebruikte waarde | Beschrijving van de gebruikte waarde |
|---|---|
| Gepland percentage voltooid | Dit is wat het percentage voltooide van de taak zou moeten zijn door te bekijken hoeveel tijd tussen het begin van de taak en vandaag wordt overgegaan. |
| Taakbudget | Dit is de waarde voor de geplande uren of de geplande kosten van de taak. |

Als het vandaag bijvoorbeeld 12 februari is en een taak gepland staat voor 10 februari tot 20 februari, moet de taak vandaag 20% voltooid zijn. Als het Begroting van de Taak (Geplande Kosten) $10.000 is, dan BCWS voor de taak is:

```
Task BCWS = 20% x $10,000 = $2,000
```

## Zoek BCWS voor een project of een taak

U kunt de waarde van de Geplande Kosten van het Werk bekijken die in een rapport of een lijst, door de kolom BCWS aan uw mening toe te voegen wordt gepland.

1. Ga naar een lijst met taken of projecten.
1. Breid uit **Weergave** en selecteert u **Nieuwe weergave** of **Weergave aanpassen**.

1. Klikken **Kolom toevoegen**.
1. In de **Tonen in deze kolom:** veldtype **BCWS** en klik om de selectie te selecteren wanneer deze in de lijst wordt weergegeven.

   ![](assets/bcws-in-project-view.png)

1. Klikken **Weergave opslaan**.
1. De **BCWS** wordt weergegeven in de weergave.
