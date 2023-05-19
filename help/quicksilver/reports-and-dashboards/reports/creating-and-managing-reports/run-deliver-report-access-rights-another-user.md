---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Een rapport uitvoeren en leveren met de toegangsrechten van een andere gebruiker
description: Door gebrek, kunnen de gebruikers de voorwerpen in een rapport slechts zien dat zij toestemmingen aan Mening hebben.
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: e68e470da3b03e418584898c4098f0be302c68ec
workflow-type: tm+mt
source-wordcount: '1206'
ht-degree: 0%

---

# Een rapport uitvoeren en leveren met de toegangsrechten van een andere gebruiker

Door gebrek, kunnen de gebruikers de voorwerpen in een rapport slechts zien dat zij toestemmingen aan Mening hebben.

U kunt alle gebruikers toestaan om de zelfde resultaten in een rapport als een andere gebruiker, ongeacht hun toegangsniveau of toestemmingsniveau op de voorwerpen binnen het rapport te zien.

Als u een rapport met de toegangsrechten van een andere gebruiker in werking stelt die hogere toegang (bijvoorbeeld, de toegangsrechten van een beheerder van Adobe Workfront) heeft, kunnen alle gebruikers die toestemmingen hebben om het rapport te bekijken de informatie in het rapport als gebruiker zien die in de rapportbouwer wordt gespecificeerd. U kunt dit instellen voor zowel rapporten die gebruikers vinden in de Workfront-interface als voor rapporten die als bijlage bij een e-mailbericht aan gebruikers worden bezorgd.

>[!TIP]
>
>U moet de opdracht **Voer dit rapport uit met de toegangsrechten van:** veld met een actieve gebruiker alleen als u het rapport wilt weergeven met de toegangsrechten van die gebruiker. Bijvoorbeeld, zou een werk-vergunning gebruiker geen toestemmingen kunnen hebben om alle punten in een rapport te zien dat door een plan-vergunning gebruiker of een Beheerder van het Systeem wordt gebouwd, tenzij het rapport met de toegangsrechten van een Planner of een Beheerder van het Systeem toont.\
Als het rapport wordt gedeeld met gebruikers met vergelijkbare toegang als de gebruiker die is opgegeven in het dialoogvenster **Voer dit rapport uit met de toegangsrechten van:** veld kunt u dit veld leeg laten.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening aan een rapport (om het geleverde rapport te bekijken)</p> <p>Rechten beheren voor een rapport (om het rapport uit te voeren)</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Een rapport weergeven met de toegangsrechten van een andere gebruiker

De **Voer dit Rapport uit met de toegangsrechten van:** het gebied verzekert een rapport de zelfde gegevens bevat, ongeacht welke gebruiker tot het rapport toegang heeft. Het rapport wordt weergegeven zoals het zou zijn voor de opgegeven gebruiker.

De gebruikers die tot het rapport toegang hebben moeten minstens de toestemmingen van de Mening op het rapport hebben om het te kunnen zien. Als de gebruiker in **Voer dit Rapport uit met de toegangsrechten van:** het veld is gedeactiveerd, wordt het rapport niet meer weergegeven voor andere gebruikers met wie het rapport wordt gedeeld.

Een rapport uitvoeren met de toegangsrechten van een andere gebruiker:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Rapporten**.

1. Selecteer het rapport dat u wilt weergeven met de toegangsrechten van een andere gebruiker.
1. Klikken **Handelingen rapporteren** en klik vervolgens op **Bewerken**.

1. Klikken **Rapportinstellingen**.

1. In de **Voer dit rapport uit met de toegangsrechten van:** veld, typt u de naam van de gebruiker die het rapport moet weergeven als, en selecteert u het rapport wanneer het in de lijst wordt weergegeven.\
   ![](assets/qs-access-rights-of-350x251.png)

   >[!NOTE]
   Gebruikers met een lager toegangsniveau die rapporten mogen samenstellen, kunnen geen andere gebruiker dan henzelf selecteren voor de **Voer dit Rapport uit met de toegangsrechten van:** veld.

1. Klikken **Gereed**.
1. Klikken **Opslaan + Sluiten**.\
   Het rapport wordt nu weergegeven voor alle gebruikers met wie het rapport wordt gedeeld alsof het is bekeken door de gebruiker die is opgegeven in het dialoogvenster **Voer dit rapport uit met de toegangsrechten van:** veld.

