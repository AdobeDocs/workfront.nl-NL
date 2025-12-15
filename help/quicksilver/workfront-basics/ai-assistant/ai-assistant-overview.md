---
title: AI Assistant in Workfront
content-type: reference
description: Meer informatie over AI-assistent in Adobe Workfront
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
source-git-commit: 44db621643c76ab1f2c1b51d5e81cb0d1f827a58
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 1%

---

# AI Assistant in Workfront

Met Workfront AI Assistant kunt u uw werk uitvoeren door informatie en suggesties in een gesprek in een natuurlijke taal aan te bieden. Met AI Assistant kunt u werken vloeiender maken met

* Werkitems of documenten samenvatten
* Instructies of referentiemateriaal voor werkprocessen vinden
* Formules genereren of controleren voor berekende velden

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td><p>Nieuw: alle</p>
       <p>of</p>
       <p>Huidig: Niet beschikbaar</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Niet beschikbaar</p></td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten voor AI Assistant

Om AI Medewerker voor uw organisatie toe te laten, **allen** van het volgende moet van toepassing zijn:

* Uw organisatie moet zijn gemigreerd naar Adobe IMS (Identity Management System)
* De Adobe Unified Experience moet worden ingeschakeld
* Uw organisatie moet een Select-, Prime- of Ultimate Workfront-abonnement hebben
* Adobe moet een ondertekende Adobe Gen AI-overeenkomst hebben in het bestand

  Voor meer informatie bij het ondertekenen van de overeenkomst, zie [&#x200B; de overeenkomst van Adobe Gen AI &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) in dit artikel ondertekenen.

## Overwegingen over AI Assistant

* AI Assistant is contextgevoelig voor de pagina die u hebt geopend. Als u bijvoorbeeld &quot;Dit project samenvatten&quot; opgeeft in AI Assistant op een projectpagina, wordt een overzicht van dat specifieke project geretourneerd.
* De Workfront-beheerder moet AI Assistant inschakelen voor gebruikers in uw organisatie. De Medewerker van AI wordt toegelaten door toegangsniveaus.

  Voor meer informatie, zie [&#x200B; toelaten of AI Medewerker &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md) onbruikbaar maken.

* Workfront Planning AI Assistant heeft andere functies dan Workfront AI Assistant.

  Voor meer informatie over AI Medewerker in de Planning van Workfront, zie [&#x200B; de Planning AI van Adobe Workfront Hulpoverzicht &#x200B;](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

* AI Assistant is momenteel alleen beschikbaar in het Engels.


## Functie beschikbaar in AI Assistant

AI Assistant biedt momenteel de volgende functionaliteit:

* Samenvattend projecten, taken, kwesties, of documenten.

  Voor meer informatie, zie [&#x200B; samenvatten gebruikend AI Medewerker &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* Instructies of referentiemateriaal uit de documentatie van Workfront op Adobe Experience League.

  Voor meer informatie, zie [&#x200B; hulp van AI Medewerker &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md) krijgen.

* Specifieke items zoeken in Workfront.

  Voor meer informatie, zie [&#x200B; Medewerker van het Gebruik AI om met projecten, taken, en kwesties &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md) te werken.

* Formules genereren of verfijnen voor berekende aangepaste velden.

  >[!NOTE]
  >
  >Deze functionaliteit is alleen beschikbaar voor organisaties op de Prime- of Ultimate Workfront-plannen.

  Voor meer informatie, zie [&#x200B; berekende gebiedsformules met AI Medewerker &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md) produceren of herzien.

* Het samenvatten van updates, geüploade documenten, en andere opmerkelijke veranderingen over uw projecten binnen de volgende termijnen: 24 uren, 3 dagen, 7 dagen in Prioriteiten.

Voor meer informatie, zie [&#x200B; Vangst op het werk in Prioriteiten &#x200B;](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).


## Objecttypen beschikbaar voor AI Assistant

De AI-assistent kan query&#39;s uitvoeren op gegevens die zijn gekoppeld aan de volgende objecttypen als de gebruiker over de geldige machtigingen in Workfront beschikt:

* Portfolio&#39;s
* Programma&#39;s
* Projecten
* Taken
* Problemen
* Aangepaste formulieren
* Gebruikers
* Workfront-planningsrecords


## AI-assistent openen

1. Bij de bovenkant van om het even welke pagina van Workfront, klik het AI Hulppictogram ![&#x200B; AI Hulppictogram &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Typ uw vraag of vraag in het paneel rechts van het scherm.

   Als u niet in dit deelvenster kunt typen, heeft uw organisatie geen ondertekende Adobe Gen AI-overeenkomst in het bestand.

1. Als de AI-assistent niet het gewenste antwoord geeft, verfijnen dan uw vraag en probeer het opnieuw.

## Onderteken de Adobe Gen AI-overeenkomst

Als uw organisatie geen ondertekende Adobe Gen AI-overeenkomst in het bestand heeft, kan AI Assistant niet worden ingeschakeld voor uw organisatie.

Als een gebruiker probeert om AI Assistant te gebruiken terwijl de Adobe Gen AI-overeenkomst niet is ondertekend, wordt een bericht weergegeven:

* Gebruikers: gebruikers worden ervan op de hoogte gesteld dat AI Assistant niet is ingeschakeld voor hun organisatie en dat zij contact kunnen opnemen met hun Workfront-beheerder om deze aan te vragen voor hun organisatie.
* Beheerders: beheerders worden ervan op de hoogte gesteld dat er geen ondertekende Adobe Gen AI-overeenkomst is en kunnen verzoeken dat een kopie van de overeenkomst ter ondertekening wordt verzonden.

De Adobe Gen AI-overeenkomst aanvragen:

1. Als Beheerder van Workfront, klik het AI Hulppictogram ![&#x200B; AI Hulppictogram &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Typ tekst in het deelvenster AI Assistant.
1. Wanneer het de overeenkomstenbericht van Adobe Gen AI verschijnt, klik **overeenkomst van het Overzicht**.
1. Voer de naam en het e-mailadres in van de persoon in uw organisatie die de Adobe Gen AI-overeenkomst zal ondertekenen.

   De overeenkomst wordt ter ondertekening naar deze persoon verzonden. Nadat de overeenkomst is ondertekend en geretourneerd, wordt deze gereviseerd door Adobe en wordt AI Assistant ingeschakeld voor uw organisatie.

   >[!NOTE]
   >
   >Sta 1 tot 3 werkdagen na ondertekening en retournering van de overeenkomst voor Adobe toe om AI Assistant te beoordelen en in te schakelen.

## Tips voor het maken van herinneringen in AI Assistant

Gebruik de volgende trefwoorden in uw vragen om context en hulp te bieden bij het zoeken naar de juiste gegevens. Trefwoorden zijn niet hoofdlettergevoelig.

Neem de uitdrukking `using (keyword)` op wanneer u een vraag opgeeft.

| Trefwoord | Effect |
|---|---|
| `workfront` | Interactie met Workfront. |
| `planning` | Interageert met de Planning van Workfront. |
| `help` | Retourneert informatie uit Experience League-documentatie. |
| `formula` | Controleert en keert formules voor gebruik in Planning, Opstelling, of douanevormen terug. |
| `health` | Controleert projectgezondheid met de Adviseur van de Gezondheid van het Project. |
| `summarize` | Hiermee geeft u een overzicht van items, bijvoorbeeld wanneer u een bestand uploadt of een project samenvat. |

>[!NOTE]
>
> Niet alle trefwoorden zijn in alle gebieden beschikbaar.
>
>* Het trefwoord `formula` is alleen beschikbaar in Planning, Setup en de Aangepaste formulierbuilder.
>* Het trefwoord `planning` is alleen beschikbaar via Workfront Planning.





