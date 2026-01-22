---
title: Aan de slag met de Adobe Workfront Planning Designer
description: Met Adobe Planning Designer kunt u een nieuwe werkruimte genereren, compleet met recordtypen en velden in Workfront Planning, objecten toevoegen aan een werkruimte of de wijzigingshistorie weergeven voor records.
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 866b237db5d109b0a435145119a6412e41d960ab
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 0%

---


<!--add these at release to the metadata:

author: Alina, Becky
feature: Workfront Planning
role: User, Admin -->

# Ga aan de slag met de Adobe Workfront Planning Designer

{{planning-important-intro}}

Met de Adobe Planning Designer aangedreven door AI kunt u een nieuwe werkruimte genereren, objecten toevoegen aan een werkruimte (recordtypen, records, weergaven of velden) of de wijzigingshistorie weergeven voor records.

>[!IMPORTANT]
>
>De plannings-Designer is momenteel alleen beschikbaar voor gebruikers die deelnemen aan het Closed Beta-programma.

Raadpleeg de volgende artikelen voor informatie over Workfront Planning:

* [Algemene informatie over Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md)
* [Aan de slag met Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Toegangsoverzicht voor Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md)


## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakketten</p></td> 
   <td> 
<p>Alle Workfront- en planningspakketten</p>
<p>Willekeurig workflowpakket en planningspakket</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Rechten beheren in een werkruimte </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr>  
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Inschrijven in het programma Closed Beta voor de Planning Designer

<!--edit this Or create a new article under Beta programs?? -->

U kunt op dit moment een verzoek indienen om deel te nemen aan het programma voor gesloten Beta voor de Planning Designer.

## Overwegingen bij de planning van Designer

