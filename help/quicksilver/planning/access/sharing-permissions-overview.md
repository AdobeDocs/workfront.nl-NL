---
title: Overzicht van deelmachtigingen in Adobe Workfront-planning
description: Niet alle gebruikers in de organisatie hebben de zelfde toegang en de toestemmingen om de Planning van Adobe Workfront te gebruiken. In dit artikel wordt algemene informatie beschreven over het delen of verwijderen van machtigingen voor een Adobe Workfront Planning-werkruimte of -weergave.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 00e58ea9a207037b701e1be010c2c4c2995d60e0
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 0%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Overzicht van het delen van machtigingen in Adobe Workfront Planning

{{planning-important-intro}}

U kunt machtigingen delen of verwijderen in een Adobe Workfront-werkruimte of -weergave voor planning.

In dit artikel worden de machtigingsniveaus voor Workfront Planning-objecten beschreven.

Zie de volgende artikelen voor informatie over het delen van werkruimten of weergaven:

* [Werkruimten delen](/help/quicksilver/planning/access/share-workspaces.md)

* [Weergaven delen](/help/quicksilver/planning/access/share-views.md)

## Objecten die u kunt delen in Adobe Workfront Planning

U kunt de volgende objecten delen:

* Werkruimten

   * U kunt werkruimten delen met personen binnen uw organisatie.
   * Wanneer u een werkruimte deelt, worden ook alle recordtypen, records en velden gedeeld die aan de werkruimten zijn gekoppeld.
   * Als u een werkruimte deelt, worden de weergaven niet gedeeld. Weergaven worden afzonderlijk gedeeld.

* Weergaven

   * U moet gebruikers, met inbegrip van de Beheerders van het Systeem, toestemmingen verlenen om tot meningen los van hun toestemmingen toegang te hebben tot werkruimten.
   * Wanneer u een weergave deelt, worden alle weergave-elementen gedeeld, inclusief filters, groeperen, sorteren of Instellingen.
   * Wanneer u een weergave deelt, worden de records die zichtbaar zijn in de weergave niet gedeeld. Records moeten worden gedeeld door werkruimten te delen.
   * U kunt een mening openbaar delen, met mensen buiten uw organisatie wanneer u een openbare verbinding voor een mening produceert.De mensen die tot de verslagpagina van een openbare verbinding toegang hebben kunnen alle verslagen en hun gebieden, met inbegrip van verbonden verslagen en gebieden bekijken.

  Voor informatie, zie [ meningen van het Aandeel ](/help/quicksilver/planning/access/share-views.md).

Intern kunt u een werkruimte of weergave delen met de volgende Workfront-entiteiten:

* Gebruikers
* Groepen

## Overwegingen bij het delen van objecten in Adobe Workfront Planning

* Uw Adobe Workfront-licentietype werkt in combinatie met uw Workfront-planningsmachtigingen en geeft u toegang tot de werkruimten en de bijbehorende objecten, en tot het weergeven, bijdragen of beheren van deze werkruimten.

  Voor informatie over hoe de vergunningstypes toestemmingsniveaus voor de Planning van Workfront beïnvloeden, zie [ het type van Vergunning overzicht wanneer het gebruiken van de Planning van Adobe Workfront ](/help/quicksilver/planning/access/license-type-overview.md).
* Systeembeheerders kunnen alle werkruimten in het systeem beheren, inclusief de werkruimten die ze niet hebben gemaakt.
* Andere gebruikers, waaronder Systeembeheerders, hebben alleen toegang tot weergaven die ze hebben gemaakt of die met hen zijn gedeeld. Systeembeheerders kunnen alleen machtigingen krijgen om een weergave te beheren.
* U kunt een koppeling naar een werkruimte of naar een weergave delen met anderen.

  De volgende scenario&#39;s bestaan:
   * Gebruikers die de koppeling naar een werkruimte ontvangen, moeten actieve gebruikers zijn en zich aanmelden bij Workfront om toegang te krijgen tot de werkruimte.
   * Gebruikers die de koppeling naar een weergave ontvangen, hebben op de volgende manieren toegang tot de weergave:

      * U moet actieve gebruikers zijn en u aanmelden bij Workfront als de koppeling naar de weergave intern is gedeeld.
      * Kan externe gebruikers naar Workfront zijn en de weergave openen via een openbaar gedeelde koppeling, zonder u aan te melden bij Workfront.

## Machtigingen delen voor Adobe Workfront Planning-objecten

