---
title: Toegang tot financiële gegevens verlenen
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-beheerder kunt u de toegang van een gebruiker tot financiële gegevens in Workfront definiëren via hun toegangsniveau.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bf4a37ee-9435-4c1c-b18c-a7338a548ab7
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# Toegang tot financiële gegevens verlenen

Als beheerder van Adobe Workfront, kunt u de toegang van een gebruiker tot het volgende door het de toegangsniveau van de gebruiker bepalen, zoals die in [Overzicht van toegangsniveaus](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md):

* Financiële informatie over projecten in Workfront
* Informatie over het budgetteren van bronnen in de hulpmiddelen voor het plannen van bronnen

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

## Overwegingen bij het verlenen van toegang tot financiële gegevens

Houd rekening met het volgende wanneer u gebruikers toegang geeft tot financiële gegevens in Workfront:

* Een gebruiker wiens toegangsniveau toegang tot financiële gegevens niet toestaat kan geen risico voor een project tot stand brengen. Zie voor meer informatie [Risico&#39;s maken en bewerken voor projecten](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
* U kunt een toegangsniveau ook gebruiken om te bepalen welke activiteiten van het Beheer van Middelen een gebruiker aan begroting of meningsmiddeltoewijzing kan aanwenden. Zie voor meer informatie [Toegang verlenen tot beheer van hulpbronnen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Gebruikerstoegang tot financiële gegevens configureren met behulp van een aangepast toegangsniveau

1. Beginnen met het maken of bewerken van het toegangsniveau, zoals wordt uitgelegd in [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik op het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Weergave** of **Bewerken** rechts van Financiële gegevens en selecteert u vervolgens de mogelijkheden die u onder **Uw instellingen nauwkeurig afstellen**.

   ![](assets/financial-data-fine-tune-nwe.png)

1. (Optioneel) In het dialoogvenster **Beheertoegang toestaan voor** selecteert u de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Wisselkoersen</td> 
      <td> <p>Voeg nieuwe valuta toe in Workfront.</p> <p>Zonder deze toegang kan de gebruiker alleen een bestaande valuta toevoegen aan een project dat hij of zij maakt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uitgaven</td> 
      <td> <p>Alle uitgaven weergeven voor objecten in Workfront.</p> <p>Hierdoor kan de gebruiker geen nieuwe kostentypen maken.</p> <p>Zonder deze toegang kan de gebruiker alleen het volgende weergeven:</p> 
       <ul> 
        <li>Uitgaven voor projecten, taken of kwesties die zij beheren</li> 
        <li>Hun eigen kosten</li> 
        <li>De kosten van hun ondergeschikten</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Als u de toegangsinstellingen wilt configureren voor andere objecten en gebieden in het toegangsniveau waaraan u werkt, gaat u verder met een van de artikelen in [Toegang tot Adobe Workfront configureren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) zoals [Toegang verlenen tot taken](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Als u klaar bent, klikt u op **Opslaan**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen. Zie voor meer informatie [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Toegang tot gedeelde financiële informatie

U kunt financiële informatie over een project, een taak, of een kwestie met andere gebruikers delen door hen toestemmingen aan het te verlenen, zoals die in worden verklaard [Financiële machtigingen delen op een object](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Wanneer u een object met een andere gebruiker deelt, worden de rechten van de ontvanger op het object bepaald door een combinatie van twee dingen:

* De machtigingen die u aan de ontvanger toekent voor het object
* De instellingen van het toegangsniveau van de ontvanger voor het objecttype

## Toegang tot financiële informatie per licentietype

Voor informatie over wat de gebruikers in elk toegangsniveau met financiële informatie kunnen doen, zie de sectie [Financiële gegevens](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) in het artikel [Beschikbare functionaliteit voor elk objecttype](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Toegang tot financiële informatie door

De volgende informatie kan u helpen begrijpen hoe te om de het niveaumontages van de Toegang te gebruiken om gebruikers&#39; toegang tot financiële gegevens te controleren.

### Geen toegang

Een gebruiker zonder toegang tot financiële gegevens heeft geen toegang tot:

* Sectie Financiën onder Project en Taakobjecten
* Bedrijfscase
* Factureringstarieven en factureringsgegevens
* Kosten per uur en facturering per uur bij gebruikersvoorkeuren

   U kunt dit configureren met het tandwielpictogram ![](assets/gear-icon-settings.png) op de knop Weergeven in stap 4 hierboven.

* Kosten per uur en facturering per uur op taakrollen

   U kunt dit configureren met het tandwielpictogram ![](assets/gear-icon-settings.png) op de knop Weergeven in stap 4 hierboven.

### Toegang weergeven

Een gebruiker met View-toegang tot financiële gegevens kan het volgende weergeven (niet bewerken):

* Sectie Financiën onder Project en Taakobjecten
* Bedrijfscase
* Factureringstarieven en factureringsgegevens
* Kosten per uur en facturering per uur bij gebruikersvoorkeuren

   U kunt dit configureren met het tandwielpictogram ![](assets/gear-icon-settings.png) op de knop Weergeven in stap 4 hierboven.

* Kosten per uur en facturering per uur op taakrollen

   U kunt dit configureren met het tandwielpictogram ![](assets/gear-icon-settings.png) op de knop Weergeven in stap 4 hierboven.

### Toegang bewerken

Een gebruiker met Edit toegang tot financiële gegevens kan het volgende bekijken en uitgeven:

* Sectie Financiën onder Project en Taakobjecten
* Bedrijfscase
* Factureringstarieven en factureringsgegevens
* Kosten per uur en facturering per uur bij gebruikersvoorkeuren

   U kunt dit configureren met het tandwielpictogram ![](assets/gear-icon-settings.png) op de knop Bewerken in stap 4 hierboven.

* Kosten per uur en facturering per uur op taakrollen

   U kunt dit configureren met het tandwielpictogram ![](assets/gear-icon-settings.png) op de knop Bewerken in stap 4 hierboven.
