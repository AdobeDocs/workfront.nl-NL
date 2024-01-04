---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Rapporten met financiële gegevens maken met unieke wisselkoersen
description: Als er in Adobe Workfront meerdere wisselkoersen zijn geconfigureerd, kunt u de financiële waarden in rapporten en lijsten zodanig instellen dat deze in een andere valuta dan de standaardvaluta worden weergegeven.
author: Nolan
feature: Reports and Dashboards
exl-id: a0837c70-8330-4c38-98dc-8cf2e7e2e4bd
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# Rapporten met financiële gegevens maken met unieke wisselkoersen

Als er in Adobe Workfront meerdere wisselkoersen zijn geconfigureerd, kunt u de financiële waarden in rapporten en lijsten zodanig instellen dat deze in een andere valuta dan de standaardvaluta worden weergegeven.

>[!IMPORTANT]
>
>Als je in een weergave een andere valuta dan de standaardvaluta selecteert, worden de koppelingen niet meer weergegeven **Meer taken toevoegen** en **Meer problemen toevoegen** onder aan een projectlijst.

Voor informatie over hoe te om de standaardmunt voor een bepaald project te veranderen, zie [De projectvaluta wijzigen](../../../manage-work/projects/project-finances/change-project-currency.md).

Als het verslag projecten met één munt bevat, worden de bedragen in groepen ook weergegeven in de standaardvaluta van het systeem.

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
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

Voordat u alternatieve valuta&#39;s kunt weergeven zoals in deze sectie wordt beschreven, moet de Workfront-beheerder eerst meerdere valuta&#39;s inschakelen en configureren in het gedeelte Setup van Workfront. Zie voor meer informatie [Wisselkoersen instellen](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Financiële waarden toepassen op een rapport {#apply-financial-values-to-a-report}

Financiële waarden tussen valuta&#39;s omzetten bij het werken met rapporten:

1. Ga naar het rapport waar u financiële waarden wilt omzetten in een andere valuta.
1. Klik op de knop **Weergave** vervolgkeuzelijst, klikken **Valuta wijzigen** Selecteer vervolgens een van de volgende valuta&#39;s waarin u de financiële waarden wilt weergeven:

   * Oorspronkelijke valuta van het project
   * Alle overige valuta&#39;s

     >[!TIP]
     >
     >U kunt alleen valuta&#39;s kiezen die eerder in Setup zijn geselecteerd.

   Met deze optie kunt u snel financiële waarden in een rapport omzetten tussen rentewaarden.

   ![Valuta wijzigen](assets/qs-change-currency-2022-350x257.png)

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: drafted this tip because I think this is confusing; this is in the step above.)</p>
   -->

   <!--
   <note type="tip">
   You can also select the Change Currency option to convert financial values in other lists.
   <br>
   <img src="assets/nwe-change-currency-new-lists-350x219.png" style="width: 350;height: 219;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   <br>
   <br>
   </note>
   -->

## De standaardvaluta weergeven voor meerdere projecten met verschillende valuta&#39;s

Wanneer u de munt op het projectniveau aanpast en u informatie van alle projecten in het zelfde rapport wilt tonen, bestaan de volgende scenario&#39;s:

