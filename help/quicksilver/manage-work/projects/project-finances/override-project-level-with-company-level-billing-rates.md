---
product-area: projects
navigation-topic: financials
title: Override Project-Level Billing Rates with Company-Level Billing Rates
description: Override Project-Level Billing Rates with Company-Level Billing Rates
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: 72511f98e05c160e2ca69def8aa3a929ed62bb40
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Override Project-Level Billing Rates with Company-Level Billing Rates

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

U kunt een project vormen om bedrijf-vlakke het factureringspercentages in plaats van project-vlakke het factureringspercentages te gebruiken.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-lidmaatschap*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten en financiële gegevens bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen voor het project beheren met beheerdersmachtigingen</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Schakel de optie Factureringssnelheden op bedrijfsniveau in

Wanneer een bedrijf met een project wordt geassocieerd en deze optie wordt toegelaten, worden de veranderingen die aan de bedrijf-vlakke het facturerings tarieven worden aangebracht met voeten getreden die het factureringstarief op het project wordt geplaatst.

Wanneer een gebruiker manueel financiën op het project herberekent, worden om het even welke veranderingen in het bedrijf-vlakke factureringspercentages toegepast. Historische inkomstenberekeningen worden ook overschreven, tenzij ze als gefactureerd worden gemarkeerd.

1. Ga naar een project.
1. Klik **Meer** menu ![](assets/qs-more-icon-on-an-object.png) naast de naam van het project in de kopbal, dan klik **geef** uit.
1. In de **sectie van de Financiën**, laat **toe toestaan bedrijf-vlakke het factureringspercentages om project-niveau het factureringspercentage** met voeten te treden.

   >[!CAUTION]
   >
   >Als u deze optie inschakelt, worden historische omzetberekeningen genegeerd, tenzij deze als gefactureerd worden gemarkeerd. U kunt de historische omzetberekeningen behouden door een factuurrecord te maken. Voor meer informatie, zie het artikel [ Factureringsverslagen ](../../../manage-work/projects/project-finances/create-billing-records.md) creëren

1. Klik **sparen Veranderingen**.

## Factureringssnelheden op bedrijfsniveau bijwerken en deze toepassen op een project

Nadat u de optie voor het overschrijven van de factureringspercentages op bedrijfsniveau voor een project hebt ingeschakeld, worden wijzigingen in de factureringstarieven van het bedrijf toegepast op het project zodra de financiën opnieuw worden berekend.

>[!NOTE]
>
>Gebruikers moeten toegang hebben tot bedrijven in hun toegangsniveau om de factureringstarieven op bedrijfsniveau bij te werken.

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Opstelling**.
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

   * Enkel project:

      1. Ga naar het project waarvoor u de factureringspercentages op bedrijfsniveau hebt aangepast.
      1. Klik **Meer** menu ![](assets/qs-more-icon-on-an-object.png) naast de projectnaam in de kopbal, dan klik **Recalculate Financiën**.
