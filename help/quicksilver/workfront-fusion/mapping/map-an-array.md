---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Wijs een serie in  [!DNL Adobe]  de Fusie van Workfront toe
description: U kunt een array toewijzen aan een moduleveld in Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: f87bc22f4ce70f266a199fcb54c5a74f9e3ba914
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# Een array toewijzen in [!DNL Adobe Workfront Fusion]

Een array is een speciaal type item dat het volgende kan bevatten:

* Een of meer tekstwaarden (eenvoudige array)
* Een of meer verzamelingen van hetzelfde type (complexe array)

>[!INFO]
>
>**Voorbeeld:** de [!UICONTROL Watch emails] module keert een serie van gehechtheid voor elke e-mail terug. Elke bijlage vertegenwoordigt een verzameling die een naam, inhoud, grootte enzovoort kan bevatten.

Voor meer informatie, zie {de gegevenstypes van 0} Punt in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).[

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] of hoger</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het [!UICONTROL Select] - of [!UICONTROL Prime] [!DNL Adobe Workfront] -abonnement hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).



## Een volledige array toewijzen

1. In de modules waaraan u de array toewijst, klikt u op het veld waar u de array wilt toewijzen. Dit is het veld waaraan de array wordt toegewezen.

1. Wijs het item toe in het vak dat wordt weergegeven.

   In het deelvenster kunt u velden op dezelfde manier toewijzen als bij elk ander type item. Als u niet elk item afzonderlijk wilt invullen, maar een andere array wilt toewijzen aan het doelveld, gebruikt u de knop [!UICONTROL Map] . In dit geval moet u ervoor zorgen dat beide arrays (de bronarray en de doelarray) dezelfde structuur hebben.

   U kunt elk gewenst aantal items aan een array toevoegen.

U kunt een array in afzonderlijke bundels verdelen met behulp van een iterator. Zie [[!UICONTROL Iterator] module in  [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/modules/iterator-module.md) voor meer informatie.

## Items toewijzen aan een nieuwe array

Met sommige velden in Workfront Fusion kunt u elementen toewijzen aan een array. U kunt bijvoorbeeld een array met items in de checklist maken in de Workfront Boards > Add checklist item module. Wanneer de module wordt uitgevoerd, worden alle items in de controlelijst aan de kaart toegevoegd.

Om het even welk modulegebied dat &quot;Add punt&quot;toont leidt tot een serie.

![ voeg punt ](assets/add-item.png) toe

Elementen toevoegen aan de array:

1. Klik **toevoegen punt**
1. Voer in het deelvenster dat wordt geopend details in over het item.
1. Klik **toevoegen**.
1. (Facultatief) herhaal stappen 1-3 voor elk element u aan de  serie wilt toevoegen.

## Matrixelementen toewijzen


### Array-elementen toewijzen op nummer

Array-elementen worden tussen vierkante haakjes weergegeven als een getal na de naam van de array. Met dit indexnummer kunt u een afzonderlijk element van een array in een veld toewijzen.

![](assets/map-array-1st-element.png)

>[!NOTE]
>
>Array-indexering in Workfront Fusion begint bij 1.

Een arrayelement toewijzen:

1. Klik op het veld waar u het element wilt toewijzen.

   Het deelvenster Toewijzing wordt geopend.

1. Zoek de array met het element dat u wilt toewijzen.
1. Klik op de vervolgkeuzepijl naast de array.
1. Klik op het element dat u wilt toewijzen.

   Het element wordt toegewezen, met index 1. Hierdoor wordt het eerste element in de array toegewezen.

1. Om een verschillend element van de serie in kaart te brengen, klik op [ 1 ] en ga het indexaantal van het serieelement in dat u wilt in kaart brengen.

   ![](assets/access-another-element.png)

### Het element van een array toewijzen met een bepaalde sleutel

Sommige arrays bevatten verzamelingen met sleutelwaardeitems, zoals metagegevens, kenmerken, enzovoort. Als u een van deze waarden wilt gebruiken, kunt u een element opzoeken op basis van de opgegeven sleutelwaarde en de bijbehorende waarde ophalen uit het waardeitem. We raden u aan een formule te gebruiken die een combinatie van de functies `map()` en `get()` gebruikt.



>[!BEGINSHADEBOX]

In het volgende voorbeeld wordt de uitvoer van de [!DNL Jira] App getoond.

![](assets/output-of-jira-app-350x100.png)

In dit voorbeeld wordt een bestandsnaam opgehaald uit een array van bijlagen, voor de specifieke bijlage met een id van 10108.

In dit voorbeeld wordt de volgende uitvoer gegenereerd:

![](assets/output-from-jira-350x261.png)

De formule kan als volgt worden toegelicht:

* `map`

   1. De eerste parameter van de functie `map()` is het gehele arrayitem.
   1. De tweede parameter is de onbewerkte naam van het waardeitem. Als u de onbewerkte naam wilt verkrijgen, plaatst u de muisaanwijzer op het item in het deelvenster [!UICONTROL mapping] :

      ![](assets/obtain-raw-name-350x124.png)

      >[!NOTE]
      >
      >Alle parameters zijn hoofdlettergevoelig. Hoewel in dit voorbeeld het label van het item alleen in hoofdletters verschilt van de onbewerkte naam, is het nodig de onbewerkte naam te gebruiken.

   1. De derde parameter is de onbewerkte naam van het sleutelitem:

      ![](assets/3rd-parameter-350x166.png)

   1. De vierde parameter is de opgegeven sleutelwaarde.

  Omdat de functie `map()` een array retourneert (omdat er meer elementen met de opgegeven sleutelwaarde kunnen zijn), is het nodig de functie `get()` toe te passen om het eerste element op te halen:

* `get`

   1. De eerste parameter van de functie `get()` is het resultaat van de functie `map()` .

   1. De tweede parameter is de index van het element. In dit voorbeeld is de index `1` .

In dit voorbeeld wordt de volgende uitvoer gegenereerd:

![](assets/output-from-jira-350x261.png)

>[!ENDSHADEBOX]

Voor meer informatie over de `map()` functie, zie [ functies van de Serie ](/help/quicksilver/workfront-fusion/functions/array-functions.md).

Voor meer informatie over de `get()` functie, zie [ Algemene functies ](/help/quicksilver/workfront-fusion/functions/general-functions.md).

## Arrayelementen omzetten in een reeks bundels

Arrays kunnen met de module [!UICONTROL Iterator] worden omgezet in een reeks bundels. Zie [[!UICONTROL Iterator] module ](/help/quicksilver/workfront-fusion/modules/iterator-module.md) voor meer informatie.

![](assets/series-of-bundles.png)

