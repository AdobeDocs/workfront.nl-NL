---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Automatische herinneringen instellen
description: Automatische herinneringen instellen
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '609'
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
   <td> <p>Systeembeheerder</p> </td> 
  </tr> 
 </tbody> 
</table>

## Automatische herinneringen instellen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **E-mail** >**Automatische herinneringen**.

1. In de **Een late melding verzenden naar** selecteert u een van de volgende opties:

   <table>
    <tr>
        <td>De gebruiker "Toegewezen aan"</td>
        <td>Selecteer deze optie als u wilt dat de gebruiker die aan een taak of kwestie wordt toegewezen een laat bericht over zijn het werkpunt ontvangt.</td>
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
        <td>(In de <b>Herinnering voor deadline verzenden naar</b> gebied.) Selecteer deze optie als u wilt dat de gebruiker die aan een taak of een kwestie wordt toegewezen, een melding ontvangt over zijn het werkpunt dat de vervaldatum nadert.</td>
        <td></td>
    </tr>
</table>

1. Selecteer de tijd die de automatische herinnering moet verzenden door de hoeveelheid tijd vóór of na de vervaldatum van het werkitem te selecteren.

   De tijd wordt berekend vanaf de geplande datum van voltooiing van de taak of afgifte.

   Geef het aantal minuten, uren, dagen, weken of maanden op om tijd toe te voegen aan de geplande Voltooiingsdatum van de taken of uitgaven. Selecteren **Verstreken minuten**, **Verstreken uren**, **Verstreken dagen**, of **Verstreken weken** om tijd toe te voegen die weekends, feestdagen en niet-werkuren omvat, zoals in uw planning is aangegeven.

   Als een taak bijvoorbeeld op vrijdag is toegewezen en een duur van 3 verstreken dagen heeft, wordt de voltooiingsdatum van de taak ingesteld op maandag (ervan uitgaande dat zaterdag en zondag een weekend zijn). Als de taak drie dagen duurt (niet is verstreken), is de datum waarop de taak is voltooid, vastgesteld op woensdag.

   ![](assets/time-increments-for-automatic-reminder.png)

1. Klikken **Opslaan**.

## Automatische herinneringen ontvangen

Als u de aangewezen entiteit bent in een Automatische herinnering, ontvangt u een e-mail wanneer de opgegeven deadline is gehaald. Voor late meldingen wordt de e-mail iedere avond verzonden totdat de taak of uitgave is voltooid.

De taken met bepaalde gebiedstypes kunnen na de gespecificeerde begindatum leveren, alhoewel zij achterstallig zijn. Bijvoorbeeld, als een taak een voorganger met een eind-Begin (fs) gebiedsdeel heeft, zal het niet in e-mail worden omvat, zelfs als het de gespecificeerde begindatum is overgegaan, omdat u niet de taak kunt beginnen tot voorganger volledig is.

Voor meer informatie over het ontvangen van e-mails met automatische herinneringen raadpleegt u de [Automatische herinneringen](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) sectie in [Adobe Workfront-berichten](../../../workfront-basics/using-notifications/wf-notifications.md).

## Automatische herinneringen verzenden

Automatische herinneringen worden verzonden zodra de door de Workfront-beheerder geselecteerde tijd is verstreken.

Als u het handmatig verzenden van de automatische herinneringse-mails wilt activeren, kunt u dit doen met Diagnostics. Voor meer informatie over toegang tot en het gebruiken van Diagnostiek in Workfront, zie [Diagnostiek gebruiken om geautomatiseerde processen te activeren](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
