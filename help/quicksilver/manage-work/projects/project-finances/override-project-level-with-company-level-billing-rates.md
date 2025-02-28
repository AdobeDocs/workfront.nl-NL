---
product-area: projects
navigation-topic: financials
title: Override project-Level het Factureren Tarieven met het bedrijf-Vlakke FactureringsTarieven
description: Override project-Level het Factureren Tarieven met het bedrijf-Vlakke FactureringsTarieven
author: Lisa
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Override project-Level het Factureren Tarieven met het bedrijf-Vlakke FactureringsTarieven

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

U kunt een project vormen om bedrijf-vlakke het factureringstarieven in plaats van project-vlakke het factureren tarieven te gebruiken.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
   <p>Nieuw: Standaard</p>
   <p>of</p>
   <p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>Toegang tot projecten en financiële gegevens bewerken</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>Machtigingen voor het project beheren met beheerdersmachtigingen</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Schakel de optie Factureringssnelheden op bedrijfsniveau in

Wanneer een bedrijf met een project wordt geassocieerd en deze optie wordt toegelaten, worden de veranderingen die aan de bedrijf-vlakke het facturerings tarieven worden aangebracht met voeten getreden die het factureringstarief op het project wordt geplaatst.

Wanneer een gebruiker manueel financiën op het project herberekent, worden om het even welke veranderingen in het bedrijf-vlakke factureringspercentages toegepast. Historische inkomstenberekeningen worden ook overschreven, tenzij ze als gefactureerd worden gemarkeerd.

1. Ga naar een project.
1. Klik het **Meer** menu ![ Meer menu ](assets/qs-more-icon-on-an-object.png) naast de naam van het project in de kopbal, dan klik **uitgeven**.
1. In de **sectie van de Financiën**, laat **toe toestaan bedrijf-vlakke het factureren tarieven om project-vlakke het factureren tarieven** met voeten te treden.

   >[!CAUTION]
   >
   >Als u deze optie inschakelt, worden historische inkomstenberekeningen genegeerd, tenzij deze als gefactureerd worden gemarkeerd. U kunt de historische inkomstenberekeningen behouden door een factureringsrecord te maken. Voor meer informatie, zie het artikel [ het factureren verslagen ](../../../manage-work/projects/project-finances/create-billing-records.md) creëren

1. Klik **sparen Veranderingen**.

## Billing Rates op bedrijfsniveau bijwerken en deze toepassen op een project

Nadat u de bedrijf-vlakke het facturerings optie van de tariefopheffing op een project hebt toegelaten, zijn de veranderingen die in de tarieven van het bedrijfs factureren van toepassing op het project wanneer de financiën worden herberekend.

>[!NOTE]
>
>Gebruikers moeten toegang hebben tot bedrijven in hun toegangsniveau om de factureringstarieven op bedrijfsniveau bij te werken.

{{step-1-to-setup}}

1. Klik **Bedrijven**.
1. Klik de naam van het bedrijf dat met het project wordt geassocieerd waarvoor u bedrijf-vlakke het factureren tariefopheffing toeliet.
1. Klik **het Factureren Tarieven** in het linkerpaneel.
1. Werk het **Facturerings Tarief van het Bedrijf** en begin/eind data voor een bestaande baanrol bij, dan druk binnengaan.

   Om een nieuwe datum toe te voegen efficiënt bedrijf het factureren tarief, selecteer een het facturerings tarief voor de baanrol en klik **uitgeven**. Voor meer informatie over datum efficiënte bedrijf het factureren tarieven, zie [ het factureringspercentages van de baanrol van de Opheffing op het bedrijfsniveau ](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

1. Voer een van de volgende handelingen uit om de bedrijfstarieven voor een of meer projecten bij te werken:

   * Meerdere projecten:

      1. Ga naar een lijst met projecten.
      1. Schakel het selectievakje in in overeenstemming met de projecten die u wilt bijwerken.
      1. Klik **uitgeven**.
      1. In de sectie van Montages, laat **toe herberekent Kosten en Opbrengsten** optie.
      1. Klik **sparen Veranderingen**.

   * Eén project:

      1. Ga naar het project waarvoor u bedrijf-vlakke het factureren tariefopheffing toeliet.
      1. Klik **Meer** menu ![ Meer menu ](assets/qs-more-icon-on-an-object.png) naast de projectnaam in de kopbal, dan klik **opnieuw berekenen Financiën**.
