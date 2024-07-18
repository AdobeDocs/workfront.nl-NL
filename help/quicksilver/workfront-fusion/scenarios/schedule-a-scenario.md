---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Een scenario plannen in Adobe Workfront Fusion
description: Door gebrek, loopt een scenario om de 15 minuten. U kunt dit veranderen door te bepalen wanneer en hoe vaak een geactiveerd scenario loopt.
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: f5549be5951a2648d6a77d25bebbd4141f18d36c
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 0%

---

# Een scenario inplannen in [!DNL Adobe Workfront Fusion]

Door gebrek, loopt een scenario om de 15 minuten. U kunt dit veranderen door te bepalen wanneer en hoe vaak een geactiveerd scenario loopt. De scenario&#39;s van de fusie kunnen worden gepland zo vaak zoals om de 5 minuten te lopen.

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
   <p>Vereiste voor verouderde licentie: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie], [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td>    </tr> 
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

## Een scenario plannen

1. Klik in de rechterbovenhoek van de vervolgkeuzelijst Scenario op **[!UICONTROL Options]** > **[!UICONTROL Scheduling]**

   of

   Klik op het pictogram **[!UICONTROL Scheduling]** (klok) op de triggermodule van het scenario.

1. Voer gegevens in de volgende velden in:

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Run scenario]</td> 
      <td> <p>Selecteer de frequentie waarmee u het scenario wilt uitvoeren, en selecteer dan het interval.</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL At regular intervals]</strong> </p> <p>Voer het aantal minuten in tussen de uitvoeringen. De standaardwaarde is 15 minuten.</p> </li> 
        <li> <p><strong>[!UICONTROL Once]</strong> </p> <p>Voer de datum en tijd in waarop het scenario moet worden uitgevoerd. Gebruik de indeling <code>MM/DD/YYYY h:mm A</code> . Voorbeeld: <code>06/25/2019 11:00 PM</code> .</p> </li> 
        <li> <p><strong>[!UICONTROL Every day]</strong> </p> <p>Voer de tijd in waarop het scenario moet worden uitgevoerd. Gebruik de indeling <code>h:mm A</code> . Voorbeeld: <code>11:00 PM</code> .</p> </li> 
        <li> <p><strong>[!UICONTROL Days of the week]</strong> </p> <p>Dagen: selecteer de dagen van de week dat u het scenario wilt lopen. U kunt een of meer dagen selecteren.</p> <p>Tijd: ga de tijd in dat u het scenario op de geselecteerde dagen wilt lopen. Gebruik de indeling <code>h:mm A</code> . Voorbeeld: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Days of the month]</strong> </p> <p>Dagen: selecteer de dagen van de maand die u het scenario wilt lopen. U kunt een of meer dagen selecteren.</p> <p>Tijd: ga de tijd in dat u het scenario op de geselecteerde dagen wilt lopen. Gebruik de indeling <code>h:mm A</code> . Voorbeeld: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Specified dates]</strong> </p> <p>Maanden: selecteer de maanden die u het scenario wilt uitvoeren. U kunt een of meer maanden selecteren.</p> <p>Dagen: selecteer de dagen van de maand die u het scenario wilt lopen. U kunt een of meer dagen selecteren.</p> <p>Tijd: ga de tijd in dat u het scenario op de geselecteerde dagen wilt lopen. Gebruik de indeling <code>h:mm A</code> . Voorbeeld: <code>11:00 PM</code></p> </li> 
       </ul> <p>Opmerking: een scenario kan alleen op die datum worden uitgevoerd als er een datum is. Een scenario dat bijvoorbeeld alleen voor de 31e van de maand is gepland, loopt niet in februari, april, juni, september of november, omdat die maanden geen 31e dag hebben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Advanced scheduling]</td> 
      <td>U kunt specifieke tijdintervallen bepalen waarin uw scenario moet lopen. U kunt tijdsintervallen van dagen, weekdagen of maanden opgeven. Klik voor elk interval op <strong>[!UICONTROL Add]</strong> en vul de velden in zoals wordt beschreven in het veld [!UICONTROL Run scenario] .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Start]</td> 
      <td>Ga de datum en de tijd in waarna u het scenario wilt lopen. Gebruik de indeling <code>MM/DD/YYYY h:mm A</code> . Voorbeeld: <code>06/25/2019 11:00 PM</code> .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL End]</td> 
      <td>Voer de datum en tijd in waarop het scenario moet worden uitgevoerd. Gebruik de indeling <code>MM/DD/YYYY h:mm A</code> . Voorbeeld: <code>06/25/2019 11:00 PM</code> .</td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **[!UICONTROL OK]** om de planningsmontages te bewaren en aan het scenario terug te keren.
