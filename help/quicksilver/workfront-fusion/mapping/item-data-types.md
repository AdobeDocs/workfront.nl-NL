---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Gegevenstypen item in  [!DNL Adobe Workfront Fusion]
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Gegevenstypen item in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ de gegevenstypes van het Punt ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/data-types/item-data-types.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

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
   <p>Vereiste voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en integratie] </p>
   </td> 
  </tr> 
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

## Gegevenstypen item

U kunt de hieronder vermelde objecttypen in een bundel opnemen.

Voor informatie over welke types van punten [!DNL Workfront Fusion] voor omzetting tussen elkaar toestaat, zie [ Druk van het Type in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Tekst</p> </td> 
   <td> <p>Het meest gangbare itemtype. Voor sommige tekstitems controleert [!DNL Adobe Workfront Fusion] of aan de maximum- of minimumlengte is voldaan of de indeling van het item is gevalideerd (e-mail, URL of bestandsnaam).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Getal</p> </td> 
   <td> <p>Voor sommige numerieke items valideert [!DNL Workfront Fusion] mogelijk de invoer voor een opgegeven bereik (de minimaal of maximaal toegestane waarde).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Boolean (Ja/Nee)</p> </td> 
   <td> <p>Dit type wordt gebruikt voor items met slechts twee mogelijke waarden: true of false. </p> <p>Bij het instellen van modules kan het type Boolean in twee verschillende vormen worden weergegeven:</p> 
    <ul> 
     <li> <p>Het verplichte selectievakje wordt weergegeven als het veld verplicht is en moet worden ingevuld.</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>Optionele velden die leeg kunnen worden gelaten, worden weergegeven als een selectievak, zodat u ze kunt selecteren op basis van drie waarden: <code>Yes</code>, <code>No</code> en <code>Not defined</code> (standaard).</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>U kunt <strong>[!UICONTROL Map]</strong> klikken als u de waarde aan een punt van een andere module moet in kaart brengen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Datum</p> </td> 
   <td> <p>Datums worden bijvoorbeeld ingevoerd in de datumnotatie ISO 8601. <code>2015-09-18T11:58Z</code> U kunt de tijdzone in uw profielmontages veranderen, zoals die in <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref"> wordt verklaard de profielmontages van de Verandering in [!DNL Adobe Workfront Fusion]</a>. </p> <p>Als u op een veld klikt waarvoor een datum is vereist, wordt een pop-upkalender weergegeven in de module-instellingen. Voor sommige items is de tijd niet vereist.</p> <p>Waarden van Date-items worden opgemaakt met de lokale tijdzone en de webtijdzone die in uw profiel zijn geselecteerd. U kunt de ISO 8601-versie van de waarde van een datumitem weergeven door de aanwijzer boven het item te plaatsen.</p> <p>Opmerking: als de ISO-waarde niet wordt weergegeven, is het item waarschijnlijk tekst, niet een datum.</p> <p>De tijd wordt ingegaan in het <code>hours:minutes:seconds</code> formaat, bijvoorbeeld, <code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Buffer (binaire gegevens)</p> </td> 
   <td> <p>Bestandsinhoud wordt meestal verzonden als inhoud van het type Buffer (afbeeldingsinhoud, videobestand en andere). In sommige gevallen worden tekstgegevens in dit type opgenomen (bijvoorbeeld een tekstbestand). [!DNL Workfront Fusion] kan tekstgegevens in binaire code automatisch omzetten in tekst en tekst in tekstgegevens in binaire code. Zie <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref"> Informatie over toewijzingsbestanden in [!UICONTROL Adobe Workfront Fusion]</a> voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Verzameling</p> </td> 
   <td> <p>Een verzameling is een item dat uit meerdere subitems bestaat. Het item Afzender in een e-mailbericht is een voorbeeld van een verzameling: het bevat de naam van de afzender (teksttype) en het e-mailadres van de afzender (teksttype).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Selecteren (menu)</p> </td> 
   <td> <p>Wanneer u de modulemontages zoals die in <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref"> worden beschreven vormt de montages van een module in [!DNL Adobe Workfront Fusion]</a>, kunt u uit verscheidene punten van het zelfde type selecteren. Een voorbeeld hiervan is het menu dat de map selecteert in de instellingen voor de modules [!DNL Dropbox] . </p> <p>Bij het instellen van modules kan het menu Selecteren in twee formulieren worden weergegeven:</p> <p> <p>Als meerdere selecties mogelijk zijn, worden meerdere items met selectievakjes weergegeven.</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>Als er maar één optie mogelijk is, wordt een vervolgkeuzemenu weergegeven.</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>Als u een punt van een andere module moet in kaart brengen, gebruik de <strong> Kaart </strong> knoop. Met deze knop wordt een tekstveld geopend in plaats van het selectiemenu. Voor meer informatie, zie <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref"> informatie van de Kaart van één module aan een andere in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Array</p> </td> 
   <td> <p>U kunt het arraytype gebruiken om met verschillende waarden van hetzelfde type te werken, waaronder verzamelingen. Een voorbeeld hiervan zijn de [!UICONTROL Email] -modules: ze retourneren een array met bijlagen en elke bijlage bevat naam, inhoud, grootte enzovoort. Voor meer informatie, zie <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref"> een serie in kaart brengen [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Validatie</p> </td> 
   <td> <p>[!DNL Workfront Fusion] kan validatie uitvoeren voor elk type item. Als een item de validatie niet doorgeeft, stopt de module de verwerking vanwege een gegevensfout. Voor meer informatie, zie <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref"> de verwerking van de Fout in [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
