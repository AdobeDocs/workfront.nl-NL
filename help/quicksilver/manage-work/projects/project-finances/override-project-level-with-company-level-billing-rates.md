---
product-area: projects
navigation-topic: financials
title: Override project-Level het Factureren Tarieven met het bedrijf-Vlakke FactureringsTarieven
description: Override project-Level het Factureren Tarieven met het bedrijf-Vlakke FactureringsTarieven
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Override project-Level het Factureren Tarieven met het bedrijf-Vlakke FactureringsTarieven

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

U kunt een project vormen om bedrijf-vlakke het factureringstarieven in plaats van project-vlakke het factureren tarieven te gebruiken.

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
   <td> <p>Toegang tot projecten en financiële gegevens bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen voor het project beheren met beheerdersmachtigingen</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Schakel de optie Factureringssnelheden op bedrijfsniveau in

Wanneer een bedrijf met een project wordt geassocieerd en deze optie wordt toegelaten, worden de veranderingen die aan de bedrijf-vlakke het facturerings tarieven worden aangebracht met voeten getreden die het factureringstarief op het project wordt geplaatst.

Wanneer een gebruiker manueel financiën op het project herberekent, worden om het even welke veranderingen in het bedrijf-vlakke factureringspercentages toegepast. Historische inkomstenberekeningen worden ook overschreven, tenzij ze als gefactureerd worden gemarkeerd.

1. Ga naar een project.
1. Klik op de knop **Meer** menu ![](assets/qs-more-icon-on-an-object.png) naast de naam van het project in de koptekst klikt u op **Bewerken**.
1. In de **Financiën** in, schakelt u de **Factureringssnelheden op bedrijfsniveau toestaan om factureringssnelheden op projectniveau te overschrijven**.

   >[!CAUTION]
   >
   >Als u deze optie inschakelt, worden historische inkomstenberekeningen genegeerd, tenzij deze als gefactureerd worden gemarkeerd. U kunt de historische inkomstenberekeningen behouden door een factureringsrecord te maken. Zie het artikel voor meer informatie [Factureringsrecords maken](../../../manage-work/projects/project-finances/create-billing-records.md)

1. Klikken **Wijzigingen opslaan**.

## Billing Rates op bedrijfsniveau bijwerken en deze toepassen op een project

Nadat u de bedrijf-vlakke het facturerings optie van de tariefopheffing op een project hebt toegelaten, zijn de veranderingen die in de tarieven van het bedrijfs factureren van toepassing op het project wanneer de financiën worden herberekend.

>[!NOTE]
>
>Gebruikers moeten toegang hebben tot bedrijven in hun toegangsniveau om de factureringstarieven op bedrijfsniveau bij te werken.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen**.
1. Klikken **Bedrijven**.
1. Klik de naam van het bedrijf dat met het project wordt geassocieerd waarvoor u bedrijf-vlakke het factureren tariefopheffing toeliet.
1. Klikken **Factureringstarieven** in het linkerdeelvenster.
1. Werk de **Factureringsgraad bedrijf** en begin-/einddatums voor een bestaande taakrol en druk vervolgens op Enter.

   Als u een nieuwe datum wilt toevoegen aan een effectieve factureringssnelheid van het bedrijf, selecteert u een factureringssnelheid voor de rol van de taak en klikt u op **Bewerken**. Voor meer informatie over de datum van de daadwerkelijke het factureringspercentages van het bedrijf, zie [Factureringstarieven voor de rol van de werknemer op bedrijfsniveau overschrijven](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

1. Voer een van de volgende handelingen uit om de bedrijfstarieven voor een of meer projecten bij te werken:

   * Meerdere projecten:

   1. Ga naar een lijst met projecten.
   1. Schakel het selectievakje in in overeenstemming met de projecten die u wilt bijwerken.
   1. Klikken **Bewerken**.
   1. Schakel in het gedeelte Instellingen het selectievakje **Herberekening van kosten en opbrengsten** -optie.
   1. Klikken **Wijzigingen opslaan**.

   * Eén project:

      1. Ga naar het project waarvoor u bedrijf-vlakke het factureren tariefopheffing toeliet.
      1. Klik op de knop **Meer** menu ![](assets/qs-more-icon-on-an-object.png) naast de projectnaam in de koptekst klikt u op **Herberekening van financiën**.
