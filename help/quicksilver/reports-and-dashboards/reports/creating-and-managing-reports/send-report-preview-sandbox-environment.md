---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Een rapport verzenden in de omgeving van de voorvertoningssandbox
description: De informatie op deze pagina verwijst naar functionaliteit die alleen beschikbaar is in de omgeving van de sandbox Voorbeeld en Aangepast vernieuwen. Deze functionaliteit is niet beschikbaar in de productieomgeving.
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---

# Een rapport verzenden in de omgeving van de voorvertoningssandbox

<!-- Audited: 11/2024 -->

De informatie op deze pagina verwijst naar functionaliteit die alleen beschikbaar is in de omgeving van de sandbox Voorbeeld en Aangepast vernieuwen. Deze functionaliteit is niet beschikbaar in de productieomgeving.

U kunt de opties voor het leveren van rapporten instellen in elke testomgeving van Adobe Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

Hoewel de testomgevingen zo dicht mogelijk bij uw productieomgeving moeten werken, verschilt bepaalde functionaliteit van uw productieomgeving.

U kunt rapporten plannen in de testmilieu&#39;s, maar de manier zij worden geleverd verschilt van hoe zij van het milieu van de Productie worden geleverd.

Voor informatie over het plannen van rapporten voor levering in het milieu van de Productie, zie [&#x200B; de leveringsoverzicht van het Rapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Afhankelijk van waar u de rapporten plant, verschilt de leveringsfunctionaliteit tussen de Voorproef en de Douane verfrist zandbakken.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
      <td> 
      <p>Nieuw:</p>
         <ul>
         <li><p>Standaard</p></li>
         </ul>
      <p>Huidige:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p></td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Rapporten plannen in de voorvertoningsomgeving

* [Rapporten plannen in de voorvertoningsomgeving](#schedule-reports-in-the-preview-environment)

### Rapporten plannen in de voorvertoningsomgeving

Of een geleverd rapport wordt geproduceerd of niet in het milieu van de Voorproef hangt af van of **e-mails van dit testmilieu** wordt toegelaten of niet ontvangt.

Voor informatie over het toelaten van e-mails van het milieu Sandbox zie [&#x200B; levering van e-mails van het milieu van de zandbak van de Voorproef &#x200B;](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md) toelaten.

![&#x200B; ontvang e-mails van zandbakoptie &#x200B;](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

Het plannen van rapporten voor levering in het milieu van de Voorproef is identiek aan het plannen van rapporten in het milieu van de Productie. Voor informatie over het plannen van een rapport voor levering, zie [&#x200B; de leveringsoverzicht van het Rapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Wanneer u een rapport voor levering in het milieu van de Voorproef plant, bestaan de volgende scenario&#39;s:

* Wanneer **e-mails van dit testmilieu** voor de gebruiker ontvangt die het rapport ontvangt, wordt geen dossier geproduceerd wanneer het plannen van het rapport voor levering.
* Wanneer **e-mails van dit testmilieu** wordt toegelaten voor de gebruiker die het rapport ontvangt, wordt het dossier dat wanneer het plannen van het rapport voor levering wordt geproduceerd toegevoegd op het lusje van Documenten van de gebruiker.

## Rapporten plannen in de omgeving van de aangepaste sandbox Vernieuwen

Of een geleverd rapport wordt geproduceerd of niet in de Douane verfrist Sandbox hangt af van of ontvangt e-mail van deze testmilieu het plaatsen of niet wordt toegelaten.

Voor informatie over het toelaten van e-mails van het milieu van de Voorproef zie de sectie [&#x200B; Mening en wijzig uw montages van het e-mailbericht &#x200B;](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) in het artikel [&#x200B; uw eigen e-mailberichten &#x200B;](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) wijzigen.

![&#x200B; ontvang e-mails van zandbakoptie &#x200B;](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

Het plannen van rapporten voor levering in het milieu van de Zandbak van de Douane verfrist zich is identiek aan het plannen van rapporten in het milieu van de Productie. Voor informatie over het plannen van een rapport voor levering, zie [&#x200B; de leveringsoverzicht van het Rapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Wanneer u een rapport voor levering in het milieu van de Zandbak van de Douane plant verfrist, bestaan de volgende scenario&#39;s:

* Wanneer de Receive e-mail van deze testomgeving voor de gebruiker wordt onbruikbaar gemaakt die het rapport ontvangt, wordt geen dossier geproduceerd wanneer het plannen van het rapport voor levering.
* Wanneer de Receive e-mails van deze testmilieu voor de gebruiker wordt toegelaten die het rapport ontvangt, wordt het rapport gemaild als gehechtheid aan het e-mailadres verbonden aan de gebruiker.

## Hoe externe gebruikers op de hoogte worden gesteld

Externe gebruikers ontvangen geen rapporten die vanuit de Workfront-testomgeving zijn verzonden en ontvangen ook geen e-mailmelding.

Externe gebruikers ontvangen alleen e-mailrapporten als deze afkomstig zijn uit een productieomgeving.
