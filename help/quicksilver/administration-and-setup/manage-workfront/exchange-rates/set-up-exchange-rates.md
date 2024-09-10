---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Wisselkoersen instellen
description: Als Adobe Workfront-beheerder kunt u wisselkoersen instellen in Workfront.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '530'
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

Wisselkoersen beïnvloeden alle financiële elementen in Workfront. De basisvaluta is de standaardvaluta voor alle projecten in het hele systeem, tenzij deze voor een bepaald project of een bepaalde functie wordt overschreven. U kunt ook selecteren om financiële informatie in valuta&#39;s beschikbaar in uw systeem te tonen die verschillend zijn dan de basisvaluta of die van het project wanneer het bekijken van hen in een rapport of een lijst. Voor meer informatie, zie [ de rapporten van financiële gegevens met unieke wisselkoersen ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md) creëren.

Raadpleeg de volgende artikelen voor meer informatie over het overschrijven van de basisvaluta in Workfront voor projecten en taakrollen:

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

1. Klik **Voorkeur van het Project** > **Tarieven van de Uitwisseling.**

1. Klik **toevoegen Valuta.**
1. Typ de naam van de valuta en klik vervolgens op de naam wanneer deze in de vervolgkeuzelijst wordt weergegeven.

1. Geef in het veld Opgeven de koers op voor de valuta die u hebt geselecteerd, aangezien deze betrekking heeft op de valuta die is ingesteld als de basisvaluta in het systeem.
1. (Optioneel) Stel de valuta in als de basis- (standaard)valuta voor Workfront.

   Dit is de valuta die als gebrek voor alle projecten en rapporten door het systeem wordt gebruikt.

1. Klik **sparen** om uw veranderingen te bewaren.

## Gebruikers toestaan de standaardvaluta voor een project te wijzigen

Gebruikers kunnen de standaardvaluta voor een project wijzigen als aan de volgende voorwaarden is voldaan:

* De gebruiker heeft een vergunning van het Plan met de administratieve toegang tot de Tarieven van de Uitwisseling.

  Voor meer informatie, zie [ gebruikers administratieve toegang van de Verlening tot bepaalde gebieden ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Op het Workfront-systeem zijn meerdere valuta&#39;s ingeschakeld.

Voor informatie over hoe de gebruikers de standaardmunt op een bepaald project kunnen veranderen, zie [ Verandering de projectmunt ](../../../manage-work/projects/project-finances/change-project-currency.md).

## Gebruikers toestaan de standaardvaluta voor een taakrol te wijzigen

Gebruikers kunnen de valuta voor een taakrol wijzigen als aan de volgende voorwaarden is voldaan:

* De gebruiker heeft een licentie voor het abonnement met beheertoegang tot taakrollen.

  Voor meer informatie, zie [ gebruikers administratieve toegang van de Verlening tot bepaalde gebieden ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* In het Workfront-systeem zijn meerdere valuta&#39;s ingeschakeld.

Voor informatie over hoe de gebruikers de standaardmunt op een bepaalde baanrol kunnen veranderen, zie [ baanrollen ](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md) creëren en beheren.
