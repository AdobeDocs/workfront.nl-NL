---
title: Vorm de Berichten van de Gebeurtenis voor Iedereen in het Systeem
description: Gebeurtenismeldingen activeren e-mails naar gebruikers wanneer een bepaalde gebeurtenis plaatsvindt. Als Adobe Workfront-beheerder of gebruiker met een Planner-toegangsniveau kunt u een gebeurtenismelding configureren voor alle gebruikers in het systeem. Configuratie van een gebeurtenismelding bestaat uit het activeren of deactiveren ervan.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: e9c6a01e80d34bc873c9a06ae0782dc65afb2445
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Gebeurtenismeldingen configureren voor iedereen in het systeem

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

Gebeurtenismeldingen activeren e-mails naar gebruikers wanneer een bepaalde gebeurtenis plaatsvindt. Als Adobe Workfront-beheerder of gebruiker met een Planner-toegangsniveau kunt u een gebeurtenismelding configureren voor alle gebruikers in het systeem. Configuratie van een gebeurtenismelding bestaat uit het activeren of deactiveren ervan.

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

Afhankelijk van de gebeurtenis die u inschakelt en de gebruiker ingeschakeld blijft op zijn eigen profiel, ontvangen gebruikers direct, dagelijks of zowel instant- als dagelijkse e-mailberichten wanneer een gebeurtenis plaatsvindt.

U moet eerst opgeven welke meldingen alle gebruikers moeten ontvangen in het gedeelte Setup van uw Workfront-exemplaar. Nadat u een melding hebt geactiveerd in het gedeelte Setup, wordt het voor elke gebruiker op de profielpagina weergegeven.

Nadat meldingen zijn geactiveerd in het gedeelte Setup en worden weergegeven op de pagina&#39;s met gebruikersprofielen, kunnen afzonderlijke gebruikers of een andere gebruiker met een licentie voor het abonnement de geactiveerde meldingen ook configureren in een gebruikersprofiel om te bepalen welke meldingen specifieke gebruikers ontvangen en hoe vaak. Voor meer informatie, zie [ uw eigen e-mailberichten wijzigen ](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Voor een lijst van alle gebeurtenisberichten die u kunt activeren en deactiveren, zie [ de berichttypes van de Gebeurtenis ](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Voor informatie over het ontgrendelen van een gebeurtenisbericht zodat de groepsbeheerders het voor hun groepen kunnen vormen, zie [ ontgrendelen of configuratie van gebeurtenisberichten voor alle groepen ](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md) en [ Mening en vormen gebeurtenisberichten voor een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

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
   <td> <p>Nieuw: Standaard</p>
 <p>of</p> 
<p>Huidig: Plan</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Planner of hoger, met administratieve toegang tot herinneringsmeldingen</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gebeurtenismeldingen configureren voor alle gebruikers

U moet meldingen inschakelen in het gedeelte Setup van Workfront voordat gebruikers de meldingen in hun afzonderlijke profielen kunnen in- of uitschakelen.

>[!TIP]
>
>U kunt geen berichten voor de Doelen van Workfront van het gebied van de Opstelling activeren. Gebruikers kunnen deze meldingen alleen activeren in hun profielen. Gebruikers met een abonnement kunnen deze activeren voor andere gebruikers. Voor informatie over het toelaten van de berichten van de Doelen van Workfront voor gebruikers, zie [ Meldingen: Doelen ](../../../workfront-basics/using-notifications/notifications-goals.md).

{{step-1-to-setup}}

1. Klik **E-mail** > **Meldingen**.

   ![ gebied van Meldingen onder opstellingsE-mail ](assets/notifications-area-under-setup-emails.png)


1. Zorg ervoor de **Berichten van de Gebeurtenis** tabel open is.
1. Schakel de schakelaar links van de naam van de gebeurtenis in of uit.

   Om de standaardberichtstatus voor een gebeurtenis te zien, zie [ de berichten van de Gebeurtenis ](../../../workfront-basics/using-notifications/event-notifications.md).

1. (Optioneel) Klik op de naam van een gebeurtenismelding om de onderwerpregel van het e-mailbericht aan te passen.

   Voor meer informatie over het aanpassen van de onderwerplijnen van e-mailberichten, zie [ E-mailonderwerpen voor gebeurtenisberichten aanpassen ](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

1. (Facultatief) als u configuratie voor een e-mailbericht wilt ontgrendelen zodat de groepsbeheerders het voor hun groepen afzonderlijk kunnen vormen, klik de knoop ![ knevel van het Slot ](assets/lock-toggle-button.png) rechts van het bericht om het aan de ontgrendelde schakelaar ![ te schakelen Ontgrendelt knevel ](assets/unlock-toggle-button.png).

   Voor meer informatie, zie [ configuratie van de Ontgrendeling of van het slot van gebeurtenisberichten voor alle groepen ](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

Gebruikers kunnen de frequentie van deze meldingen aanpassen in hun gebruikersprofiel.