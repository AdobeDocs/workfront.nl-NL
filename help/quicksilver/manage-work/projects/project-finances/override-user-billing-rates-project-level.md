---
content-type: overview
product-area: projects
navigation-topic: financials
title: De Tarieven van de Facturering van de Gebruiker op het Niveau van het Project met voeten treden
description: In dit artikel wordt beschreven hoe u de factureringssnelheden van de systeemgebruiker voor een project kunt overschrijven.
author: Lisa
feature: Work Management
exl-id: eb7dbb6f-a31c-4569-be54-9a151dcf4135
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

# Opheffing van factureringstarieven voor gebruikers op projectniveau

Als projectmanager, kunt u specificeren wat het het facturerings tarief voor een gebruiker op een specifiek project is. Dit factureringstarief op projectniveau treedt het factureringstarief op het systeemniveau voor deze gebruiker met voeten. Workfront gebruikt het factureringstarief op projectniveau van de gebruiker om opbrengst te berekenen, in plaats van het systeem-vlakke factureringstarief te gebruiken.

In dit artikel wordt beschreven hoe u de factureringssnelheden van de systeemgebruiker voor een project kunt overschrijven.

Voor algemene informatie over het met voeten treden van factureringspercentages voor projecten en het berekenen van projectopbrengst, zie [&#x200B; Overzicht van het met voeten treden van het facturerings tarieven en het berekenen van opbrengst op een project &#x200B;](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Voor meer informatie over het berekenen van opbrengst op het project, zie [&#x200B; Overzicht van opbrengst en kostenhiërarchie &#x200B;](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) en de [&#x200B; Berekeningen van de Inkomsten voor Taken die op Gebruiker en de sectie van de Taken van de Rol &#x200B;](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments) in het artikel [&#x200B; Overzicht van het Factureren en van de Inkomsten &#x200B;](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md) worden gebaseerd.

>[!NOTE]
>
>In het geval van werkelijke inkomsten mogen de factureringstarieven die worden toegepast op uren die worden toegevoegd aan een factureringsrecord dat als facturering is gemarkeerd, niet worden beïnvloed door overschrijvingen van factureringstarieven die plaatsvinden nadat de factureringsrecord is gefactureerd.

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
   <td> <p>Toegang tot projecten en financiële gegevens bewerken</p>
       <p><p>U moet ook een van de volgende opties hebben:</p> 
        <ul> 
          <li> <p>Het toegangsniveau voor systeembeheerders. </li> 
          <li> <p><b> Gebruikers </b> het plaatsen in uw toegangsniveau dat aan <b> wordt gevormd geeft </b> toegang uit, met <b> creeert </b> en minstens één van de twee <b> die gebruikers Admin </b> opties onder <b> worden toegelaten verfijnen uw montages </b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Van deze twee opties, als <b> Admin van de Gebruiker (de Gebruikers van de Groep) </b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td> 
   <td>Machtigingen beheren voor het project met de optie Financiële gegevens bewerken </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Override User Billing Rates at the project level

Wanneer u het factureringstarief van een gebruiker op een project met voeten treedt, kunt u efficiënte data toewijzen en elke datumwaaier heeft een verschillend tarief. Als u geen effectieve datums toewijst, wordt de tariefoverschrijving die u invoert, gebruikt voor de volledige duur van het project om de inkomsten te berekenen.

Om een gebruiker met voeten te treden die tarief voor een project factureert:

1. Ga naar het project u het factureren voor wilt met voeten treden.
1. Klik **Tarieven** in het linkerpaneel. U zou kunnen moeten eerst klikken **tonen Meer**.
1. Klik het **Factureren** lusje als het niet reeds wordt geselecteerd.
1. Klik **toevoegen het FactureringsTarief** > **Nieuwe het FactureringsTarief van de Gebruiker**.

   Het vak Nieuwe factureringssnelheid van gebruiker wordt geopend.

1. Op het **gebied van de Gebruiker**, selecteer de gebruiker u het het factureren tarief voor wilt veranderen.
1. Selecteer de **Valuta** voor de het factureren tariefopheffing.
1. Op het **FactureringsTarief** gebied, ga de eerste het factureren tariefopheffing in.
1. (Facultatief) klik **toevoegen datageffect** om meer het factureren tariefoverschrijvingen toe te voegen.
1. (Voorwaardelijk) als u veelvoudige het facturerings tarief met voeten treedt, specificeer de volgende informatie voor elke rij:

   * **het Facturerings Tarief**: de waarde van het factureringstarief tijdens de gespecificeerde tijdspanne.
   * **Datum van het Begin**: de datum wanneer de het factureren tariefopheffing begint.
   * **Datum van het Eind**: de datum wanneer de het factureren tariefopheffing beëindigt.

   ![&#x200B; het Nieuwe vakje van het Tarief van het Facturerings van de Gebruiker dat efficiënte data &#x200B;](assets/new-user-billing-rate-on-project2.png) toont

   Workfront past het tarief van de opheffingsgebruiker op de uren toe die tijdens deze tijdkaders wanneer het berekenen van opbrengst op het project voorkomen.

   Met Workfront kunt u tussenruimten tussen overschrijvende tijdframes weglaten, maar u ontvangt een waarschuwing om te bevestigen dat dit opzettelijk is.

   U wordt niet vereist om een Datum van het Begin voor het eerste met voeten treden tarief, noch een Datum van het Eind voor het laatste met voeten treden tarief te specificeren.

   Als u slechts één het factureren tariefopheffing ingaat, is dat tarief van toepassing voor de volledige duur van het project. Als u veelvoudige datum-efficiënte overschrijvingen toevoegt, veronderstelt Workfront dat de eerste opheffing op alle uren vóór zijn Einddatum van toepassing is, en de laatste opheffing is op alle uren na zijn Datum van het Begin van toepassing.

   Workfront gaat ervan uit dat de eerste overschrijvingsrente wordt toegepast op alle uren met een datum die ouder is dan de Einddatum van de eerste overschrijving en dat de laatste overschrijvingsrente wordt toegepast op alle uren met een datum die nieuwer is dan de Begindatum van de laatste overschrijving.

   Als een uur vóór de Geplande Datum van het Begin van het project wordt geregistreerd, wordt het zeer eerste het factureringstarief gebruikt.

   Als een uur na de Geplande Datum van de Voltooiing van het project wordt geregistreerd, wordt het zeer laatste het factureringstarief gebruikt.

1. Klik **sparen**.
