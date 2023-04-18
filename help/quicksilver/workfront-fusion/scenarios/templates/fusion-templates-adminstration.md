---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion Templates-beheer
description: Als beheerder hebt u toestemming om sjablonen die door anderen zijn gemaakt, weer te geven, te wijzigen, te hernoemen, te publiceren, goed te keuren en te verwijderen. U kunt deze handelingen uitvoeren via het dialoogvenster [!UICONTROL Templates] pagina in de [!DNL Adobe Workfront Fusion Administration] gebied.
author: Becky
feature: Workfront Fusion
exl-id: 63c14183-0d22-44f3-87e5-c311cfbf5540
source-git-commit: bcca026e193e66cfb92ab9a0fb1aaf1eeb6892fb
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Sjabloonbeheer

Als beheerder hebt u toestemming om sjablonen die door anderen zijn gemaakt, weer te geven, te wijzigen, te hernoemen, te publiceren, goed te keuren en te verwijderen. U kunt deze handelingen uitvoeren via het dialoogvenster [!UICONTROL Templates] pagina in de [!DNL Adobe Workfront Fusion Administration] gebied.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] of hoger</p> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licentie**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p><p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>U moet een Workfront Fusion-beheerder zijn voor uw organisatie.</p> </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Weergave [!DNL Workfront Fusion] sjablonen als beheerder

Een tabel weergeven met alle gemaakte sjablonen en de bijbehorende statussen:

1. Klikken **[!UICONTROL Administration]** in het linkernavigatievenster om het dialoogvenster [!UICONTROL Administration] gebied.
1. Klikken **[!UICONTROL Templates]** in het linkernavigatievenster.

Er zijn drie kolommen met betrekking tot de publicatiestatus van sjablonen. Een vinkje in een kolom geeft het volgende aan:

* **[!UICONTROL Published]**: Deze sjablonen zijn momenteel zichtbaar in het dialoogvenster [!UICONTROL Team templates] in de gebruikersinterface.
* **[!UICONTROL Requested approval]**: Deze templates wachten op goedkeuring. Ze zijn momenteel zichtbaar in het dialoogvenster [!UICONTROL Team templates] in de gebruikersinterface.
* **[!UICONTROL Approved]**: Deze sjablonen zijn goedgekeurd. Ze zijn momenteel zichtbaar in het dialoogvenster [!UICONTROL Public templates] in de standaardgebruikersinterface.

>[!NOTE]
>
>Sjablonen met het vinkje in het dialoogvenster [!UICONTROL Requested approval] en in de [!UICONTROL Approved] de kolom is reeds goedgekeurd en openbaar gemaakt, maar er is een nieuwere versie van hen die op uw goedkeuring wachten.

## Bewerken [!DNL Workfront Fusion] sjablonen als beheerder

1. Klikken **[!UICONTROL Administration]** in het linkernavigatievenster om het dialoogvenster [!UICONTROL Administration] gebied.
1. Klikken **[!UICONTROL Templates]** in het linkernavigatievenster.
1. Klikken **[!UICONTROL Detail]** rechts van de sjabloon die u wilt bewerken.

U kunt de sjabloon nu bewerken, net als een sjabloon bewerken als een gebruiker die geen beheerder is. In de [!UICONTROL Options] in de rechterbovenhoek, is er één extra optie - het diagram van de SVG dat u van de code van de SVG voorziet. Bovendien is het publicatieproces hetzelfde als in het geval van een standaardgebruiker. Raadpleeg de sectie Publishing and sharing templates voor meer informatie.

Voor informatie over specifieke sjabloonopties die u kunt bewerken, raadpleegt u [Nieuwe sjablonen maken in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md).

Voor informatie over het publiceren van sjablonen raadpleegt u [Publiceren en delen [!DNL Adobe Workfront Fusion] sjablonen](../../../workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

## Goedkeuren of afwijzen [!DNL Workfront Fusion] sjablonen

Als u een sjabloon goedkeurt, wordt deze zichtbaar in het dialoogvenster [!UICONTROL Public templates] en beschikbaar voor alle gebruikers. Als u een sjabloon weigert, wordt deze verwijderd uit de [!UICONTROL Public templates] en stelt het ter beschikking slechts aan het team dat het creeerde.

1. Klikken **[!UICONTROL Administration]** in het linkernavigatievenster om het dialoogvenster [!UICONTROL Administration] gebied.
1. Klikken **[!UICONTROL Templates]** in het linkernavigatievenster.
1. Als u een sjabloon wilt goedkeuren, klikt u op **[!UICONTROL Approve]** rechts van de sjabloon.
1. Als u een sjabloon wilt weigeren, klikt u op **[!UICONTROL Disapprove]** rechts van de sjabloon.

>[!NOTE]
>
>Als u de sjabloon goedkeurt die eerder is goedgekeurd en vervolgens is bewerkt, wordt de oorspronkelijke sjabloon overschreven door uw tweede goedkeuring.

## Een scenario klonen als een sjabloon

Als beheerder, hebt u de capaciteit om een scenario als malplaatje te klonen.

Voor instructies over het klonen van een scenario als malplaatje, zie [Een sjabloon maken op basis van een scenario](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md#create-a-template-from-a-scenario) in [Nieuwe sjablonen maken in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/templates/create-new-fusion-templates.md)
