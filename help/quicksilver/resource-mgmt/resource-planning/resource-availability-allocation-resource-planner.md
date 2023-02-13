---
product-area: resource-management
navigation-topic: resource-planning
title: Beschikbaarheid en toewijzing van bronnen controleren met de Adobe Workfront Resource Planner
description: U kunt de beschikbaarheid van uw middelen en de hoeveelheid gepland of begroot werk voor uw projecten in de Planner van het Middel bekijken. Deze waarden worden weergegeven in Uren, FTE (Full Time Equivalent) of Kostenbedragen en worden in kolommen geordend.
author: Alina
feature: Resource Management
exl-id: 5b3e52a6-af9b-4e68-8d6e-43a5151a2a2c
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: tm+mt
source-wordcount: '1270'
ht-degree: 0%

---

# Beschikbaarheid en toewijzing van bronnen controleren met de Adobe Workfront Resource Planner

U kunt de beschikbaarheid van uw middelen en de hoeveelheid gepland of begroot werk voor uw projecten in de Planner van het Middel bekijken. Deze waarden worden weergegeven in Uren, FTE (Full Time Equivalent) of Kostenbedragen en worden in kolommen geordend.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Pro en hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Controleren of hoger </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot het volgende weergeven of vergroten:</p> 
    <ul> 
     <li> <p>Bronbeheer</p> </li> 
     <li> <p>Financiële gegevens</p> </li> 
     <li> <p>Gebruikers</p> </li> 
     <li> <p>Projecten</p> </li> 
    </ul> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De mening of hogere toestemmingen aan de projecten u in de Planner van het Middel wilt bekijken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

<!--note from the table about the license: Review or higher: 
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (waiting on Vazgen to confirm - working differenly in classic)
      </MadCap:conditionalText>
     -->

## Vereisten

