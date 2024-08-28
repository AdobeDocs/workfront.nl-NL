---
title: Overzicht recordtypen
description: Recordtypen zijn de bouwstenen van een Adobe Workfront-werkruimte voor planning.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: a3006a05b7003e638596c2754b77e914083a5643
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---


# Overzicht van recordtypen

{{planning-important-intro}}

In tegenstelling tot Workfront waar de objecttypen vooraf zijn gedefinieerd, kunt u in Adobe Workfront Planning uw eigen objecttypen maken. In Workfront zijn bijvoorbeeld al de objecttypen Programma, Portfolio, Project, Taak of Probleem gemaakt.

Workfront Planning-objecttypen worden &#39;recordtypen&#39; genoemd en bestaan alleen wanneer gebruikers ze maken. Recordtypen zijn de bouwstenen van een Workfront-werkruimte voor planning. Voor informatie over werkruimten, zie [ werkruimten ](/help/quicksilver/planning/architecture/create-workspaces.md) creëren.

## Overzicht van recordtypen

In de Planning van Workfront, kunt u de types van douaneverslag tot stand brengen die aan de behoeften van uw organisatie voldoen.

Voor informatie over het creëren van verslagtypes, zie [ recordtypes ](/help/quicksilver/planning/architecture/create-record-types.md) creëren.

* Wanneer u een werkruimte maakt op basis van een sjabloon, worden recordtypen gemaakt in de volgende werkruimtesecties:

   * **Operationele Types van Verslag**: De types van verslag die strategische plannen, initiatieven, of gepland werk vertegenwoordigen. Campagne, Activiteit, Tactiek, Opportunity zijn bijvoorbeeld operationele recordtypen.
   * **Taxonomies**: De types van verslag die attributen over een operationeel verslagtype vangen. Regio, Adres, Publiek zijn bijvoorbeeld taxonomieën.

* Wanneer u een recordtype maakt in een werkruimte die u zelf hebt gemaakt, kunt u het recordtype in elke gewenste sectie plaatsen die u in de werkruimte maakt.
* Wanneer u een recordtype maakt, kunnen alleen u en de personen die u toegangsrechten tot de werkruimte geven, het recordtype weergeven.
* U moet een werkruimte maken voordat u recordtypen voor de werkruimte kunt maken.
* Voor beperkingen over hoeveel verslagtypes u in één werkruimte of instantie van Workfront kunt hebben, zie [ overzicht van de objectbeperkingen van de Planning van Adobe Workfront ](/help/quicksilver/planning/general/limitations-overview.md).


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Wrorkfront Planning record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

Although creating taxonomies is identical to creating operational record types, Workfront Planning distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

## Similarities and differences between operational record types and taxonomies

The following table illustrates some of the similarities and differences between operational record types and taxonomies: 

| Record type and characteristic                              | Operational Record Type | Taxonomy Record Type |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| They are part of a workspace                                |            ✓            |           ✓          |
| You can create them automatically, from a workspace template                    |            ✓            |           ✓          |
| You can create them manually, from scratch                    |            ✓            |           ✓          |
| You can create them by copying and pasting information from an external file or list                   |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file                    |            ✓            |                     |
| You can create read-only record types by connecting to object types from other applications                    |            ✓            |                     |
| They represent work-related objects                         |            ✓            |                      |
| They represent attributes about work-related objects        |                         |           ✓          |
| You can create from scratch                                 |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file            |            ✓            |                      |
| You can connect the record type to an object from another application|            ✓            |                      |
| You can connect to other record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->