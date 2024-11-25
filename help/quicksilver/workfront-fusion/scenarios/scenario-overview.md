---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Overzicht van Adobe Workfront Fusion-scenario
description: Adobe Workfront Fusion vereist naast een Adobe Workfront-licentie een Adobe Workfront Fusion-licentie.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: f8ea4a1c40cd3fc4664a5a3b1c3a900e874d78b1
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] scenario-overzicht

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] vereist een [!DNL Adobe Workfront Fusion] licentie naast een [!DNL Adobe Workfront license] .

>[!IMPORTANT]
>
>[!DNL Workfront Fusion] -scenario&#39;s mogen niet worden verward met [!DNL Workfront Scenario Planner] -scenario&#39;s. Voor informatie over [!DNL Workfront Scenario Planner] scenario&#39;s, zie [ het  [!DNL Scenario Planner]  overzicht ](../../scenario-planner/scenario-planner-overview.md).

De rol van [!DNL Adobe Workfront Fusion] is om uw processen te automatiseren zodat u zich op nieuwe taken kunt concentreren eerder dan het herhalen van de zelfde taken opnieuw en opnieuw. Het werkt door acties binnen en tussen apps en de diensten te verbinden om een scenario tot stand te brengen dat uw gegevens automatisch overbrengt en transformeert. Het scenario dat u voor gegevens in een app of service maakt, verwerkt die gegevens om het gewenste resultaat te verkrijgen.

Een scenario bestaat uit een reeks modules die aangeven hoe gegevens binnen een app moeten worden getransformeerd of moeten worden overgebracht tussen apps en webservices.

## Overzicht van Scenario-elementen

Een scenario is gebouwd van verschillende elementen. Door de terminologie van deze elementen te begrijpen, is het gemakkelijker om de documentatie te gebruiken.

### Scenario

A **scenario** is een user-created reeks geautomatiseerde stappen, die worden gecreeerd om gegevens te bewegen en te manipuleren. De term &quot;scenario&quot; verwijst naar de gehele groep van verbonden stappen.

![ Scenario ](assets/entire-scenario-scenario.png)

### Trigger

Een scenario begint met a **trekker**. De trekkerstalen voor nieuwe en bijgewerkte gegevens, en beginnen het scenario wanneer bepaalde die voorwaarden in de module worden gevormd van toepassing zijn. Triggers kunnen worden gevormd om een scenario op een programma (opiniepeiling) te beginnen, of wanneer de gegevensveranderingen (onmiddellijk) voorkomen.

![ Trekker ](assets/scenario-trigger.png)

### Module

De trekker wordt gevolgd door een aantal **modules**. Een module vertegenwoordigt één enkele stap in een scenario dat een specifieke actie uitvoert. De modules worden gevormd en samen geketend om scenario&#39;s tot stand te brengen.

![ Module ](assets/scenario-module.png)

### Route

Een scenario kan in **routes** worden verdeeld. Een route is een sectie van het scenario dat voor een bepaalde bundel van gegevens kan of niet kan worden gebruikt. Routes worden opstelling gebruikend een routermodule en filters.

![ Route ](assets/scenario-route.png)

### Scenario-segment

Een scenario segment is een sectie van een scenario dat uit een reeks aangrenzende modules bestaat die allen met de zelfde toepassing verbinden. Scenario-segmenten vertegenwoordigen vaak een korte workflow in de toepassing.

![ segment Scenario ](assets/scenario-segment.png)

### Connector

Een schakelaar is de reeks modules voor een bepaalde toepassing. Workfront Fusion biedt connectors aan voor veel gangbare werktoepassingen, zoals Workfront, Salesforce en Jira, en generieke connectors die voor elke webservice kunnen worden gebruikt.

![ Schakelaars ](assets/scenario-connectors.png)



## Voorbeeld: Processen automatiseren binnen [!DNL Adobe Workfront]

>[!NOTE]
>
>Deze functionaliteit is beschikbaar voor de volgende licenties:
>
>* [!UICONTROL [!DNL Workfront Fusion] for Work Automation]
>* [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]

Met [!DNL Workfront Fusion] kunt u eenvoudige of complexe workflows automatiseren binnen [!DNL Workfront] , zodat u tijd bespaart en ervoor zorgt dat het proces consistent wordt uitgevoerd.

In dit voorbeeld wordt het scenario geactiveerd wanneer een opgegeven veld in een taak of probleem in [!DNL Workfront] verandert. Wanneer teweeggebracht, krijgt het scenario informatie in het verwante project en leidt tot een op maat gemaakte update voor een persoon die aan een specifieke rol op het project wordt toegewezen.

![](assets/fusion-template-example-350x102.png)

## Voorbeeld: [!DNL Workfront] verbinden met een andere app of webservice

>[!NOTE]
>
>Deze functionaliteit is beschikbaar voor de volgende licentie:
>
>* [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]
>

[!DNL Workfront Fusion] kan ook verbinding maken met andere apps en webservices. U kunt gegevens uit andere toepassingen openen, importeren, bewerken of exporteren, en deze integreren met Workfront of met elkaar. Veel toepassingen hebben toegewezen [!DNL Workfront Fusion] -connectors. Als er geen specifieke connector is voor de toepassing waartoe u toegang wilt hebben, kunt u de modules [!UICONTROL HTTP] of [!UICONTROL SOAP] van [!DNL Workfront Fusion] gebruiken om via de API verbinding met de toepassing te maken.

In dit voorbeeld wordt het scenario geactiveerd wanneer een gebruiker aan een [!DNL Excel] -spreadsheet wordt toegevoegd. Het scenario controleert of de gebruiker zich in [!DNL Workfront] bevindt. Als dat niet het geval is, wordt de gebruiker in [!DNL Workfront] gemaakt en wordt de Workfront-gebruikersnaam weer aan het werkblad toegevoegd.

![](assets/fusion-integration-example--350x171.png)

Voor een lijst van specifieke schakelaars, zie [ Apps en hun modules ](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] kan verbinding maken met vrijwel elke webservice. Als de app waarmee u wilt werken geen toegewezen [!DNL Workfront Fusion] -connector heeft, kunt u de volgende modules gebruiken om rechtstreeks verbinding te maken met de webservice:
>
>* [[!UICONTROL HTTP] modules ](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP] module ](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON] modules ](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>
