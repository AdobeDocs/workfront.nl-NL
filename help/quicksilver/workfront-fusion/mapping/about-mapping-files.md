---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Bestanden toewijzen in [!DNL Adobe Workfront Fusion]
description: Sommige modules kunnen bestanden verwerken. Deze modules kunnen een uitvoerbestand retourneren dat voor verdere verwerking moet worden verzonden of een bestand vereisen dat voor verwerking aan hen wordt doorgegeven. Voordat deze modules kunnen samenwerken om bestanden te verwerken, moeten ze aan elkaar worden toegewezen.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Bestanden toewijzen in [!DNL Adobe Workfront Fusion]

Sommige modules kunnen bestanden verwerken. Deze modules kunnen een uitvoerbestand retourneren dat voor verdere verwerking moet worden verzonden of een bestand vereisen dat voor verwerking aan hen wordt doorgegeven. Voordat deze modules kunnen samenwerken om bestanden te verwerken, moeten ze aan elkaar worden toegewezen.

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
  </tr>  </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Toewijzingsbestanden

Modules die bestanden kunnen bewerken, vereisen twee informatie:

* Bestandsnaam
* Bestandsinhoud (gegevens)

Wanneer u een dossier in kaart brengt, kiest u de modules in uw scenario waarvan u de gegevens wilt verkrijgen. De bestandsnaam en de bestandsinhoud worden vervolgens automatisch toegewezen zoals ze zijn.

>[!NOTE]
>
>Als u een bestand vanaf een URL moet verwerken, raden we u aan het `HTTP > Get a File` -module om het bestand te downloaden van de URL en het bestand vervolgens toe te wijzen vanuit de `HTTP > Get a File` aan het gewenste gebied van de module in uw scenario.

>[!INFO]
>
>**Voorbeeld:** In dit voorbeeld wordt getoond hoe u documenten kunt downloaden van [!DNL Adobe Workfront] tot [!DNL Google Drive]. De [!DNL Workfront] trigger [!UICONTROL Watch Record] retourneert gedetailleerde informatie over elk document, inclusief naam en id.
>
>De volgende module, [!UICONTROL Download Document]worden de feitelijke gegevens gedownload zodat deze naar Google Drive kunnen worden geüpload.
>
>Deze informatie toewijzen aan [!DNL Google Drive] om het te kunnen uploaden, moet u het brondossier specificeren waarvan de informatie zal worden in kaart gebracht. Als u [!DNL Workfront] > [!UICONTROL Download Document] optie onder het bronbestand, [!DNL Workfront Fusion] Wijst de bestandsnaam en de bestandsinhoud zodanig toe dat het document [!DNL Workfront] wordt geüpload naar de opgegeven Google-map.
>
>![](assets/wf-download-document-350x605.png)
>
>Als u echter de naam van het bestand wilt wijzigen, maar de gegevens wilt behouden zoals deze zijn, kunt u de opdracht [!UICONTROL Map] om de bestandsnaam en de bestandsinhoud afzonderlijk toe te wijzen. U voert de volledige bestandsnaam in, inclusief de extensie. Tekstopmaak en binaire indelingen, zoals foto&#39;s, video&#39;s en PDF, worden ondersteund.
>
>![](assets/use-the-map-option-350x358.png)
