---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Voorkeuren voor beheer van bronnen configureren
description: Als  [!DNL Adobe Workfront]  beheerder, kunt u de Voorkeur van het Beheer van het Middel voor uw systeem vormen. Deze voorkeur van het Beheer van het Middel bepaalt hoe de gebruikersbeschikbaarheid of de capaciteit en FTE voor het  [!DNL Workfront]  middel die en planningshulpmiddelen plannen worden berekend.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 7f0aac7c8519b1e570e29fedf1492918e8120ad2
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# [!UICONTROL Resource Management] -voorkeuren configureren

<!-- Audited: 5/2025 -->

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Als [!DNL Adobe Workfront] -beheerder kunt u de [!UICONTROL Resource Management] -voorkeuren voor uw systeem configureren. Deze voorkeuren bepalen hoe de beschikbaarheid of capaciteit van gebruikersuren of FTE wordt berekend voor de [!DNL Workfront] -programma&#39;s voor het plannen en plannen van bronnen.

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
   <td><p>Nieuw: Standaard</p>
   of
   <p>Huidig: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>Systeembeheerder</td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informatie waarmee rekening wordt gehouden bij de berekening van de capaciteit van een gebruiker

Bij het berekenen van de capaciteit van een gebruiker houdt Workfront rekening met de volgende informatie:

* Het aantal geplande uren, zoals gedefinieerd in het schema van de gebruiker of het standaardschema van het Workfront-systeem.
* De Uitzonderingen van het programma (afhankelijk van welk Programma wordt gebruikt, kan het de uitzonderingen van het programma van de gebruiker, of die verbonden aan het StandaardProgramma van Workfront zijn).
* De time-out van de gebruiker.
* De waarde van het voltijdequivalent ([!UICONTROL FTE]) van de gebruiker of dat van het [!DNL Workfront] -systeem. De waarde [!UICONTROL FTE] is gelijk aan 1 wanneer de gebruiker voltijds werkt, zoals gedefinieerd in het schema.
* De waarde van [!UICONTROL Work Time] voor de gebruiker, die verwijst naar de tijd die de gebruiker besteedt aan projectgerelateerd werk. Dit omvat geen overheadtijd, zoals vergaderingen en opleiding. De waarde [!UICONTROL Work Time] is gelijk aan 1 wanneer de gebruiker de volledige tijd beschikbaar is voor het werk, zoals aangegeven in [!UICONTROL FTE] of het schema. Dit houdt in dat de gebruiker geen tijd doorbrengt aan niet-projectgerelateerd werk, zoals vergaderingen of trainingen.


Voor informatie over planning en het plannen van middelen in [!DNL Workfront], zie [ begonnen worden met het Beheer van het Middel ](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## [!UICONTROL Resource Management] -voorkeuren configureren

>[!NOTE]
>
>Omdat dit een globale het plaatsen is, beïnvloedt deze selectie alle berekeningen voor het volledige systeem, voor alle gebruikers, in alle hulpmiddelen van het middelbeheer.

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Resource Management]**.
1. Selecteer een van de volgende methoden om de beschikbaarheid van gebruikers in [!DNL Workfront] te berekenen:

   * **het StandaardProgramma**: [!DNL Workfront] gebruikt het StandaardProgramma van het systeem en individuele VTE van de gebruiker om de Beschikbare Uren van de gebruiker in middelbeheersinstrumenten te berekenen.

     Voor meer informatie, zie [ een programma ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren en [ geef het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uit.

     Als deze optie is geselecteerd, berekent Workfront de beschikbare uren van de gebruiker aan de hand van de volgende formule:


     `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


     >[!INFO]
     >
     >Als het standaardschema bijvoorbeeld 40 uur per week is, is de FTE in het profiel van de gebruiker 0,5, heeft de gebruiker 1 uur van Tijd van één dag, en [!UICONTROL Work Time] in het profiel van de gebruiker 0,5, en de gebruiker is beschikbaar voor daadwerkelijke projectwerk gedurende 9,5 uur per week.
     >
     >Als de gebruiker 1 uur van Tijd van één dag heeft, zullen hun Beschikbare Uren als volgt worden berekend:
     >
     >
     >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`
     >

     <!--This used to be the calculation before we implemented the Work Time field: 
    
      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the [!UICONTROL FTE] in the profile of the user is 0.5, the user is available to work for 20 hours a week.
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
      -->



     <!--      
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>In the Production environment: (NOTE: this is the old way it was working, before the 22.2 release)</p><p><code>User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) * User FTE value</code></p>      
      <div class="example" data-mc-autonum="<b>Example: </b>">      
      <span class="autonumber"><span><b>Example: </b></span></span>      
      <div>      
      <p>For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week.</p>      
      <p>If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:</p>      
      <p><code>User Daily Available Hours = (40 - 1)* 0.5 = 19.5 hours</code></p>      
      </div>      
      </div></li>      
      -->

   * **het Programma van de Gebruiker**: [!DNL Workfront] gebruikt het programma van de gebruiker evenals [!UICONTROL Default Schedule] van het systeem om de Beschikbare [!UICONTROL FTE] waarde van de gebruiker in middelbeheersinstrumenten te berekenen. De beschikbare uren worden alleen berekend volgens het schema van de gebruiker en de waarde van [!UICONTROL FTE] van de gebruiker wordt genegeerd. Dit is de standaardinstelling.

     Voor meer informatie, zie [ een programma ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren en [ geef het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uit.

     >[!NOTE]
     >
     >Als de gebruiker niet aan een programma wordt geassocieerd, worden de Beschikbare Uren voor de gebruiker berekend gebruikend slechts [!UICONTROL Default Schedule].

     De beschikbare uren voor de gebruiker worden berekend met de volgende formule:


     `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


     Beschikbaar [!UICONTROL FTE] voor de gebruiker wordt berekend door de volgende formule:


     `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


     >[!INFO]
     >
     >Als de [!UICONTROL Default Schedule] bijvoorbeeld 40 uur per week is, is het schema van de gebruiker 30 uur per week, de [!UICONTROL Work Time] van de gebruiker 0,5 en de [!UICONTROL FTE] van de gebruiker 0,35.
     >
     >Als de gebruiker 2 uur korting op één dag heeft, wordt de wekelijkse beschikbaarheid van de gebruiker [!UICONTROL FTE] als volgt berekend:
     >
     >
     >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`
     >

     <!--This used to be the calculation before we implemented the Work Time field: 
      

      The Available hours for the user are calculated by the following formula:

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```  

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the schedule of the user is 30 hours a week, the [!UICONTROL FTE] of the user is 0.70.
      >  
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      > 
      >```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```
      -->

1. Klik op **[!UICONTROL Save]**.
