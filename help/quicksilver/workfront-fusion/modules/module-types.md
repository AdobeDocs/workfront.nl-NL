---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Typen modules
description: "Adobe Workfront Fusion maakt onderscheid tussen vijf typen modules: actiemodules, zoekmodules, triggermodules, aggregators en iterators. Samenvoegmachines en iterators zijn voor geavanceerde scenario's."
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Typen modules

A[!UICONTROL dobe Workfront Fusion] onderscheidt vijf typen modules: actiemodules, zoekmodules, triggermodules, aggregators en iterators. Samenvoegapparatuur en iterators zijn geschikt voor geavanceerde scenario&#39;s.

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
   <td>Uw organisatie moet Adobe Workfront Fusion en Adobe Workfront aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Actiemodules

Modules van de actie zijn het gemeenschappelijkste type van module. Een typische actiemodule keert één enkele bundel terug, die dan tot de volgende module voor verwerking overgaat.

In tegenstelling tot triggermodules kunnen actiemodules aan het begin, midden of einde van een scenario worden geplaatst. Scenario&#39;s kunnen een onbeperkt aantal actiemodules bevatten.

>[!INFO]
>
>**Voorbeelden:**
>
>* **[!DNL Workfront]>[!UICONTROL Upload a file]** een bestand verzenden naar [!DNL Workfront] en retourneert de id ervan.
>* **[!UICONTROL Image]>[!UICONTROL Resize]** ontvangt een afbeelding, wijzigt de grootte van de afbeelding in de opgegeven afmetingen en geeft de gewijzigde afbeelding door aan de volgende actie.

Het type Handeling heeft vier subtypen: Maken, lezen, bijwerken en verwijderen. Het subtype Update laat de volgende drie verrichtingen toe:

* **De inhoud van een veld wissen**. Deze bewerking vindt plaats wanneer de inhoud van het veld wordt geëvalueerd om het trefwoord te wissen (niet te verwarren met *leeg*).

  ![](assets/erase-content-of-field.png)

* **De inhoud van een veld ongewijzigd laten**. Deze bewerking vindt plaats wanneer het veld leeg blijft of wanneer de inhoud van het veld wordt geëvalueerd naar leeg (weergegeven als null in JSON).

  ![](assets/leave-content-field-unchanged-350x231.png)

* **De inhoud van een veld vervangen**. Deze operatie vindt plaats in alle andere gevallen dan de twee hierboven beschreven gevallen.

>[!NOTE]
>
>* Als u de `erase` in het deelvenster Toewijzing is de module geen updatemodule of is deze niet bijgewerkt naar de meest recente specificaties voor de app.
>* &quot;[!UICONTROL Empty]&quot; wijzigt de inhoud van het veld niet. Als u het veld moet wissen, gebruikt u de volgende formule:
>
>![](assets/formula-ifempty-name-erase.png)
>
>Het is momenteel niet mogelijk een veld ongewijzigd te laten wanneer de inhoud ervan als leeg wordt beschouwd.

## Zoeken in modules

Een typisch Onderzoek keert nul, één, of meerdere bundels terug, die dan tot de volgende module voor verwerking overgaan.

U kunt zoeken aan het begin, midden of einde van een scenario plaatsen.

Scenario&#39;s kunnen een onbeperkt aantal zoekopdrachten bevatten.

>[!INFO]
>
>**Voorbeeld:**
>
>**[!DNL Workfront]>[!UICONTROL Read Related Records]**  leest records die overeenkomen met de zoekquery die u opgeeft, in een bepaald bovenliggend object

## Triggermodules

Triggers genereren bundels wanneer er een wijziging is opgetreden in een bepaalde service. De wijziging kan bestaan uit het maken van nieuwe records, het verwijderen van records, het bijwerken van records, enzovoort.

Elke trigger kan nul, een of meer bundels retourneren die vervolgens worden doorgegeven aan de volgende module voor verwerking.

Triggers kunnen alleen aan het begin van een scenario worden geplaatst.

Elk scenario kan slechts één trekker bevatten.

[!DNL Workfront Fusion] maakt onderscheid tussen twee typen triggers: Opiniepeilingtriggers en Instant-triggers.

