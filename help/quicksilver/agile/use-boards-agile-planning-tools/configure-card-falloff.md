---
filename: configure-card-falloff.md
content-type: reference
navigation-topic: boards
title: Wegvallen van kaart configureren
description: U kunt een kaart zodanig configureren dat kaarten volgens een schema worden gearchiveerd of van de kaart worden gehaald.
author: Lisa
feature: Agile
exl-id: 0e4f6b3c-75aa-4314-9cb0-737e5a9d3bda
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 0%

---

# Afvalfunctie van kaart configureren

U kunt een kaart zodanig configureren dat kaarten volgens een schema worden gearchiveerd of &#39;van de kaart vallen&#39;. U kunt kaarten in een bepaalde kolom instellen om over een bepaald aantal dagen of weken van het bord af te vallen.

Wanneer een kaart van het bord valt, wordt deze gearchiveerd. U kunt gearchiveerde kaarten met een filter weergeven. Voor meer informatie, zie [ Filter en onderzoek in een raad ](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> 
   <p>Nieuw: [!UICONTROL Contributor] of hoger</p> 
   <p>of</p>
   <p>Huidig: [!UICONTROL Request] of hoger</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afvalfunctie van kaart configureren

{{step1-to-boards}}

1. Toegang tot een bord. Voor informatie, zie [ creeer of geef een raad ](../../agile/get-started-with-boards/create-edit-board.md) uit.
1. Klik op **[!UICONTROL Configure]** rechts van de board om het deelvenster Configureren te openen.
1. Vouw **[!UICONTROL Cards]** uit.
1. Schakel **[!UICONTROL Automatically archive cards from the board]** in.

   ![ de wegvalmontages van de Kaart ](assets/card-falloff-switch.png)

1. Selecteer wanneer u kaarten van het bord wilt archiveren. U kunt maximaal 8 weken of tot 60 dagen kiezen.

   De datum wordt bepaald vanaf wanneer de kaart voor het laatst is gewijzigd.

1. Selecteer uit welke kolom de kaarten moeten worden verwijderd.
1. Klik op **[!UICONTROL Save]** in het bevestigingsbericht.
1. Klik op **[!UICONTROL Hide configure]** om het deelvenster [!UICONTROL Configure] te sluiten. De configuratie-instellingen worden automatisch toegepast wanneer u de kaart vernieuwt.
