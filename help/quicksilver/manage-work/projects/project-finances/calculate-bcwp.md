---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Berekenen van begrote kosten van uitgevoerd werk (BCWP)
description: Ook gekend als Geëiste Waarde, is de Begrotte Kosten van het Gepresteerde Werk (BCWP) metrische projectprestaties die de hoeveelheid taak vertegenwoordigt die eigenlijk op het tijdstip heeft voltooid dat deze metrisch wordt berekend.
author: Alina
feature: Work Management
exl-id: 203709a7-e522-4875-b3eb-40b967a938ec
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# Berekenen van begrote kosten van uitgevoerd werk (BCWP)

## Overzicht van de begrote kosten van het uitgevoerde werk (BCWP)

Ook gekend als Geëiste Waarde, is de Begrotte Kosten van het Gepresteerde Werk (BCWP) metrische projectprestaties die de hoeveelheid taak vertegenwoordigt die eigenlijk op het tijdstip heeft voltooid dat deze metrisch wordt berekend.

Adobe Workfront berekent de begrote Kosten van het Gepresteerde Werk (BCWP) voor zowel projecten als taken.

Overweeg het volgende wanneer het herzien van de waarden voor BCWP op een taak of een project:

* Workfront berekent BCWP voor een taak die op uw configuratie voor de Methode van de Index van Prestaties (PMI) van het project wordt gebaseerd.

  U kunt uw project vormen om PMI te berekenen gebruikend uren of kosten en BCWP wordt ook berekend gebruikend de zelfde waarden.

  Voor informatie over het vormen hoe BCWP wordt berekend, zie de sectie [ vormen hoe BCWP ](#configure-how-bcwp-is-calculated) in dit artikel wordt berekend.

* Workfront berekent BCWP voor een project door alle waarden BCWP van alle oudertaken en individuele taken op het project toe te voegen.

  De waarden van kindtaken worden niet toegevoegd aan BCWP van het project.

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
   <td> <p>Toegang tot projecten bewerken</p> <p>Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het project beheren</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Vorm hoe BCWP wordt berekend {#configure-how-bcwp-is-calculated}

U kunt vormen of BCWP in uren of kosten door te vormen wordt berekend hoe de Methode van de Index van Prestaties (PIM) van het project wordt berekend.

1. Ga naar een project en breid **Details van het Project** in het linkerpaneel uit.
1. Op het **gebied van de Financiën**, bepaal de plaats van het **gebied van de Methode van de Index van Prestaties** en klik tweemaal om het uit te geven.

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. Selecteer een van de volgende opties:

   | Optie | Hoe de berekening wordt uitgevoerd |
   |---|---|
   | Op uurbasis | Workfront berekent BCWP gebruikend de Geplande Uren van de taken. |
   | Op basis van kosten | Workfront berekent BCWP gebruikend de Geplande Kosten van de taken. |

1. Klik **sparen Veranderingen**.

Het BCWP van de taken op het project wordt berekend aan de hand van uren of kosten.

## BCWP berekenen

Workfront berekent de Gefabriceerde Kosten van het Gepresteerde Werk (BCWP) voor een taak of een project gebruikend de volgende formules:

```
Task BCWP = Actual Percent Complete x Task Budget
```

```
Project BCWP = SUM(BCWP values of all parent and individual tasks)
```

Bij deze berekening worden de volgende waarden gebruikt:

| Gebruikte waarde | Beschrijving van de gebruikte waarde |
|---|---|
| Werkelijk percentage voltooid | Dit is het werkelijke percentage van de taak zoals deze wordt weergegeven in Workfront. |
| Taakbudget | Dit is de waarde voor de geplande uren of de geplande kosten van de taak. |

Bijvoorbeeld, als het daadwerkelijke percentage volledig van de taak 25% is en de Begroting van de Taak of de Geplande Kosten $10.000 is, dan BCWP voor de taak is:

```
BCWP = 25% x $10,000 = $2,500
```

## Zoek BCWP voor een project of een taak

U kunt de waarde van de Begrotende Kosten van het Werk bekijken dat in een rapport of een lijst wordt uitgevoerd, door de kolom BCWP aan uw mening toe te voegen.

1. Ga naar een lijst met taken of projecten.
1. Breid het **menu van de Mening** uit en selecteer **Nieuwe Mening** of **aanpassen Mening**.

1. Klik **toevoegen Kolom**.
1. In **toon in deze kolom:** gebiedsbegin typend **BCWP** en klik om het te selecteren wanneer het in de lijst toont.

   ![](assets/bcwp-project-view.png)

1. Klik **sparen Mening**.
1. Het BCWP- gebiedsvertoningen in de mening.