* Als u de Designer voor planning wilt gebruiken, moet uw organisatie voldoen aan de vereisten voor het gebruik van de Workfront AI Assistant.

  Voor details, zie [&#x200B; Vereisten aan AI Medewerker &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

* Om de Planning Designer te gebruiken, moet een systeembeheerder het in het gebied van de Voorkeur van het Systeem van uw Opstelling toelaten.

* U kunt herinneringen gebruiken om de voorwerpen van de Planning te bouwen of door de Medewerker van Workfront te gebruiken AI van het Gebied van de Planning, of door de Planning Designer te gebruiken.

* De acties die door de Medewerker van AI in het Gebied van de Planning of worden uitgevoerd door de Planning Designer zijn in de context van uw toestemmingen van de Planning van Workfront en uw toegangsniveau van Workfront.

  Raadpleeg de volgende artikelen voor meer informatie:

   * [Overzicht van het delen van machtigingen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Overzicht van licentietype bij gebruik van Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Wijzigingen die door de planningsDesigner namens de gebruiker zijn aangebracht, worden bijgehouden in het historievenster van de record.

* Met opdrachten kunt u handelingen ongedaan maken. U kunt bijvoorbeeld &quot;Laatste wijziging ongedaan maken&quot; typen om de wijziging ongedaan te maken.

* Wanneer het creëren van, het bijwerken van, of het schrappen van een voorwerp door de Planning Designer, toont het de voorgenomen acties en verzoekt om bevestiging. U kunt de acties vervolgens bevestigen of annuleren.

* Wanneer u werkruimten en recordtypen maakt met de Designer voor planning, worden ook automatisch weergaven en velden gemaakt.

## Momenteel beschikbare functionaliteit voor de Planning Designer

U kunt of de Planning Designer of de Medewerker van AI gebruiken om het even welke volgende acties uit te voeren:

* Werkruimten maken en configureren

* Recordtypen maken

* Ontwerpvelden of formuleringsvelden

* Records maken, verwijderen, dupliceren en herstellen

* Een veld in een record bewerken, bijwerken of toevoegen

* Records koppelen aan andere records

* Historie van recordwijziging openen

* Aangepaste weergaven maken

* Maak records door een document te importeren.

  Het maken van records uit een geïmporteerd document is alleen beschikbaar in de plannings-Designer en niet in de AI-assistent.

  Voor informatie over de toegelaten dossiertypes en de grootte, zie de &quot;sectie van de Garanties van het Document&quot;in het artikel [&#x200B; Vulling van de Vorm van het Gebruik aangedreven door AI om een verzoek in te vullen gebruikend herinneringen of documenten &#x200B;](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## De Planing Designer voor uw organisatie inschakelen

Als beheerder van Workfront, moet u eerst de Planning Designer voor uw organisatie toelaten.

<!--add steps here-->

1. Meld u als systeembeheerder aan bij Workfront.
1. Klik **&#x200B;**&#x200B;Belangrijkste het menupictogram van het Hoofdmenu ![&#x200B; &#x200B;](assets/main-menu-shell.png) in de upper-left hoek van het scherm, dan klik **Opstelling**.
1. Klik **Systeem** > in het linkerpaneel, dan ga naar het **AI voorkeur** gebied.
1. Schakel de volgende instellingen in:
   * **laat AI** toe
   * **Opt binnen aan AI Bèta&#39;s**
   * **Planning Designer**

   ![&#x200B; plannende Designer die in de Voorkeur van het Systeem plaatst &#x200B;](assets/planning-designer-toggle-in-system-preferences.png)
1. Klik **sparen**.

   Alle gebruikers in het systeem die een Standaard vergunning hebben kunnen nu het **Ontwerp met AI** knoop op de belangrijkste pagina van Werkruimten in het planningsgebied zien. <!--check screen shot-->

   ![&#x200B; Ontwerp met AI knoop op de pagina van Werkruimten &#x200B;](assets/design-with-ai-button-on-workspaces-page.png)

   Alle gebruikers kunnen nu de Planning Designer starten en gebruiken om Workfront Planning-objecten te maken en bij te werken.

## Objecten maken of bijwerken met de planningsversie van Designer

U kunt voorwerpen in de Planning van Workfront tot stand brengen of bijwerken hetzij door de Planning Designer, of de Medewerker van AI te gebruiken, tenzij anders gespecificeerd.

1. Login aan Workfront, dan klik het **pictogram van het Belangrijkste Menu** het belangrijkste menu van Lijnen ![&#x200B; in de upper-left hoek.](assets/lines-main-menu.png)

1. Klik **Planning**. Het planningsgebied wordt geopend.

1. Klik **Ontwerp met AI**.

   Het **Planning Designer** venster opent.

   ![&#x200B; plannend het venster van Designer &#x200B;](assets/planning-designer-window.png)

1. Typ in de beschikbare ruimte opdrachten voor de AI-assistent en klik vervolgens op Enter wanneer u klaar bent.

   <!--add screen shot-->

   U kunt bijvoorbeeld een aanvraag typen die vergelijkbaar is met de onderstaande aanvragen:

   * Een werkruimte maken en configureren met vijf recordtypen voor het beheren van campagnes

   * Maak marketingcampagnes voor elke maand van het lopende jaar

   * Een campagneveld voor Status toevoegen voor de werkruimte Marketing Design

   * Alle records in de status Stale verwijderen

   * Alle planningscampagnes bijwerken naar de status Actief

   * Campagnes aansluiten op persoonlijke gegevens in de werkruimte Marketing Design

   * De wijzigingshistorie weergeven voor de campagne &quot;Valentijnsdag&quot;

   * Een tijdlijnweergave maken voor campagnes in de werkruimte Marketing Design

   * Maak records door een document te importeren. Het maken van records uit een geïmporteerd document is alleen beschikbaar in de plannings-Designer en niet in de AI-assistent.

   <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

1. Nadat u een succesvol antwoord hebt ontvangen, volgt u de koppelingen in het snelle gebied om het object van uw verzoek te maken, bij te werken of te bekijken.

   Als u ermee akkoord gaat uw objecten te maken, worden de wijzigingen rechts van het snelle gebied weergegeven.

   U kunt werkruimten, recordtypen, velden, weergaven en records in het voorvertoningsgebied rechts van de vraag bekijken.
1. (Optioneel) Typ aanvullende vragen om uw objecten verder te bewerken.
1. (Optioneel) Klik op het **pictogram** pictogram ![&#x200B; van de voorvertoning van de AI-werkruimte verbergen of weergeven &#x200B;](assets/hide-show-preview-screen-in-planning-designer.png) om het voorvertoningsscherm rechts te openen of te sluiten.
1. Klik de **Open werkruimte in nieuw lusjepictogram** ![&#x200B; Open werkruimte in nieuw lusjepictogram &#x200B;](assets/open-workspace-on-new-tab-icon.png) om de werkruimte te openen u in een nieuw lusje bijwerkt.
1. Klik het **Dichte** pictogram **X** om de Planning Designer te sluiten en het gebied van Werkruimten te openen.
1. Open de werkruimte die u hebt bewerkt met de Designer voor planning en breng verdere wijzigingen in de objecten aan.




