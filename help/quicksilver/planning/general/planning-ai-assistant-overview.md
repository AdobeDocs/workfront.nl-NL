---
title: Adobe Workfront Planning AI Assistant - Overzicht
description: U kunt de AI-assistent gebruiken om records te genereren, bij te werken of te verwijderen die zijn gebaseerd op de context van de huidige pagina en de recordstructuur. De bevelen van de gebruiker en de uitvoering van AI van die bevelen werken samen om ervoor te zorgen dat de veranderingen door AI worden aangebracht nauwkeurig in uw milieu worden weerspiegeld.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: 179a20f1ae6ab723963cc78e9573560968500ac5
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---


# Adobe Workfront Planning AI Assistant - overzicht

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->


{{planning-important-intro}}

Met de AI-assistent kunt u records genereren, bijwerken of verwijderen op basis van de context en de recordstructuur van de huidige pagina.

De bevelen van de gebruiker en de uitvoering van AI van die bevelen werken samen om ervoor te zorgen dat de veranderingen door AI worden aangebracht nauwkeurig in uw milieu worden weerspiegeld.

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

## Overwegingen over de AI-assistent

* De AI-assistent moet zijn ingeschakeld voor uw organisatie voordat deze beschikbaar is voor gebruikers in uw bedrijf. Voor informatie, zie [&#x200B; AI Hulpoverzicht &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
* Nadat Workfront de AI Assistant voor uw organisatie heeft ingeschakeld, is deze beschikbaar voor de Workfront-hoofdbeheerder. Voor informatie, zie [&#x200B; basisinformatie voor uw systeem &#x200B;](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md) vormen.

* De Workfront-beheerder moet de AI-assistent inschakelen voor alle andere gebruikers. Voor meer informatie, zie [&#x200B; toelaten of AI Medewerker &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md) onbruikbaar maken.

* De AI Assistant werkt in de context van elke pagina. De aanvragen die u voor de AI-assistent indient, moeten verwijzen naar functionaliteit die beschikbaar is op de pagina die u hebt geopend.

* De acties die door de AI Medewerker in het Gebied van de Planning worden uitgevoerd zijn in de context van uw toestemmingen van de Planning van Workfront en uw toegangsniveau van Workfront. Raadpleeg de volgende artikelen voor meer informatie:

   * [Overzicht van het delen van machtigingen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Overzicht van licentietype bij gebruik van Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Wijzigingen die de AI-assistent namens de gebruiker aanbrengt, worden bijgehouden in het deelvenster Historie van de record.

* De acties van de AI-assistent zijn permanent en kunnen onomkeerbaar zijn. Zo kan het verwijderen van een veld niet ongedaan worden gemaakt. Controleer alle acties die door de AI-assistent zijn voorgesteld voordat u deze accepteert.

* Wanneer u een object maakt, bijwerkt of verwijdert via AI Assistant, geeft AI Assistant de beoogde acties weer en wordt om bevestiging gevraagd. U kunt de acties vervolgens bevestigen of annuleren.

## Momenteel beschikbare functionaliteit voor de AI-assistent

Momenteel is de AI Assistant beschikbaar in het planningsgebied van Workfront voor de volgende pagina&#39;s:

* Workspace-pagina
* Tekstpagina opnemen
* Pagina opnemen

Met de AI-assistent kunt u op dit moment de volgende handelingen uitvoeren:

* Zoeken naar records. U kunt zoeken op informatie in alle recordvelden.
* Records maken. Een id met een koppeling naar de nieuwe record wordt weergegeven nadat de record is gemaakt. U kunt opgeven welke velden u wilt bijwerken tijdens het maken, zoals datums of beschrijving.
* Maak records op basis van een document dat u uploadt. Workfront ondersteunt de volgende documentindelingen voor de AI Assistant:

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT en de meeste afbeeldingsindelingen
* Velden bijwerken voor de records die u op het scherm ziet
* Records verwijderen
* Recten herstellen die u zojuist hebt verwijderd


## AI Assistant zoeken in Workfront-planning

U kunt de AI-assistent vinden op de volgende gebieden van de Workfront-planning:

* De hoofdnavigatiebalk, in de rechterbovenhoek van het scherm.
* Binnen het detailsgebied van een record, nadat u de record in de voorvertoning hebt geopend of nadat u de recordpagina hebt geopend.

## De AI-assistent openen in het planningsgebied

1. Login aan Workfront, dan klik het **pictogram van het Belangrijkste Menu** het belangrijkste menu van Dots ![&#x200B; in de hoger-juiste hoek van het scherm, of het &#x200B;](assets/dots-main-menu.png) Belangrijkste **pictogram** het belangrijkste menu van Lijnen ![&#x200B; in de upper-left hoek, als beschikbaar.](assets/lines-main-menu.png)

. Klik **Planning**. Het planningsgebied wordt geopend.

1. Klik a **werkruimtekaart**.

1. (Facultatief) klik a **verslagtype kaart**.

1. (Facultatief) klik a **verslag** om de 2&rbrace; Details van het verslag **pagina te openen.**

1. Klik het **AI Hulppictogram** in de hoger-juiste hoek van het scherm in de globale navigatiebar of in de hoger-juiste hoek van de voorproef of de pagina van het verslag.

   ![&#x200B; AI Hulp pictogram &#x200B;](assets/ai-assistant-icon-highlighted.png)

1. Typ in de beschikbare ruimte opdrachten voor de AI-assistent en klik vervolgens op Enter wanneer u klaar bent.

   ![&#x200B; AI Medewerker paneel met lege beveldoos &#x200B;](assets/ai-assistant-panel-with-empty-command-box.png)

   U kunt bijvoorbeeld een van de volgende typen:

   * Maak een campagne met een startdatum van 4 juli en een einddatum van 30 juli
   * Het veld Beschrijving van de record in de zomercampagne bijwerken met de datum die moet worden bepaald
   * Laatste record verwijderen
   * De record herstellen

   Een visuele indicator toont terwijl de Medewerker AI bevelen verwerkt, die verwachtingen voor reactietijd plaatsen.

   Na ontvangst van een succesvolle reactie, volg de verstrekte verbindingen of merk de veranderingen op de linkerzijde op.



