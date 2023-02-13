---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Aangepaste secties maken
description: De informatie die u in de [!DNL Workfront] De webtoepassing wordt standaard vaak weergegeven in de secties in het linkerdeelvenster. Elke sectie bevat verschillende informatie over een [!DNL Workfront] gebied of object.
author: Lisa
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# Aangepaste secties maken

## [!DNL Adobe Workfront] secties

De informatie die u in de [!DNL Workfront] De webtoepassing wordt standaard vaak weergegeven in de secties van het linkerdeelvenster. Elke sectie bevat verschillende informatie over een [!DNL Workfront] gebied of object.\
Voor meer informatie over de standaardgebieden van [!DNL Workfront], zie het artikel [De standaardinstelling [!DNL Adobe Workfront] layout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Naast de secties die bij [!DNL Workfront] standaard kunt u een dashboard toevoegen waarop u informatie kunt weergeven die relevant is voor uw workflow. U kunt geen dashboard toevoegen aan alle gebieden en objecten.

In de volgende tabel worden alle [!DNL Workfront] gebieden en objecten die secties in het linkerdeelvenster bevatten en die kunnen worden aangepast:

| **[!DNL Workfront]gebied of object** | **Standaardsysteemsecties** | **Aangepaste secties** |
|---|---|---|
| [!UICONTROL Projects] gebied | ✓ | ✓ |
| [!UICONTROL Team] | ✓ |   |
| [!UICONTROL Requests] gebied | ✓ |   |
| [!UICONTROL Timesheets] gebied | ✓ |   |
| [!UICONTROL Portfolio] | ✓ | ✓ |
| [!UICONTROL Program] | ✓ | ✓ |
| [!UICONTROL Project] | ✓ | ✓ |
| [!UICONTROL Task] | ✓ |  ✓ |
| [!UICONTROL Issue] |  ✓ |  ✓ |
| [!UICONTROL User] |  ✓ |  ✓ |
| [!UICONTROL Document] |  ✓ |  ✓ |

{style=&quot;table-layout:auto&quot;}

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td>[!UICONTROL Reviewer] of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td>Toegang tot het objecttype weergeven</td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Een dashboard toevoegen in het linkerdeelvenster van een [!DNL Workfront] object of gebied

Voordat u een dashboard kunt toevoegen, moet u het dashboard maken met alle informatie die u op het wilt weergeven. U kunt ook een externe pagina maken.\
Raadpleeg het artikel voor meer informatie over het maken van dashboards [Een dashboard maken](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
Raadpleeg het artikel voor meer informatie over het maken van externe pagina&#39;s [Een externe webpagina insluiten in een dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

Nadat u het dashboard of de externe pagina hebt gemaakt, kunt u deze toevoegen aan het linkerdeelvenster.

1. Ga naar een van de [!DNL Workfront] gebieden of objecten waar u een aangepaste sectie kunt toevoegen in het linkerdeelvenster.\
   of
1. Ga naar een object waar u een [!UICONTROL dashboard] in het linkerdeelvenster.\
   Ga voor meer informatie over welke gebieden en objecten u aangepaste secties kunt toevoegen [[!DNL Adobe Workfront] secties](#adobe-workfront-sections).
1. Klikken **[!UICONTROL Add dashboard]** in het linkerdeelvenster.
1. Typ een naam voor het dashboard in het dialoogvenster **[!UICONTROL Quick link name]** veld. Dit is alleen voor u zichtbaar.
1. Typ de naam van een bestaand dashboard of een externe pagina in het dialoogvenster **[!UICONTROL Choose a dashboard]** selecteert u het dashboard wanneer het in de lijst wordt weergegeven.
1. Klik op **[!UICONTROL Add]**.
1. (Optioneel) Sleep de secties in de volgorde waarin u ze wilt weergeven.

   De bovenste sectie is de standaardsectie voor de pagina.

   De secties die u voor afzonderlijke objecten hebt gemaakt, worden weergegeven wanneer u toegang hebt tot alle objecten van hetzelfde type en deze alleen voor u beschikbaar zijn.

## De dashboards van de vertoning in het linkerpaneel van voorwerpen

Zie de sectie voor meer informatie over het toevoegen van een dashboard onder een object [[!UICONTROL Add a dashboard] in het linkerdeelvenster van een Workfront-object of -gebied](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) in dit artikel.

Wanneer u een dashboard toevoegt aan een aangepaste sectie onder een object, fungeert het object als een filter voor het dashboard. Bijvoorbeeld, als u een taakrapport op een dashboard toevoegt en u het dashboard aan een project toevoegt, toont de douanesectie die het dashboard op het project bevat slechts taken op het project u bekijkt.

De volgende objecten worden gefilterd voor het object waaronder ze worden weergegeven, als dat object in de hiërarchie hoger is dan ze:

* Project
* Taak
* Probleem
* Goedkeuringsproces
* Opmerking
* Document

Zie de sectie voor meer informatie over de hiërarchie en de onderlinge afhankelijkheid van objecten [Interdependentie en hiërarchie van objecten](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) in het artikel [Objecten in Adobe Workfront begrijpen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Het linkerdeelvenster in een lay-outsjabloon aanpassen

Wanneer u dashboards aan uw [!DNL Workfront] zijn alleen zichtbaar voor u.

U kunt de secties in [!DNL Workfront] en deel de nieuwe lay-out met verscheidene gebruikers in een lay-outmalplaatje. Alleen een systeem- of groepsbeheerder kan deze delen met andere gebruikers in een lay-outsjabloon. Voor meer informatie over het aanpassen van het linkerpaneel met een lay-outmalplaatje, zie [Het linkerdeelvenster aanpassen met een lay-outsjabloon](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