* Als u een rapport maakt dat financiële informatie ophaalt uit twee of meer projecten waarop verschillende valuta&#39;s zijn toegepast, geeft het samenvattingsoverzicht standaard de standaardvaluta van het systeem weer, zoals geselecteerd door de Workfront-beheerder.
* Als u een rapport maakt voor twee of meer projecten die dezelfde valuta hebben, maar verschillen van de standaardvaluta van het systeem, worden de bedragen in de groepen weergegeven met de standaardvaluta van het systeem.
* Als u een rapport maakt voor twee of meer projecten met taaktaken die zijn gekoppeld aan een valutaoverschrijving, converteert Workfront de financiële informatie van de overschreven valutakoersen van de rol naar de valuta van het project (wanneer u de oorspronkelijke valuta van het project in de weergave selecteert) of naar een andere valuta die u selecteert wanneer u het rapport weergeeft. Voor informatie over het overschrijven van de valuta van een functie raadpleegt u [Taakrollen maken en beheren](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Twee projecten met aangepaste valuta&#39;s weergeven in een rapport:

1. Maak twee projecten met verschillende toegepaste valuta.

   ![](assets/qs-currency-350x217.png)

1. Log uren op beide projecten.

   Voor meer informatie over logboektijd, zie [Logtijd](../../../timesheets/create-and-manage-timesheets/log-time.md).

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png)en klik vervolgens op **Rapportage**.
1. Klikken **Nieuw rapport** vervolgens **Projectrapport**.
1. In de **Kolommen (weergave)** tabblad, voegt u een **Werkelijke kosten** kolom en vat het samen door **Som**.

   Voor informatie over hoe te om een kolom tot stand te brengen, zie [Overzicht van weergaven in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. In de **Groepen** tabblad, een **Geplande afsluitdatum** groeperen.

   Voor informatie over het maken van een groep raadpleegt u [Overzicht van groepen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. In de **Filters** tab, filter toevoegen voor **Projectnaam** en selecteert u de twee projecten met de verschillende valuta&#39;s.

   Voor informatie over het maken van een filter raadpleegt u [Overzicht van filters](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klikken **Opslaan + Sluiten**.

   Het totaal van **Werkelijke kosten** wordt in de Groepering weergegeven met behulp van de standaardvaluta van het systeem, ongeacht de valuta van de projecten in het rapport.

   ![Valuta weergegeven in groep](assets/qs-currency-displayed-in-groupings-2022-350x292.png)

   Als de twee projecten verschillende valuta&#39;s van elkaar hebben, verschijnt de systeemstandaardvaluta ook in de Groepering van het rapport.

## Toon de Valuta van het Project in een rapport op het projectniveau

Als een groepering op een taak of een uurlijst binnen een project wordt toegepast, worden de sommen in het groeperen getoond in de munt van het project.

1. Maak een project met een aangepaste valuta, anders dan de standaardvaluta van het systeem.
1. Ga naar het project en zorg ervoor dat het uren omvat die voor taken zijn geregistreerd.

   Voor meer informatie over logboektijd, zie [Logtijd](../../../timesheets/create-and-manage-timesheets/log-time.md).

   >[!NOTE]
   >
   >De taken zouden aan gebruikers of baanrollen met Tarief per de kostentarieven van uren moeten worden toegewezen.

1. Klikken **Taken**.
1. Breid uit **Weergave** vervolgkeuzelijst en selecteert u **Nieuwe weergave**.
1. Toevoegen **Werkelijke kosten** in de nieuwe Mening als nieuwe kolom, en vat het door samen **Som**.
1. Klikken **Gereed** en klik vervolgens op **Weergave opslaan**.
1. Breid uit **Groepering** vervolgkeuzelijst en selecteert u **Nieuwe groepering**.
1. Toevoegen **Werkelijke afsluitdatum** in de nieuwe groep als een nieuw veld, klikt u op **Groepering opslaan**.

   De **Werkelijke kosten** de kolom vat in de nieuwe Groepering samen en toont het totaal in de valuta van het project.

## Rapporten bewerken met unieke valuta&#39;s

De financiële gebieden in een rapport zijn niet editable tot u het rapport verandert plaatsend om de originele munt voor projecten te tonen.

Een financieel veld in een rapport online bewerken:

1. Navigeer naar een rapport.

   >[!NOTE]
   >
   >Als de standaardvaluta niet wordt weergegeven voor een lijst in een ander gebied, kunt u de weergave bewerken en de standaardvaluta weergeven.\
   >Zie de sectie in dit artikel voor informatie over het wijzigen van de valuta in een weergave [Financiële waarden toepassen op een rapport](#apply-financial-values-to-a-report).

1. Klikken **Handelingen rapporteren** selecteert u vervolgens **Bewerken**.
1. Klikken **Rapportinstellingen**.
1. Klik op de knop **Standaardvaluta** vervolgkeuzelijst, selecteert u vervolgens **Oorspronkelijke valuta van het project**.

   ![](assets/qs-report-settings-default-currency-350x370.png)

1. Klikken **Gereed**.
