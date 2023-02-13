---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Door SDL beheerde vertaalmodules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u uw SDL Beheerde Vertaalrekening met veelvoudige derdetoepassingen en de diensten verbinden.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# [!DNL SDL Managed Translation] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u uw [!DNL SDL Managed Translation] account voor meerdere toepassingen en services van derden.

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

## [!DNL SDL Managed Translation] Modules

>[!NOTE]
>
>De verrichtingonderbreking voor vraag aan [!DNL SDL Managed Translation] is **120 seconden**.

### Bestanden

#### [!UICONTROL Download Translated File]

Deze module wint de inhoud van één enkel vertaald dossier, binnen het gespecificeerde project terug. Als het gewenste bestand nog niet de status Downland heeft, is het mogelijk dat de inhoud van het bestand nog niet volledig is vertaald. Als het bestand de status Downloaden heeft en u hebt het opgehaald, moet u controleren of het bestand is voltooid met de opdracht `Cancel or Complete File` methode.

#### [!UICONTROL Upload a File]

Deze module staat uploads van dossiers voor vertaling of voor opneming in een vertaalproject als verwijzingsmateriaal toe. Uploads moeten worden verzonden met behulp van multipart/form-data en kunnen meerdere bestanden bevatten. U geeft de `ProjectOptionId` die moeten worden gebruikt om de geüploade bestanden te evalueren. Hiermee bepaalt u of elk bestand dat u uploadt, mogelijk kan worden omgezet of als referentiemateriaal moet worden verwerkt. In het geval van archieven (`zip `, `rar`, `7z`, `tar` (bestanden) de app controleert de inhoud van het archief en geeft aan of het archief als geheel kan worden vertaald of dat het een combinatie van vertaalbare en niet-vertaalbare bestanden bevat.

>[!NOTE]
>
>Het uploaden van meerdere bestanden tegelijk wordt afgeraden, omdat dit de impact van een fout kan vergroten.

#### [!UICONTROL Add a Reference File]

Deze module voegt een referentiebestand toe.

### Projecten

#### [!UICONTROL Create a project]

Deze module leidt tot het gespecificeerde project.

#### Een project annuleren of voltooien

Deze module annuleert of voltooit het gespecificeerde project. Als het project op download wacht, overgaat het project door om het even welke definitieve stappen in het werkschema, en uiteindelijk beweegt zich om te voltooien. Als het project op goedkeuring wacht of de selectie van de leverancier wordt geannuleerd. Als het project op een andere status is, zal het verzoek ontbreken.

#### [!UICONTROL Download Project Zip]

Deze module haalt de `zip` bestand met vertaalde bestanden voor het opgegeven project.

#### [!UICONTROL Read a Project]

Deze module krijgt het gespecificeerde project.

#### [!UICONTROL Get Projects at Status]

Deze module krijgt alle beschikbare projecten in de gespecificeerde status. Met deze methode kunnen de resultaten worden geplakt door `$top`, `$skip`, en `$orderby` queryparameters.

#### [!UICONTROL Get Projects List]

Haalt een eenvoudige lijst op van alle projecten, die algemene informatie over elk project verstrekken. Met deze methode kunnen de resultaten pagina&#39;s zijn, door `$top`, `$skip`, en `$orderby` queryparameters.

#### [!UICONTROL Search Project Creation Options]

Deze module krijgt de Opties van de Making van het Project.

### Overige

#### [!UICONTROL Make an API Call]

Deze module voert een willekeurige geautoriseerde API-aanroep uit.
