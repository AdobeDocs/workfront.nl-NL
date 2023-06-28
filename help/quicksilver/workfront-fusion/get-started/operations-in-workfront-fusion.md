---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Bewerkingen in Adobe Workfront Fusion
description: Een bewerking in Adobe Workfront Fusion is een taak die door een module wordt uitgevoerd. Voor het volgen van doeleinden, is om het even welke succesvolle actie die door een module wordt uitgevoerd een verrichting.
author: Becky
feature: Workfront Fusion
source-git-commit: 8d82fd10a6742f13f62b5479fafa5b42e567700f
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Bewerkingen in [!DNL Adobe Workfront Fusion]

Een bewerking in [!DNL Adobe Workfront Fusion] is een taak die door een module wordt uitgevoerd. Voor het volgen van doeleinden, is om het even welke succesvolle actie die door een module wordt uitgevoerd een verrichting.

## Overwegingen bij het tellen van het aantal verrichtingen

* In het algemeen wordt elke succesvolle uitvoering in de stap beschouwd als een bewerking.

* De eerste module in een scenario loopt slechts eenmaal en wordt altijd geteld als één verrichting, zelfs als het geen bundel terugkeert.

* Het aantal keren dat de rest van de gebruikte modules afhangt van het aantal bundels dat zij moeten verwerken.  Één looppas van een module voor één bundel is één verrichting. Een uitzondering hierop is de aggregatormodule, die wordt geteld als één bewerking per set bundels die wordt verwerkt.

* Bewerkingen worden geteld bij de [!UICONTROL Finalization] fase van de uitvoering van een scenario.

* De volgende zijn **niet** geteld als bewerkingen:

   * Alle filterstappen.

   * Elke handeling die fouten of haltes oplevert.

   * Om het even welke route die niet loopt omdat de regels van de route niet werden voldaan, zoals reserve of gehandicapte routes.

   * Om het even welke actie die niet loopt, of omdat een filter geen gegevens door toeliet of omdat het scenario wegens een fout werd gestopt.

## Bedrijfslimieten

Uw organisatie heeft mogelijk een limiet voor maandelijkse bewerkingen. Dit is gebaseerd op de [!DNL Workfront] plan dat uw organisatie heeft aangeschaft. De [!UICONTROL Ultimate] [!DNL Workfront] het plan biedt onbeperkte verrichtingen aan.

Als uw organisatie een maandelijkse limiet heeft, ontvangt u een melding wanneer u de limiet bijna hebt bereikt. Als u de limiet overschrijdt, [!DNL Workfront] zal contact opnemen met uw organisatie om ervoor te zorgen dat uw abonnement aan uw behoeften voldoet.

## Het aantal bewerkingen weergeven dat in de afgelopen 30 dagen is uitgevoerd

U kunt een grafiek zien waarin het aantal uitgevoerde bewerkingen wordt weergegeven. Deze grafieken zijn beschikbaar op de volgende locaties:

* **Organisatie-dashboard**: Door de gehele organisatie gebruikte activiteiten
* **Teamdashboard**: Bewerkingen die worden gebruikt door scenario&#39;s die eigendom zijn van dit team ([!DNL Adobe Experience Cloud] alleen)
* **Detailpagina Scenario**: Bewerkingen die door dit scenario worden gebruikt ([!DNL Adobe Experience Cloud] alleen)

