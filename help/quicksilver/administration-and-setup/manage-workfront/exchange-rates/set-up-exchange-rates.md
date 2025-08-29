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
source-git-commit: dc820b4012fec494ce5ebb1baefb4ee0df214916
workflow-type: tm+mt
source-wordcount: '647'
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

Wisselkoersen beïnvloeden alle financiële elementen in Workfront. De basisvaluta is de standaardvaluta voor alle projecten in het hele systeem, tenzij deze voor een bepaald project of een bepaalde functie wordt overschreven. De huidige basis of de standaardmunt wordt vermeld met een pictogram ![ Standaard muntpictogram ](assets/default-icon.png) in de lijst. U kunt ook selecteren om financiële informatie in valuta&#39;s beschikbaar in uw systeem te tonen die verschillend zijn dan de basisvaluta of die van het project wanneer het bekijken van hen in een rapport of een lijst. Voor meer informatie, zie [ de rapporten van financiële gegevens met unieke wisselkoersen ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md) creëren.

Raadpleeg de volgende artikelen voor meer informatie over het overschrijven van de basisvaluta in Workfront voor projecten en functies:

* [ verander de projectmunt ](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Taakrollen maken en beheren](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

De manier waarop u wisselkoersen instelt, bepaalt of gebruikers de wisselkoersen voor een bepaald project kunnen wijzigen.

>[!IMPORTANT]
>
>De wisselkoersen in Workfront zijn niet dynamisch. De waarde die u instelt, moet worden bijgewerkt wanneer er wisselkoerswijzigingen optreden.

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
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

     De nieuwe standaardvaluta wordt bijgewerkt met het pictogram.

     >[!NOTE]
     >
     >De standaardvaluta wordt altijd als eerste in de lijst weergegeven, ongeacht hoe de lijst wordt gesorteerd.

1. (Facultatief) om een munt te schrappen, selecteer de controledoos naast de muntnaam en selecteer **Schrapping** in de actiebar bij de bodem van het scherm. U kunt de standaardvaluta niet verwijderen.

## Gebruikers toestaan de standaardvaluta voor een project te wijzigen

Gebruikers kunnen de standaardvaluta voor een project wijzigen als aan de volgende voorwaarden is voldaan:

* De gebruiker heeft een Standaard of vergunning van het Plan met de administratieve toegang tot de Tarieven van de Uitwisseling.

  Voor meer informatie, zie [ gebruikers administratieve toegang van de Verlening tot bepaalde gebieden ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Op het Workfront-systeem zijn meerdere valuta&#39;s ingeschakeld.

Voor informatie over hoe de gebruikers de standaardmunt op een bepaald project kunnen veranderen, zie [ Verandering de projectmunt ](../../../manage-work/projects/project-finances/change-project-currency.md).

## Gebruikers toestaan de standaardvaluta voor een taakrol te wijzigen

Gebruikers kunnen de valuta voor een taakrol wijzigen als aan de volgende voorwaarden is voldaan:

* De gebruiker heeft een Standard- of Plan-licentie met beheertoegang tot Job Roles.

  Voor meer informatie, zie [ gebruikers administratieve toegang van de Verlening tot bepaalde gebieden ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* In het Workfront-systeem zijn meerdere valuta&#39;s ingeschakeld.

Voor informatie over hoe de gebruikers de standaardmunt op een bepaalde baanrol kunnen veranderen, zie [ baanrollen ](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md) creëren en beheren.


<!--The default currency is the currency that is used as the default for all projects and reports throughout the system. The current default is indicated with an icon ![Default currency icon](assets/default-icon.png).-->
