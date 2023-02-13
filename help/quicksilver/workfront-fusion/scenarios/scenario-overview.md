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
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] scenario-overzicht

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] vereist een [!DNL Adobe Workfront Fusion] naast een [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>[!DNL Workfront Fusion] scenario&#39;s mogen niet worden verward met [!DNL Workfront Scenario Planner] scenario&#39;s. Voor informatie over [!DNL Workfront Scenario Planner] scenario&#39;s, zie [De [!DNL Scenario Planner] overzicht](../../scenario-planner/scenario-planner-overview.md).

De rol van [!DNL Adobe Workfront Fusion] is om uw processen te automatiseren zodat u zich op nieuwe taken kunt concentreren eerder dan het herhalen van de zelfde taken opnieuw en opnieuw. Het werkt door acties binnen en tussen apps en de diensten te verbinden om een scenario tot stand te brengen dat uw gegevens automatisch overbrengt en transformeert. Het scenario dat u voor gegevens in een app of service maakt, verwerkt die gegevens om het gewenste resultaat te verkrijgen.

Een scenario bestaat uit een reeks modules die aangeven hoe gegevens binnen een app moeten worden getransformeerd of moeten worden overgebracht tussen apps en webservices.

## Voorbeeld: Processen automatiseren binnen [!DNL Adobe Workfront]

>[!NOTE]
>
>Deze functionaliteit is beschikbaar voor de volgende licenties:
>
>* [!UICONTROL [!DNL Workfront Fusion] for Work Automation]
>* [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]
>


[!DNL Workfront Fusion] kunt u eenvoudige of complexe workflows automatiseren binnen [!DNL Workfront], tijd besparen en ervoor zorgen dat het proces consistent wordt uitgevoerd.

In dit voorbeeld wordt het scenario geactiveerd wanneer een opgegeven veld wordt gewijzigd in een taak of probleem in [!DNL Workfront]. Wanneer teweeggebracht, krijgt het scenario informatie in het verwante project en leidt tot een op maat gemaakte update voor een persoon die aan een specifieke rol op het project wordt toegewezen.

![](assets/fusion-template-example-350x102.png)

## Voorbeeld: Verbinding maken [!DNL Workfront] naar een andere app of webservice

>[!NOTE]
>
>Deze functionaliteit is beschikbaar voor de volgende licentie:
>
>* [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]
>


[!DNL Workfront Fusion] kan ook verbinding maken met andere apps en webservices. U kunt gegevens uit andere toepassingen openen, importeren, bewerken of exporteren, en deze integreren met Workfront of met elkaar. Veel toepassingen zijn toegewezen [!DNL Workfront Fusion] connectors. Als er geen specifieke connector is voor de toepassing waartoe u toegang wilt hebben, kunt u [!DNL Workfront Fusion]s [!UICONTROL HTTP] of [!UICONTROL SOAP] modules om met de toepassing door zijn API te verbinden.

In dit voorbeeld wordt het scenario geactiveerd wanneer een gebruiker aan een [!DNL Excel] spreadsheet. Het scenario controleert of de gebruiker binnen is [!DNL Workfront]. Als dat niet het geval is, wordt de gebruiker in het scenario gemaakt [!DNL Workfront] en voegt de Workfront-gebruikersnaam weer toe aan het spreadsheet.

![](assets/fusion-integration-example--350x171.png)

Voor een lijst van specifieke schakelaars, zie [Apps en modules daarvan](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] kan verbinding maken met bijna elke webservice. Als de app waarmee u wilt werken, geen specifieke [!DNL Workfront Fusion] kunt u de volgende modules gebruiken om rechtstreeks verbinding te maken met de webservice:
>
>* [[!UICONTROL HTTP] modules](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP] module](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON] modules](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>

