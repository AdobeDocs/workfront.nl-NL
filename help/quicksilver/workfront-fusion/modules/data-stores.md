---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Gegevensopslag in  [!DNL Adobe Workfront Fusion]
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1277'
ht-degree: 0%

---

# Gegevensopslag in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ creeer en beheer gegevensopslag ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/data-stores.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

Een gegevensopslag, gelijkend op een gegevensbestand of een eenvoudige lijst, kan gegevens van scenario&#39;s opslaan, die het mogelijk maken om gegevens tussen individuele scenario&#39;s of scenario looppas over te brengen. U kunt een gegevensopslag gebruiken om nieuwe gegevens van diverse systemen tijdens synchronisatie op te slaan.

Met de gegevensopslagmodules kunt u de volgende handelingen uitvoeren voor records in de [!DNL Adobe Workfront Fusion] gegevensopslag:

* Toevoegen
* Vervangen
* Bijwerken
* Ophalen
* Verwijderen
* Zoeken
* Aantal

Voor informatie bij het gebruiken van de modules van de gegevensopslag, zie [[!UICONTROL Data store] modules ](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

Ga voor een video-introductie over gegevensopslag in Workfront Fusion naar:

* [ de Opslag van Gegevens ](https://video.tv.adobe.com/v/3427029/){target=_blank}

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> <p>Nieuw: [!UICONTROL Standard]</p><p>of</p><p>Huidig: [!UICONTROL Work] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidig: Geen [!DNL Workfront Fusion] vereiste licentie.</p>
   <p>of</p>
   <p>Verouderd: alle </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Nieuw:</p> <ul><li>[!UICONTROL Select] of [!UICONTROL Prime] [!DNL Workfront] Plan: Uw organisatie moet het abonnement aanschaffen [!DNL Adobe Workfront Fusion] .</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Overzicht: [!DNL Workfront Fusion] is opgenomen.</li></ul>
   <p>of</p>
   <p>Huidig: Uw organisatie moet [!DNL Adobe Workfront Fusion] aanschaffen.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Gegevensruimte beschikbaar

<!--If your organization is on the new Workfront plan model (Select, Prime, and Ultimate packages), your total data store size is:-->

Als uw organisatie zich op het nieuwe het planmodel van Workfront (Uitgezochte, Prime, en de pakketten van Ultimate) bevindt, beïnvloedt het plan van uw organisatie de grootte en het aantal gegevensopslag beschikbaar uw instantie van Fusion.

### Ultimate-plan

Fusion-instanties op het Ultimate-pakket ontvangen:

* 100 MB aan ruimte
* 50 gegevensopslag

### Abonnementen selecteren en Prime

Fusion-instanties op de pakketten Select of Prime ontvangen:—>

* 100 MB voor de eerste 500K verrichtingen.

* 10 MB voor elke extra 100K-bewerking.

  Een organisatie met 600K-bewerkingen ontvangt bijvoorbeeld 110 MB.

Uw organisatie kan tot 50 gegevensopslag hebben. De gecombineerde grootte van deze gegevensopslag kan niet de totale grootte van de gegevensopslag van uw organisatie overschrijden.

## Een gegevensopslag maken in [!DNL Workfront Fusion]

* [De gegevensopslag instellen](#set-up-the-data-store)
* [De gegevensstructuur instellen](#set-up-the-data-structure)

### De gegevensopslag instellen

Voordat u een gegevensopslag in een module kunt gebruiken, moet u de gegevensopslag maken in [!DNL Workfront Fusion] .

>[!NOTE]
>
>Uw organisatie heeft een beperkt aantal beschikbare gegevensopslagruimten. Als u probeert meer gegevensopslagruimten te maken dan beschikbaar is, retourneert [!DNL Workfront] een [!UICONTROL Maximum stores reached] -fout.
>
>Voor meer informatie, zie [ Maximale opslag bereikte fout ](#maximum-stores-reached-error) in dit artikel.

1. Meld u aan bij uw [!DNL Workfront Fusion] -account.
1. Klik op **[!UICONTROL Data stores]** in het navigatievenster aan de linkerkant.
1. Klik op **[!UICONTROL Add data store]** in de rechterbovenhoek van het scherm.
1. Voer instellingen in voor de nieuwe gegevensopslag.

   Een bolde titel op een gebied in een module [!DNL Workfront Fusion] wijst op een vereiste het plaatsen.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Data store name] </td> 
      <td> <p>Voer een naam in voor de gegevensopslag. </p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Data Structure]</p> </td> 
      <td> <p>Een gegevensstructuur is een lijst van de kolommen voor een lijst. Deze lijst geeft de kolomnaam en het gegevenstype aan.</p> <p>Voer een van de volgende handelingen uit:</p> 
       <ul> 
        <li style="font-weight: bold;">Selecteer een gegevensstructuur die al is gemaakt</li> 
        <li> <p style="font-weight: bold;">Een nieuwe gegevensstructuur toevoegen</p> <p>Klik op <strong>[!UICONTROL Add]</strong> om een nieuwe gegevensstructuur te maken.</p> <p>Voor meer informatie, zie de <a href="#set-up-the-data-structure" class="MCXref xref"> Opstelling de sectie van de gegevensstructuur </a> in dit artikel.</p> </li> 
        <li style="font-weight: bold;"> <p>Het veld leeg laten</p> <p style="font-weight: normal;">Als u geen gegevensstructuur selecteert of toevoegt, zal het gegevensbestand slechts de primaire sleutel bevatten. Een dergelijk databasetype is handig als u alleen sleutels wilt opslaan en alleen wilt weten of een bepaalde sleutel al dan niet bestaat in de database.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Data storage size in MB]</p> </td> 
      <td> <p>Wijs de grootte voor de gegevensopslag toe vanuit uw totale interne gegevensopslag.</p> <p> De standaardwaarde is 10 MB. Als u minder dan 10 MB aan niet toegewezen ruimte van de Opslag van Gegevens van uw toewijzing 95 MB hebt, is de standaardgrootte de hoeveelheid niet toegewezen opslag.  <p>Opmerking: het gereserveerde bedrag kan op elk gewenst moment worden gewijzigd.</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### De gegevensstructuur instellen

1. Klik op **[!UICONTROL Add]** wanneer u een gegevensopslag maakt of bewerkt.
1. Configureer de volgende velden in het vak **[!UICONTROL Add data structure]** dat wordt weergegeven:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Data structure name]</td> 
      <td> <p> Voer een naam in voor de nieuwe gegevensstructuur.</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Specification]</p> </td> 
      <td> <p>Voer een van de volgende handelingen uit om de kolommen in de gegevensopslagruimte in te stellen.</p> 
       <ul> 
        <li> <p>Klik op <strong>[!UICONTROL Add item]</strong> om handmatig de eigenschappen van één kolom op te geven.</p> <p>Voer de <strong>[!UICONTROL Name]</strong> en <strong>[!UICONTROL Type]</strong> in voor de kolom in de gegevensopslagruimte en definieer de corresponderende eigenschappen.</p> </li> 
        <li> <p>Klik op <strong>[!UICONTROL Generator]</strong> om de kolommen te bepalen uit de voorbeeldgegevens die u opgeeft.</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b> Voorbeeld: </b></span></span> 
          <p>Met de volgende JSON-voorbeeldgegevens worden bijvoorbeeld drie kolommen gemaakt: naam, leeftijd en telefoonnummer. Telefoonnummer is een verzameling mobiele en vaste telefoonnummers.</p> 
          <p><code>&lbrace;</code> </p> 
          <p><code>"name":"John",</code> </p> 
          <p><code>"age":30,</code> </p> 
          <p><code>"phone number": &lbrace;</code> </p> 
          <p><code>"mobile":"987654321",</code> </p> 
          <p><code>"landline":"123456789"</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p>De lege kolommen in de mening van de gegevensopslag:</p> 
          <p> <img src="assets/empty-columns-350x132.png" style="width: 350;height: 132;"> </p> 
          <p>Vervolgens kunt u handmatig waarden aan de gegevensopslag toevoegen of de modules voor gegevensopslag van [!DNL Workfront Fusion] gebruiken.</p> 
         </div> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Strict] </td> 
      <td> <p>Schakel deze optie in om ervoor te zorgen dat de lading overeenkomt met de gegevensstructuren. De ladingen die extra punten bevatten die niet in de gegevensstructuur worden gespecificeerd worden verworpen.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Een bestaande gegevensopslag bewerken

