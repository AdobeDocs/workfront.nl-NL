---
title: Toegang verlenen tot rapporten, dashboards en kalenders
user-type: administrator
product-area: system-administration;dashboards;calendars
navigation-topic: configure-access-to-workfront
description: Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot rapporten, dashboards, en kalenders in Workfront te bepalen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 776bb223-3481-4ea9-8049-276b2dec95c5
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Toegang verlenen tot rapporten, dashboards en kalenders

Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot rapporten, dashboards, en kalenders te bepalen, zoals die in [ het overzicht van de Niveaus van de Toegang ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) wordt verklaard.

Deze toegang omvat ook toegang tot externe pagina&#39;s. Voor informatie over Externe Pagina&#39;s, zie [ Toegang van de Verlening tot financiële gegevens ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

>[!NOTE]
>
>* Als u gebruikers toegang tot rapporten, dashboards, en kalenders wilt verlenen, moet u die gebruikers ook toegang tot filters, meningen, en groeperingen geven. Voor instructies, zie [ toegang van de Verlening tot filters, meningen, en groeperingen ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).
>* Wanneer iemand een rapport, een dashboard, of een kalender met een andere gebruiker deelt, worden de rechten van de ontvanger op het bepaald door een combinatie van twee dingen: Het de toegangsniveau dat van de ontvanger voor rapporten, dashboards, en kalenders _plaatst en_ om het even welke toestemmingen die de aandeelhouder voor het rapport, het dashboard, of de kalender verleende
>
>Voor informatie over toestemmingengebruikers kunnen op een rapport, een dashboard, of een kalender verlenen wanneer het delen van het, zie [ rapporten van het Aandeel, dashboards, en kalenders ](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Toegang van gebruikers tot rapporten, dashboards en kalenders configureren met behulp van een aangepast toegangsniveau

1. Beginnen creërend of het uitgeven van het toegangsniveau, zoals die in [ wordt verklaard creeer of wijzig douanetoegangsniveaus ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Mening** of **geef** knoop aan het recht van Rapporten uit, dan selecteer de capaciteiten u onder **wilt verlenen - verbeter uw montages**.

   ![ reports_access.png ](assets/reports-access.png)

   De volgende opties zijn standaard ingeschakeld:

   * **creeer**
   * **Schrapping**
   * **Mening Ingebouwde Rapporten**: Dit moet worden geselecteerd om rapporten te zien die door Workfront worden gebouwd.
   * **Aandeel**
   * **de Rapporten van het Aandeel Openbaar**: De rapporten kunnen openbaar worden gedeeld, door een openbare verbinding met het rapport met iedereen te delen die geen rekening van Workfront heeft. U moet deze optie selecteren om dit deelniveau mogelijk te maken.
   * **Deel Systeem-breed**: De rapporten kunnen met iedereen in het systeem worden gedeeld die een vergunning van Workfront heeft. U moet deze optie selecteren om dit deelniveau mogelijk te maken.

     Voor informatie over het delen van rapporten, dashboards, en kalenders, zie [ rapporten van het Aandeel, dashboards, en kalenders ](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Facultatief) om toegangsmontages voor andere voorwerpen en gebieden in het toegangsniveau te vormen u aan werkt, ga met één van de artikelen voort die in [ worden vermeld toegang tot Adobe Workfront ](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [ toegang van de Verlening tot taken ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [ toegang van de Verlening tot financiële gegevens ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wanneer u wordt gebeëindigd, klik **sparen**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen. Voor meer informatie, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

## Toegang tot rapporten, dashboards en kalenders per licentietype

Voor informatie over welke gebruikers in elk toegangsniveau met kwesties kunnen doen, zie de sectie [ Rapporten ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) in de artikel [ Functionaliteit beschikbaar voor elk objecten type ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Toegang tot gedeelde rapporten, dashboards, en kalenders

Als eigenaar of schepper van een rapport, een dashboard, of een kalender, kunt u het met andere gebruikers delen door hen toestemmingen aan het te verlenen, zoals die in [ rapporten van het Aandeel, dashboards, en kalenders ](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md) worden verklaard.

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
