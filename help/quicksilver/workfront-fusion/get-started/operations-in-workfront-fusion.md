---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Bewerkingen in Adobe Workfront Fusion
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 34268fb6-e485-42be-b751-3ee79bbf5797
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Bewerkingen in [!DNL Adobe Workfront Fusion]



>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ Verrichtingen ](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/operations-in-workfront-fusion.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

Een bewerking in [!DNL Adobe Workfront Fusion] is een taak die door een module wordt uitgevoerd. Voor het volgen van doeleinden, is om het even welke succesvolle actie die door een module wordt uitgevoerd een verrichting.

## Overwegingen bij het tellen van het aantal verrichtingen

* In het algemeen wordt elke succesvolle uitvoering in de stap beschouwd als een bewerking.

* De eerste module in een scenario loopt slechts eenmaal en wordt altijd geteld als één verrichting, zelfs als het geen bundel terugkeert.

* Het aantal keren dat de rest van de gebruikte modules afhangt van het aantal bundels dat zij moeten verwerken.  Één looppas van een module voor één bundel is één verrichting. Een uitzondering hierop is de aggregatormodule, die wordt geteld als één bewerking per set bundels die wordt verwerkt.

* Bewerkingen worden meegeteld in het [!UICONTROL Finalization] -werkgebied van de uitvoering van een scenario.

* Het volgende wordt **niet** geteld als verrichtingen:

   * Alle filterstappen.

   * Elke handeling die fouten of haltes oplevert.

   * Om het even welke route die niet loopt omdat de regels van de route niet werden voldaan, zoals reserve of gehandicapte routes.

   * Om het even welke actie die niet loopt, of omdat een filter geen gegevens door toeliet of omdat het scenario wegens een fout werd gestopt.

## Bedrijfslimieten

Uw organisatie heeft mogelijk een limiet voor maandelijkse bewerkingen. Dit is gebaseerd op het [!DNL Workfront] -abonnement dat uw organisatie heeft aangeschaft. Het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement biedt onbeperkte bewerkingen.

Als uw organisatie een maandelijkse limiet heeft, ontvangt u een melding wanneer u de limiet bijna hebt bereikt. Als u de limiet overschrijdt, neemt [!DNL Workfront] contact op met uw organisatie om ervoor te zorgen dat uw abonnement aan uw behoeften voldoet.

## Het aantal bewerkingen weergeven dat in de afgelopen 30 dagen is uitgevoerd

U kunt een grafiek zien waarin het aantal uitgevoerde bewerkingen wordt weergegeven. Deze grafieken zijn beschikbaar op de volgende locaties:

* **dashboard van de Organisatie**: Verrichtingen die door de volledige organisatie worden gebruikt
* **dashboard van het Team**: Verrichtingen die door scenario&#39;s worden gebruikt die door dit team ([!DNL Adobe Experience Cloud] slechts) worden bezeten
* **de detailspagina van het Scenario**: Verrichtingen die door dit scenario worden gebruikt ([!DNL Adobe Experience Cloud] slechts)
