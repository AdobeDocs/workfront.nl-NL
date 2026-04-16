---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Wisselkoersen instellen
description: Wisselkoersen beïnvloeden alle financiële elementen in Workfront. De basisvaluta is de standaardvaluta voor alle projecten in het hele systeem.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: dc71072107ce80f6cb9033fcb17fe4ac74d5af18
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Wisselkoersen instellen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Als Adobe Workfront-beheerder kunt u wisselkoersen instellen in Workfront. Dit omvat het volgende:

* De standaardvaluta voor het Workfront-systeem instellen
* Opwaardering van de wisselkoersen in Workfront in overeenstemming met de huidige wisselkoersen
* De wisselkoersen voor meerdere valuta&#39;s configureren (hierdoor kunnen gebruikers een standaardvaluta kiezen voor afzonderlijke projecten)

Wisselkoersen beïnvloeden alle financiële elementen in Workfront. De basisvaluta is de standaardvaluta voor alle projecten en rapporten in het hele systeem, tenzij deze voor een bepaald project of een bepaalde functie wordt overschreven. De huidige basis of de standaardmunt wordt vermeld met een pictogram ![ Standaard muntpictogram ](assets/default-icon.png) in de lijst. U kunt ook selecteren om financiële informatie in valuta&#39;s beschikbaar in uw systeem te tonen die verschillend zijn dan de basisvaluta of die van het project wanneer het bekijken van hen in een rapport of een lijst. Voor meer informatie, zie [ de rapporten van financiële gegevens met unieke wisselkoersen ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md) creëren.

Raadpleeg de volgende artikelen voor meer informatie over het overschrijven van de basisvaluta in Workfront voor projecten en functies:

* [ verander de projectmunt ](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Taakrollen maken en beheren](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

De manier waarop u wisselkoersen instelt, bepaalt of gebruikers de wisselkoersen voor een bepaald project kunnen wijzigen.

>[!IMPORTANT]
>
>De wisselkoersen in Workfront zijn niet dynamisch. De waarde die u instelt, moet worden bijgewerkt wanneer er wisselkoerswijzigingen optreden.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Voor het instellen van wisselkoersen: elk Workfront- of workflowpakket</p>
       <p>Effectieve datums toepassen op wisselkoersen: Workflow Ultimate-pakket</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>Systeembeheerder</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Wisselkoersen instellen

{{step-1-to-setup}}

1. Klik **Voorkeur van het Project** > **Tarieven van de Uitwisseling**.
1. Klik **toevoegen munt**.
1. In **voeg munt** doos toe, begin typend de naam van de munt, dan klik het wanneer het in de drop-down lijst verschijnt.
1. Op het **Wisselkoers** gebied, ga het tarief voor de munt in die u selecteerde, vergeleken met de munt die als basismunt in het systeem wordt geplaatst.
1. Klik **toevoegen** om de nieuwe munt en zijn wisselkoers toe te voegen.
1. (Optioneel) Voer een van de volgende handelingen uit als u de basisvaluta (de standaardvaluta) wilt wijzigen:

   * Selecteer de controledoos naast de valutanaam en selecteer **maak Gebrek** in de actiebar bij de bodem van het scherm.
   * Beweeg over de muntnaam en klik **Meer** menu dat verschijnt. Dan, uitgezochte **maak Gebrek**.

     De nieuwe standaardmunt wordt bijgewerkt met het pictogram van de pictogram ![ Standaardmunt ](assets/default-icon.png).

     >[!NOTE]
     >
     >De standaardvaluta wordt altijd als eerste in de lijst weergegeven, ongeacht hoe de lijst wordt gesorteerd.

1. (Facultatief) om een munt te schrappen, selecteer de controledoos naast de muntnaam en selecteer **Schrapping** in de actiebar bij de bodem van het scherm. U kunt de standaardvaluta niet verwijderen.

## Ingangsdata voor de wisselkoersen van een valuta instellen

Effectieve datums voor de wisselkoersen van een valuta zijn zodanig geconfigureerd dat een koerswaarde op een bepaalde datum eindigt en een andere koers begint. De wisselkoers voor de correcte datum wordt vervolgens in de financiële berekeningen gebruikt.

{{step-1-to-setup}}

1. Klik **Voorkeur van het Project** > **Tarieven van de Uitwisseling**.
1. Selecteer een munt in de lijst, en klik **beheert data** op de actiebar.
1. Voor **(muntnaam) de datum efficiënte tarieven** dialoog, kies een **Datum van het Eind** voor de huidige wisselkoers.

   of

   Kies de Datum van het a **Begin** voor de nieuwe wisselkoers.

   De eerste wisselkoers heeft geen begindatum en de laatste koers heeft geen einddatum. Sommige datums worden automatisch toegevoegd. Als de eerste koers bijvoorbeeld geen einddatum heeft en u een wisselkoers toevoegt met een begindatum van 1 december 2025, wordt een einddatum van 30 november 2025 toegevoegd aan de eerste koers, zodat er geen hiaten bestaan.

   ![ de efficiënte dialoog van de Uitwisseling van de Datum ](assets/euro-date-effective-rates.png)

1. Typ de nieuwe **het tarief van de Uitwisseling** waarde.
1. (Facultatief) klik **toevoegen datumefficiënte tarief** om meer wisselkoersen met efficiënte data voor deze munt toe te voegen.
1. Klik **sparen**.

## Gebruikers toestaan de standaardvaluta voor een project te wijzigen

Gebruikers kunnen de standaardvaluta voor een project wijzigen als aan de volgende voorwaarden is voldaan:

* De gebruiker heeft een Standaard of vergunning van het Plan met administratieve toegang tot de Tarieven van de Uitwisseling.

  Voor meer informatie, zie [ gebruikers administratieve toegang van de Verlening tot bepaalde gebieden ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Op het Workfront-systeem zijn meerdere valuta&#39;s ingeschakeld.

Voor informatie over hoe de gebruikers de standaardmunt op een bepaald project kunnen veranderen, zie [ Verandering de projectmunt ](../../../manage-work/projects/project-finances/change-project-currency.md).

## Gebruikers toestaan de standaardvaluta voor een taakrol te wijzigen

Gebruikers kunnen de valuta voor een taakrol wijzigen als aan de volgende voorwaarden is voldaan:

* De gebruiker heeft een Standard- of Plan-licentie met beheertoegang tot Job Roles.

  Voor meer informatie, zie [ gebruikers administratieve toegang van de Verlening tot bepaalde gebieden ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* In het Workfront-systeem zijn meerdere valuta&#39;s ingeschakeld.

Voor informatie over hoe de gebruikers de standaardmunt op een bepaalde baanrol kunnen veranderen, zie [ baanrollen ](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md) creëren en beheren.



