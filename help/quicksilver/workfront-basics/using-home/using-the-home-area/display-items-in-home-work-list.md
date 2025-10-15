---
product-area: projects
navigation-topic: use-the-home-area
title: Items weergeven in de [!UICONTROL Worklist] in het begingebied
description: Elke widget bevat een eigen werklijst. De werklijsten tonen alle het werkpunten die aan u worden toegewezen. U kunt bepalen welke items in uw [!UICONTROL worklist] worden weergegeven met behulp van filters en groepen.
author: Courtney
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: 41f58261d4f2e6075187886b371a23eb5e97d823
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# Items weergeven in het [!UICONTROL worklist] gebied in het [!UICONTROL Home] gebied

<!-- Audited: 1/2024 -->

Elke widget bevat een eigen werklijst. De werklijsten tonen alle het werkpunten die aan u worden toegewezen. U kunt bepalen welke items in uw [!UICONTROL worklist] worden weergegeven met behulp van filters en groepen.

>[!IMPORTANT]
>
>* Voor het weergeven van taken en problemen in de Home-widgets moet het bovenliggende project de status Huidig hebben of een status die gelijk is aan de huidige status.
>* Projecten moeten ook de status Huidig hebben of een status die gelijk is aan de huidige status die wordt weergegeven in Home.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie</strong></td> 
   <td><ul><li>[!UICONTROL Contributor] alleen voor goedkeuringen</li> <li>[!UICONTROL Standard] of hoger voor alle andere objecten</li> <p>of</p> 
  </ul><ul><li>[!UICONTROL Review] alleen voor goedkeuringen</li> <li>[!UICONTROL Work] of hoger voor alle andere objecten</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau</strong></td> 
   <td> <p>[!UICONTROL View] of betere toegang tot Projecten, Taken, Kwesties, en Documenten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Contribute-machtigingen of hoger voor de taken en problemen waaraan u moet werken</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten voor werkitems die in de werklijst moeten worden weergegeven

Er zijn ingebouwde vereisten waarvoor de het werkpunten in bepaalde widgetwerklijst tonen. De werkpunten moeten aan deze vereisten voldoen om in de volgende werklijsten van widget te verschijnen.

### Mijn taakwidget

De taken moeten aan de volgende vereisten voldoen om in Mijn widget van Taken te verschijnen:

* De taakstatus komt niet overeen met Voltooid.
* De aangemelde gebruiker moet aan de taak worden toegewezen.
* De taakstatus is niet gelijk aan Gereed.
* Het project de taak tot behoort moet in een status zijn die met Huidig vergelijkt.


### Widget Mijn problemen

De problemen moeten aan de volgende vereisten voldoen om in Mijn Kwesties widget te verschijnen:

* De aangemelde gebruiker moet aan de uitgave worden toegewezen.
* De uitgiftestatus komt niet overeen met Voltooid.
* Er is geen onopgelost object gekoppeld aan het probleem.
* De uitgiftestatus is niet gelijk aan Done.
* Het project tot de kwestie behoort moet in een status zijn die met Huidig vergelijkt.

### Widget Mijn teams

De verzoeken van het team moeten aan de volgende vereisten voldoen om in Mijn widget van Teams te verschijnen:

* De aangemelde gebruiker behoort tot het team waaraan het werkitem is toegewezen.
* De status van het werkitem komt niet overeen met Voltooid.
* Aan het werkitem is geen onopgeloste goedkeuringsprocedure gekoppeld.
* Het het werkpunt is geen terugkomende taak.
* Het project het het werkpunt tot behoort moet in een status zijn die met Huidig vergelijkt.

## Uw werk filteren

U kunt items filteren in de widget [!UICONTROL Worklist] als u alleen bepaalde typen items wilt zien. U kunt bijvoorbeeld het filter Mijn werk [!UICONTROL Worklist] filteren om alleen uitgaven of aanvragen weer te geven.

>[!NOTE]
>
>De filteropties worden opgeslagen in de browser. Als u consequent dezelfde browser gebruikt op dezelfde computer (en de sitegegevens niet wist), veranderen de geselecteerde filters niet. Als u van browser of computer verandert, dan keren de filters aan de standaardoptie terug, die met alle gedeselecteerde filters is.

Uw werk filteren:

1. Klik het **[!UICONTROL Main Menu]** ![ Belangrijkste pictogram van het Menu ](assets/main-menu-icon.png) in de hoger-juiste hoek, dan klik **[!UICONTROL Home]**.
1. (Voorwaardelijk) klik **aanpassen** om het even welke volgende widgets toe te voegen:

   | Widget | Beschrijving |
   |--------------|---------------------------------------------------------------------------------------------------|
   | Borden | Hiermee geeft u alle borden weer die u hebt gemaakt of die u hebt uitgenodigd te gebruiken |
   | Mijn werk | Hiermee geeft u taken en problemen weer die aan u zijn toegewezen |
   | Mijn projecten | De projecten van vertoningen die u hebt of projecten u hebt |
   | Mijn taken | Hiermee geeft u aan u toegewezen taken weer |
   | Mijn problemen | Hier ziet u de problemen die aan u zijn toegewezen |
   | Mijn verzoeken | Alle verzoeken weergeven die u hebt verzonden |
   | Mijn goedkeuring | Toont al uw hangende, toegewezen, gedelegeerde en verzonden goedkeuringen |

