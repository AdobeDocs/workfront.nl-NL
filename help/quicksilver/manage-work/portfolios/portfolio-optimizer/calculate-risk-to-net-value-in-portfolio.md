---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Het risico voor de nettowaarde in een portefeuille berekenen
description: In de Portfolio Optimizer, [!UICONTROL Risk to Net Value] de indicator meet het Potentiële Risico rekening houdend met de Netto Waarde die door alle projecten wordt verstrekt die in de Optimizer van de Portfolio worden getoond.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 0%

---

# De [!UICONTROL Risk to Net Value] in een portfolio

In de [!UICONTROL Portfolio Optimizer]de [!UICONTROL Risk to Net Value] de indicator meet het potentiële risico, rekening houdend met [!UICONTROL Net Value] verstrekt door alle projecten die in [!UICONTROL Portfolio Optimizer]. 

Om de meest efficiënte oplossing binnen de portfolio te bereiken, wilt u dat de [!UICONTROL Risk] de indicator is laag en de [!UICONTROL Net Value] de indicator is hoog. 

De [!UICONTROL Risk] en [!UICONTROL Net Value] indicatoren worden weergegeven vanuit het perspectief van hun onderlinge relatie.

[!DNL Adobe Workfront] berekent de [!UICONTROL Risk] en [!UICONTROL Net Value] indicatoren met behulp van de volgende formules:

* De [!UICONTROL Risk] de indicator wordt berekend met behulp van de volgende formule:

   ```
   Risk indicator = Risk / (Risk + Net Value)
   ```

* De [!DNL Net Value] de indicator wordt berekend met behulp van de volgende formules:

   ```
   Net Value indicator = 1 - Risk / (Risk + Net Value)
   ```

   of

   ```
   Net Value indicator = Net Value / (Risk + Net Value)
   ```

>[!NOTE]
>
>De [!UICONTROL Risk to Net Value] de indicator berekent gebaseerd op de projecten die u in toont [!UICONTROL Portfolio Optimizer], en niet op alle projecten die met de portefeuille verband houden. 
