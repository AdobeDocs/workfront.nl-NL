---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Objecten delen zonder meldingen te genereren
description: Ontdek hoe u objecten kunt delen en voorkomen dat meldingen over deze wijziging worden verzonden. Dit is vooral handig wanneer u objecten bulksgewijs deelt.
author: Alina
feature: Get Started with Workfront
source-git-commit: b14dd633edec3e9746f7f1412445b74bcd37a676
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---


# Objecten delen zonder meldingen te genereren

<!--Audited: 12/2024-->

Wanneer u een object deelt in Adobe Workfront, ontvangen de personen met wie u het object deelt een e-mailbericht over het delen.

Het ontvangen van een e-mailbericht wanneer iemand een object met u deelt, is belangrijk om op de hoogte te zijn van deze wijziging. Te veel meldingen kunnen echter te verwarrend zijn voor gebruikers. Als u een groot aantal objecten tegelijk met gebruikers wilt delen, voorkomt u verwarring door meldingen tijdelijk uit te schakelen.

Personen ontvangen e-mailmeldingen wanneer de volgende instellingen tegelijkertijd zijn ingeschakeld:

* Een of beide van de volgende gebeurtenismeldingen zijn ingeschakeld op systeem- of groepsniveau:

   * Object delen over gebruiker
   * Het Aandeel van voorwerp aan Team wordt toegelaten op het systeem of groepsniveau.
* Een of beide van de volgende e-mailmeldingen zijn ingeschakeld in het profiel van de gebruiker:

   * Iemand deelt een object met mij
   * Iemand deelt een object met mijn team

Als u meerdere objecten moet delen met meerdere personen (in bulk), maar u wilt niet dat deze personen e-mailmeldingen over deze wijziging ontvangen, gaat u als volgt te werk:

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben om objecten te delen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuwe licentie: standaard</p> 
   of
   <p>Huidige licentie: abonnement</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot of hoger weergeven voor de objecten die u wilt delen</p>
   <p>Toegang voor gebruikers bewerken</p>
   <p><b>OPMERKING</b></p>
   <p> U moet een systeem- of groepsbeheerder zijn om de status van gebeurtenismeldingen voor het systeem of de groep te controleren</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen of hoger weergeven voor de objecten die u wilt delen</p></td> 
  </tr> 
 </tbody> 
</table>

*Voor meer informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Objecten delen zonder meldingen te genereren

1. Zorg ervoor dat de volgende **Meldingen van de Gebeurtenis** op het systeem of groepsniveau worden toegelaten:

   * **het Aandeel van Objecten aan Gebruiker**
   * **het Aandeel van Objecten aan Team wordt toegelaten op het systeem of groepsniveau**.

   Voor informatie, zie [&#x200B; gebeurtenisberichten voor iedereen in het systeem &#x200B;](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md) vormen.

   Als deze gebeurtenismeldingen niet zijn ingeschakeld, worden de meldingen over het delen van een object niet naar de gebruikers verzonden. Als één of allebei worden toegelaten, ga met de volgende stappen verder.

{{step-1-to-users}}

1. Selecteer veelvoudige gebruikers in de lijst, dan klik **Meldingen** > **Diverse**.
1. Schakel een of beide van de volgende meldingen uit (afhankelijk van welke meldingen op systeem- of groepsniveau zijn ingeschakeld):

   * **Iemand deelt een voorwerp met me**
   * **Iemand deelt een voorwerp met mijn team**

   Zorg ervoor dat alle geselecteerde gebruikers deze meldingen hebben geselecteerd voordat u ze uitschakelt. Op deze manier kunt u ze weer bulksgewijs inschakelen voor alle objecten nadat u de objecten hebt gedeeld.

1. Klik **sparen Veranderingen**.
1. Ga naar een lijst van voorwerpen die u wilt delen en de voorwerpen selecteren, dan het **pictogram van het Aandeel** bij de bovenkant van de lijst klikken.

   Voor informatie over het delen van een voorwerpen in bulk, zie [&#x200B; een voorwerp &#x200B;](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md) delen.

1. Ga terug naar de lijst met gebruikers voor wie u de meldingen hebt uitgeschakeld en selecteer dezelfde gebruikers.
1. Selecteer de zelfde gebruikers in de lijst, dan klik **Meldingen** > **Diverse**.
1. Schakel een of beide van de volgende meldingen in (afhankelijk van welke meldingen op systeem- of groepsniveau zijn ingeschakeld):

   * **Iemand deelt een voorwerp met me**
   * **Iemand deelt een voorwerp met mijn team**

1. Klik **sparen Veranderingen**.

   De objecten zijn gedeeld met de geselecteerde gebruikers en geen van hen heeft e-mailmeldingen over deze wijziging ontvangen.






