---
title: Aan de slag met de Adobe Workfront Planning Designer
description: Met Adobe Planning Designer kunt u een nieuwe werkruimte genereren, compleet met recordtypen en velden in Workfront Planning, of objecten toevoegen aan een werkruimte of de wijzigingshistorie weergeven voor records.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: bf34bfa2059d227eca3faa3d719adcf4d711e457
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 0%

---


# Ga aan de slag met de Adobe Workfront Planning Designer

{{planning-important-intro}}

Met Adobe Planning Designer kunt u een nieuwe werkruimte genereren, compleet met recordtypen en velden in Workfront Planning, of objecten toevoegen aan een werkruimte of de wijzigingshistorie weergeven voor records.

>[!IMPORTANT]
>
>De Planning Designer is momenteel alleen beschikbaar voor gebruikers die deelnemen aan de gesloten bètafase.

## Toegangsvereisten <!--edit theses-->

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

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Inschrijven in het programma Closed Beta voor de Planning Designer

<!--edit this Or create a new article under Beta programs?? -->

U kunt op dit moment een verzoek indienen om deel te nemen aan het programma voor gesloten Beta voor de Planning Designer.

## Overwegingen bij de planning van Designer

<!--these are from the AI Assistant - edit these-->

* Als u de Planning Designer wilt gebruiken, moet u eerst de AI Assistant voor uw organisatie inschakelen. De AI Assistant is alleen beschikbaar voor iedereen in uw organisatie als het volgende is ingeschakeld:

   * De AI-assistent moet zijn ingeschakeld voor uw organisatie voordat deze beschikbaar is voor gebruikers in uw bedrijf. Voor informatie, zie [ AI Hulpoverzicht ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
   * Nadat Workfront de AI Assistant voor uw organisatie heeft ingeschakeld, is deze beschikbaar voor de Workfront-hoofdbeheerder. Voor informatie, zie [ basisinformatie voor uw systeem ](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md) vormen.

   * De Workfront-beheerder moet de AI-assistent inschakelen voor alle andere gebruikers. Voor meer informatie, zie [ toelaten of AI Medewerker ](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md) onbruikbaar maken.

   * De AI Assistant werkt in de context van elke pagina. De aanvragen die u voor de AI-assistent indient, moeten verwijzen naar functionaliteit die beschikbaar is op de pagina die u hebt geopend.

* Om de Planning Designer te gebruiken, moet een systeembeheerder het in het gebied van de Voorkeur van het Systeem van uw Opstelling toelaten.

* De acties die door de AI Medewerker in het Gebied van de Planning worden uitgevoerd zijn in de context van uw toestemmingen van de Planning van Workfront en uw toegangsniveau van Workfront. Raadpleeg de volgende artikelen voor meer informatie:

   * [Overzicht van het delen van machtigingen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Overzicht van licentietype bij gebruik van Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Wijzigingen die de AI-assistent namens de gebruiker aanbrengt, worden bijgehouden in het deelvenster Historie van de record.

* Met opdrachten kunt u handelingen ongedaan maken. U kunt bijvoorbeeld &quot;Laatste wijziging ongedaan maken&quot; typen om de wijziging ongedaan te maken.

* Wanneer u een object maakt, bijwerkt of verwijdert via AI Assistant, geeft AI Assistant de beoogde acties weer en wordt om bevestiging gevraagd. U kunt de acties vervolgens bevestigen of annuleren.

—>

## Momenteel beschikbare functionaliteit voor de Planning Designer

<!--edit these- they are from the Ai Assistant: 

Currently, the AI Assistant is available in the Planning area of Workfront for the following pages:

* Workspace page
* Record type page
* Record page

You can use the AI Assistant to perform the following actions, at this time:

* Search for records. You can search by information contained in any record fields. 
* Create records. An ID with a link to the new record displays after the record is created. You can specify the fields you want to update during the creation process, like dates or description. 
* Create records based on a document that you upload. Workfront supports the following document formats for the AI Assistant:

    PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT, and most image formats
* Update fields for the records you see on the screen
* Delete records
* Restore records that you just deleted

-->

U kunt of de Planning Designer of de Medewerker van AI gebruiken om het even welke volgende acties uit te voeren:

* Werkruimten maken en configureren

* Recordtypen maken

* Ontwerpvelden of formuleringsvelden

* Records maken, verwijderen, dupliceren en herstellen

* Een veld in een record bewerken, bijwerken of toevoegen

* Records koppelen aan andere records

* Historie van recordwijziging openen

* Aangepaste weergaven maken

* Maak records door een document te importeren. Het maken van records uit een geïmporteerd document is alleen beschikbaar in de plannings-Designer en niet in de AI-assistent. <!--add information about supported files-->

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Zoek de plannings-Designer in Workfront Planning

U kunt tot de Planning Designer van de belangrijkste pagina van de Planning van Workfront toegang hebben.

<!--add screen shot-->

U kunt de Medewerker van AI ook gebruiken om uit de zelfde functionaliteit voordeel te halen die de Planning Designer verstrekt.

## De Planing Designer voor uw organisatie inschakelen

Als beheerder van Workfront, moet u eerst de Planning Designer voor uw organisatie toelaten.

<!--add steps here-->

## Objecten maken of bijwerken met de planningsversie van Designer

U kunt voorwerpen in de Planning van Workfront tot stand brengen of bijwerken hetzij door de Planning Designer, of de Medewerker van AI te gebruiken, tenzij anders gespecificeerd.

1. Login aan Workfront, dan klik het **pictogram van het Belangrijkste Menu** het belangrijkste menu van Dots ![ in de hoger-juiste hoek van het scherm, of het ](assets/dots-main-menu.png) Belangrijkste **pictogram** het belangrijkste menu van Lijnen ![ in de upper-left hoek, als beschikbaar.](assets/lines-main-menu.png)

1. Klik **Planning**. Het planningsgebied wordt geopend.

1. Klik **Ontwerp met AI**.

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

   Een visuele voorvertoning wordt weergegeven met een voorbeeld van wat de assistent kan bouwen.

1. Nadat u een succesvol antwoord hebt ontvangen, volgt u de koppelingen in de opdrachtregel om het object van uw verzoek te maken, bij te werken of te bekijken.




