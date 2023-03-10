---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Voorkeuren voor beheer van bronnen configureren
description: Als [!DNL Adobe Workfront] beheerder u kunt de Voorkeur van het Beheer van het Middel voor uw systeem vormen. Deze voorkeuren voor het beheer van bronnen bepalen hoe de beschikbaarheid of capaciteit van de gebruiker en de FTE worden berekend voor de [!DNL Workfront] hulpmiddelen voor het plannen en plannen van bronnen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 921749caf6a61fa4f0efae9357c6e05c581421c5
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# Configureren [!UICONTROL Resource Management] voorkeuren

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Als [!DNL Adobe Workfront] beheerder u kunt vormen [!UICONTROL Resource Management] Voorkeuren voor uw systeem. Deze voorkeuren bepalen hoe de beschikbaarheid of capaciteit van gebruikersuren of FTE wordt berekend voor de [!DNL Workfront] hulpmiddelen voor het plannen en plannen van bronnen.

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
   <td> <p>Toegangsniveau van systeembeheerder</p> <p>Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> <p><b>OPMERKING</b>:

Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## Informatie waarmee rekening wordt gehouden bij de berekening van de capaciteit van een gebruiker

Bij het berekenen van de capaciteit van een gebruiker houdt Workfront rekening met de volgende informatie:

* Het aantal geplande uren, zoals gedefinieerd in het Plan van de gebruiker of het systeem van Workfront [!UICONTROL Default Schedule]
* [!UICONTROL Schedule] [!UICONTROL Exceptions] (afhankelijk van [!UICONTROL Schedule] wordt gebruikt, kan het de uitzonderingen van het programma van de gebruiker zijn, of die verbonden aan [!DNL Workfront] [!UICONTROL Default Schedule])
* Tijd van gebruiker uitgeschakeld
* De waarde van het voltijdequivalent ([!UICONTROL FTE]) van de gebruiker of die van de [!DNL Workfront] systeem. De [!UICONTROL FTE] is gelijk aan 1 wanneer de gebruiker voltijds werkt, zoals bepaald in het programma.
* De waarde van [!UICONTROL Work Time] voor de gebruiker die naar tijd verwijst die de gebruiker aan project-verwant werk besteedt. Dit omvat geen overheadtijd, zoals vergaderingen en opleiding. De [!UICONTROL Work Time] is gelijk aan 1 wanneer de gebruiker beschikbaar voor het werk de volledige tijd zoals die door wordt aangegeven [!UICONTROL FTE] of het programma, wat betekent dat ze geen tijd besteden aan niet-projectgerelateerd werk zoals vergaderingen of trainingen.


Voor informatie over planning en het plannen van middelen in [!DNL Workfront], zie [Aan de slag met Resource Management](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Configureren [!UICONTROL Resource Management] voorkeuren

>[!NOTE]
>
>Omdat dit een globale het plaatsen is, beïnvloedt deze selectie alle berekeningen voor het volledige systeem, voor alle gebruikers, in alle hulpmiddelen van het middelbeheer.

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).
1. Klik op **[!UICONTROL Resource Management]**.
1. Selecteer een van de volgende methoden om de beschikbaarheid van gebruikers te berekenen in [!DNL Workfront]:

   * **Het standaardschema**: [!DNL Workfront] gebruikt het Standaardschema van het systeem en individuele VTE van de gebruiker om de Beschikbare Uren van de gebruiker in hulpmiddelen van het middelbeheer te berekenen.

      Voor meer informatie over programma&#39;s, zie [Een schema maken](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Voor meer informatie over de locatie van de waarde van de [!UICONTROL FTE], zie  [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront berekent de beschikbare uren van een gebruiker met de volgende formule als de Workfront-beheerder de optie [!UICONTROL Default Schedule]:


      `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


      >[!INFO]
      >
      >Als het standaardschema bijvoorbeeld 40 uur per week is, is de FTE in het profiel van de gebruiker 0,5, heeft de gebruiker 1 uur van Tijd van één dag en de [!UICONTROL Work Time] in het profiel van de gebruiker is 0 , 5 , de gebruiker 9 , 5 uur per week beschikbaar voor projectwerk .
      >
      >Als de gebruiker 1 uur van Tijd van één dag heeft, zullen hun Beschikbare Uren als volgt worden berekend:
      >
      >
      >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`

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

   * **Het schema van de gebruiker**: [!DNL Workfront] gebruikt het programma van de gebruiker evenals [!UICONTROL Default Schedule] van het systeem om de beschikbare [!UICONTROL FTE] waarde van de gebruiker in hulpmiddelen van het middelbeheer. De beschikbare uren worden alleen berekend volgens het schema van de gebruiker. De waarde van de [!UICONTROL FTE] van de gebruiker wordt genegeerd. Dit is de standaardinstelling.

      Voor meer informatie over programma&#39;s, zie [Een schema maken](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Voor meer informatie over [!UICONTROL Schedule], zie  [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      >[!NOTE]
      >
      >Als de gebruiker niet aan een programma wordt geassocieerd, worden de Beschikbare Uren voor de gebruiker berekend gebruikend slechts [!UICONTROL Default Schedule].

      De beschikbare uren voor de gebruiker worden berekend met de volgende formule:


      `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


      Beschikbaar [!UICONTROL FTE] voor de gebruiker wordt berekend aan de hand van de volgende formule:


      `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


      >[!INFO]
      >
      >Als de [!UICONTROL Default Schedule] is 40 uur per week, is het programma van de gebruiker 30 uur per week, en de gebruiker [!UICONTROL Work Time] is 0,5 de [!UICONTROL FTE] van de gebruiker 0,35 is.
      >
      >Als de gebruiker 2 uur korting op één dag heeft, is de wekelijkse beschikbaarheid [!UICONTROL FTE] wordt als volgt berekend:
      >
      >
      >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`

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