1. Klik het **pictogram van de Filter** ![ pictogram van de Filter ](assets/filter-nwepng.png) {in de rechterbovenhoek van widgetwerklijst.
1. Kies a **Voorgesteld** filter of een filter dat u hebt gecreeerd.
Voor gedetailleerde informatie over gesuggereerde filters, zie [ overzicht van widgetfilters van het Huis ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/widget-filter-overview-home.md).
1. (Facultatief) knevel **filters van de Stapel** om veelvoudige filteropties te selecteren.

   ![ Mijn open filter van de Taak ](assets/my-task-filter-open.png)


## Uw werk groeperen

U kunt de widget [!UICONTROL worklist] groeperen om uw werkitems geordend te houden.

Uw werklijst groeperen:

1. Klik het **[!UICONTROL Main Menu]** ![ Belangrijkste pictogram van het Menu ](assets/main-menu-icon.png) in de hoger-juiste hoek, dan klik **[!UICONTROL Home]**.
1. (Voorwaardelijk) klik **aanpassen** om het even welke volgende widgets toe te voegen:

   | Widget | Beschrijving |
   |--------------|---------------------------------------------------------------------------------------------------|
   | Borden | Hiermee geeft u alle borden weer die u hebt gemaakt of die u hebt uitgenodigd te gebruiken |
   | Mijn werk | Hiermee geeft u taken en problemen weer die aan u zijn toegewezen |
   | Mijn projecten | De projecten van vertoningen die u hebt of projecten u hebt |
   | Mijn taken | Hiermee geeft u aan u toegewezen taken weer |
   | Mijn problemen | Hier ziet u de problemen die aan u zijn toegewezen |
   | Mijn verzoeken | Alle verzoeken weergeven die u hebt verzonden |
   | Mijn goedkeuring | Toont al uw hangende, toegewezen, gedelegeerde en verzonden goedkeuringen |

1. Klik het **pictogram van de Groep** ![ van de Groep ](assets/group-icon.png) pictogram van de Groep in de rechterbovenhoek van de widgetwerklijst.
1. Kies a **Voorgestelde** groepering of groepering die u hebt gecreeerd.
   ![ Uitgebreide Groepering ](assets/grouping-expanded.png)


## Kolommen voor werklijsten aanpassen

U kunt kiezen welke kolommen worden weergegeven in de widgetwerklijst:

1. Klik het **[!UICONTROL Main Menu]** ![ Belangrijkste pictogram van het Menu ](assets/main-menu-icon.png) in de hoger-juiste hoek, dan klik **[!UICONTROL Home]**.
1. (Voorwaardelijk) klik **aanpassen** om het even welke volgende widgets toe te voegen:

   | Widget | Beschrijving |
   |--------------|---------------------------------------------------------------------------------------------------|
   | Borden | Hiermee geeft u alle borden weer die u hebt gemaakt of die u hebt uitgenodigd te gebruiken |
   | Mijn werk | Hiermee geeft u taken en problemen weer die aan u zijn toegewezen |
   | Mijn projecten | De projecten van vertoningen die u hebt of projecten u hebt |
   | Mijn taken | Hiermee geeft u aan u toegewezen taken weer |
   | Mijn problemen | Hier ziet u de problemen die aan u zijn toegewezen |
   | Mijn verzoeken | Alle verzoeken weergeven die u hebt verzonden |
   | Mijn goedkeuring | Toont al uw hangende, toegewezen, gedelegeerde en verzonden goedkeuringen |

1. Klik het **pictogram van de Kolom** ![ pictogram van de 1} Kolom {in de rechterbovenhoek van de widgetwerklijst.](assets/column-icon.png)
1. Schakel de kolommen in of uit, afhankelijk van uw voorkeuren.
1. (Facultatief) klik het **pictogram van de Belemmering** ![ pictogram van de Belemmering ](assets/drag-icon.png) om de kolommen opnieuw in orde te brengen.
   ![ Uitgebreide Kolommen ](assets/columns-expanded.png)


## Te late objecten weergeven

[!DNL Adobe Workfront] gebruikt de volgende datums om te bepalen of werkverzoeken te laat zijn:

* **Taken**: [!UICONTROL Planned Completion Date]
* **Kwesties**: [!UICONTROL Planned Completion Date]
* **Documenten**: [!UICONTROL Submitted date]
* **Timesheets**: [!UICONTROL Submitted date]
* **goedkeurt**: [!UICONTROL Submitted date]
* **Goedkeuringen van het Bewijs**: [!UICONTROL Proof deadline]


