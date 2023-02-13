---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Overzicht van typen taakafhankelijkheid
description: De Types van afhankelijkheid verwijzen naar het voorgangersverband tussen taken. Zij bepalen wanneer de afhankelijke taak kan beginnen of eindigen gebaseerd op het begin of het eind van zijn voorganger.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Overzicht van typen taakafhankelijkheid

De Types van afhankelijkheid verwijzen naar het voorgangersverband tussen taken. Zij bepalen wanneer de afhankelijke taak kan beginnen of eindigen gebaseerd op het begin of het eind van zijn voorganger.

>[!IMPORTANT]
>
>Adobe Workfront beperkt niet de afhankelijke taken van aanvang of het beëindigen gebaseerd op de gebiedstypes tenzij de voorgangersverhoudingen worden afgedwongen. Voor informatie over het afdwingen van voorgangers raadpleegt u [Voorgangers afdwingen](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

U moet het Type van Afhankelijkheid van een voorgangersverhouding specificeren wanneer u dit verband tussen uw taken vestigt.

Voor meer informatie over predecessors raadpleegt u [Overzicht van voorgangers van taken](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Hieronder vindt u de Workfront-afhankelijke typen:

* **Voltooien-Begin (fs)**: De voorgaande taak moet zijn voltooid voordat de afhankelijke taak kan worden gestart. Dit is het standaardgebiedstype, dat wordt gebruikt wanneer geen ander gebiedstype wordt gespecificeerd.
* **Voltooien-Voltooien (ff)**: De voorgaande taak moet zijn voltooid voordat de afhankelijke taak kan worden voltooid.
* **Start (ss)**: De voorgangertaak moet beginnen voordat de afhankelijke taak kan worden gestart. U kunt de afhankelijke taak niet starten tenzij de voorganger ten minste is gestart.
* **Start-Finish (sf)**: De voorgangertaak moet beginnen voordat de afhankelijke taak kan worden voltooid. U kunt de afhankelijke taak beginnen alvorens voorganger begint, maar u kunt niet het voltooien tenzij voorganger begon.
* **Gepland-begin (sd)**: Dit plant een taak als Afwerking-Begin, maar het daadwerkelijke handhavingstype is een Afwerking-Afwerking. Wanneer u dit gebruikt, is de afhankelijke taak gepland om te beginnen nadat de voorgangertaak wordt voltooid. Nochtans, maakt de handhaving het zodat kan de afhankelijke taak op om het even welk ogenblik beginnen, maar kan niet beëindigen tot de voorgangerstaak wordt gebeëindigd.
