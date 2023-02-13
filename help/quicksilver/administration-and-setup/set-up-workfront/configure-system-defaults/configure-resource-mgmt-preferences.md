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
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Configureren [!UICONTROL Resource Management] voorkeuren

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Als [!DNL Adobe Workfront] beheerder u kunt vormen [!UICONTROL Resource Management] Voorkeuren voor uw systeem. Deze voorkeuren bepalen hoe de beschikbaarheid of capaciteit van de gebruiker en de FTE worden berekend voor de [!DNL Workfront] hulpmiddelen voor het plannen en plannen van bronnen.

Voor informatie over planning en het plannen van middelen in [!DNL Workfront], zie [Aan de slag met Resource Management](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Toegangsvereisten

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
   <td> <p>Toegangsniveau van systeembeheerder</p> <p>Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configureren [!UICONTROL Resource Management] voorkeuren

>[!NOTE]
>
>Omdat dit een globale instelling is, beïnvloedt deze selectie alle berekeningen voor het volledige systeem, voor alle gebruikers, in alle hulpmiddelen van het middelbeheer, en voor alle Pools van het Middel.

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).
1. Klik op **[!UICONTROL Resource Management]**.
1. Selecteer een van de volgende methoden om de beschikbaarheid van gebruikers te berekenen in [!DNL Workfront]:

   * **Het standaardschema**: [!DNL Workfront] gebruikt het standaardschema van het systeem en de individuele VTE van de gebruiker om de Beschikbare Uren van de gebruiker in hulpmiddelen van het middelbeheer te berekenen.\

      Voor meer informatie over programma&#39;s, zie [Een schema maken](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Voor meer informatie over de waarde van de gebruiker FTE, zie  [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      Workfront berekent de beschikbare uren van een gebruiker met de volgende formule wanneer de Workfront-beheerder Standaardschema kiest:

      ```
      User Available Hours = (Default Schedule Hours - Exceptions) * FTE - Time off hours
      ```

      **Voorbeeld:**\
      Als het standaardschema bijvoorbeeld 40 uur per week is en de FTE in het profiel van de gebruiker 0,5 is, kan de gebruiker 20 uur per week werken.

      Als de gebruiker 1 uur van Tijd van één dag heeft, zullen hun Beschikbare Uren als volgt worden berekend:

      ```
      User Available Hours = (40 * 0.5) - 1 = 19 hours
      ```

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

   * **Het schema van de gebruiker**: [!DNL Workfront] gebruikt het programma van de gebruiker evenals het StandaardProgramma van het systeem om de Beschikbare FTE waarde van de gebruiker in middelbeheersinstrumenten te berekenen. De beschikbare uren worden alleen berekend volgens het schema van de gebruiker. De waarde van de FTE van de gebruiker wordt genegeerd. Dit is de standaardinstelling.

      >[!NOTE]
      >
      >Als de gebruiker niet aan een programma wordt geassocieerd, worden de Beschikbare Uren voor de gebruiker berekend gebruikend het StandaardProgramma.

      De beschikbare VTE voor de gebruiker wordt berekend door de volgende formule:

      ```
      User Available FTE = (Hours from the Schedule of the User - Time off hours) / Default Schedule Hours
      ```

      **Voorbeeld:** Bijvoorbeeld, als het Standaard Programma 40 uren per week is en het programma van de gebruiker 30 uren per week is, FTE van de gebruiker is 0.75.

      Als de gebruiker 2 uur van Tijd van één dag heeft, zal hun Wekelijks Beschikbare VTE als volgt worden berekend:

      ```
      User Weekly Available FTE = (30-2) / 40 = 0.70
      ```

1. Klik op **[!UICONTROL Save]**.
