---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Modules archiveren
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# [!UICONTROL Archive] modules

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ modules van het Archief ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/archive-modules.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

In een [!DNL Adobe Workfront Fusion] scenario, kunt u een archief, zoals een gecomprimeerd dossier, in uw scenario gebruiken, toestaand u om het in uw automatiseringen of integraties te gebruiken.

Als u instructies bij het creëren van een scenario nodig hebt, zie [ een scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) creëren. Voor informatie over modules, zie [ Modules in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## [!UICONTROL Archive] modules en hun velden

Wanneer u [!UICONTROL Archive] modules configureert, geeft [!DNL Workfront Fusion] de onderstaande velden weer. Daarnaast kunnen aanvullende [!UICONTROL Archive] -velden worden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Voor meer informatie, zie [ informatie van de Kaart van één module aan een andere in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Extract an archive]](#extract-an-archive)
* [[!UICONTROL Create an archive]](#create-an-archive)
* [[!UICONTROL Inflate]](#inflate)
* [[!UICONTROL Deflate]](#deflate)

## [!UICONTROL Extract an archive]

Deze actiemodule extraheert een bestand dat u uit een archief identificeert.

De module retourneert de id van het bestand en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p> Selecteer het bestand dat u wilt extraheren. Dit dossier kan van een vorige module (zoals [!DNL Workfront] worden in kaart gebracht &gt; [!UICONTROL Download a document] module).</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Voorbeeld:** krijg het dossier van het PIT van de bepaalde [!DNL Dropbox] omslag (bijvoorbeeld, Archives), haalt het uit gebruikend de [!UICONTROL Archive] module en verzendt geciteerde dossiers naar het gewenste e-mailadres als gehechtheid met [!UICONTROL Email] of [!DNL Gmail] module.
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL Create an archive]

Deze aggregatormodule voegt de gewenste bestanden toe aan een [!UICONTROL ZIP] - of [!UICONTROL TAR] -archief.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source module]</td> 
   <td> <p> Selecteer de module waarvan u de bestanden wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>Selecteer of u bestanden wilt toevoegen aan een [!UICONTROL ZIP] archief of een [!UICONTROL TAR] archief.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comment]</td> 
   <td>Voer een opmerking in die u aan het archief wilt toevoegen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group by]</td> 
   <td> <p>Definieer een expressie waarop u de geaggregeerde uitvoer wilt groeperen. Deze expressie kan een of meer toegewezen items bevatten. De geaggregeerde gegevens worden vervolgens in groepen verdeeld op basis van de waarde van deze expressie. Elke groep voert als een afzonderlijke bundel met een sleutel (de geëvalueerde uitdrukking) en een waarde (de samengevoegde tekst) uit. U kunt de sleutel als filter in verdere modules gebruiken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Selecteer deze optie om het scenario te stoppen als er geen resultaten zijn.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archive name]</td> 
   <td> <p> Voer een naam in voor het gemaakte archief. Voeg geen extensie toe.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Voorbeeld:** bekijk inkomende e-mails gebruikend [!DNL Gmail] > [!UICONTROL Watch emails] module. Als een e-mail wordt ontvangen, worden de bijlagen herhaald in afzonderlijke bundels, vervolgens naar het [!DNL ZIP] -bestand gearchiveerd en in de gedefinieerde map Dropbox opgeslagen.
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL Inflate]

Deze transformatormodule decomprimeert binaire gegevens met behulp van een inflatiealgoritme.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>Voer de gegevens in die u wilt decomprimeren of wijs deze toe met behulp van de inflate-functie.</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL Deflate]

Deze transformatormodule comprimeert binaire gegevens met behulp van een deflatiealgoritme.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>Voer de gegevens in die u wilt comprimeren of wijs deze toe met de functie deflate.</p> </td> 
  </tr> 
 </tbody> 
</table>
