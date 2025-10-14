---
title: Toegang tot financiële gegevens verlenen
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-beheerder kunt u de toegang van een gebruiker tot financiële gegevens in Workfront definiëren via hun toegangsniveau.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bf4a37ee-9435-4c1c-b18c-a7338a548ab7
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 0%

---

# Toegang tot financiële gegevens verlenen

{{highlighted-preview}}

Als beheerder van Adobe Workfront, kunt u de toegang van een gebruiker tot het volgende door het de toegangsniveau van de gebruiker bepalen, zoals die in [&#x200B; wordt verklaard het overzicht van de Niveaus van de Toegang &#x200B;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md):

* Financiële informatie over projecten in Workfront
* Informatie over het budgetteren van bronnen in de hulpmiddelen voor het plannen van bronnen

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
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw beheerder van Workfront als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override=""> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Overwegingen bij het verlenen van toegang tot financiële gegevens

Houd rekening met het volgende wanneer u gebruikers toegang geeft tot financiële gegevens in Workfront:

* Een gebruiker van wie het toegangsniveau toegang tot financiële gegevens niet toestaat kan geen risico voor een project tot stand brengen. Voor meer informatie, zie [&#x200B; risico&#39;s op projecten &#x200B;](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md) creëren en uitgeven.
* U kunt een toegangsniveau ook gebruiken om te bepalen welke activiteiten van het Beheer van Middelen een gebruiker aan begroting of meningsmiddeltoewijzing kan aanwenden. Voor informatie, zie [&#x200B; toegang van de Verlening tot het Beheer van het Middel &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Gebruikerstoegang tot financiële gegevens configureren met behulp van een aangepast toegangsniveau

1. Beginnen creërend of het uitgeven van het toegangsniveau, zoals die in [&#x200B; wordt verklaard creeer of wijzig douanetoegangsniveaus &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Mening** of **geef** knoop aan het recht van Financiële Gegevens uit, dan selecteer de capaciteiten u onder **wilt verlenen - verbeter uw montages**.

   ![](assets/financial-data-fine-tune-nwe.png)

1. (Facultatief) in **sta administratieve toegang voor** gebied toe, selecteer de volgende opties:

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

1. (Facultatief) om toegangsmontages voor andere voorwerpen en gebieden op het toegangsniveau te vormen u aan werkt, ga met één van de artikelen voort die in [&#x200B; worden vermeld toegang tot Adobe Workfront &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) zoals [&#x200B; toegang van de Verlening tot taken &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Wanneer u wordt gebeëindigd, klik **sparen**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen. Voor meer informatie, zie [&#x200B; het profiel van een gebruiker &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

## Toegang tot gedeelde financiële informatie

U kunt financiële informatie over een project, een taak, of een kwestie met andere gebruikers delen door hen toestemmingen aan het te verlenen, zoals die in [&#x200B; worden verklaard de financiële toestemmingen van het Aandeel op een voorwerp &#x200B;](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

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

Voor informatie over welke gebruikers in elk toegangsniveau met financiële informatie kunnen doen, zie de sectie [&#x200B; Financiële gegevens &#x200B;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) in de artikel [&#x200B; Functionaliteit beschikbaar voor elk objecten type &#x200B;](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Toegang tot financiële informatie door

De volgende informatie kan u helpen begrijpen hoe te om de het niveaumontages van de Toegang te gebruiken om gebruikers&#39; toegang tot financiële gegevens te controleren.

### Geen toegang

Een gebruiker zonder toegang tot financiële gegevens heeft geen toegang tot het volgende:

* Sectie Financiën onder Project en Taakobjecten
* Bedrijfscase
* Factureringstarieven en factureringsgegevens
* <span class="preview"> kaarten van het Tarief </span>
* Kosten per uur en facturering per uur bij gebruikersvoorkeuren

  U kunt dit configureren met het tandwielpictogram ![](assets/gear-icon-settings.png) op de knop Weergave in stap 4 hierboven.

* Kosten per uur en facturering per uur op taakrollen

  U kunt dit configureren met het tandwielpictogram ![](assets/gear-icon-settings.png) op de knop Weergave in stap 4 hierboven.

### Toegang weergeven

Een gebruiker met View-toegang tot financiële gegevens kan het volgende weergeven (niet bewerken):

* Sectie Financiën onder Project en Taakobjecten
* Bedrijfscase
* Factureringstarieven en factureringsgegevens
* Kosten per uur en facturering per uur bij gebruikersvoorkeuren

  U kunt dit configureren met het tandwielpictogram ![](assets/gear-icon-settings.png) op de knop Weergave in stap 4 hierboven.

* Kosten per uur en facturering per uur op taakrollen

  U kunt dit configureren met het tandwielpictogram ![](assets/gear-icon-settings.png) op de knop Weergave in stap 4 hierboven.

### Toegang bewerken

Een gebruiker met Edit toegang tot financiële gegevens kan het volgende bekijken en uitgeven:

* Sectie Financiën onder Project en Taakobjecten
* Bedrijfscase
* Factureringstarieven en factureringsgegevens
* <span class="preview"> kaarten van het Tarief </span>
* Kosten per uur en facturering per uur bij gebruikersvoorkeuren

  U kunt dit configureren met het tandwielpictogram ![](assets/gear-icon-settings.png) op de knop Bewerken in stap 4 hierboven.

* Kosten per uur en facturering per uur op taakrollen

  U kunt dit configureren met het tandwielpictogram ![](assets/gear-icon-settings.png) op de knop Bewerken in stap 4 hierboven.