### Opiniepeilingtriggers

Opiniepeilingen leiden regelmatig tot opiniepeiling van een bepaalde service, zelfs als er sinds de vorige uitvoering geen wijzigingen zijn aangebracht. Wij adviseren dat u een scenario plant dat een opiniepeilingtrekker bevat om met regelmatige intervallen te lopen. Als er een *wijzigen*, retourneert de trigger bundels met informatie over de wijziging. Als er geen *wijzigen*, voert de trigger geen bundels uit. Voor instructies bij het plannen van een scenario, zie [Een scenario plannen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

Met opiniepeilingtriggers kunt u de eerste bundel selecteren die ze via het deelvenster Epoch moeten uitvoeren. Het deelvenster wordt automatisch weergegeven nadat u een trigger hebt opgeslagen of de triggerinstellingen hebt gewijzigd. Zie voor meer informatie [Kiezen waar een triggermodule begint in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>De instellingen in het deelvenster tijdperk zijn alleen van invloed op de eerste uitvoering van de module. Zodra de module wordt uitgevoerd, onthoudt het de laatste outputbundel en verwijdert het de montages die via het paneel van het tijdperk worden gemaakt.

>[!INFO]
>
>**Voorbeelden:**
>
>* **[!DNL Workfront]>[!UICONTROL Watch records]** retourneert bestanden die nieuw zijn toegevoegd sinds de laatste keer dat het scenario werd uitgevoerd
>
>* **[!DNL Google Sheets]>[!UICONTROL Watch Rows]** retourneert nieuwe rijen die door de gebruiker zijn toegevoegd sinds de laatste keer dat het scenario werd uitgevoerd

### Instant triggers

Met instant triggers kan de service een melding sturen [!DNL Workfront Fusion] over een *wijzigen* onmiddellijk. Wij adviseren dat u een scenario plant dat een onmiddellijke trekker bevat om onmiddellijk te lopen. Zie voor instructies [Een scenario plannen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md). Zie ook [Instant triggers (webhaken) in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) voor details over hoe de inkomende gegevens worden behandeld.

>[!INFO]
>
>**Voorbeelden:**
>
>* **[!DNL Workfront]>[!UICONTROL Watch Events]** retourneert informatie wanneer een bepaald type gebeurtenis plaatsvindt in Workfront, zoals het maken van een taak.
>* **[!DNL Google Sheets]>[!UICONTROL Watch Changes]** geeft informatie weer wanneer een cel wordt bijgewerkt.

## Samenvoegapparatuur

Een aggregator is een type module dat meerdere bundels opneemt tot één bundel.

Elke aggregator keert slechts één bundel terug, die dan tot de volgende module voor verdere verwerking overgaat.

U kunt aggregators slechts in het midden van een scenario plaatsen.

Scenario&#39;s kunnen een onbeperkt aantal aggregators bevatten.

>[!INFO]
>
>**Voorbeelden:**
>
>* **[!UICONTROL Archive]>[!UICONTROL Create an archive]** de ontvangen bestanden comprimeren naar een zip-archief
>* **[!UICONTROL CSV]>[!UICONTROL Aggregate to CSV]** Hiermee worden meerdere tekenreeksen uit een CSV-bestand samengevoegd in één rij
>* **[!UICONTROL Tools]>[!UICONTROL Text aggregator]** combineert meerdere tekenreeksen tot één tekenreeks

Zie voor meer informatie [Samenvoegmodule in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Iteratoren

Een iterator is een type module dat arrays splitst in meerdere afzonderlijke bundels.

Elke iterator keert één of meerdere bundels terug, die dan tot de volgende module voor verwerking overgaan.

U kunt Iterators slechts in het midden van een scenario plaatsen.

Scenario&#39;s kunnen een onbeperkt aantal iterators bevatten.

>[!INFO]
>
>**Voorbeeld:**
>
>**[!UICONTROL Email]>[!UICONTROL Retrieve attachments]** Hiermee wordt een array van bijlagen opgedeeld in afzonderlijke bundels

Zie voor meer informatie [Interventiemodule in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) en [Een array toewijzen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
