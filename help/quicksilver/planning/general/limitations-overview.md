---
title: Overzicht van objectbeperkingen voor Adobe Workfront-planning
description: De Planning van Adobe Workfront heeft grenzen voor hoeveel voorwerpen u in uw geval kunt tot stand brengen. Objectlimieten zijn ingesteld om de productprestaties te verbeteren en uw ervaring met Workfront Planning te verbeteren.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: f252140e4fec01c7bb8092804532d79954cef618
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Overzicht van beperkingen van Adobe Workfront-planningsobjecten

De Planning van Adobe Workfront heeft grenzen voor hoeveel voorwerpen u in uw geval kunt tot stand brengen. Objectlimieten zijn ingesteld om de productprestaties te verbeteren en uw ervaring met Workfront Planning te verbeteren.

In de volgende tabel staan de limieten voor het aantal objecten dat u kunt maken in Workfront Planning. De beperkingen zijn aan verandering onderhevig naarmate we de volgende ontwikkelingsfasen ingaan.

| Object Adobe Workfront Planning | Limiet |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Aantal werkruimten voor één Workfront-instantie | 1.000 |
| Aantal secties voor één werkruimte | 50 |
| Aantal recordtypen voor één werkruimte | 1.000 (dit omvat recordtypen van alle secties en die die wanneer het gebruiken van een werkruimtesjabloon worden gecreeerd) |
| Aantal records voor één recordtype | 50.000 |
| Aantal velden voor één recordtype of taxonomie | 500 |
| Aantal tekens voor een tekstveld | 1.000 tekens |
| Grootte van het bestand dat u in een tabel met recordtypen kunt plakken | 1 MB |
| Grootte van het bestand dat u kunt importeren via de API voor een recordtype-tabel | 1,5 MB |
| De snelheid waarmee API-aanvragen kunnen worden ingediend | 200 verzoeken per minuut |
| Grootte CSV-bestand dat u kunt importeren* | 5 MB |
| Aantal weergaven dat een gebruiker voor één recordtype kan maken | 100 |

<!--add to the table above: Maximum number of views created by one use 100 -->

>[!IMPORTANT]
>
>*Deze functie is tijdelijk uitgeschakeld en is later beschikbaar.

<!--At GA, replace the table above with this:

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   unlimited*                                                                                                        |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   25,000                                                                                                        |
|     Number of records for one workspace                                               |   25,000 for customers with the Planning plan <br> 500,000 for customers with the Planning Plus  plan                                                                                                         |
|     Number of total records for one instance of Workfront Planning type                                               |   500,000 for customers with the Planning plan <br>2 million for customers with the Planning Plus plan                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Size of CSV of Excel file you can import** | 5MB |
| Number of views one user can create for one record type | 100 |

*We recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.
**This functionality has been temporarily disabled and it will be available at a later date.
-->