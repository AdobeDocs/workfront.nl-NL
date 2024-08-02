---
title: Overzicht van het delen van machtigingen in Adobe Workfront Planning
description: U kunt machtigingen delen of verwijderen in een Adobe Workfront-werkruimte of -weergave voor planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 1ffd8a3dbb31154186dc37132c7e77c35de42ac3
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Overzicht van het delen van machtigingen in Adobe Workfront Planning

{{planning-important-intro}}

U kunt machtigingen delen of verwijderen in een werkruimte of weergave in Adobe Workfront Planning.

In dit artikel worden de machtigingsniveaus voor Workfront Planning-objecten beschreven.

Zie de volgende artikelen voor informatie over het delen van werkruimten of weergaven:

* [Werkruimten delen](/help/quicksilver/planning/access/share-workspaces.md)

* [Weergaven delen](/help/quicksilver/planning/access/share-views.md)

## Objecten die u kunt delen in Adobe Workfront Planning

U kunt de volgende objecten delen:

* Werkruimten

   * U kunt werkruimten delen met personen binnen uw organisatie.
   * Wanneer u een werkruimte deelt, worden ook alle recordtypen, records en velden gedeeld die aan de werkruimten zijn gekoppeld. Weergaven worden niet gedeeld.

* Weergaven

   * U moet gebruikers, inclusief systeembeheerders, machtigingen geven om toegang te krijgen tot weergaven die los staan van hun machtigingen voor toegang tot werkruimten.
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
| Maken | ✓ |            |       |
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