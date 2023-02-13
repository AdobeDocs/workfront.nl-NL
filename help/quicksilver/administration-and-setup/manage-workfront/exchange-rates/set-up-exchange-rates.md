---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Als Adobe Workfront-beheerder kunt u wisselkoersen instellen in Workfront.
description: Wisselkoersen instellen
feature: System Setup and Administration
role: Admin
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '560'
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

Wisselkoersen hebben invloed op alle financiële elementen in Workfront. De basisvaluta is de standaardvaluta voor alle projecten in het hele systeem, tenzij deze voor een bepaald project of een bepaalde functie wordt overschreven. U kunt ook selecteren om financiële informatie in valuta&#39;s beschikbaar in uw systeem te tonen die verschillend zijn dan de basisvaluta of die van het project wanneer het bekijken van hen in een rapport of een lijst. Zie voor meer informatie [Rapporten met financiële gegevens maken met unieke wisselkoersen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Raadpleeg de volgende artikelen voor meer informatie over het overschrijven van de basisvaluta in Workfront voor projecten en taakrollen:

* [De projectvaluta wijzigen](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Taakrollen maken en beheren](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

De manier waarop u wisselkoersen instelt, bepaalt of gebruikers de wisselkoersen voor een bepaald project kunnen wijzigen.

>[!IMPORTANT]
>
>De wisselkoersen in Workfront zijn niet dynamisch; de waarde die u instelt, moet worden bijgewerkt wanneer er wisselkoerswijzigingen optreden.

## Toegangsvereisten

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Wisselkoersen instellen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Projectvoorkeuren** > **Wisselkoersen.**

1. Klikken **Valuta toevoegen.**
1. Typ de naam van de valuta en klik vervolgens op de naam wanneer deze in de vervolgkeuzelijst wordt weergegeven.

1. Geef in het veld Opgeven de koers op voor de valuta die u hebt geselecteerd, aangezien deze betrekking heeft op de valuta die is ingesteld als de basisvaluta in het systeem.
1. (Optioneel) Stel de valuta in als de basis- (standaard)valuta voor Workfront.

   Dit is de valuta die als gebrek voor alle projecten en rapporten door het systeem wordt gebruikt.

1. Klikken **Opslaan** om uw wijzigingen op te slaan.

## Gebruikers toestaan de standaardvaluta voor een project te wijzigen

Gebruikers kunnen de standaardvaluta voor een project wijzigen als aan de volgende voorwaarden is voldaan:

* De gebruiker heeft een vergunning van het Plan met de administratieve toegang tot de Tarieven van de Uitwisseling.

   Zie voor meer informatie [Gebruikers administratieve toegang verlenen tot bepaalde gebieden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Op het Workfront-systeem zijn meerdere valuta&#39;s ingeschakeld.

Voor informatie over hoe de gebruikers de standaardmunt op een bepaald project kunnen veranderen, zie [De projectvaluta wijzigen](../../../manage-work/projects/project-finances/change-project-currency.md).

## Gebruikers toestaan de standaardvaluta voor een taakrol te wijzigen

Gebruikers kunnen de valuta voor een taakrol wijzigen als aan de volgende voorwaarden is voldaan:

* De gebruiker heeft een licentie voor het abonnement met beheertoegang tot taakrollen.

   Zie voor meer informatie [Gebruikers administratieve toegang verlenen tot bepaalde gebieden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* In het Workfront-systeem zijn meerdere valuta&#39;s ingeschakeld.

Voor informatie over hoe gebruikers de standaardvaluta voor een bepaalde taakrol kunnen wijzigen, raadpleegt u [Taakrollen maken en beheren](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
