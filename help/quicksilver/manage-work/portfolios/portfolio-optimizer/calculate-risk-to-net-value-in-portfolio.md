---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Het risico voor de nettowaarde in een portefeuille berekenen
description: In de Optimizer van het Portfolio, meet de [!UICONTROL Risk to Net Value] indicator het Potentiële Risico rekening houdend met de Netto Waarde die door alle projecten wordt verstrekt die in Optimizer van het Portfolio worden getoond.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 0%

---

# De [!UICONTROL Risk to Net Value] in een portfolio berekenen

In de [!UICONTROL Portfolio Optimizer] -indicator meet de [!UICONTROL Risk to Net Value] -indicator het potentiële risico, rekening houdend met de [!UICONTROL Net Value] -waarde die wordt geboden door alle projecten die in de [!UICONTROL Portfolio Optimizer] -code worden weergegeven. 

Om de meest efficiënte oplossing in het portfolio te bereiken, moet u controleren of de indicator [!UICONTROL Risk] laag is en de indicator [!UICONTROL Net Value] hoog. 

De indicatoren [!UICONTROL Risk] en [!UICONTROL Net Value] worden weergegeven vanuit het perspectief van hun onderlinge relatie.

[!DNL Adobe Workfront] berekent de indicatoren [!UICONTROL Risk] en [!UICONTROL Net Value] met behulp van de volgende formules:

* De indicator [!UICONTROL Risk] wordt berekend met de volgende formule:

  ```
  Risk indicator = Risk / (Risk + Net Value)
  ```

* De indicator [!DNL Net Value] wordt berekend met de volgende formules:

  ```
  Net Value indicator = 1 - Risk / (Risk + Net Value)
  ```

  of

  ```
  Net Value indicator = Net Value / (Risk + Net Value)
  ```

>[!NOTE]
>
>De indicator [!UICONTROL Risk to Net Value] berekent op basis van de projecten die u in [!UICONTROL Portfolio Optimizer] weergeeft en niet op alle projecten die aan het portfolio zijn gekoppeld. 