U kunt de eigenschappen en inhoud van een bestaande gegevensopslag bewerken in het [!UICONTROL Data Store] -gebied van [!DNL Workfront Fusion] .

* [De eigenschappen van een gegevensopslagruimte bewerken](#edit-the-properties-of-a-data-store)
* [De inhoud van een gegevensopslagruimte bewerken](#edit-the-contents-of-a-data-store)

### De eigenschappen van een gegevensopslagruimte bewerken

De eigenschappen van een gegevensopslag omvatten de gegevensstructuur die de gegevensopslag gebruikt, evenals de grootte van de gegevensopslag.

1. Klik op **[!UICONTROL Data Store]** ![](assets/data-store-icon.png) in het navigatievenster aan de linkerkant om het [!UICONTROL Data Store] -gebied te openen.
1. Klik op **[!UICONTROL Edit]** ![](assets/data-store-edit.png) naast de gegevensopslagruimte die u wilt bewerken.
1. (Optioneel) Als u de gegevensstructuur die door deze gegevensopslag wordt gebruikt, wilt wijzigen in een andere bestaande gegevensstructuur, selecteert u deze in de vervolgkeuzelijst **[!UICONTROL Data structure]** .

   of

   (Facultatief) als u de gegevensstructuur wilt veranderen die door deze gegevensopslag aan een volledig nieuwe gegevensstructuur wordt gebruikt, zie [ Opstelling de gegevensstructuur ](#set-up-the-data-structure) in dit artikel.

1. (Optioneel) Wijzig de grootte van de gegevensopslagruimte door de nieuwe grootte in te voeren in het veld **[!UICONTROL Data storage size in MB]** .
1. Klik op **[!UICONTROL Save]**.

### De inhoud van een gegevensopslagruimte bewerken

1. Klik op het pictogram **[!UICONTROL Data Store]** ![](assets/data-store-icon.png) in het navigatievenster aan de linkerkant om het [!UICONTROL Data Store] -gebied te openen.
1. Klik op **[!UICONTROL Browse]** naast de gegevensopslagruimte die u wilt bewerken.
1. (Optioneel) U kunt kolommen opnieuw ordenen door deze naar de gewenste locatie te slepen.
1. (Optioneel) [!UICONTROL Edit] één cel door op het pictogram **[!UICONTROL Edit]** in die cel te klikken en vervolgens de gewenste waarde in te voeren.
1. (Optioneel) Voeg een nieuw item aan de gegevensopslag toe door op **[!UICONTROL Add]** te klikken en vervolgens de gegevens voor het nieuwe item in te voeren.
1. Klik op **[!UICONTROL Save]**.

## Problemen oplossen

* [Verloren gegevens uit een gegevensopslagruimte herstellen](#restoring-lost-data-from-a-data-store)
* [Fout: onvoldoende ruimte](#out-of-space-error)
* [Maximum aantal winkels bereikt fout](#maximum-stores-reached-error)

### Verloren gegevens uit een gegevensopslagruimte herstellen

Er is momenteel geen gereedschap waarmee u het herstellen van verloren gegevens kunt automatiseren.

#### Workaround

1. Onderzoek alle uitvoeringslogboeken van scenario&#39;s waar de punten aan de gegevensopslag werden opgenomen.

   Voor meer informatie bij het onderzoeken van uitvoeringslogboeken, zie [ Mening de uitvoeringshistorie van een scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. Kopieer de gegevens.
1. Voeg de gegevens opnieuw in de gegevensopslag in.

   Voor informatie bij het opnemen van gegevens in een gegevensopslag, zie [ de inhoud van een gegevensopslag ](#edit-the-contents-of-a-data-store) in dit artikel uitgeven.

### [!UICONTROL Out of space] fout

Er treedt een [!UICONTROL Out of Space] -fout op omdat aan uw eerder gemaakte gegevensopslagruimten al opslagruimte is toegewezen.

#### Workaround

1. Bewerk de bestaande gegevensopslagruimten om minder ruimte te gebruiken. Hierdoor komt er ruimte vrij voor uw nieuwe gegevensopslag.

   Voor meer informatie, zie [ de eigenschappen van een gegevensopslag ](#edit-the-properties-of-a-data-store) in dit artikel uitgeven.

>[!NOTE]
>
>Wij adviseren dat u niet al uw ruimte aan één enkele gegevensopslag toewijst tenzij u zeker bent u niet meer gegevensopslag zult vereisen.

### [!UICONTROL Maximum stores reached] fout

Er treedt een [!UICONTROL Maximum stores reached] -fout op omdat uw organisatie alle beschikbare gegevensopslagruimten heeft gebruikt. Een organisatie heeft een aantal beschikbare gegevensopslag gelijk aan tweemaal het aantal beschikbare scenario&#39;s. Daarom hangt het totale aantal beschikbare gegevensopslag van het plan af u hebt gekocht.

Als uw organisatie bijvoorbeeld een abonnement met 15 scenario&#39;s heeft aangeschaft, kan de organisatie maximaal 30 gegevensopslagruimten hebben.

#### Workaround

Als u het aantal bestaande gegevensopslagruimten wilt verminderen, kunt u een van de volgende handelingen uitvoeren:

* Bestaande gegevensopslagruimten combineren
* Ongebruikte gegevensopslagruimten verwijderen
