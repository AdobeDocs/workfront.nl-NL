---
title: Toegang verlenen tot rapporten, dashboards en kalenders
user-type: administrator
product-area: system-administration;dashboards;calendars
navigation-topic: configure-access-to-workfront
description: Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot rapporten, dashboards, en kalenders in Workfront te bepalen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 776bb223-3481-4ea9-8049-276b2dec95c5
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Toegang verlenen tot rapporten, dashboards en kalenders

Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot rapporten, dashboards, en kalenders te bepalen, zoals die in [Overzicht van toegangsniveaus](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Deze toegang omvat ook toegang tot externe pagina&#39;s. Voor informatie over externe pagina&#39;s raadpleegt u [Toegang tot financiële gegevens verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

>[!NOTE]
>
>* Als u gebruikers toegang tot rapporten, dashboards, en kalenders wilt verlenen, moet u die gebruikers ook toegang tot filters, meningen, en groeperingen geven. Zie voor instructies [Toegang verlenen tot filters, weergaven en groepen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).
>* Wanneer iemand een rapport, dashboard, of kalender met een andere gebruiker deelt, worden de rechten van de ontvanger op het bepaald door een combinatie van twee dingen: De het toegangsniveau van de ontvanger het plaatsen voor rapporten, dashboards, en kalenders _en_ om het even welke toestemmingen die de deler voor het rapport, het dashboard of de kalender verleende
>
>Voor informatie over toestemmingen kunnen de gebruikers op een rapport, een dashboard, of een kalender verlenen wanneer het delen van het, zie [Rapporten, dashboards en kalenders delen](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

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
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Gebruikerstoegang tot rapporten, dashboards, en kalenders vormen gebruikend een niveau van de douanetoegang

1. Beginnen met het maken of bewerken van het toegangsniveau, zoals wordt uitgelegd in [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik op het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Weergave** of **Bewerken** rechts van Rapporten selecteert u vervolgens de mogelijkheden die u onder **Uw instellingen nauwkeurig afstellen**.

   ![reports_access.png](assets/reports-access.png)

   De volgende opties zijn standaard ingeschakeld:

   * **Maken**
   * **Verwijderen**
   * **Ingebouwde rapporten weergeven**: Dit moet worden geselecteerd om rapporten te zien die door Workfront worden opgesteld.
   * **Delen**
   * **Rapporten openbaar delen**: Rapporten kunnen openbaar worden gemaakt door een openbare link naar het rapport te delen met iedereen die geen Workfront-account heeft. U moet deze optie selecteren om dit deelniveau mogelijk te maken.
   * **Delen op systeemniveau**: Rapporten kunnen worden gedeeld met iedereen in het systeem die een Workfront-licentie heeft. U moet deze optie selecteren om dit deelniveau mogelijk te maken.

      Voor informatie over het delen van rapporten, dashboards, en kalenders raadpleegt u [Rapporten, dashboards en kalenders delen](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Optioneel) Als u de toegangsinstellingen wilt configureren voor andere objecten en gebieden in het toegangsniveau waaraan u werkt, gaat u verder met een van de artikelen in [Toegang tot Adobe Workfront configureren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [Toegang verlenen tot taken](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [Toegang tot financiële gegevens verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Als u klaar bent, klikt u op **Opslaan**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen. Zie voor meer informatie [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Toegang tot rapporten, dashboards en kalenders per licentietype

Voor informatie over wat de gebruikers in elk toegangsniveau met kwesties kunnen doen, zie de sectie [Rapporten](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) in het artikel [Beschikbare functionaliteit voor elk objecttype](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Toegang tot gedeelde rapporten, dashboards, en kalenders

Als eigenaar of maker van een rapport, dashboard, of kalender, kunt u het met andere gebruikers delen door hen toestemmingen aan het te verlenen, zoals die in [Rapporten, dashboards en kalenders delen](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

Wanneer u een object met een andere gebruiker deelt, worden de rechten van de ontvanger op het object bepaald door een combinatie van twee dingen:

* De machtigingen die u aan de ontvanger toekent voor het object
* De instellingen van het toegangsniveau van de ontvanger voor het objecttype
