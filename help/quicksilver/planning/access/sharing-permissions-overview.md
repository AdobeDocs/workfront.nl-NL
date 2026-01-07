---
title: Overzicht van deelmachtigingen in Adobe Workfront-planning
description: Niet alle gebruikers in de organisatie hebben de zelfde toegang en de toestemmingen om de Planning van Adobe Workfront te gebruiken. In dit artikel wordt algemene informatie beschreven over het delen of verwijderen van machtigingen voor een Adobe Workfront Planning-werkruimte of -weergave.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# Overzicht van het delen van machtigingen in Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->



{{planning-important-intro}}

U kunt machtigingen delen of verwijderen voor een Adobe Workfront-werkruimte, recordtype of weergave.

U kunt ook aanvraagformulieren voor planning delen. Voor informatie, zie [ creeer en beheer een verzoekvorm in de Planning van Adobe Workfront ](/help/quicksilver/planning/requests/create-request-form.md).

In dit artikel worden de machtigingsniveaus voor Workfront Planning-werkruimten, recordtypen, records, velden en weergaven beschreven.

## Objecten die u kunt delen in Adobe Workfront Planning

U kunt sommige objecten van de Planning van Workfront manueel delen, terwijl andere voorwerpen deze toestemmingen van andere voorwerpen erven.

U kunt de volgende objecten handmatig delen in Workfront Planning:

* Werkruimten

   * U kunt werkruimten delen met personen binnen uw organisatie.
   * Wanneer u een werkruimte deelt, worden ook alle recordtypen, records en velden gedeeld die aan de werkruimten zijn gekoppeld.
   * Als u een werkruimte deelt, worden de weergaven niet gedeeld. Weergaven worden afzonderlijk gedeeld.

  Voor meer informatie, zie [ werkruimten van het Aandeel ](/help/quicksilver/planning/access/share-workspaces.md)

* Recordtypen

   * U kunt recordtypen delen met personen binnen uw organisatie.
   * Het niveau van toestemmingen die voor de werkruimte worden verleend toont als Geërfte toestemmingen voor het verslagtype.
   * U kunt een recordtype niet delen met een hoger machtigingsniveau dan de gebruiker in de werkruimte heeft.

  Voor meer informatie, zie [ recordtypes van het Aandeel ](/help/quicksilver/planning/access/share-record-types.md).


* Weergaven

   * U moet gebruikers, met inbegrip van de Beheerders van het Systeem, toestemmingen verlenen om tot meningen los van hun toestemmingen toegang te hebben tot werkruimten.
   * Wanneer u een weergave deelt, worden alle weergave-elementen gedeeld, inclusief filters, groeperen, sorteren of Instellingen.
   * Wanneer u een weergave deelt, worden de records die zichtbaar zijn in de weergave niet gedeeld. Records moeten worden gedeeld door werkruimten te delen.
   * U kunt een mening openbaar delen, met mensen buiten uw organisatie wanneer u een openbare verbinding voor een mening produceert.De mensen die tot de verslagpagina van een openbare verbinding toegang hebben kunnen alle verslagen en hun gebieden, met inbegrip van verbonden verslagen en gebieden bekijken.

  Voor meer informatie, zie [ meningen van het Aandeel ](/help/quicksilver/planning/access/share-views.md).

## Overwegingen bij het delen van objecten in Adobe Workfront Planning

* Uw Adobe Workfront-licentietype werkt in combinatie met uw Workfront-planningsmachtigingen en geeft u toegang tot de werkruimten en de bijbehorende objecten, en tot het weergeven, bijdragen of beheren van deze werkruimten.

  Voor informatie over hoe de vergunningstypes toestemmingsniveaus voor de Planning van Workfront beïnvloeden, zie [ het type van Vergunning overzicht wanneer het gebruiken van de Planning van Adobe Workfront ](/help/quicksilver/planning/access/license-type-overview.md).
* Systeembeheerders kunnen alle werkruimten in het systeem beheren, inclusief de werkruimten die ze niet hebben gemaakt.
* Andere gebruikers, waaronder Systeembeheerders, hebben alleen toegang tot weergaven die ze hebben gemaakt of die met hen zijn gedeeld. Systeembeheerders kunnen alleen machtigingen krijgen om een weergave te beheren.

* Wanneer u werkruimten en recordtypen deelt met anderen, wordt het machtigingsniveau van het recordtype automatisch overgeërfd aan de records en velden die aan deze werkruimten zijn gekoppeld.

  >[!IMPORTANT]
  >
  >Als de instantie van uw organisatie van Workfront aan de Adobe Verenigde Ervaring is genegeerd, moeten de gebruikers u de voorwerpen van de Planning met wilt delen aan Adobe Admin Console worden toegevoegd. U kunt planningsobjecten niet delen met Workfront-gebruikers die niet aan de Adobe Admin Console zijn toegevoegd.

