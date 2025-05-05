---
product-area: reporting
keywords: gebruiker,delegatie,rapport,afgevaardigde,goedkeuring
navigation-topic: create-and-manage-reports
title: Rapport gebruikersdelegatie maken
description: Een gebruikersdelegatierapport maken
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Een gebruikersdelegatierapport maken

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

In Adobe Workfront, kunnen de gebruikers project delegeren, taak, en goedkeuringen aan andere gebruikers uitgeven om ervoor te zorgen dat hun goedkeuringen worden beheerd wanneer zij uit bureau zijn. De gebruikers met een vergunning van het Plan kunnen een rapport van de Delegatie van de Gebruiker tot stand brengen om te zien:

* Wie zijn taak, kwestie, en projectgoedkeuringen aan een andere gebruiker heeft gedelegeerd
* Welke gebruikers taak, kwestie, en projectgoedkeuringen hebben gedelegeerd die aan hen worden toegewezen

* Begindatum en einddatum van de delegaties

Meer leren over het delegeren van goedkeuringen, zie [ de goedkeuringsverzoek van de Afgevaardigde ](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn more about delegating work, see <a href="../../../workfront-basics/manage-your-account-and-profile/manage-time-off/personal-time-off.md" class="MCXref xref">Log personal time off and delegate your work</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn how to manage delegated work in Home, see [future link here].</p>
-->

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
      <td> 
      <p>Nieuw:</p>
         <ul>
         <li><p>Standaard</p></li>
         </ul>
      <p>Huidige:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor de onderdelen waarvan de goedkeuringen zijn gedelegeerd en voor de gebruikers die bij de delegatie zijn betrokken</p></td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een gebruikersdelegatierapport maken

1. Klik het **pictogram van het 1&rbrace; pictogram van het Belangrijkste Menu ![ ](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik** Rapporten **.**

1. Klik **Nieuw Rapport**, dan uitgezochte **Delegatie van de Gebruiker**.

   ![ Nieuwe delegatie van de rapportgebruiker ](assets/classic-new-report-user-delegation-350x644.png)

   De volgende gebieden tonen in dit rapport door gebrek:

   | Veld | Beschrijving |
   |---|---|
   | **van Gebruiker** | Dit is de gebruiker die hun taak, kwestie, en projectgoedkeuringen aan een andere gebruiker delegeert. |
   | **aan Gebruiker** | Dit is de gebruiker die taak, kwestie, en projectgoedkeuringen heeft die aan hen worden gedelegeerd. |
   | **Datum van het Begin** | Dit is het begin van de wachttijd voor de gebruiker die de delegaties heeft gemaakt. |
   | **Datum van het Eind** | Dit is het einde van de wachttijd voor de gebruiker die de delegaties heeft gemaakt. |

   {style="table-layout:auto"}

1. (Optioneel) In de rapportbuilder wijzigt u het volgende:

   * Kolommen (weergave)
   * Groepen
   * Filters
   * Diagram

   Meer over deze eigenschappen leren, zie [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

1. Nadat u klaar bent met het bouwen van uw rapport, klik **sparen + Sluiten**.

   Het rapport wordt weergegeven.