>[!IMPORTANT]
Het ingaan van een andere gebruiker dan het programma geopende gebruiker voor **Voer dit rapport uit met de toegangsrechten van:** het gebied beïnvloedt de informatie die in het rapport wordt getoond als het rapport een filter bevat dat een vervanging gebruikt die naar de het programma geopende gebruiker verwijst. Het rapport wordt weergegeven op basis van de waarde die is opgegeven in het dialoogvenster **Voer dit rapport uit met de toegangsrechten van:** in plaats van wat wordt gedefinieerd in het jokertekenfilter.
Voor meer informatie over vervangingen voor gebruikersgebieden, zie de &quot;Op gebruiker-gebaseerde variabelen&quot;sectie in [Variabelen van jokerfilter](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Een rapport leveren met de toegangsrechten van een andere gebruiker

U kunt rapporten instellen die als bijlage bij een e-mailbericht moeten worden bezorgd. U kunt opstelling deze geleverde rapporten aan vertoning aangezien zij voor gebruikers van een hoger toegangsniveau tonen, zodat kunnen alle gebruikers de zelfde informatie in de geleverde rapporten zien. De gebruikers die het rapport zullen zien dat in e-mail wordt geleverd moeten aan Send aan lijst van ontvangers binnen de rapportlevering worden toegevoegd. Raadpleeg het artikel voor meer informatie over het instellen van een rapport voor levering [Overzicht van levering rapporteren](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Een rapport leveren met de toegangsrechten van een andere gebruiker:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Rapporten**.

1. Selecteer het rapport dat u wilt leveren met de toegangsrechten van een andere gebruiker.
1. Klik op de naam van het rapport om het te selecteren.
1. Klikken **Handelingen rapporteren**.
1. Klikken **Rapport verzenden**.

1. In de **Dit rapport leveren met de toegangsrechten van:** veld, typt u de naam van de gebruiker die het rapport moet weergeven alsof het in een e-mailbericht wordt verzonden en selecteert u deze vervolgens wanneer het rapport in de lijst wordt weergegeven. Het gebrek is de naam van de gebruiker die het rapport bouwt.\
   ![](assets/qs-send-report-access-rights-of-350x446.png)

   >[!NOTE]
   Gebruikers met een lager toegangsniveau die rapporten mogen samenstellen, kunnen geen andere gebruiker dan henzelf selecteren voor de **Dit rapport leveren met de toegangsrechten van:** veld.

1. Selecteer **Indeling** u wilt dat het rapport in de e-mail wordt weergegeven:

   * HTML
   * PDF
   * MS Excel
   * MS Excel (.xlsx)
   * TSV

1. Klikken **Nu verzenden** om het onmiddellijk te verzenden.\
   of\
   Klikken **Herhalende levering maken** om een terugkomende levering voor het rapport te plannen.\
   Raadpleeg het artikel voor meer informatie over rapportleveringen [Overzicht van levering rapporteren](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Beperkingen voor rapporten met een kolom Bron

In de volgende rapporten wordt een kolom Bron weergegeven waarin u informatie over het bovenliggende object kunt weergeven:

* Problemen melden
* Uur
* Documentrapporten

Als de gebruikers geen toestemmingen aan het oudervoorwerp van een kwestie, een uur, of een document hebben, toont de Bronkolom van het rapport leeg, zelfs wanneer het rapport aan vertoning wordt gevormd, of met de toegangsrechten van een andere gebruiker moet worden geleverd.

Om informatie over het oudervoorwerp in het rapport te tonen, adviseren wij toevoegend een kolom voor het oudervoorwerp waar u de naam van de ouder kunt tonen.

Bijvoorbeeld, kunt u om het even welke volgend aan een rapport met een Bronkolom toevoegen:

* De kolommen van de Naam van het Project, van de Naam van de Taak, of van de Naam van de Uitgave aan een document of een uurrapport.
* De kolommen van de Naam van het Project of van de Naam van de Taak aan een probleemrapport.
* Een kolom die expressies in tekstmodus gebruikt die naar alle drie objecten verwijzen. Hier volgt een voorbeeld van een uurrapport:

   `displayname=Custom Source`

   `linkedname=opTask`

   `namekey=view.relatedcolumn`

   `namekeyargkey.0=opTask`

   `namekeyargkey.1=name`

   `textmode=true`

   `valueexpression=IF(!ISBLANK({opTaskID}),{opTask}.{name},IF(!ISBLANK({taskID}),{task}.{name},IF(!ISBLANK({projectID}),{project}.{name},IF(!ISBLANK({timesheetID}),CONCAT({owner}.{name}," ",{timesheet}.{startDate}," - ",{timesheet}.{endDate}),""))))`

   `valueformat=HTML`

   Voor informatie over de weergaven van de tekstmodus raadpleegt u [Een weergave bewerken in de tekstmodus](../text-mode/edit-text-mode-in-view.md).