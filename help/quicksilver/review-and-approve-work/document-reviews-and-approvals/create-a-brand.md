---
product-area: documents
navigation-topic: approvals
title: Merken maken en beheren voor de Content Reviewer
description: Merken maken en beheren voor de Content Reviewer
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b2788f3f-43d2-46f3-8502-bb833f8a0970
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 243aa2b0893e3034d37b959384a50b8a5e4a4bf0
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# Merken maken en beheren voor de Content Reviewer

De Content Reviewer gebruikt richtlijnen van het merk om de inhoud tijdens het revisieproces te evalueren. U kunt in Workfront merken maken door PDF-bestanden te uploaden die uw merkrichtlijnen bevatten of door handmatig merkelementen in te voeren.

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
   <td role="rowheader">Admin Console-machtigingen*</td> 
   <td> <p>Je moet GenStudio Brand Manager zijn.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

* Uw instantie van Workfront moet Verenigde Goedkeuringen hebben toegelaten.

* Uw organisatie moet GenStudio Foundation hebben.
   * Content Reviewer in Workfront biedt de functionaliteit die in GenStudio Foundation beschikbaar is voor workflows voor het beoordelen en goedkeuren van bedrijfsmiddelen. U hoeft GenStudio Foundation niet rechtstreeks te openen om uw werk te voltooien. Je toegang tot GenStudio Foundation-functionaliteit via Content Reviewer valt onder de voorwaarden van je Workfront-contract.
* Adobe moet een ondertekende Adobe Gen AI-overeenkomst in het bestand hebben.
Voor meer informatie bij het ondertekenen van de overeenkomst, zie [ Ondertekenen de overeenkomst van Adobe Gen AI ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).


## Vereisten

1. Voordat u merken kunt maken, moet u toegang verlenen tot merkmachtigingen in de Admin Console en in Workfront. Voor instructies, zie [ toegang van de Verlening tot merktoestemmingen ](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md).


## Een merk maken met een PDF

{{step-1-to-setup}}

1. In het linkerpaneel, ga naar **Overzicht en Goedkeuring** > **Merken**.
1. Klik **voeg merk** in de hoger-juiste hoek van het scherm toe.
1. Geef het merk een naam.
1. Klik **uploaden PDFs** om merkdossiers te uploaden.
   ![ uploadt brandmerk pdfs ](assets/upload-PDF.png)
1. Klik **verdergaan**.
1. Upload één of meerdere dossiers van PDF die uw merkrichtlijnen bevatten, dan klik **merk** toevoegen.
1. Nadat de bestanden zijn geüpload, controleert u de geëxtraheerde merkelementen om te controleren of deze overeenkomen met de richtlijnen voor uw merk.

   >[!IMPORTANT]
   >
   >Richtlijnen worden gegenereerd op basis van uw bestanden en generatieve AI-technologie en zijn mogelijk onjuist. Lees de uitgepakte richtlijnen voor ontbrekende of onjuiste details en bewerk deze voordat u dit merk publiceert.

1. Wanneer gebeëindigd, publiceer **** om het merk voor de Recensent van de Inhoud beschikbaar te maken.

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
        <td>Logo</td>
        <td>Neem de officiële logo's van het merk op.</td>
    </tr>
    <tr>
        <td>Kleuren</td>
        <td>Geef het kleurenpalet van het merk op.</td>
    </tr>
    </table>

   ![ voeg merkelementen manueel toe ](assets/brand-elements.png)


1. Wanneer gebeëindigd, publiceer **** om het merk voor de Recensent van de Inhoud beschikbaar te maken.


## Tips en trucs voor het schrijven van merkrichtlijnen

*  Schrijf merkrichtlijnen die meetbare criteria beschrijven. De Content Reviewer evalueert inhoud letterlijk, zodat objectieve regels consistentere scores opleveren dan subjectieve scores.

* Zoek naar woorden als &quot;mijden,&quot; &quot;houden,&quot; of &quot;zorg ervoor&quot;in uw richtlijnen. Deze signalen geven vaak een regel aan die u kunt aanscherpen. Vervang de vage instructie door een specifieke lijst met woorden, indelingen of beperkingen. Vervang bijvoorbeeld &quot;algemene skinkenslikés vermijden&quot; door &quot;geen gnar,&quot;&quot;pow,&quot; of &quot;shred&quot; gebruiken.

* Als je de subjectiviteit niet kunt verwijderen, versmal het. Brede adjecten vervangen door specifieke beperkingen. Zo wordt &#39;Direct en actiegericht&#39; bijvoorbeeld &#39;Direct en actiegericht&#39;, worden vulwoorden en afdekkingstaal weggelaten.