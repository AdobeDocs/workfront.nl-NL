---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Typedruk in Adobe Workfront Fusion
description: In dit document wordt beschreven hoe [!DNL Adobe Workfront Fusion] gedraagt zich in situaties wanneer het waarden in verwachte en onverwachte gegevensformaten ontvangt.
author: Becky
feature: Workfront Fusion
exl-id: 847a17c9-bd67-4132-81a8-2a5fe8d516cb
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%

---

# Afgedwongen typegebruik in [!DNL Adobe Workfront Fusion]

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
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td> 
  </tr> 
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

### Afgedwongen typegebruik

In dit document wordt beschreven hoe [!DNL Adobe Workfront Fusion] gedraagt zich in situaties wanneer het waarden in verwachte en onverwachte gegevensformaten ontvangt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Verwacht</th> 
   <th>Ontvangen</th> 
   <th> <p>Beschrijving</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>array </td> 
   <td>array </td> 
   <td> <p>De waarde wordt ongewijzigd overgedragen.</p> </td> 
  </tr> 
  <tr> 
   <td>array </td> 
   <td>overige </td> 
   <td> <p>Als de ontvangen waarde niet van het matrixtype is, [!DNL Workfront Fusion] wordt een array gemaakt en de ontvangen waarde wordt het eerste (en enige) element.</p> </td> 
  </tr> 
  <tr> 
   <td>boolean </td> 
   <td>boolean </td> 
   <td> <p>De waarde wordt ongewijzigd overgedragen.</p> </td> 
  </tr> 
  <tr> 
   <td>boolean </td> 
   <td>getal </td> 
   <td> <p>De waarde wordt omgezet in logische ja, zelfs als de waarde 0 is.</p> </td> 
  </tr> 
  <tr> 
   <td>boolean </td> 
   <td>text </td> 
   <td> <p>Als de waarde gelijk is aan false of als de waarde leeg is, wordt deze omgezet in logische Nee. Als niet, wordt het omgezet in logische ja.</p> </td> 
  </tr> 
  <tr> 
   <td>boolean </td> 
   <td>overige </td> 
   <td> <p>De waarde wordt in logische Ja omgezet wanneer de ontvangen waarde bestaat (is niet null).</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>buffer </td> 
   <td> <p>De waarde wordt alleen ongewijzigd overgedragen als de codepage naar verwachting is. Indien de codepagina afwijkt, [!DNL Workfront Fusion] zal proberen om de ontvangen waarde in de gevraagde codepage om te zetten. Als deze conversie niet wordt ondersteund, [!DNL Workfront Fusion] retourneert een validatiefout.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>boolean </td> 
   <td> <p>De waarde wordt omgezet in tekst (true/false) en vervolgens in binaire gegevens volgens de bovenstaande stappen voor het omzetten in tekst.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>date </td> 
   <td> <p>De waarde wordt omgezet in ISO 8601-tekst en vervolgens in binaire gegevens volgens de stappen die worden beschreven voor het omzetten in tekst.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>getal </td> 
   <td> <p>De waarde wordt omgezet in tekst en vervolgens in binaire gegevens volgens de stappen hierboven voor het omzetten in tekst.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>text </td> 
   <td> <p>De waarde wordt omgezet in binaire gegevens en gecodeerd zoals verwacht. Als de verwachte codering niet is opgegeven, wordt utf8-codering gebruikt.</p> </td> 
  </tr> 
  <tr> 
   <td>buffer </td> 
   <td>overige </td> 
   <td> <p>[!DNL Workfront Fusion] retourneert een validatiefout.</p> </td> 
  </tr> 
  <tr> 
   <td>collectie </td> 
   <td>collectie </td> 
   <td> <p>De waarde wordt ongewijzigd overgedragen.</p> </td> 
  </tr> 
  <tr> 
   <td>collectie </td> 
   <td>overige </td> 
   <td> <p>[!DNL Workfront Fusion] retourneert een validatiefout.</p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>date </td> 
   <td> <p>De waarde wordt ongewijzigd overgedragen.</p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] probeert de tekst om te zetten in een datum. Als de conversie mislukt, wordt een validatiefout geretourneerd. Datum moet dag, maand en jaar bevatten. Datum kan tijd en tijdzone bevatten. De standaardtijdzone is gebaseerd op uw instellingen. Voorbeelden:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>date </td> 
   <td>overige </td> 
   <td> <p>[!DNL Workfront Fusion] retourneert een validatiefout.</p> </td> 
  </tr> 
  <tr> 
   <td>getal </td> 
   <td>getal </td> 
   <td> <p>De waarde wordt ongewijzigd overgedragen.</p> </td> 
  </tr> 
  <tr> 
   <td>getal </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] probeert de tekst om te zetten in een getal. Als de conversie mislukt, wordt een validatiefout geretourneerd.</p> </td> 
  </tr> 
  <tr> 
   <td>getal </td> 
   <td>overige </td> 
   <td> <p>[!DNL Workfront Fusion] retourneert een validatiefout.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>text </td> 
   <td> <p>De waarde wordt ongewijzigd overgedragen.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>array </td> 
   <td> <p>Als de opgegeven array conversie naar tekst ondersteunt, wordt de waarde omgezet. Zo niet, [!DNL Workfront Fusion] retourneert een validatiefout.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>boolean </td> 
   <td> <p>De waarde wordt omgezet in tekst (true/false).</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>buffer </td> 
   <td> <p>Als tekstcodering is opgegeven voor binaire gegevens, wordt de waarde omgezet in tekst. Zo niet, [!DNL Workfront Fusion] retourneert een validatiefout.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>date </td> 
   <td> <p>De waarde wordt omgezet in ISO 8601-tekst.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>getal </td> 
   <td> <p>De waarde wordt geconverteerd naar tekst.</p> </td> 
  </tr> 
  <tr> 
   <td>text </td> 
   <td>overige </td> 
   <td> <p>[!DNL Workfront Fusion] retourneert een validatiefout.</p> </td> 
  </tr> 
  <tr> 
   <td>tijd </td> 
   <td>tijd </td> 
   <td> <p>De waarde wordt ongewijzigd overgedragen.</p> </td> 
  </tr> 
  <tr> 
   <td>tijd </td> 
   <td>text </td> 
   <td> <p>[!DNL Workfront Fusion] zal proberen tijd in de uren om te zetten:minutes:secondenformaat. Als de conversie mislukt, wordt een validatiefout geretourneerd.</p> </td> 
  </tr> 
  <tr> 
   <td>tijd </td> 
   <td>overige </td> 
   <td> <p>[!DNL Workfront Fusion] retourneert een validatiefout.</p> </td> 
  </tr> 
 </tbody> 
</table>
