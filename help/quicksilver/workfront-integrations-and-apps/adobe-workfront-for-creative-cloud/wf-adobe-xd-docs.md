---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: XD tekengebieden uploaden naar Workfront
description: U kunt uw tekengebieden uploaden als documenten voor een snelle revisie en goedkeuring of eenvoudig in Adobe Workfront opslaan.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---


# [!DNL XD] tekengebieden als documenten uploaden naar [!DNL Workfront]

U kunt uw tekengebieden uploaden als documenten voor een snelle revisie en goedkeuring of eenvoudig in [!DNL Adobe Workfront] opslaan.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <!-- <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> -->
   <td role="rowheader">Product</td> 
   <td>U moet een [!DNL Adobe Creative Cloud] licentie hebben naast een [!DNL Workfront] licentie.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang bewerken tot [!UICONTROL Documents]</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de [!DNL Workfront] -beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>[!UICONTROL View] toegang tot of hoger voor het object waar u een document wilt uploaden.</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

+++

## Vereisten

* U moet de plug-in [!DNL Adobe Workfront for XD] installeren voordat u XD tekengebieden als documenten kunt uploaden naar Workfront.

Voor instructies, zie [&#x200B; installeren  [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Een nieuw document toevoegen

1. Klik op het pictogram **[!UICONTROL Menu]** in de rechterbovenhoek en selecteer vervolgens **[!UICONTROL Work List]** . U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![&#x200B; pictogram van het Menu &#x200B;](assets/menu-350x440.png)

1. Ga naar het werkitem waar u een document wilt uploaden.
1. Klik het **[!UICONTROL Document]** pictogram van het pictogram van het 1&rbrace; Document ![&#128279;](assets/documents.png) in de navigatiebar.

1. Klik op **[!UICONTROL New File]** onder aan de plug-in.
1. Selecteer het te uploaden tekengebied.

   >[!TIP]
   >
   >Als u meerdere tekengebieden wilt selecteren, klikt u en sleept u de muis over de gewenste tekengebieden.
1. (Optioneel) Typ een opmerking in het **[!UICONTROL Updates]** -gebied.
1. Kies de **[!UICONTROL Asset Type]** in de vervolgkeuzelijst:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL Export Format]</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>De tekengebieden worden als een PNG-bestand geüpload naar het tabblad [!UICONTROL Documents] van het tijdelijke item in [!DNL Workfront] . </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>De tekengebieden worden als een JPG geüpload naar het tabblad [!UICONTROL Documents] van het werkitem in [!DNL Workfront] . <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>De tekengebieden worden als een SVG geüpload naar het tabblad [!UICONTROL Documents] van het werkitem in [!DNL Workfront] . </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>Kies als u geselecteerde artboards als a <strong> Enig dossier van PDF </strong> of <strong> Veelvoudige dossiers van PDF </strong> wilt uploaden. De tekengebieden worden als een PDF geüpload naar het tabblad [!UICONTROL Documents] van het werkitem in [!DNL Workfront] .</td>
     </tr>
    </tbody>
   </table>


1. Klik op **[!UICONTROL Upload]**.\
   Het document wordt weergegeven in het gebied [!UICONTROL Documents] in de plug-in en de bureaubladtoepassing.

## Een nieuwe versie toevoegen

1. Klik op het pictogram **[!UICONTROL Menu]** in de rechterbovenhoek en selecteer vervolgens **[!UICONTROL Work List]** . U kunt het menu ook gebruiken om naar bovenliggende objecten te navigeren.

   ![&#x200B; pictogram van het Menu &#x200B;](assets/menu-350x440.png)

1. Ga naar het werkitem waar u een document wilt uploaden.
1. Klik het **[!UICONTROL Document]** pictogram van het pictogram van het 1&rbrace; Document ![&#128279;](assets/documents.png) in de navigatiebar.

1. Klik op het document waaraan u een nieuwe versie wilt toevoegen.
1. Klik op **[!UICONTROL New version]** onder aan de plug-in.
1. Selecteer de tekengebieden die u wilt uploaden.

   >[!NOTE]
   >
   >Als u een nieuwe versie van een SVG, PNG of JPG wilt uploaden, kunt u slechts één tekengebied uploaden.

1. (Optioneel) Typ een opmerking in het **[!UICONTROL Updates]** -gebied.

1. Kies de **[!UICONTROL Asset Type]** in de vervolgkeuzelijst:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">Exportindeling</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>Het tekengebied wordt als een PNG-bestand geüpload naar het tabblad [!UICONTROL Documents] van het tijdelijke item in [!DNL Workfront] . </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>Het tekengebied wordt als een JPG geüpload naar het tabblad [!UICONTROL Documents] van het werkitem in [!DNL Workfront] . <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>Het tekengebied wordt als een SVG geüpload naar het tabblad [!UICONTROL Documents] van het werkitem in [!DNL Workfront] . </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>De tekengebieden worden als een PDF geüpload naar het tabblad [!UICONTROL Documents] van het werkitem in [!DNL Workfront] .</p>
      <p><strong> Nota </strong>: U kunt slechts één artboard voor een nieuwe documentversie uploaden.</p>
      </td>
     </tr>
    </tbody>
   </table>

1. Klik op **[!UICONTROL Upload]**.\
   Het document wordt weergegeven in het gebied [!UICONTROL Documents] in de plug-in en de bureaubladtoepassing.