De tabellen in de volgende secties tonen het machtigingsniveau dat u kunt selecteren bij het delen van een werkruimte of weergave en welke functionaliteit op elk niveau is toegestaan.

>[!IMPORTANT]
>
>Niet alle gebruikers kunnen de hieronder beschreven toestemmingsniveaus hebben. De individuele vergunning van gebruikers bepaalt welk niveau van toestemmingen zij voor de voorwerpen van de Planning van Workfront kunnen ontvangen.
>
>Alleen gebruikers met een standaardlicentie (of abonnement) kunnen beschikken over Contribute- of beheermachtigingen voor werkruimten en de machtiging Beheren voor weergaven.
> 
>Gebruikers met alle andere licentietypen kunnen weergavemachtigingen hebben voor werkruimten en weergaven.
>
>Voor informatie, zie [ het type van Vergunning overzicht wanneer het gebruiken van de Planning van Adobe Workfront ](/help/quicksilver/planning/access/license-type-overview.md).


### Workspace-machtigingen

U moet gebruikers toestemming geven aan werkruimten om hen toegang tot de volgende entiteiten te verlenen:

* Werkruimten
* Recordtypen
* Records
* Velden

Hieronder vindt u de machtigingsniveaus voor werkruimten:

|        | Beheren | Contribute | Weergave |
|--------|--------|------------|-------|
| Bewerken | ✓ |            |       |
| Delen | ✓ |            |       |
| Verwijderen | ✓ |            |       |
| Weergave | ✓ | ✓ | ✓ |

### Machtigingen voor recordtype

De toestemmingen van het Type van verslag worden geërft wanneer u toestemmingen aan de werkruimte verleent.

Hieronder vindt u de machtigingsniveaus voor recordtypen:


|        | Beheren | Contribute | Weergave |
|--------|--------|------------|-------|
| Maken | ✓ |            |       |
| Verwijderen | ✓ |            |       |
| Bewerken | ✓ |            |       |
| Weergave | ✓ | ✓ | ✓ |

### Machtigingen opnemen

De toestemmingen van het verslag worden geërft wanneer u toestemmingen aan de werkruimte verleent.

Hieronder vindt u de machtigingsniveaus voor records:


|        | Beheren | Contribute | Weergave |
|--------|--------|------------|-------|
| Maken | ✓ | ✓ |       |
| Verwijderen | ✓ | ✓ |       |
| Bewerken | ✓ | ✓ |       |
| Weergave | ✓ | ✓ | ✓ |

### Veldmachtigingen

De toestemmingen van het gebied worden geërft wanneer u toestemmingen aan de werkruimte verleent.
De volgende machtigingen verwijzen naar de velden zelf en niet naar de waarden die aan elk veld zijn gekoppeld. Als u veldwaarden wilt bewerken, moet u over machtigingen beschikken om records te bewerken.

|        | Beheren | Contribute | Weergave |
|--------|--------|------------|-------|
| Maken | ✓ |            |       |
| Verwijderen | ✓ |            |       |
| Bewerken | ✓ |            |       |
| Weergave | ✓ | ✓ | ✓ |


### Machtigingen weergeven

U moet afzonderlijke machtigingen verlenen om weergaven op te nemen. Het verlenen van toestemmingen aan de werkruimte verleent geen toestemmingen aan de verslagmeningen in de werkruimte.

U moet gebruikers toestemming geven om weergaven weer te geven, zodat ze toegang hebben tot de volgende weergave-elementen:

* Filters
* Zichtbaarheid veld
* Sorteren
* Groepering
* Rijhoogte
* Instellingen

U kunt weergaven intern of openbaar delen.

Hier volgen de machtigingsniveaus voor weergaven en weergave-elementen:

| Intern delen | Beheer (alleen uitgenodigde personen hebben toegang) | Weergave (alleen uitgenodigde personen hebben toegang) | Iedereen in de werkruimte kan* weergeven |
|--------|--------|-------|------------------------------|
| Bewerken | ✓ |       |                            |
| Verwijderen | ✓ |       |                            |
| Delen | ✓ |       |                           |
| Weergave | ✓ | ✓ | ✓ |
| Toepassen | ✓ | ✓ | ✓ |

| Openbare delen | Weergave |
|--------|-------|
| Weergave | ✓ |
| Toepassen | ✓ |

*Gebruikers moeten over weergave- of hogere machtigingen voor een werkruimte beschikken om toegang te krijgen tot deze weergave.

<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |  


|        | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Access the view  | ✓      | ✓     | ✓                          |
| Apply temporary filters, groupings, sort  | ✓      | ✓     | ✓                          |
-->