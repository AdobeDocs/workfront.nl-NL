---
title: De activiteit per teamvisualisatie bekijken in Uitgebreide analyse
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: De activiteit door teamvisualisatie toont activiteiten die tijdens een specifiek tijdkader voor een huisteam gebeuren, toestaand u om te begrijpen hoe de verschillende huisteams hun tijd in Adobe Workfront besteedden. Afhankelijk van de manier waarop uw team in Workfront is ingesteld, kan deze visualisatie u verschillende inzichten geven en verschillende vragen beantwoorden.
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# De activiteit per teamvisualisatie bekijken in Uitgebreide analyse

De activiteit door teamvisualisatie toont activiteiten die tijdens een specifiek tijdkader voor een huisteam gebeuren, toestaand u om te begrijpen hoe de verschillende huisteams hun tijd in Adobe Workfront besteedden. Afhankelijk van de manier waarop uw team in Workfront is ingesteld, kan deze visualisatie u verschillende inzichten geven en verschillende vragen beantwoorden.

>[!NOTE]
>
>De activiteitenvisualisatie van het Project is gelijkaardig aan deze visualisatie, maar het toont activiteit die op mensen wordt gebaseerd die aan projecten eerder dan aan mensen worden toegewezen aan een huisteam wordt toegewezen.\
>Voor informatie over de activiteit van het Project visualisatie, zie [De visualisatie van projectactiviteit weergeven in Verbeterde analyse](../enhanced-analytics/project-activity-overview.md).

![](assets/activity-by-team-350x113.png)

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront-plan</a>*</td> 
   <td> <p>Zakelijk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Overzicht van Adobe Workfront-licenties</a>*</td> 
   <td> <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten weergeven</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt.<br>Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Weergave</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

Voor eerste vereisten voor het gebruik van Enhanced Analytics raadpleegt u de sectie &quot;Voorwaarden&quot; in [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## Begrijp de Activiteit door teamvisualisatie

De verschillende activiteiten worden in verschillende kleuren weergegeven om een overzicht te geven van specifieke gebeurtenissen tijdens de gefilterde periode:

* **Gebruikers aangemeld**: Paarse dozen laten zien dat mensen in het huisteam zich op die dag hebben aangemeld. Een donkerdere tint geeft een groter aantal personen aan die zich aanmelden.

   ![](assets/project-activity-users-logged-in.png)

* **Wijziging taakstatus**: Roze dozen tonen dat de mensen op het huisteam de status van een taak op die dag veranderden. Een donkerdere schaduw geeft aan dat er een groter aantal taakstatussen wordt gewijzigd.

   ![](assets/project-activity-task-status-changes.png)

* **Voltooide taken**: Blauwe dozen laten zien dat mensen in het team van huis die dag een taak hebben voltooid. Een donkerdere schaduw geeft een hoger aantal taken aan die worden voltooid.

   ![](assets/project-activity-tasks-completed.png)

Als u de muisaanwijzer boven een vak houdt, wordt exact aangegeven hoe vaak de handeling op een bepaalde dag is voltooid. U kunt een team selecteren om een onderbreking van deze activiteiten door elke persoon op het huisteam te zien.

Aan de hand van deze informatie kunt u bepalen:

* Welke activiteiten doen zich voor binnen een huisteam en in welk tempo?
* Welke huisteams worden overwerkt of gebruiken meer het systeem.
* Als de distributie van het werk voor het huisteam aangewezen is.

Ga voor meer informatie over de beste gegevens voor deze visualisatie naar [Overzicht van uitgebreide analyses](../enhanced-analytics/enhanced-analytics-overview.md).

## De activiteit per teamvisualisatie weergeven

1. Klik op het pictogram Hoofdmenu ![](assets/main-menu-icon-16x12.png)selecteert u vervolgens **Analyse**.
1. Selecteer in het linkerdeelvenster de optie **Mensen**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Optioneel) Als u een ander datumbereik wilt gebruiken, selecteert u nieuwe begin- en einddatums in het filter voor het datumbereik.

   ![](assets/filters-select-date-range-350x344.png)

   Voor informatie over het gebruik van het filter Datumbereik raadpleegt u [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Voorwaardelijk) als u uw filter van het Team niet hebt geplaatst, voeg de filter van het Team toe en selecteer elk team dat u gegevens voor wilt zien.

   Voor meer informatie over het toevoegen van filters in Verbeterde analysemogelijkheden raadpleegt u [Filters toepassen in uitgebreide analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nadat u filters hebt toegevoegd, worden er gegevens voor maximaal 50 projecten weergegeven en blijven de filters actief, zelfs nadat u de pagina hebt verlaten of zich hebt afgemeld bij Workfront.

1. (Optioneel) Als u wilt inzoomen op een datumbereik, selecteert u een punt in de visualisatie voor het begin van het datumbereik en sleept u naar het einde van het datumbereik.

   Alle andere visualisaties worden bijgewerkt naar hetzelfde datumbereik en er wordt een tijdframefilter gemaakt.

   ![](assets/timeframe-filter-350x220.png)

1. Klik op een teamnaam

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   meer details te zien over de activiteiten die door het team van de woning zijn voltooid.

   De lijst breidt zich uit om de activiteiten van elke persoon te tonen die aan het huisteam wordt toegewezen.

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. Houd de muisaanwijzer boven een gekleurd vak om de datum te zien waarop gebruikers een handeling hebben uitgevoerd en het aantal keren dat de handeling die dag is voltooid.

   Donkere kleuren geven een hogere activiteit aan.

   ![](assets/activity-by-team-activity-pop-up-350x155.png)

1. (Optioneel) Als u de visualisatiegegevens wilt exporteren, klikt u op het pictogram Exporteren ![](assets/export.png) in de rechterbovenhoek van de visualisatie selecteert u de exportindeling:

   * **Diagram (PNG)**
   * **Gegevenstabel (XSLX)**

