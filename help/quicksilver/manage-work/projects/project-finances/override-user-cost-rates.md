---
content-type: overview
product-area: projects
navigation-topic: financials
title: De Tarieven van de Kosten van de Gebruiker op het Niveau van het Project met voeten treden
description: In dit artikel wordt beschreven hoe u de kostentarieven voor systeemgebruikers voor een project kunt overschrijven.
author: Lisa
feature: Work Management
exl-id: ff1110fd-2d24-48a7-8000-712e551ca61a
source-git-commit: e3d4ffe2d42f9de3000df0ba1a924ca36fea9248
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# Override user cost rates at the project level

U kunt specificeren wat het kostentarief voor een gebruiker op een specifiek project is. Dit op projectniveau kostentarief treedt het kostentarief op het systeemniveau voor deze gebruiker met voeten. Workfront gebruikt het kostenpercentage op projectniveau van de functie om kosten te berekenen in plaats van het kostenpercentage op systeemniveau te gebruiken.

In dit artikel wordt beschreven hoe u de kostentarieven voor systeemgebruikers voor een project kunt overschrijven.

Voor meer informatie over het berekenen van kosten op het project, zie [ Overzicht van opbrengst en kostenhiërarchie ](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) en [ de kosten van het Spoor ](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

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
   <td>Machtigingen beheren voor het project met onder andere Kostentarieven bewerken </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

De gebruiker moet de **tariefopheffing van Kosten toegestaan** gebied hebben dat op hun gebruikersprofiel wordt toegelaten. Wanneer een gebruiker het toegelaten gebied van de kostenopheffing niet heeft, worden de kosten met voeten getreden niet toegestaan voor die gebruiker op om het even welk project, en het systeem gebruikt het tarief op het gebruikersprofiel om kosten te berekenen.

Voor meer informatie, zie [ het profiel van een gebruiker ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

## Override user cost rates at the project level

1. Ga naar het project u kostentarieven voor wilt met voeten treden.
1. Klik **Tarieven** in het linkerpaneel. U zou kunnen moeten eerst klikken **tonen Meer**.
1. Klik het **lusje van Kosten** als het niet reeds wordt geselecteerd.
1. Klik **toevoegen Kostentarief** > **Nieuwe Kostentarief van de Gebruiker**.

   Het vak Nieuwe kostenpercentage gebruiker wordt geopend.

1. Op het **gebied van de Gebruiker**, selecteer de gebruiker u het kostentarief voor wilt veranderen.
1. Selecteer de **Valuta** voor de opheffing van het kostentarief.
1. Op het **gebied van het Tarief van 0} Kosten {, ga de eerste kostentariefopheffing in.**
1. (Facultatief) klik **toevoegen datumeffectief tarief** om meer kostentariefoverschrijvingen toe te voegen.

   >[!NOTE]
   >
   >Als u één enkele tariefopheffing ingaat, is het van toepassing voor het volledige leven van het project.
   >Als u verschillende tarieven in tijd wilt hebben, kunt u veelvoudige datum-efficiënte overschrijvingen toevoegen.

1. (Voorwaardelijk) als u veelvoudige kostentarief met voeten treedt toevoegt, specificeer de volgende informatie voor elke rij:

   * **Tarief van Kosten**: de waarde van het kostentarief tijdens de gespecificeerde tijdspanne.
   * **Datum van het Begin**: de datum wanneer de kostentariefopheffing begint.
   * **Datum van het Eind**: de datum wanneer de kostentariefopheffing beëindigt.

   ![ het Nieuwe vakje van de Tarief van de Kosten van de Gebruiker die efficiënte data tonen ](assets/new-user-cost-rate-box.png)

   Workfront past het tarief van de opheffingsbaan op de uren toe die tijdens deze tijdkaders voorkomen wanneer het berekenen van kosten op het project.

   Met Workfront kunt u tussenruimten tussen overschrijvende tijdframes weglaten, maar u ontvangt een waarschuwing om te bevestigen dat dit opzettelijk is.

   U wordt niet vereist om een Datum van het Begin voor het eerste met voeten treden tarief, noch een Datum van het Eind voor het laatste met voeten treden tarief te specificeren.

   Wij adviseren dat u het Standaardtarief voor het eerste met voeten getreden tarief gebruikt.

   Workfront gaat ervan uit dat de eerste overschrijvingsrente wordt toegepast op alle uren met een datum die ouder is dan de Einddatum van de eerste overschrijving en dat de laatste overschrijvingsrente wordt toegepast op alle uren met een datum die nieuwer is dan de Begindatum van de laatste overschrijving.

   Als een uur vóór de Geplande Datum van het Begin van het project wordt geregistreerd, wordt het zeer eerste kostentarief gebruikt.

   Als een uur na de Geplande Datum van de Voltooiing van het project wordt geregistreerd, wordt het zeer laatste kostentarief gebruikt.

1. Klik **sparen**.