* U kunt de voorwerpen van de Planning op de volgende manieren delen:

   * Intern kunt u een werkruimte, weergave of recordtype delen met de volgende Workfront-entiteiten:

      * Gebruikers
      * Groepen
      * Teams
      * Bedrijven
      * Functies

     U kunt een planningsobject delen met maximaal 100 entiteiten per object.

   * Intern, door een verbinding aan een werkruimte of aan een mening met andere gebruikers van de Planning te delen. De volgende scenario&#39;s bestaan:

      * Gebruikers die de koppeling naar een werkruimte ontvangen, moeten actieve gebruikers zijn en zich aanmelden bij Workfront om toegang te krijgen tot de werkruimte.
      * Gebruikers die een koppeling voor intern delen voor een weergave ontvangen, moeten actieve gebruikers zijn en zich aanmelden bij Workfront om toegang te krijgen tot de weergave.
   * Extern, door een koppeling Openbaar delen naar een weergave te delen met externe gebruikers die geen Workfront-account hebben.

## Machtigingen delen voor Adobe Workfront Planning-objecten

De tabellen in de volgende secties tonen het machtigingsniveau dat u kunt selecteren bij het delen van een werkruimte of weergave en welke functionaliteit op elk niveau is toegestaan.

>[!IMPORTANT]
>
>Niet alle gebruikers kunnen de hieronder beschreven toestemmingsniveaus hebben. De individuele vergunning van gebruikers bepaalt welk niveau van toestemmingen zij voor de voorwerpen van de Planning van Workfront kunnen ontvangen.
>
>Alleen gebruikers met een standaardlicentie (of abonnement) kunnen beschikken over Contribute- of Beheren-machtigingen voor werkruimten en de machtiging Beheren voor weergaven.
> 
>Gebruikers met alle andere licentietypen kunnen weergavemachtigingen hebben voor werkruimten en weergaven.
>
>Voor informatie, zie [ het type van Vergunning overzicht wanneer het gebruiken van de Planning van Adobe Workfront ](/help/quicksilver/planning/access/license-type-overview.md).


### Machtigingen voor werkruimten

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

### Machtigingen om gegevenstypen op te nemen

<!-- old access:
In the Production environment, Record Type permissions are always inherited when you grant permissions to the workspace.

The following are the levels of permissions for record types: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

-->

De toestemmingen van het Type van verslag worden altijd geërft wanneer u toestemmingen aan de werkruimte verleent.

U kunt de erfrechten van het recordtype verwijderen die u van de werkruimte hebt ontvangen.

U kunt gebruikers lagere machtigingen geven voor het recordtype dan in de werkruimte.

U kunt echter niet het volgende doen:

* Verleen hogere toestemmingen voor het verslagtype dan gebruikers op de werkruimte hebben.
* Geef werkruimtemanagers lagere machtigingen voor een recordtype.
* Verwijder de toestemmingen van de Mening aan het verslagtype of de werkruimte door gebruikers uit de verslagtype toestemmingen te verwijderen.

De volgende scenario&#39;s bestaan:

| Workspace-machtigingen | Automatische overerfde machtigingen voor een recordtype | Mogelijke rechten voor het type record wanneer de overerfde machtigingen zijn uitgeschakeld (handmatig toegekend) |
|--------|--------|-------------|
| Beheren | Beheren | Rechten beheren, verwijderen* |
| Contribute | Contribute | Contribute, View, Remove permissions* |
| Weergave | Weergave | Machtigingen weergeven, verwijderen* |

>[!NOTE]
>
>Wanneer u machtigingen verwijdert uit een recordtype, behouden gebruikers nog steeds de weergavemachtigingen voor de werkruimte en alle recordtypen, tenzij u hun machtigingen uit de werkruimte verwijdert.

### Machtigingen voor records

De toestemmingen van het verslag worden geërft van het verslagtype, wanneer u toestemmingen aan de werkruimte en het verslagtype verleent.

Hieronder vindt u de machtigingsniveaus voor records:


|        | Beheren | Contribute | Weergave |
|--------|--------|------------|-------|
| Maken | ✓ | ✓ |       |
| Verwijderen | ✓ | ✓ |       |
| Bewerken | ✓ | ✓ |       |
| Weergave | ✓ | ✓ | ✓ |

### Machtigingen om velden op te nemen

De toestemmingen van het gebied worden geërft van het verslagtype, wanneer u toestemmingen aan de werkruimte en het verslagtype verleent.

De volgende machtigingen verwijzen naar de velden zelf en niet naar de waarden die aan elk veld zijn gekoppeld. Als u veldwaarden wilt bewerken, moet u over machtigingen beschikken om records te bewerken.

|        | Beheren | Contribute | Weergave |
|--------|--------|------------|-------|
| Maken | ✓ |            |       |
| Verwijderen | ✓ |            |       |
| Bewerken | ✓ |            |       |
| Weergave | ✓ | ✓ | ✓ |


### Rechten voor weergaven

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
