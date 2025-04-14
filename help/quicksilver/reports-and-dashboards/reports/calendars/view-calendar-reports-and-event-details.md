---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Kalenderrapporten en gebeurtenisdetails weergeven
description: U kunt kalenderrapporten en gebeurtenisdetails bekijken die u creeerde of met u in Adobe Workfront werd gedeeld.
author: Lisa
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: 3e5fdb157a6ff29daf964b505d3a0bf4f9842e88
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 0%

---

# Kalenderrapporten en gebeurtenisdetails weergeven

U kunt kalenderrapporten en gebeurtenisdetails bekijken die u creeerde of met u in Adobe Workfront werd gedeeld.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td><p>Nieuw: Medewerker</p>
       <p>of</p>
       <p>Huidig: Verzoek</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>[!UICONTROL View] of betere toegang tot [!UICONTROL Reports] , [!UICONTROL Dashboards] , en [!UICONTROL Calendars]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>[!UICONTROL View] of hogere machtigingen voor het kalenderrapport</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een kalenderrapport weergeven

<!--{{step1-to-calendars}}-->

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Calendars]**.

   Afhankelijk van uw toegangsniveau, zou u de volgende vermelde kalenders kunnen zien:

   * Uw standaardkalender [!DNL Adobe Workfront]

     Workfront maakt een kalender voor u op basis van de projecten, taken en problemen die aan u zijn toegewezen of die zijn toegewezen aan teams, groepen of rollen waaraan u bent toegewezen.

   * Door u gemaakte kalenders

     Om over het creëren van kalenders te leren, zie [ overzicht van de rapporten van de Kalender ](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

   * Kalenders die andere gebruikers met u hebben gedeeld

     Zie [[!UICONTROL Share a calendar] report ](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md) voor meer informatie over het delen van kalenders.

1. (Voorwaardelijk) klik **[!UICONTROL View]** drop-down, dan selecteer de kalenderduur u wilt bekijken.
   ![ de duur van de Kalender ](assets/view-menu-calendar-report-350x189.png)
U kunt uit de volgende meningen van het kalenderrapport kiezen:

   * **[!UICONTROL Month]**: geeft vier weken van de kalender weer
   * **[!UICONTROL Week]**: geeft een week van de kalender weer
   * **[!UICONTROL Gantt]**: geeft een doorlopende weergave van de kalender weer

     U kunt meer gebeurtenissen in een [!UICONTROL Gantt] weergave zien door omlaag of zijwaarts te schuiven. Een ladend symbool verschijnt aangezien de gegevens voor de mening worden bevolkt.

   >[!NOTE]
   >
   >In de weergaven [!UICONTROL Month] en [!UICONTROL Week] hebben gebeurtenissen die nu of in de toekomst plaatsvinden (inclusief gebeurtenissen die meerdere dagen beslaan, zolang ze vandaag of een toekomstige dag bevatten) een arcering die overeenkomt met de kleur in de project- of kalendergroep. Gebeurtenissen in het verleden hebben een lichtere arcering om aan te geven dat deze niet langer actueel zijn, maar u kunt deze gebeurtenissen wel selecteren en weergeven.

1. (Optioneel) Als u de kalender weergeeft in de weergaven [!UICONTROL Month] of [!UICONTROL Week] , kunt u de kalenderweergave wijzigen met de volgende opties:

   * weekends opnemen of uitsluiten:

      1. Klik op de werkbalk **[!UICONTROL Calendar]** op **[!UICONTROL Calendar Actions]** en selecteer vervolgens in de vervolgkeuzelijst de optie **[!UICONTROL Show Weekend]** of **[!UICONTROL Hide Weekend]** .

   * De weergegeven datums snel wijzigen:

      1. Klik op de werkbalk **[!UICONTROL Calendar]** op de pijl naar links van de datumindicator om terug te gaan in de kalender of op de pijl naar rechts om vooruit te gaan.

         ![ klik pijl om datum ](assets/click-arrows-to-change-dates-calendar-report.png) te veranderen\
         De weergegeven datums worden aangepast met een interval dat is gebaseerd op de huidige kalenderweergave. Als u bijvoorbeeld de kalender weergeeft in de [!UICONTROL Week] -weergave, wordt de kalender een week vooruit of een week terug weergegeven, afhankelijk van de pijl die u selecteert.

      1. (Facultatief) om aan de huidige dag terug te keren, klik [!UICONTROL **vandaag**].


1. (Optioneel) Als u een kalender in een volledig scherm wilt weergeven, klikt u op de pijlen op het volledige scherm aan de rechterkant van de **[!UICONTROL Calendar]** -werkbalk.
   ![ klik pijl om datum ](assets/click-arrows-to-change-dates-calendar-report.png) te veranderen\
   Druk op Esc om terug te keren naar de normale weergave van de kalender.

1. (Optioneel) Als u de gebeurtenissen voor een aan de kalender gekoppelde project- of kalendergroep wilt verbergen, wist u de project- of kalendergroep in de projectlijst.
   ![ de gebeurtenissen van de Huid ](assets/hide-events-for-project-or-cal-grouping.png)
U kunt de gebeurtenissen weer zichtbaar maken door de [!UICONTROL project] - of kalendergroep in de projectlijst te selecteren.

## Gebeurtenisdetails van kalenderrapporten weergeven

U kunt de details van een gebeurtenis in een kalender zien, voor zowel huidige als eerdere gebeurtenissen.

1. Ga naar de gebeurtenis waarvoor u de details wilt kennen, en klik dan de gebeurtenis. De details worden in een deelvenster aan de rechterkant geopend.
1. (Optioneel) Klik op de titel van het object om het bijbehorende project, de bijbehorende taak of uitgave te openen.
