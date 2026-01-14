---
product-area: documents
navigation-topic: approvals
title: Brandmerken instellen voor de AI Reviewer
description: Brandmerken instellen voor de AI Reviewer
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: cf1d4bfeedb94e8607dad47177d804169254ee85
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Brandmerken instellen voor de AI Reviewer

>[!IMPORTANT]
>
>Deze functie is momenteel in bèta.

De AI Reviewer gebruikt merkrichtlijnen om inhoud tijdens het revisieproces te evalueren. U kunt in Workfront merken maken door PDF-bestanden te uploaden die uw merkrichtlijnen bevatten of door handmatig merkelementen in te voeren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet systeembeheerder zijn.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Console-machtigingen</td> 
   <td> <p>Je moet GenStudio Brand Manager gebruiken.</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Vereisten

* Uw organisatie moet zijn gemigreerd naar Adobe IMS (Identity Management System).
* Uw instantie van Workfront moet Verenigde Goedkeuringen hebben toegelaten.
  <!--* Your organization must have GenStudio Foundation.-->
* Adobe moet een ondertekende Adobe Gen AI-overeenkomst in het bestand hebben.
Voor meer informatie bij het ondertekenen van de overeenkomst, zie [ Ondertekenen de overeenkomst van Adobe Gen AI ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).

## Een merk maken met een PDF

{{step-1-to-setup}}

1. In het linkerpaneel, ga naar **Overzicht en Goedkeuring** > **Merken**.
1. Klik **voeg merk** in de hoger-juiste hoek van het scherm toe.
1. Geef het merk een naam.
1. Klik op PDF&#39;s uploaden om bestanden met een merk te uploaden.
   ![ uploadt brandmerk pdfs ](assets/upload-PDF.png)
1. Klik **verdergaan**.
1. Upload één of meerdere dossiers van PDF die uw merkrichtlijnen bevatten, dan klik **merk** toevoegen.
1. Nadat de bestanden zijn geüpload, controleert u de geëxtraheerde merkelementen om te controleren of deze overeenkomen met de richtlijnen voor uw merk.

   >[!IMPORTANT]
   >
   >Richtlijnen worden gegenereerd op basis van uw bestanden en generatieve AI-technologie en zijn mogelijk onjuist. Lees de uitgepakte richtlijnen voor ontbrekende of onjuiste details en bewerk deze voordat u dit merk publiceert.

1. Wanneer gebeëindigd, publiceer **** om het merk voor de AI Recensent beschikbaar te maken.

## Handmatig een merk maken

{{step-1-to-setup}}

1. In het linkerpaneel, ga naar **Overzicht en Goedkeuring** > **Merken**.
1. Klik **voeg merk** in de hoger-juiste hoek van het scherm toe.
1. Geef het merk een naam.
1. Klik **toevoegen manueel** om een merk met individuele elementen tot stand te brengen.
1. Vul zo nodig de merkgegevens in. U kunt de volgende elementen toevoegen:

   <table>
    <tr>
        <td>Wanneer gebruiken</td>
        <td>Laat de marketeers weten wanneer ze dit merk moeten gebruiken.</td>
    </tr>
    <tr>
        <td>Richtlijnen voor stem</td>
        <td>Zorg voor begeleiding bij de toon en de stijl van de stem van het merk.</td>
    </tr>
    <tr>
        <td>Richtlijnen voor afbeeldingen</td>
        <td>Geef de typen afbeeldingen op die u wilt uitlijnen met de identiteit van het merk.</td>
    </tr>
    <tr>
        <td>Kanaalrichtlijnen</td>
        <td>Geef een overzicht van de geschikte kanalen voor merkcommunicatie.</td>
    </tr>
    <tr>
        <td>logo</td>
        <td>Neem de officiële logo's van het merk op.</td>
    </tr>
    <tr>
        <td>Kleuren</td>
        <td>Geef het kleurenpalet van het merk op.</td>
    </tr>
    </table>

   ![ voeg merkelementen manueel toe ](assets/brand-elements.png)


1. Wanneer gebeëindigd, publiceer **** om het merk voor de AI Recensent beschikbaar te maken.
