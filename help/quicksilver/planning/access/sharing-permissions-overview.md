---
title: Overzicht van het delen van machtigingen in Adobe Workfront Planning
description: U kunt machtigingen delen of verwijderen in een Adobe Workfront-werkruimte of -weergave voor planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 3856e56036a9845387d7dc6498a6f20728c8234a
workflow-type: tm+mt
source-wordcount: '696'
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

## Overwegingen bij het delen van objecten in Adobe Workfront Planning

* Het Adobe Workfront-licentietype werkt in combinatie met uw Workfront-planningsbevoegdheden en geeft u toegang tot objecten bij het gebruik van Workfront Planning. U kunt objecten ook toevoegen of beheren.

  Voor informatie over hoe de vergunningstypes toestemmingsniveaus voor de Planning van Workfront beïnvloeden, zie [Overzicht van licentietype bij gebruik van Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Systeembeheerders kunnen werkruimten beheren en delen die andere gebruikers hebben gemaakt.
* Als u geen systeembeheerder bent, kunt u aan werkruimten bijdragen die door anderen worden gecreeerd als zij met u worden gedeeld.
* U kunt werkruimten of weergaven niet bulksgewijs delen.
* U kunt een werkruimte of een weergave delen met de volgende entiteiten:
   * Gebruikers
   * Groepen
     <!--* You can share a view publicly, with people outside your organization when you generate a public link for a view.People accessing the record page from a public link can view all records and their fields, including connected records and fields.-->
* Andere gebruikers, waaronder Systeembeheerders, hebben alleen toegang tot weergaven die ze hebben gemaakt of die met hen zijn gedeeld. Systeembeheerders kunnen alleen machtigingen krijgen om een weergave te beheren.
* U kunt een koppeling naar een werkruimte of naar een weergave vanuit een pagina met recordtypen delen met anderen. Gebruikers die de koppeling ontvangen, moeten actieve gebruikers zijn en zich aanmelden bij Workfront om toegang te krijgen tot de werkruimte of de pagina met recordtypen die wordt weergegeven in de geselecteerde weergave.

## Machtigingen delen voor Adobe Workfront Planning-objecten

De tabellen in de volgende secties tonen het machtigingsniveau dat u kunt selecteren bij het delen van een werkruimte of weergave en welke functionaliteit op elk niveau is toegestaan.

>[!IMPORTANT]
>
>Niet alle gebruikers kunnen de hieronder beschreven toestemmingsniveaus hebben. De individuele vergunning van gebruikers bepaalt welk niveau van toestemmingen zij voor de voorwerpen van de Planning van Workfront kunnen ontvangen.
>
>Zie voor meer informatie [Overzicht van licentietype bij gebruik van Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Werkruimtemachtigingen

U moet gebruikers toestemming geven aan werkruimten om hen toegang tot de volgende entiteiten te verlenen:

* Werkruimten
* Recordtypen
* Records
* Velden
* Weergaven*

  *U kunt alle gebruikers met Weergave- of hogere machtigingen ook toegang geven tot de weergaven in de werkruimte. Dit is een extra toestemming die u moet toelaten wanneer het delen van een mening. Zie voor meer informatie [Weergaven delen](/help/quicksilver/planning/access/share-views.md).

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
| Toepassen | ✓ | ✓ | ✓ |

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