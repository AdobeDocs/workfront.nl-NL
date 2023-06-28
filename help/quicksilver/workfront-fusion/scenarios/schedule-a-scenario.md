---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Een scenario plannen in Adobe Workfront Fusion
description: Door gebrek, loopt een scenario om de 15 minuten. U kunt dit veranderen door te bepalen wanneer en hoe vaak een geactiveerd scenario loopt.
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

# Een scenario plannen in [!DNL Adobe Workfront Fusion]

Door gebrek, loopt een scenario om de 15 minuten. U kunt dit veranderen door te bepalen wanneer en hoe vaak een geactiveerd scenario loopt.

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
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor arbeidsautomatisering en -integratie],  [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td>    </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereisten: Als u de [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Oudere productvereisten: Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Een scenario plannen

1. Klik in de rechterbovenhoek van de vervolgkeuzelijst Scenario op **[!UICONTROL Options]** > **[!UICONTROL Scheduling]**

   of

   Klik op de knop **[!UICONTROL Scheduling]** pictogram (klok) op de de trekkermodule van het scenario.

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
        <li> <p><strong>[!UICONTROL Once]</strong> </p> <p>Voer de datum en tijd in waarop het scenario moet worden uitgevoerd. De indeling gebruiken <code>MM/DD/YYYY h:mm A</code>. Voorbeeld: <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Every day]</strong> </p> <p>Voer de tijd in waarop het scenario moet worden uitgevoerd. De indeling gebruiken <code>h:mm A</code>. Voorbeeld: <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Days of the week]</strong> </p> <p>Dagen: Selecteer de dagen van de week die u het scenario wilt lopen. U kunt een of meer dagen selecteren.</p> <p>Tijd: Voer de tijd in waarop het scenario op de geselecteerde dagen moet worden uitgevoerd. De indeling gebruiken <code>h:mm A</code>. Voorbeeld: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Days of the month]</strong> </p> <p>Dagen: Selecteer de dagen van de maand die u het scenario wilt lopen. U kunt een of meer dagen selecteren.</p> <p>Tijd: Voer de tijd in waarop het scenario op de geselecteerde dagen moet worden uitgevoerd. De indeling gebruiken <code>h:mm A</code>. Voorbeeld: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Specified dates]</strong> </p> <p>Maanden: Selecteer de maanden die u het scenario wilt in werking stellen. U kunt een of meer maanden selecteren.</p> <p>Dagen: Selecteer de dagen van de maand die u het scenario wilt lopen. U kunt een of meer dagen selecteren.</p> <p>Tijd: Voer de tijd in waarop het scenario op de geselecteerde dagen moet worden uitgevoerd. De indeling gebruiken <code>h:mm A</code>. Voorbeeld: <code>11:00 PM</code></p> </li> 
       </ul> <p>Opmerking: Er moet een datum zijn waarop een scenario op die datum kan worden uitgevoerd. Een scenario dat bijvoorbeeld alleen voor de 31e van de maand is gepland, loopt niet in februari, april, juni, september of november, omdat die maanden geen 31e dag hebben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Advanced scheduling]</td> 
      <td>U kunt specifieke tijdintervallen bepalen waarin uw scenario moet lopen. U kunt tijdsintervallen van dagen, weekdagen of maanden opgeven. Voor elk interval klikt u op <strong>[!UICONTROL Add]</strong> en vult de velden in zoals beschreven in het dialoogvenster [!UICONTROL Run scenario] veld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Start]</td> 
      <td>Ga de datum en de tijd in waarna u het scenario wilt lopen. De indeling gebruiken <code>MM/DD/YYYY h:mm A</code>. Voorbeeld: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL End]</td> 
      <td>Voer de datum en tijd in waarop het scenario moet worden uitgevoerd. De indeling gebruiken <code>MM/DD/YYYY h:mm A</code>. Voorbeeld: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **[!UICONTROL OK]** om de planningsmontages te bewaren en aan het scenario terug te keren.
