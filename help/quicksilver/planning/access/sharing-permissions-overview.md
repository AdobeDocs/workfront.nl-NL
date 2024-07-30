---
title: Overzicht van het delen van machtigingen in Adobe Workfront Planning
description: U kunt machtigingen delen of verwijderen in een Adobe Workfront-werkruimte of -weergave voor planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 6f1f669f7e2235637864a92a40aadbfb19b4310b
workflow-type: tm+mt
source-wordcount: '692'
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

  Wanneer u een werkruimte deelt, worden ook alle recordtypen, records en velden gedeeld die aan de werkruimten zijn gekoppeld. Weergaven worden niet gedeeld.

* Weergaven

   * U moet gebruikers, inclusief systeembeheerders, machtigingen geven om toegang te krijgen tot weergaven die los staan van hun machtigingen voor toegang tot werkruimten. Voor informatie, zie [ meningen van het Aandeel ](/help/quicksilver/planning/access/share-views.md).
     <!--* You can share a view publicly, with people outside your organization when you generate a public link for a view.People accessing the record page from a public link can view all records and their fields, including connected records and fields.-->
     <!--move the link above to the end of this section-->

U kunt een werkruimte of een weergave delen met de volgende entiteiten:

* Gebruikers
* Groepen

## Overwegingen bij het delen van objecten in Adobe Workfront Planning

* Uw Adobe Workfront-licentietype werkt in combinatie met uw Workfront-planningsmachtigingen en geeft u toegang tot de werkruimten en de bijbehorende objecten, en tot het weergeven, bijdragen of beheren van deze werkruimten.

  Voor informatie over hoe de vergunningstypes toestemmingsniveaus voor de Planning van Workfront beïnvloeden, zie [ het type van Vergunning overzicht wanneer het gebruiken van de Planning van Adobe Workfront ](/help/quicksilver/planning/access/license-type-overview.md).
* Systeembeheerders kunnen alle werkruimten in het systeem beheren, inclusief de werkruimten die ze niet hebben gemaakt.
* Andere gebruikers, waaronder Systeembeheerders, hebben alleen toegang tot weergaven die ze hebben gemaakt of die met hen zijn gedeeld. Systeembeheerders kunnen alleen machtigingen krijgen om een weergave te beheren.
* U kunt een koppeling naar een werkruimte of naar een weergave delen met anderen.

  Gebruikers die de koppeling ontvangen, moeten actieve gebruikers zijn en zich aanmelden bij Workfront om toegang te krijgen tot de werkruimte of de pagina met recordtypen die wordt weergegeven in de geselecteerde weergave.

  <!--Replace the text from "users who receive ..." with the following when public sharing of views releases:
    The following scenarios exist:
        * Users who receive the link to a workspace must be active users and log in to Workfront to be able to access the workspace.
        * Users who receive the link to a view can access the view in the following ways: 
        
            * Must be active users and log in to Workfront
            * Can be external users to Workfront and access the view from a publicly shared link, without logging in to Workfront. -->

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


<!--You can share views internally or publicly. -->

Hier volgen de machtigingsniveaus voor weergaven en weergave-elementen:

|        | Beheer (alleen uitgenodigde personen hebben toegang) | Weergave (alleen uitgenodigde personen hebben toegang) | Iedereen in de werkruimte kan* weergeven |
|--------|--------|-------|------------------------------|
| Bewerken | ✓ |       |                            |
| Verwijderen | ✓ |       |                            |
| Delen | ✓ |       |                           |
| Weergave | ✓ | ✓ | ✓ |
| De weergave openen | ✓ | ✓ | ✓ |
| Tijdelijke filters, groepen, sorteren toepassen | ✓ | ✓ | ✓ |

*Gebruikers moeten over weergave- of hogere machtigingen voor een werkruimte beschikken om toegang te krijgen tot deze weergave.

<!--Replace the table above with the following when public sharing releases: 

|   Internal sharing     | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Apply  | ✓      | ✓     | ✓                          |

|   Public sharing      | View  |
|--------|-------|
| View   | ✓     |
| Apply  | ✓     |
-->


<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |    
-->