---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Automatische herinneringen instellen
description: U kunt automatische herinneringen instellen om e-mailmeldingen te activeren wanneer alle taken of problemen opeisbaar zijn, te laat of bijna op de geplande voltooiingsdatum.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: e34abb5ff1068de99eaba33dc95287164e556742
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---

# Automatische herinneringen instellen

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als Adobe Workfront-beheerder kunt u automatische herinneringen instellen om e-mailmeldingen te activeren wanneer alle taken of problemen moeten worden uitgevoerd, laat of vlak bij de geplande voltooiingsdatum. Nadat u deze instellingen hebt geconfigureerd, kunnen gebruikers automatische herinneringen niet uitschakelen.

Voor late meldingen wordt de e-mail iedere avond verzonden totdat de taak of uitgave is voltooid.

Een automatische herinnering kan naar één of meerdere van het volgende worden verzonden:

* De gebruikers die aan een taak of kwestie worden toegewezen
* De directe manager van de gebruiker
* De manager van de directe manager

>[!NOTE]
>
>U kunt de inhoud of de onderwerpregel van het e-mailbericht dat wordt geactiveerd door een automatische herinnering niet wijzigen.

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
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Systeembeheerder</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Automatische herinneringen instellen

{{step-1-to-setup}}

1. Klik **E-mail** > **Automatische Herinneringen**.

1. In **verzend een laat bericht naar** gebied, selecteer om het even welke volgende opties:

   <table>
    <tr>
        <td>De gebruiker "Toegewezen aan"</td>
        <td>Selecteer deze optie als u wilt dat de gebruiker die aan een taak of kwestie wordt toegewezen een laat bericht over zijn het werkpunt ontvangt dat laat is.</td>
        <td></td>
    </tr>
    <tr>
        <td>De manager van de gebruiker</td>
        <td>Selecteer deze optie als u wilt dat de manager van de gebruiker een laat bericht over het het werkpunt van zijn direct rapport wordt ontvangen dat laat is.</td>
        <td></td>
    </tr>
    <tr>
        <td>De manager van de manager</td>
        <td>Selecteer deze optie als u wilt dat de manager van de directe manager een laat bericht over een het werkpunt van één van hun directe gebruikers ontvangt die van het rapport te laat zijn.</td>
        <td></td>
    </tr>
    <tr>
        <td>De gebruiker "Toegewezen aan"</td>
        <td>(In <b> verzend eindherinnering aan </b> gebied.) Selecteer deze optie als u wilt dat de gebruiker die aan een taak of een kwestie wordt toegewezen, een melding ontvangt over zijn het werkpunt dat de vervaldatum nadert.</td>
        <td></td>
    </tr>
   </table>

1. Selecteer de tijd die de automatische herinnering moet verzenden door de hoeveelheid tijd vóór of na de vervaldatum van het werkitem te selecteren.

   De tijd wordt berekend vanaf de geplande datum van voltooiing van de taak of afgifte.

   Geef het aantal minuten, uren, dagen, weken of maanden op om tijd toe te voegen aan de geplande Voltooiingsdatum van de taken of uitgaven. Selecteer **Verstreken notulen**, **Verstreken Uren**, **Verstreken Dagen**, of **Verstreken Weken** om tijd toe te voegen die om het even welke weekends, vakantie, en niet-werkuren zoals vermeld in uw programma omvat.

   Als een taak bijvoorbeeld op vrijdag is toegewezen en een duur van 3 verstreken dagen heeft, wordt de voltooiingsdatum van de taak ingesteld op maandag (ervan uitgaande dat zaterdag en zondag een weekend zijn). Als de taak drie dagen duurt (niet is verstreken), is de datum waarop de taak is voltooid, vastgesteld op woensdag.

   {de toename van 0} Tijd ![](assets/time-increments-for-automatic-reminder.png)

1. Klik **sparen**.

## Automatische herinneringen ontvangen

Als u de aangewezen entiteit bent in een Automatische herinnering, ontvangt u een e-mail wanneer de opgegeven deadline is gehaald. Voor late meldingen wordt de e-mail iedere avond verzonden totdat de taak of uitgave is voltooid.

De taken met bepaalde gebiedstypes kunnen na de gespecificeerde begindatum leveren, alhoewel zij achterstallig zijn. Bijvoorbeeld, als een taak een voorganger met een eind-Begin (fs) gebiedsdeel heeft, zal het niet in e-mail worden omvat, zelfs als het de gespecificeerde begindatum is overgegaan, omdat u niet de taak kunt beginnen tot voorganger volledig is.

Voor meer informatie over het ontvangen van Automatische herinneringen e-mails, zie de [ Automatische herinneringen ](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) sectie in [ de berichten van Adobe Workfront ](../../../workfront-basics/using-notifications/wf-notifications.md).

## Automatische herinneringen verzenden

Automatische herinneringen worden verzonden zodra de door de Workfront-beheerder geselecteerde tijd is verstreken.

Als u het handmatig verzenden van de automatische herinneringse-mails wilt activeren, kunt u dit doen met Diagnostics. Voor meer informatie over de toegang tot van en het gebruiken van Diagnostiek in Workfront, zie [ Diagnose van het Gebruik om geautomatiseerde processen ](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md) teweeg te brengen.
