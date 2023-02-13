---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: SOAP-module
description: U kunt de module SOAP gebruiken om verbinding te maken met SOAP API's in Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 752e0766-25f2-4d22-bed5-7c931284258d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---

# [!UICONTROL SOAP] module

U kunt de [!UICONTROL SOAP] module voor verbinding maken met [!UICONTROL SOAP] API&#39;s in [!UICONTROL Adobe Workfront Fusion].

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] of hoger</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Met de [!UICONTROL SOAP] module

De [!UICONTROL SOAP] -module bevindt zich momenteel in bètaversie en biedt geen ondersteuning voor:

* Elementen opnieuw definiëren
* Beperkingen voor breukcijfers
* Totaal aantal getalbeperkingen
* Beperkingen voor witruimte
* Meerdere onderdelen in invoer- en uitvoerberichten. Er worden slechts enkelvoudige berichten ondersteund
* Aangepast XML-schema-elementen gedefinieerd met behulp van [[!UICONTROL SOAP] Codering](http://schemas.xmlsoap.org) schema&#39;s en elementen.

>[!INFO]
>
>**Voorbeeld:**
>  
>Het volgende wordt niet correct herkend door [!UICONTROL Workfront Fusion]:
>
>
```
><complexType name="ArrayOfFloat">
>
>   
  <complexContent>
>
>      
     <restriction base="soapenc:Array">
>
>         
        <attribute ref="soapenc:arrayType"
>
>            
           wsdl:arrayType="xsd:integer[]"/>
>
>      
     </restriction>
>
>   
  </complexContent>
>
>
</complexType>
>```

Het omvat de `soapenc:Array`, `soapenc:arrayType` en `wsdl:arrayType` verwijzingen, die nog niet worden ondersteund in [!UICONTROL Workfront Fusion].

## Workaround

Als de [!UICONTROL SOAP] De module weigert om het WSDL-bestand te verwerken of veroorzaakt verschillende fouten in de configuratie van de module. U kunt proberen de universele **[!UICONTROL HTTP]>[!UICONTROL Make a request]** in plaats daarvan:

1. In [!DNL Workfront Fusion], maakt u een nieuw scenario.
1. Voeg de **[!UICONTROL HTTP]>[!UICONTROL Make a request]** in het scenario.
1. Open de configuratie van de module en vul de volgende velden in:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method]</td> 
      <td> <p>[!UICONTROL POST]</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Body type]</td> 
      <td> <p>[!UICONTROL Raw]</p> </td> [!UICONTROL ]
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Content type]</td> 
      <td> <p>[!UICONTROL XML (application/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parse response]</td> 
      <td>[!UICONTROL Enabled]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. Open een nieuw venster of tabblad van een webbrowser.
1. Plak de URL van WSDL in de adresbalk van de webbrowser en haal het XML-bestand op.

   De WSDL-URL eindigt gewoonlijk met `?wsdl`, maar niet noodzakelijk, bijvoorbeeld `http://voip.ms/api/v1/server.wsdl`.

1. Als het WSDL-bestand niet rechtstreeks in de webbrowser wordt weergegeven, opent u het gedownloade bestand in een teksteditor.
1. Zoeken naar `<service>` of `<wsdl:service>` tag:

   ![](assets/service-350x65.png)

1. Kopieer de URL vanaf de locatie `location` kenmerk.
1. In [!DNL Workfront Fusion]plakken, plakt u de URL in het URL-veld van de HTTP-module.
1. Open de [Online [!UICONTROL SOAP] Client](https://wsdlbrowser.com/) in een nieuw venster/tabblad van een webbrowser.
1. Plak de URL van WSDL in het veld WSDL URL.
1. Klik op **[!UICONTROL Browse]**.
1. Kiezen uit de lijst met functies naar links, bijvoorbeeld `getLanguages`.
1. Kopieer de inhoud van de [!UICONTROL Request XML] tekstgebied.
1. In [!UICONTROL Workfront Fusion]plakken, plakt u de gekopieerde inhoud in het URL-veld van de module.
1. Geef waarden op voor de geselecteerde parameters door de vraagtekens te vervangen door werkelijke waarden:

   ![](assets/request-xml-350x172.png)

1. Sluit de configuratie van de module door te klikken **[!UICONTROL OK]**.
1. Voer het scenario of de module uit.
