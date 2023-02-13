---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Gegevenstypen item in [!DNL Adobe Workfront Fusion]
description: Uw [!DNL Adobe Workfront Fusion] scenario's kunnen de hieronder vermelde soorten punten in een bundel bevatten.
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Gegevenstypen item in [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Gegevenstypen item

U kunt de hieronder vermelde objecttypen in een bundel opnemen.

Voor informatie over welke soorten items [!DNL Workfront Fusion] staat conversie tussen elkaar toe, zie [Afgedwongen typegebruik in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Tekst</p> </td> 
   <td> <p>Het meest gangbare itemtype. Voor sommige tekstitems: [!DNL Adobe Workfront Fusion] Hiermee wordt gecontroleerd of de maximale of minimale toegestane lengte is bereikt of of de indeling van het item is gevalideerd (e-mail, URL of bestandsnaam).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Getal</p> </td> 
   <td> <p>Voor sommige numerieke items: [!DNL Workfront Fusion] kan de invoer voor een opgegeven bereik (de minimaal of maximaal toegestane waarde) valideren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Boolean (Ja/Nee)</p> </td> 
   <td> <p>Dit type wordt gebruikt voor items met slechts twee mogelijke waarden: true of false. </p> <p>Bij het instellen van modules kan het type Boolean in twee verschillende vormen worden weergegeven:</p> 
    <ul> 
     <li> <p>Het verplichte selectievakje wordt weergegeven als het veld verplicht is en moet worden ingevuld.</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>Optionele velden die leeg kunnen worden gelaten, worden weergegeven als een selectievak, zodat u kunt kiezen uit drie waarden: <code>Yes</code>, <code>No</code>, en <code>Not defined</code> (standaard).</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>U kunt op <strong>[!UICONTROL Map]</strong> als u de waarde aan een punt van een andere module moet in kaart brengen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Datum</p> </td> 
   <td> <p>Datums worden bijvoorbeeld ingevoerd in de datumnotatie ISO 8601. <code>2015-09-18T11:58Z</code>. U kunt de tijdzone wijzigen in uw profielinstellingen, zoals wordt uitgelegd in <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Profielinstellingen wijzigen in [!DNL Adobe Workfront Fusion]</a>. </p> <p>Als u op een veld klikt waarvoor een datum is vereist, wordt een pop-upkalender weergegeven in de module-instellingen. Voor sommige items is de tijd niet vereist.</p> <p>Waarden van Date-items worden opgemaakt met de lokale tijdzone en de webtijdzone die in uw profiel zijn geselecteerd. U kunt de ISO 8601-versie van de waarde van een datumitem weergeven door de aanwijzer boven het item te plaatsen.</p> <p>Opmerking: Als de ISO-waarde niet wordt weergegeven, is het item waarschijnlijk tekst, niet een datum.</p> <p>De tijd wordt ingevoerd in de <code>hours:minutes:seconds</code> opmaak, bijvoorbeeld<code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Buffer (binaire gegevens)</p> </td> 
   <td> <p>Bestandsinhoud wordt meestal verzonden als inhoud van het type Buffer (afbeeldingsinhoud, videobestand en andere). In sommige gevallen worden tekstgegevens in dit type opgenomen (bijvoorbeeld een tekstbestand). [!DNL Workfront Fusion] kan tekstgegevens in binaire code automatisch omzetten in tekst en tekst in tekstgegevens in binaire code. Zie voor meer informatie <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">Bestanden toewijzen in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Verzameling</p> </td> 
   <td> <p>Een verzameling is een item dat uit meerdere subitems bestaat. Het item van de afzender in een e-mailbericht is een voorbeeld van een verzameling: het bevat de naam van de afzender (teksttype) en het e-mailadres van de afzender (teksttype).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Selecteren (menu)</p> </td> 
   <td> <p>Wanneer u de modulemontages zoals die worden beschreven in vormt <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">De instellingen van een module configureren in [!DNL Adobe Workfront Fusion]</a>, kunt u verschillende items van hetzelfde type selecteren. Een voorbeeld hiervan is het menu dat de map selecteert in de instellingen voor de [!DNL Dropbox] modules. </p> <p>Bij het instellen van modules kan het menu Selecteren in twee formulieren worden weergegeven:</p> <p> <p>Als meerdere selecties mogelijk zijn, worden meerdere items met selectievakjes weergegeven.</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>Als er maar één optie mogelijk is, wordt een vervolgkeuzemenu weergegeven.</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>Als u een punt van een andere module moet in kaart brengen, gebruik <strong>Kaart</strong> knop. Met deze knop wordt een tekstveld geopend in plaats van het selectiemenu. Zie voor meer informatie <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Array</p> </td> 
   <td> <p>U kunt het arraytype gebruiken om met verschillende waarden van hetzelfde type te werken, waaronder verzamelingen. Een voorbeeld is het [!UICONTROL Email] modules: ze retourneren een array met bijlagen en elke bijlage bevat naam, inhoud, grootte enzovoort. Zie voor meer informatie <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">Een array toewijzen in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Validatie</p> </td> 
   <td> <p>[!DNL Workfront Fusion] kan validatie uitvoeren voor elk type item. Als een item de validatie niet doorgeeft, stopt de module de verwerking vanwege een gegevensfout. Zie voor meer informatie <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">Fout bij verwerken in [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
