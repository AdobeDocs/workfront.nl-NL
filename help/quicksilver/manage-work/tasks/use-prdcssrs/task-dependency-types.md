---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Overzicht van de Types van Afhankelijkheid van de Taak
description: De Types van afhankelijkheid verwijzen naar het voorgangersverband tussen taken. Zij bepalen wanneer de afhankelijke taak kan beginnen of eindigen gebaseerd op het begin of het eind van zijn voorganger.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Overzicht van typen taakafhankelijkheid

<!-- Audited: 12/2023 -->

De Types van afhankelijkheid verwijzen naar het voorgangersverband tussen taken. Zij bepalen wanneer de afhankelijke taak kan beginnen of eindigen gebaseerd op het begin of het eind van zijn voorganger.

>[!IMPORTANT]
>
>Adobe Workfront beperkt niet de afhankelijke taken van aanvang of het beëindigen gebaseerd op de gebiedstypes tenzij de voorgangersverhoudingen worden afgedwongen. Voor informatie over het afdwingen van predecessors, zie [ predecessors ](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md) afdwingen.

U moet het Type van Afhankelijkheid van een voorgangersverhouding specificeren wanneer u dit verband tussen uw taken vestigt.

Voor meer informatie over predecessors, zie [ Overzicht van taakvoordecessors ](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Hieronder vindt u de Workfront-afhankelijke typen:

* **eind-Begin (fs)**: De voorgangerstaak moet beëindigen alvorens de afhankelijke taak kan beginnen. Dit is het standaardgebiedstype, dat wordt gebruikt wanneer geen ander gebiedstype wordt gespecificeerd.
* **afwerking-Afwerking (ff)**: De voorgangerstaak moet beëindigen alvorens de afhankelijke taak kan beëindigen.
* **Begin-Begin (s)**: De voorgangertaak moet beginnen alvorens de afhankelijke taak kan beginnen. U kunt de afhankelijke taak niet starten tenzij de voorganger ten minste is gestart.
* **begin-Afwerking (sf)**: De voorgangertaak moet beginnen alvorens de afhankelijke taak kan beëindigen. U kunt de afhankelijke taak beginnen alvorens voorganger begint, maar u kunt niet het voltooien tenzij voorganger begon.
* **Gepland-Begin (sd)**: Dit plant een taak als Voltooien-Begin, maar het daadwerkelijke handhavingstype is een Finish-Finish. Wanneer u dit gebruikt, is de afhankelijke taak gepland om te beginnen nadat de voorgangertaak wordt voltooid. Nochtans, maakt de handhaving het zodat kan de afhankelijke taak op om het even welk ogenblik beginnen, maar kan niet beëindigen tot de voorgangerstaak wordt gebeëindigd.

>[!NOTE]
>
>De afkortingen voor de Types van Afhankelijkheid worden gebruikt in taaklijsten om voorgangersverhoudingen te bepalen. Voor meer informatie, zie [ Voorbeelden van voorgangerswaarden in een taaklijst ](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list) in [ Overzicht van taakvoorgangers ](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md).

