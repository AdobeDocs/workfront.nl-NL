---
title: Overzicht van het delen van machtigingen in Adobe Maestro
description: U kunt machtigingen delen of verwijderen in een Adobe Maestro-werkruimte of -weergave.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 86f9a88518c8a03643061b3328719d2da4016f2b
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Overzicht van het delen van machtigingen in Adobe Maestro

{{maestro-important-intro}}

U kunt machtigingen delen of verwijderen in een Adobe Maestro-werkruimte of -weergave.

In dit artikel worden de machtigingsniveaus voor Maestro-objecten beschreven.

Zie de volgende artikelen voor informatie over het delen van werkruimten of weergaven:

* [Werkruimten delen](/help/quicksilver/maestro/access/share-workspaces.md)

* [Weergaven delen](/help/quicksilver/maestro/access/share-views.md)

## Objecten die u kunt delen in Adobe Maestro

U kunt de volgende objecten delen in Maestro:

* Werkruimten

  Wanneer u een werkruimte deelt, worden ook alle recordtypen, records en velden gedeeld die aan de werkruimten zijn gekoppeld. Weergaven worden niet gedeeld.

* Weergaven

## Overwegingen bij het delen van objecten in Maestro

* U moet over de volgende licentie beschikken om werkruimten te maken in Maestro:

   * Nieuw prijsmodel: standaardlicentie
   * Huidige prijsmodel: licentie voor abonnementen.

  Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)
* Systeembeheerders kunnen werkruimten beheren en delen die andere gebruikers hebben gemaakt.
* Als u geen systeembeheerder bent, kunt u aan werkruimten bijdragen die door anderen worden gecreeerd als zij met u worden gedeeld.
* U kunt werkruimten niet bulksgewijs delen.
* U kunt een werkruimte delen met de volgende entiteiten:
   * Gebruikers
   * Groepen
* Andere gebruikers, waaronder Systeembeheerders, hebben alleen toegang tot weergaven die ze hebben gemaakt of die met hen zijn gedeeld.
* U kunt een koppeling naar een werkruimte of naar een weergave vanuit een pagina met recordtypen delen met anderen. Gebruikers die de koppeling ontvangen, moeten actieve gebruikers zijn en zich aanmelden bij Workfront om toegang te krijgen tot de werkruimte of de pagina met recordtypen die wordt weergegeven in de geselecteerde weergave.

## Machtigingen delen voor Maestro-objecten

De tabellen in de volgende secties tonen het machtigingsniveau dat u kunt selecteren bij het delen van een Maestro-werkruimte of -weergave en welke functionaliteit elk niveau toestaat.

### Werkruimtemachtigingen

|        | Beheren | Contribute | Weergave |
|--------|--------|------------|-------|
| Bewerken | ✓ |            |       |
| Delen | ✓ |            |       |
| Verwijderen | ✓ |            |       |
| Weergave | ✓ | ✓ | ✓ |

### Machtigingen voor recordtype

De toestemmingen van het Type van verslag worden geërft wanneer u toestemmingen aan de werkruimte verleent.

|        | Beheren | Contribute | Weergave |
|--------|--------|------------|-------|
| Maken | ✓ |            |       |
| Verwijderen | ✓ |            |       |
| Bewerken | ✓ |            |       |
| Weergave | ✓ | ✓ | ✓ |

### Machtigingen opnemen

De toestemmingen van het verslag worden geërft wanneer u toestemmingen aan de werkruimte verleent.

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

|        | Beheren | Weergave |
|--------|--------|-------|
| Bewerken | ✓ |       |
| Verwijderen | ✓ |       |
| Weergave | ✓ | ✓ |
| Toepassen | ✓ | ✓ |