U moet aan alle voorwaarden voldoen die worden vereist om met de Planner van het Middel te werken. Zie voor meer informatie [Overzicht van de bronnenplanner](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

>[!IMPORTANT]
>
>Als om het even welke eerste vereisten die voor de correcte functionaliteit van de Planner van het Middel worden vereist ontbreken, kunnen sommige aantallen nul zijn, of de Begrotingshours zouden kunnen worden gedimd.

## Beschikbaarheid en toewijzing van middelen

De kolommen die de beschikbaarheid en de toewijzing van uw middelen tonen veranderen afhankelijk van welke mening u op de Planner van het Middel van toepassing bent. Voor informatie over het tonen van de informatie in de Planner van het Middel door Project, Rol, of Gebruiker zie [Overzicht van de navigatie in de bronnenplanner](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Overweeg het volgende wanneer het veranderen van uw mening in de Planner van het Middel:

* Wanneer u het **Weergeven op project** of **Weergeven op rol** kunt u de volgende kolommen zien:

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: Alina: (some of the information in this area is also covered in Calculating Costs in the RP - https://workfront.zendesk.com/hc/en-us/articles/115004186433 - update this article also, when changes here occur)
  </MadCap:conditionalText>
  -->



   * Beschikbare uren, VTE of Kosten
   * Geplande uren, VTE of Kosten
   * Beoogde uren, VTE, of Kosten
   * Uren, FTE of Kostenvariatie
   * Nettouren, VTE of Kosten

* Wanneer u het **Weergeven op gebruiker** kunt u de volgende kolommen zien:

   * Beschikbare uren of FTE
   * Geplande uren of VTE
   * Uur- of FTE-verschil
   * Percentage toegewezen uren

>[!TIP]
>
>De informatie is niet beschikbaar als Kosten bij toepassing van de **Weergeven op gebruiker** aan de Planner van het Middel.
>
>Voor meer informatie over wat elke kolom toont, muis over de naam van de kolom waarin het aantal wordt getoond.\
>![Net_hours_res_planner_mouse_over.png](assets/net-hours-res-planner-mouse-over-350x95.png)
>
>Zie de volgende artikelen voor meer informatie over de gegevens die in elke kolom worden weergegeven:
>
>* [Overzicht van uren, FTE, en kosteninformatie in de mening van het Project en van de Rol van de Planner van het Middel](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)
>* [Beschikbare, geplande en Werkelijke uren of FTE weergeven in de bronnenplanner bij gebruik van de gebruikersweergave](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)
>


## Informatie weergeven per uur, VTE of Kosten

1. Ga naar de bronnenplanner.

   Door gebrek, informatievertoningen door Uren in de Planner van het Middel.

1. Vouw het keuzemenu uit.\
   ![Hours_font_or_cost_dropdown.png](assets/hours-fte-or-cost-dropdown.png)

1. Selecteer een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Uren</td> 
      <td>De beschikbaarheid en de toewijzingsinformatie van vertoningen in Uren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">FTE</td> 
      <td> <p>Geeft informatie over beschikbaarheid en toewijzing in FTE weer.</p> <p>Voor meer informatie over hoe FTE in de Planner van het Middel wordt berekend, zie <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kosten</td> 
      <td> <p>De beschikbaarheid en de toewijzingsinformatie van vertoningen door kosten, als u de Planner van het Middel in het Project of de meningen van de Rol bekijkt. De gegevens geven waarden weer in de valuta van uw systeem. De Workfront-beheerder definieert de systeemvaluta. Ga voor meer informatie over het instellen van de systeemvaluta in Workfront naar <a href="../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Wisselkoersen instellen</a>.</p> <p><b>OPMERKING</b>

   U moet gebruikers en baanrollen met de Tarieven van Kosten per Uur associëren om de informatie van Kosten in de Planner van het Middel te tonen.<br style="font-style: italic;">Voor meer informatie over het associëren van de Tarieven van Kosten per Uur met baanrollen, zie <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Taakrollen maken en beheren</a>.<br style="font-style: italic;">Voor meer informatie over het koppelen van Kosten per uur aan gebruikers, zie <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Gebruikersprofiel bewerken</a>.<br style="font-style: italic;">Voor meer informatie over hoe de Kosten in de Planner van het Middel worden berekend, zie <a href="../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md" class="MCXref xref">Kosten berekenen in de bronnenplanner </a>.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Aanpassen</td> 
      <td>Creeert een douanemening van de kolommen die in de Planner van het Middel tonen. Selecteer de opties die u wilt weergeven in de functie Bronnen, zoals beschreven in de onderstaande stappen. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Voorwaardelijk) Als u **Aanpassen** geeft u opties aan in het dialoogvenster **Weergegeven metriek aanpassen** aan opstelling uw douanemening.

   ![](assets/planner-customize-view-box-350x114.png)

1. In de **Type weergave** Selecteer een van de volgende weergaven in de linkerkolom:

   * Project
   * Rol
   * Gebruiker

1. In de **Geselecteerde items weergeven** selecteert u het type informatie dat u wilt weergeven in de kolommen van de geselecteerde weergave. In de volgende tabel wordt aangegeven welke opties beschikbaar zijn in elke weergave:

   | **Option** | Gebruikersweergave | Projectweergave | Rolweergave |
   |---|---|---|---|
   | Beschikbaar | ✔ | ✔ | ✔ |
   | Geplant | ✔ | ✔ | ✔ |
   | begroot |   | ✔ | ✔ |
   | Variantie |   | ✔ | ✔ |
   | Netto |   | ✔ | ✔ |
   | Werkelijk | ✔ |   |   |
   | Verschil | ✔ |   |   |
   | Percentage | ✔ |   |   |

1. Selecteren **Geplande (PLN) waarden in NETTOberekeningen gebruiken** om Gepland in plaats van begrote informatie te gebruiken wanneer het berekenen van de Netto waarden in de mening van het Project en van de Rol.

   Bij het selecteren van deze optie berekent Workfront de nettowaarden met behulp van de volgende formule:

   ```
   Net = Available - Planned
   ```

   >[!TIP]
   >
   >**Deze optie wordt alleen toegepast als u ten minste één optie selecteert om de weergave in de sectie Geselecteerde items weergeven aan te passen.**

1. Klikken **Opslaan**.

   De aangepaste weergave met de geselecteerde kolommen wordt weergegeven.

   In het vervolgkeuzemenu Uren geeft de aangepaste weergave als Aangepast weer.

   >[!NOTE]
   >
   >U kunt slechts één aangepaste weergave hebben.

   ![](assets/planner-hours-drop-down-with-custom-and-customize-option-183x281.png)

## Het diagram Gebruikerstoewijzing weergeven

U kunt de Geplande Toewijzing van gebruikers tegen hun beschikbaarheid in een grafiek tonen.

De toewijzing van gebruikers weergeven in een grafiek:

1. Ga naar de bronnenplanner.

   Voor meer informatie over de toegang tot van de Planner van het Middel, zie [Bronnen zoeken](../../resource-mgmt/resource-planning/get-started-resource-planner.md#accessing-the-resource-planner) in het artikel [Overzicht van de bronnenplanner](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

1. Selecteren **Weergeven op gebruiker**.

   >[!TIP]
   >
   >U kunt de grafiek van de Toewijzing van de Gebruiker slechts in de Mening van de Gebruiker bekijken.

1. Klik op de knop **Toewijzingsschema gebruiker** pictogram ![RP_user_assign_chart.png](assets/rp-user-allocation-chart.png) om de volgende informatie weer te geven:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beschikbaarheid % zonder overtoewijzing voor alle gebruikers</td> 
      <td>Dit is de hoeveelheid tijd dat alle gebruikers voor het werk in een tijdspanne beschikbaar zijn, die als percentage van hun totale beschikbare tijd wordt getoond. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Overtoewijzing % voor alle gebruikers </td> 
      <td> <p>Dit is de hoeveelheid tijd dat de gebruikers in een tijdspanne worden overgealloceerd, die als percentage van de totale beschikbare tijd wordt getoond.</p> <p><b>OPMERKING</b>

   Er vindt een overtoewijzing plaats wanneer de geplande uren hoger zijn dan de beschikbare uren. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Onderbenutting % voor alle gebruikers</td> 
      <td> <p>Dit is de hoeveelheid tijd die gebruikers in een tijdsperiode onderbenut worden, getoond als percentage van de totale beschikbare tijd.</p> <p><b>OPMERKING</b>

   Er is sprake van onderbenutting wanneer de geplande uren lager zijn dan de beschikbare uren. </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Er is een overtoewijzing voor ten minste één gebruiker gedurende deze periode</td> 
      <td>Dit geeft aan dat er sprake is van een overallocatie voor ten minste één gebruiker in een tijdsperiode, hoewel de totale hoeveelheid tijd van alle gebruikers niet wordt overschreden voor de tijdsperiode.<br>U moet door de lijst van gebruikers scrollen en de uren voor de gebruiker die wordt oververdeeld worden benadrukt in rood.</td> 
     </tr> 
    </tbody> 
   </table>

   ![RP__user_assign_chart_Dec._7_2017.png](assets/rp--user-allocation-chart-dec.-7--2017-350x148.png)

1. (Optioneel) Klik op de knop **Overtoewijzing % voor alle gebruikers** in het diagram.\
   Alle gebruikers die zijn oververdeeld, worden rood gemarkeerd.
1. (Optioneel) Klik op de knop **Onderbenutting % voor alle gebruikers** in het diagram.\
   Alle gebruikers die onvoldoende worden gebruikt, worden in blauw gemarkeerd.

1. (Optioneel) Klik op het pictogram van de indicator ![one_user_overassign_marker.png](assets/one-user-overallocation-marker.png) dat aantoont waar u minstens één gebruiker hebt oververdeeld.\
   De gebruikers die zijn oververdeeld, worden rood gemarkeerd.

1. (Optioneel) Vernieuw de pagina om het diagram samen te vouwen.
