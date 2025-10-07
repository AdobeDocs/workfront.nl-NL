---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Een dashboard toevoegen in het linkerdeelvenster van een Workfront-object of -gebied
description: De informatie u in de  [!DNL Workfront]  Webtoepassing ziet wordt vaak getoond in de secties in het linkerpaneel door gebrek. Elke sectie bevat verschillende informatie over a  [!DNL Workfront]  gebied of voorwerp.
author: Becky and Lisa
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 0efbc6051443d8e0ed96512b72d0949b288f7c2d
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---

# Een dashboard toevoegen in het linkerdeelvenster van een Workfront-object of -gebied

## [!DNL Adobe Workfront] secties

De informatie die u in de [!DNL Workfront] webtoepassing ziet, wordt standaard vaak in de linkerdeelvensters weergegeven. Elke sectie bevat verschillende informatie over een [!DNL Workfront] -gebied of -object.

Voor meer informatie over de standaardgebieden van [!DNL Workfront], zie het artikel [&#x200B; Ongeveer de standaard  [!DNL Adobe Workfront]  lay-out &#x200B;](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Naast de secties die standaard bij [!DNL Workfront] worden geleverd, kunt u een dashboard toevoegen waarop u informatie kunt weergeven die relevant is voor uw workflow. U kunt geen dashboard toevoegen aan alle gebieden en objecten.

In de volgende tabel worden alle [!DNL Workfront] -gebieden en -objecten weergegeven die secties in het linkerdeelvenster bevatten en die met een dashboard kunnen worden aangepast:

| **[!DNL Workfront]gebied of object** | **Standaard systeemsecties** | **Dashboards** |
|---|---|---|
| [!UICONTROL Projects] -gebied | ✓ | ✓ |
| [!UICONTROL Team] | ✓ |   |
| [!UICONTROL Requests] -gebied | ✓ |   |
| [!UICONTROL Timesheets] -gebied | ✓ |   |
| [!UICONTROL Portfolio] | ✓ | ✓ |
| [!UICONTROL Program] | ✓ | ✓ |
| [!UICONTROL Project] | ✓ | ✓ |
| [!UICONTROL Task] | ✓ |  ✓ |
| [!UICONTROL Issue] |  ✓ |  ✓ |
| [!UICONTROL User] |  ✓ |  ✓ |
| [!UICONTROL Document] |  ✓ |  ✓ |
| [!UICONTROL Resourcing] -gebied | ✓ | ✓ |

{style="table-layout:auto"}

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td>[!UICONTROL Reviewer] of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>Toegang tot het objecttype weergeven</td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan of vergunningstype u hebt, contacteer uw [!DNL Workfront] beheerder.

## Een dashboard toevoegen in het linkerdeelvenster van een [!DNL Workfront] -object of -gebied

Voordat u een dashboard kunt toevoegen, moet u het dashboard maken met alle informatie die u op het wilt weergeven. U kunt ook een externe pagina maken.

Voor meer informatie over de bouw van dashboards, zie het artikel [&#x200B; een dashboard &#x200B;](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md) creëren.

Voor meer informatie over de bouw van externe pagina&#39;s, zie het artikel [&#x200B; een externe Web-pagina in een dashboard &#x200B;](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md) inbedden.

Nadat u het dashboard of de externe pagina hebt gemaakt, kunt u deze aan het linkerdeelvenster toevoegen.

1. Ga naar een van de [!DNL Workfront] -gebieden of -objecten waar u een dashboard kunt toevoegen in het linkerdeelvenster.

   Voor meer informatie over welke gebieden en voorwerpen u dashboards aan kunt toevoegen, zie [[!DNL Adobe Workfront]  secties &#x200B;](#adobe-workfront-sections).

1. Klik op **[!UICONTROL Add a Dashboard]** in het linkerdeelvenster.
1. Typ een naam voor het dashboard in het veld **[!UICONTROL Quick link name]** . Dit is alleen voor u zichtbaar.
1. Typ de naam van een bestaand dashboard of een externe pagina in het veld **[!UICONTROL Choose a dashboard]** en selecteer vervolgens het dashboard wanneer dit in de lijst wordt weergegeven.
1. Klik op **[!UICONTROL Add]**.
1. (Optioneel) Sleep de secties in de volgorde waarin u ze wilt weergeven.

   De bovenste sectie is de standaardsectie voor de pagina.

   De dashboards die u hebt toegevoegd, zijn alleen voor u beschikbaar.

## De dashboards van de vertoning in het linkerpaneel van voorwerpen

Zie de sectie [[!UICONTROL Add a dashboard] in het linkerdeelvenster van een Workfront-object of -gebied &#x200B;](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) in dit artikel voor meer informatie over het toevoegen van een dashboard onder een object.

Wanneer u een dashboard toevoegt aan het linkerpaneel van een voorwerp, dienst het voorwerp als filter voor het dashboard. Bijvoorbeeld, als u een taakrapport op een dashboard toevoegt en u het dashboard aan een project toevoegt, toont het dashboard slechts taken van het project u bekijkt.

De volgende objecten worden gefilterd voor het object waaronder ze worden weergegeven, als dat object in de hiërarchie hoger is dan ze:

* Project
* Taak
* Probleem
* Goedkeuringsproces
* Opmerking
* Document

Voor meer informatie over de hiërarchie en de onderlinge afhankelijkheid van voorwerpen, zie de sectie [&#x200B; Interdependentie en hiërarchie van voorwerpen &#x200B;](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) in het artikel [&#x200B; voorwerpen in Adobe Workfront &#x200B;](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) begrijpen.

## Het linkerdeelvenster in een lay-outsjabloon aanpassen

Wanneer u dashboards aan uw [!DNL Workfront] instantie toevoegt, zijn zij slechts zichtbaar aan u.

Alleen een systeem- of groepsbeheerder kan dashboards delen met andere gebruikers in een lay-outsjabloon. Voor meer informatie over het aanpassen van het linkerpaneel met een lay-outmalplaatje, zie [&#x200B; het linkerpaneel aanpassen gebruikend een lay-outmalplaatje &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
