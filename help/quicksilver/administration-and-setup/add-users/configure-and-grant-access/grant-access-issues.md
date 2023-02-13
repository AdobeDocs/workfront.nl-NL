---
title: Toegang verlenen tot kwesties
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-beheerder kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot problemen in Workfront te definiëren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3c15f90f-ce87-484d-93a7-9eeb2963a798
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Toegang verlenen tot kwesties

Als beheerder van Adobe Workfront, kunt u een toegangsniveau gebruiken om de toegang van een gebruiker tot kwesties te bepalen, zoals die in [Overzicht van toegangsniveaus](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Voor informatie over het gebruiken van douanetoegangsniveaus om gebruikers&#39; toegang tot andere objecten types in Workfront te beheren, zie [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

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

## Gebruikerstoegang verlenen voor problemen met behulp van een aangepast toegangsniveau

1. Beginnen met het maken of bewerken van het toegangsniveau, zoals wordt uitgelegd in [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik op het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Weergave** of **Bewerken** rechts van Issues en selecteer vervolgens de mogelijkheden die u onder **Uw instellingen nauwkeurig afstellen**.

1. (Optioneel) Als u overerfde machtigingen voor uitgaven van objecten met een hogere classificatie wilt beperken, klikt u op **Aanvullende beperkingen instellen** selecteert u vervolgens **Documenttoegang nooit overerven van projecten, taken, problemen, enzovoort**.

1. (Optioneel) Als u de toegangsinstellingen wilt configureren voor andere objecten en gebieden in het toegangsniveau waaraan u werkt, gaat u verder met een van de artikelen in [Toegang tot Adobe Workfront configureren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), zoals [Toegang verlenen tot taken](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) en [Toegang tot financiële gegevens verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Als u klaar bent, klikt u op **Opslaan**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen. Zie voor meer informatie [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Toegang tot uitgiften per licentietype

Voor informatie over wat de gebruikers in elk toegangsniveau met kwesties kunnen doen, zie de sectie [Problemen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#issues) in het artikel [Beschikbare functionaliteit voor elk objecttype](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Toegang tot gedeelde problemen

Als eigenaar of maker van een uitgave kunt u deze delen met andere gebruikers door hun machtigingen te verlenen, zoals wordt uitgelegd in [Een uitgave delen](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

<!--
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
-->

Wanneer u een object met een andere gebruiker deelt, worden de rechten van de ontvanger op het object bepaald door een combinatie van twee dingen:

* De machtigingen die u aan de ontvanger toekent voor het object
* De instellingen van het toegangsniveau van de ontvanger voor het objecttype

Ook, als toegestaan door hun toegangsniveau, kunnen de gebruikers tot een kwestie door objecten hiërarchie toegang krijgen: als een gebruiker reeds toestemming op het ouderproject of de taak van een kwestie heeft, hebben zij ook toestemming op de kwestie (zie Stap 3 hierboven). Wanneer u een uitgave deelt, kunt u een lijst van de gebruikers zien die toestemmingen aan het hebben geërft.

![](assets/inherited-permissions.png)
