---
product-area: projects
navigation-topic: financials
title: Opheffing taakroltarieven op projectniveau
description: Als projectmanager, kunt u specificeren wat het het facturerings tarief voor een baanrol op een specifiek project is. Dit factureringstarief op projectniveau treedt het factureringstarief op het systeemniveau voor deze baanrol met voeten. Workfront gebruikt het factureringstarief op projectniveau van de baanrol om opbrengst te berekenen, in plaats van het systeem-vlakke factureringstarief te gebruiken.
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
source-git-commit: eb3db3b056cea359f77e56f77d6e9520954e2abb
workflow-type: tm+mt
source-wordcount: '850'
ht-degree: 0%

---

# De Factureringstarieven van de Rol van de Opheffing van de Taak op het projectniveau

Als projectmanager, kunt u specificeren wat het het facturerings tarief voor een baanrol op een specifiek project is. Dit factureringstarief op projectniveau treedt het factureringstarief op het systeemniveau voor deze baanrol met voeten. Workfront gebruikt het factureringstarief op projectniveau van de baanrol om opbrengst te berekenen, in plaats van het systeem-vlakke factureringstarief te gebruiken.

In dit artikel wordt beschreven hoe u de factureringssnelheden voor de rol van het systeem voor een project kunt overschrijven.

Voor algemene informatie over het met voeten treden van de het factureringspercentages van de baanrol voor projecten en het berekenen van de opbrengsten van het project, zie [ Overzicht van het met voeten treden van de Facturerings van de Rol van de Taak en het berekenen van Inkomsten op een project ](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Voor meer informatie over welke baanrol wordt gebruikt om opbrengst op het project te berekenen, zie de &quot;Begrijpende Berekeningen van de Ontvangsten voor Taken die op Gebruiker en van de Rol&quot;sectie in het artikel [ Overzicht van het Factureren en de Ontvangsten ](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) worden gebaseerd.

>[!NOTE]
>
>In het geval van werkelijke inkomsten mogen de factureringstarieven die worden toegepast op uren die worden toegevoegd aan een factureringsrecord dat als facturering is gemarkeerd, niet worden beïnvloed door overschrijvingen van factureringstarieven die plaatsvinden nadat de factureringsrecord is gefactureerd.

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
   <td> <p>Toegang tot projecten en financiële gegevens bewerken</p> <p>Administratieve toegang tot functies</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>Machtigingen beheren voor het project met de optie Financiële gegevens bewerken </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De Factureringstarieven van de Rol van de Opheffing van de Taak op het projectniveau

U kunt het factureringspercentage van een taakrol op een project op de volgende manieren overschrijven:

* Eenmaal, door een nieuw tarief voor de baanrol te selecteren.\
  Het nieuwe tarief wordt gebruikt voor de volledige duur van het project, om inkomsten te berekenen.

* Verscheidene tijden, door verscheidene nieuwe tarieven voor specifieke datumwaaiers te selecteren.\
  U kunt voor elk opgegeven datumbereik een andere frequentie gebruiken.

* U kunt nieuwe het factureren tarieven aan een projectmalplaatje toevoegen en die tarieven worden het factureren van het project wanneer u het project van dat malplaatje creeert. Voor informatie over het uitgeven van malplaatjes, zie [ projectmalplaatjes ](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) uitgeven.

>[!TIP]
>
>U kunt de factureringssnelheden van gebruikers voor een project niet overschrijven.

Een factureringssnelheid voor een project overschrijven:

1. Ga naar het project u het factureren voor wilt met voeten treden.
1. Klik **het Factureren Tarieven** in het linkerpaneel.
1. Klik **toevoegen het FactureringsTarief** > **Nieuw het Factureren Tarief**.

   Het vak Nieuwe factureringsfrequentie wordt geopend.

1. Op het **gebied van de Rol van de Baan 0}, selecteer de baanrol u het facturerings tarief voor wilt veranderen.**

   ![ met voeten treden facturerend tarief op project ](assets/override-billing-rate-on-project-nwe-350x310.png)

   Het **Standaard het FactureringsTarief** gebied toont het systeem-vlakke tarief voor deze baanrol.

1. In het **Facturerings 1** gebied van Tarieven, ga de éénmalige het facturerings tariefopheffing in, dan klik **sparen** om het facturerings tarief één keer met voeten te treden

   of

   Klik **toevoegen Tarief** om meer het factureren tariefoverschrijvingen toe te voegen.

1. (Voorwaardelijk) Als u meer dan één het factureren tariefopheffing toevoegt, specificeer de volgende informatie:

   * **het Factureren Tarieven 1**: de waarde van het Facturerings Tarief van het begin van het project tot de eerste datum van de eerste opheffing. Dit is typisch het zelfde bedrag zoals het **Gebrek Tarief**.
   * **Datum van het Begin**: dit is de datum wanneer het StandaardTarief beëindigt.
   * **Datum van het Eind**: de datum wanneer de nieuwe het factureren tariefopheffing beëindigt.

   ![ new_billing_rate_with_adjustment_dates.png ](assets/new-billing-rate-with-adjustment-dates-350x266.png)

1. De tijdzone voor de data die u selecteert, wordt onder in het vak Nieuwe factureringssnelheid weergegeven. Dit is de tijdzone verbonden aan uw instantie van Workfront, zoals aangetoond in het gebied van Info van de Klant van Opstelling. Voor informatie, zie [ basisinformatie voor uw systeem ](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md) vormen.
1. Workfront past het tarief van de opheffingsbaan op de uren toe die tijdens de gespecificeerde tijdkaders voorkomen wanneer het berekenen van opbrengst op het project.
1. Er mogen geen tussenruimten zijn tussen de tijdframes van twee overschrijvingssnelheden. De **Datum van het Begin** van een met voeten getreden tarief zou de dag onmiddellijk na de **Datum van het Eind** van de vorige met voeten getreden datum moeten zijn.

1. U kunt geen begindatum opgeven voor de eerste overschrijvingsfrequentie en geen einddatum voor de laatste overschrijvingsfrequentie.\
   Wij adviseren dat u het Standaardtarief voor het eerste met voeten getreden tarief gebruikt.\
   Workfront gaat ervan uit dat de eerste overschrijvingsrente wordt toegepast op alle uren met een datum die ouder is dan de Einddatum van de eerste overschrijving en dat de laatste overschrijvingsrente wordt toegepast op alle uren met een datum die nieuwer is dan de Begindatum van de laatste overschrijving.\
   Als een uur vóór de Geplande Datum van het Begin van het project het programma wordt geopend wordt het zeer eerste het factureringstarief gebruikt.\
   Als een uur na de Geplande Datum van de Voltooiing van het project het programma wordt geopend wordt het zeer laatste factureringstarief gebruikt.

1. Klik **sparen**.
