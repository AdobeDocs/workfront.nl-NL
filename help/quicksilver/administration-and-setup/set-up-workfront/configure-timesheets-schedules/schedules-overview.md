---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: gebruiker,plannen
navigation-topic: configure-timesheets-and-schedules
title: Overzicht van schema's
description: U kunt uw werkweek definiëren met behulp van schema's. U kunt een programma met een gebruiker of een project associëren. Dit maakt [!DNL Adobe Workfront] om tijdlijnen en de beschikbaarheid van de gebruiker te berekenen. Zie Een schema maken voor instructies.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: b3ec7af8032e077736df1f48a9a4990b8c11922f
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 0%

---

# Overzicht van schema&#39;s

U kunt uw werkweek bepalen gebruikend programma&#39;s en een programma associëren met een gebruiker of een project. Dit maakt [!DNL Adobe Workfront] om tijdlijnen en de beschikbaarheid van de gebruiker te berekenen. Zie voor instructies [Een schema maken](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Houd rekening met het volgende wanneer u werkt met planningen in Workfront:

* De [!DNL Workfront] de beheerder identificeert de uren van verrichting voor de organisatie in een programma.

  Op dezelfde manier kan een groepsbeheerder de bedrijfsuren van een programma identificeren dat door een groep wordt beheerd die zij leiden.

  Voor meer informatie over groepsbeheerders, zie [Groepbeheerders](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

  Een schema kan bijvoorbeeld als volgt worden gedefinieerd: maandag tot en met vrijdag, 08.00 tot 17.00 uur, met een pauze voor de lunch.

* [!DNL Workfront] gebruikt het programma om te bepalen wanneer de het werkdag begint en beëindigt.

  Dit belet niet dat een gebruiker aan het werk werkt of het werk voltooit in [!DNL Workfront] buiten de normale kantooruren. Over het algemeen, is het niet noodzakelijk om een nieuw programma of een planningsuitzondering tot stand te brengen om zich op het werk te concentreren dat in de avond wordt gepland.

  Uw organisatie kan ook flexibele aankomsttijden voor uw werkdag hebben. U kunt een reeks werknemers hebben die bij 8 AM en een andere reeks aankomt die bij 9 AM aankomt. Het is niet nodig om unieke schema&#39;s voor elke groep tot stand te brengen, als de groepen gelijkaardige of identieke programma&#39;s hebben. Maar als de groepen drastisch verschillende programma&#39;s hebben, zouden hun gebruikers aan unieke programma&#39;s moeten worden geassocieerd. Een werknemer begrijpt of een opdracht om 17.00 uur moet worden voltooid, dit betekent dat het werk tegen het einde van de werkdag moet zijn gedaan, ongeacht het tijdstip waarop zij aan het werk komen.

* Wij adviseren dat u afzonderlijke programma&#39;s voor elke tijdzone verbonden aan de organisatie creeert.

  U kunt een specifieke tijdzone voor elk programma toewijzen om ervoor te zorgen dat het werk geschikt is gepland voor gebruikers die in verschillende tijdzones werken.

* De [!DNL Workfront] Het standaardProgramma wordt gebruikt in chronologieberekeningen wanneer de gebruikers of de projecten niet met een programma worden geassocieerd.

  Het standaardschema wordt geleverd met uw [!DNL Workfront] en kan alleen worden verwijderd als het wordt vervangen door een nieuw schema dat u maakt.

* Naast het berekenen van tijdlijnen, [!DNL Workfront] gebruikt programma&#39;s om gebruikersbeschikbaarheid te berekenen.

  >[!IMPORTANT]
  >
  >[!DNL Workfront] gebruikt of de gebruiker of het projectprogramma om middelbeschikbaarheid in de Planner van het Middel te bepalen. Welk schema wordt gebruikt hangt van af wat [!DNL Workfront] beheerder geselecteerd voor de [!UICONTROL Calculate Resource Availability Using] instellen. Voor informatie over de montages van het Beheer van het Middel, zie [Voorkeuren voor beheer van bronnen configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Hiërarchie van schema&#39;s

Als een taak aan een gebruiker wordt toegewezen die met een programma wordt geassocieerd, en op een project verblijft dat met een tweede programma wordt geassocieerd, hebt u minstens 2 programma&#39;s die potentieel op uw chronologieberekeningen zouden kunnen worden toegepast.

>[!IMPORTANT]
>
>[!DNL Workfront] gebruikt het programma van een gebruiker slechts wanneer [!UICONTROL Calculate Resource Availability Using] instellen op [!UICONTROL The User's Schedule] in de [!UICONTROL Resource Management] gebied van [!UICONTROL Setup]. Voor informatie over de [!UICONTROL Calculate Resource Availability Using] het plaatsen beïnvloedt welk programma voor het Beheer van het Middel wordt gebruikt, zie [Voorkeuren voor beheer van bronnen configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

De volgorde waarin de schema&#39;s door het systeem worden gebruikt wanneer er meer dan één bestaat, is:

* Wanneer een gebruiker aan een taak wordt toegewezen, [!DNL Workfront] gebruikt het programma van de gebruiker voor het berekenen van de chronologie van de taak. Dit omvat ook de persoonlijke tijd van de gebruiker. Het schema van het project wordt genegeerd.

  Zie voor meer informatie over persoonlijke tijd [Persoonlijke tijd uit configureren](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* Wanneer de veelvoudige gebruikers aan een taak worden toegewezen, en de gebruikers verschillende programma&#39;s tijdens het tijdkader van de taak hebben, [!DNL Workfront] gebruikt één van beide volgende programma&#39;s, zoals die in [!UICONTROL Project Preferences] gebied van [!UICONTROL Setup]:

   * Het schema van de gebruiker die als primaire ontvanger is aangewezen
   * Het programma verbonden aan het project.

     Voor meer informatie over projectvoorkeur, zie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Als de gebruiker die aan de taak wordt toegewezen geen programma heeft, of de taak slechts aan een baanrol, een team wordt toegewezen, of unassigned is, [!DNL Workfront] gebruikt het projectprogramma voor de chronologieberekeningen.
* Als de gebruiker aan de taak wordt toegewezen geen programma heeft, of de taak slechts aan een baanrol, een team, of unassigned, en het project heeft geen programma, dan wordt toegewezen [!DNL Workfront] gebruikt het schema in het systeem dat als StandaardProgramma voor chronologieberekeningen wordt aangewezen.

  ![](assets/default-schedule.png)

## Samenwerking in [!DNL Workfront] over tijdzones

Voor informatie over het gebruiken van programma&#39;s om gebruikers te helpen binnen samenwerken [!DNL Workfront] over tijdzones heen, zie [Werken in tijdzones](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
