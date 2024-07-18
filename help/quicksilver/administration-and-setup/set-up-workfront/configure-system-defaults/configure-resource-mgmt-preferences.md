---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Voorkeuren voor beheer van bronnen configureren
description: Als  [!DNL Adobe Workfront]  beheerder kunt u de Voorkeur van het Beheer van het Middel voor uw systeem vormen. Deze voorkeur van het Beheer van het Middel bepaalt hoe de gebruikersbeschikbaarheid of de capaciteit en FTE voor het  [!DNL Workfront]  middel die en planningshulpmiddelen plannen worden berekend.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 921749caf6a61fa4f0efae9357c6e05c581421c5
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# [!UICONTROL Resource Management] -voorkeuren configureren

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Als [!DNL Adobe Workfront] -beheerder kunt u de [!UICONTROL Resource Management] -voorkeuren voor uw systeem configureren. Deze voorkeuren bepalen hoe de beschikbaarheid of capaciteit van gebruikersuren of FTE wordt berekend voor de [!DNL Workfront] -programma&#39;s voor het plannen en plannen van bronnen.

## Toegangsvereisten

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>
   <p>Current license: [!UICONTROL Standard]</p>
   
   Or
   
   <p>Legacy license: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System Administrator access level</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: 
   
   If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegangsniveau van systeembeheerder</p> <p>Voor meer informatie, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> een gebruiker volledige administratieve toegang verlenen </a>.</p> <p><b> NOTA </b>:

Als u nog steeds geen toegang hebt, vraagt u de [!DNL Workfront] -beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr> 
 </tbody> 
</table>

## Informatie waarmee rekening wordt gehouden bij de berekening van de capaciteit van een gebruiker

Bij het berekenen van de capaciteit van een gebruiker houdt Workfront rekening met de volgende informatie:

* Het aantal geplande uren, zoals gedefinieerd in het Programma van de gebruiker of het Workfront-systeem [!UICONTROL Default Schedule]
* [!UICONTROL Schedule] [!UICONTROL Exceptions] (afhankelijk van welke [!UICONTROL Schedule] wordt gebruikt, kan dit de uitzonderingen zijn van het programma van de gebruiker, of die zijn gekoppeld aan het [!DNL Workfront] [!UICONTROL Default Schedule] )
* Tijd van gebruiker uitgeschakeld
* De waarde van het voltijdequivalent ([!UICONTROL FTE]) van de gebruiker of dat van het [!DNL Workfront] -systeem. De waarde [!UICONTROL FTE] is gelijk aan 1 wanneer de gebruiker voltijds werkt, zoals gedefinieerd in het schema.
* De waarde van [!UICONTROL Work Time] voor de gebruiker die verwijst naar de tijd die de gebruiker besteedt aan projectgerelateerd werk. Dit omvat geen overheadtijd, zoals vergaderingen en opleiding. De waarde [!UICONTROL Work Time] is gelijk aan 1 wanneer de gebruiker de volledige tijd beschikbaar is voor het werk, zoals aangegeven in [!UICONTROL FTE] of het schema. Dit houdt in dat de gebruiker geen tijd doorbrengt aan niet-projectgerelateerd werk, zoals vergaderingen of trainingen.


Voor informatie over planning en het plannen van middelen in [!DNL Workfront], zie [ begonnen worden met het Beheer van het Middel ](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## [!UICONTROL Resource Management] -voorkeuren configureren

>[!NOTE]
>
>Omdat dit een globale het plaatsen is, beïnvloedt deze selectie alle berekeningen voor het volledige systeem, voor alle gebruikers, in alle hulpmiddelen van het middelbeheer.

1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in [!DNL Workfront] en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png) .
1. Klik op **[!UICONTROL Resource Management]**.
1. Selecteer een van de volgende methoden om de beschikbaarheid van gebruikers in [!DNL Workfront] te berekenen:

   * **het StandaardProgramma**: [!DNL Workfront] gebruikt het StandaardProgramma van het systeem en individuele VTE van de gebruiker om de Beschikbare Uren van de gebruiker in middelbeheersinstrumenten te berekenen.

     Voor meer informatie over programma&#39;s, zie [ een programma ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

     Voor meer informatie over het lokaliseren van de waarde van de gebruiker [!UICONTROL FTE], zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

     Workfront berekent de beschikbare uren van een gebruiker met de volgende formule wanneer de Workfront-beheerder de optie [!UICONTROL Default Schedule] kiest:


     `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


     >[!INFO]
     >
     >Als het standaardschema bijvoorbeeld 40 uur per week is, is de FTE in het profiel van de gebruiker 0,5, heeft de gebruiker 1 uur Tijd korting op één dag en is de [!UICONTROL Work Time] in het profiel van de gebruiker 0,5, is de gebruiker 9,5 uur per week beschikbaar voor daadwerkelijk projectwerk.
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

   * **het Programma van de Gebruiker**: [!DNL Workfront] gebruikt het programma van de gebruiker evenals [!UICONTROL Default Schedule] van het systeem om de Beschikbare [!UICONTROL FTE] waarde van de gebruiker in middelbeheersinstrumenten te berekenen. De beschikbare uren worden alleen berekend volgens het schema van de gebruiker. De waarde van [!UICONTROL FTE] van de gebruiker wordt genegeerd. Dit is de standaardinstelling.

     Voor meer informatie over programma&#39;s, zie [ een programma ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

     Voor meer informatie over gebruiker [!UICONTROL Schedule], zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

     >[!NOTE]
     >
     >Als de gebruiker niet aan een programma wordt geassocieerd, worden de Beschikbare Uren voor de gebruiker berekend gebruikend slechts [!UICONTROL Default Schedule].

     De beschikbare uren voor de gebruiker worden berekend met de volgende formule:


     `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


     Beschikbaar [!UICONTROL FTE] voor de gebruiker wordt berekend door de volgende formule:


     `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


     >[!INFO]
     >
     >Als de [!UICONTROL Default Schedule] bijvoorbeeld 40 uur per week is, is het programma van de gebruiker 30 uur per week en is de [!UICONTROL Work Time] van de gebruiker 0,5 de [!UICONTROL FTE] van de gebruiker 0,35.
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
