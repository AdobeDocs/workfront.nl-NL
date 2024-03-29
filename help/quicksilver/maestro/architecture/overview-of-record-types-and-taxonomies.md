---
title: Overzicht van recordtypen
description: Recordtypen zijn de bouwstenen van een Adobe Workfront-planningswerkruimte.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Overzicht van recordtypen

{{maestro-important-intro}}

In tegenstelling tot Workfront waar de objecttypen vooraf zijn gedefinieerd, kunt u in Adobe Workfront-planning uw eigen objecttypen maken. In Workfront zijn bijvoorbeeld al de objecttypen Programma, Portfolio, Project, Taak of Probleem gemaakt.

Workfront-planningsobjecttypen worden &#39;recordtypen&#39; genoemd en u kunt ze allemaal maken en aanpassen. Recordtypen zijn de bouwstenen van een Workfront-planningswerkruimte. Zie voor informatie over werkruimten [Werkruimten maken](../architecture/create-workspaces.md).

## Overzicht van recordtypen

In Workfront-planning kunt u aangepaste recordtypen maken die aan de behoeften van uw organisatie voldoen.

* Wanneer u een werkruimte maakt op basis van een sjabloon, worden recordtypen gemaakt in de volgende werkruimtesecties:

   * [Operationele recordtypen](#operational-record-type): Een recordtype dat strategische plannen, initiatieven of gepland werk vertegenwoordigt. Campagne, Activiteit, Tactiek, Opportunity kunnen bijvoorbeeld operationele recordtypen zijn.
   * [Taxonomieën](#taxonomy): Typen opnemen die kenmerken vastleggen over een operationeel recordtype. Regio, Adres, Publiek kunnen bijvoorbeeld taxonomieën zijn.

* Wanneer u een recordtype maakt in een werkruimte die u zelf hebt gemaakt, kunt u het recordtype in elke gewenste sectie plaatsen die u in de werkruimte maakt.
* Wanneer u een recordtype maakt, kunnen alleen u en de personen die u toegangsrechten tot de werkruimte geven, het recordtype weergeven.
* U moet een werkruimte maken voordat u recordtypen voor de werkruimte kunt maken.
* U kunt in totaal 1.000 recordtypen in één werkruimte hebben, ongeacht het aantal secties in de werkruimte. Dit zijn recordtypen die u helemaal zelf maakt of die bij het gebruik van een sjabloon worden gemaakt.


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Maestro record type that represents work-related objects.  

![](assets/operational-record-type-blank.png)

For more information about operational record types including how to create them, see [Create record types](../architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

![](assets/taxonomy-record-type-blank.png)

For more information about taxonomy record types, see [Create a taxonomy](../architecture/create-a-taxonomy.md). 

Although creating taxonomies is identical to creating operational record types, Maestro distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

For more information, see [Create a taxonomy](../architecture/create-a-taxonomy.md). 

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
| You can connect to other Maestro record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->