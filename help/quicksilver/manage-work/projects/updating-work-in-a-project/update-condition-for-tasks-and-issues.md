---
product-area: projects
navigation-topic: update-work-in-a-project
title: Voorwaarde voor bijwerken voor taken en problemen
description: De voorwaarde van een taak of een kwestie is een vlag die op het wordt geplaatst om erop te wijzen hoe het gaat. Dit is anders dan de status van het werkitem, die de huidige fase van de ontwikkeling van het item aangeeft.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 18dfb67626982d73ad33871b8afce4a3f0d4cdb3
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Voorwaarde voor bijwerken voor taken en problemen

De voorwaarde van een taak of een kwestie is een vlag die op het wordt geplaatst om erop te wijzen hoe het gaat. Dit is anders dan de status van het werkitem, die de huidige fase van de ontwikkeling van het item aangeeft.

U kunt de voorwaarde van een taak of een kwestie of automatisch of manueel plaatsen.

De Adobe Workfront-beheerder kan aangepaste voorwaarden voor uw omgeving maken, zoals beschreven in [Een aangepaste voorwaarde maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)

<!--You can manually update the Condition of a task or issue if you are assigned to it or if you have permissions to it, as described in the [Access requirements](#access-requirements) section of this article.-->

## Toegangsvereisten {#access-requirements}

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td>

Voor de nieuwe vergunningen:
<ul><li><p>Standaard voor taken</p></li>
   <li><p>Medewerker of hoger voor problemen</p></li></ul>


Voor huidige licenties:
<ul><li><p>Werk of hoger voor taken</p></li>
   <li><p>Aanvraag of hoger voor problemen</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten weergeven of vergroten</p> <p>Toegang tot taken en problemen bewerken </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor taken en uitgaven om hun voorwaarde weer te geven</p>
   <p>Machtigingen beheren voor taken en uitgaven om de voorwaarde bij te werken</p>
  </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt. Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## De voorwaarde van taken en problemen opzoeken

De voorwaarden worden weergegeven als een vlag die is gekoppeld aan taken of problemen. Ze kunnen ook worden gekoppeld aan een getal dat in rapporten kan worden weergegeven in plaats van aan het label. Zie voor meer informatie over het koppelen van voorwaarden aan getallen [Een aangepaste voorwaarde maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

U kunt de Voorwaarde van taken en kwesties in rapporten en lijsten de plaats bepalen wanneer u het gebied van de Voorwaarde in een Mening of Groepering toont.

>[!NOTE]
>
>Wanneer het woord &quot;voorwaarde&quot;op het gebied van de Naam van het Gebied van een rapport van de Ingang van het Dagboek toont, wijst dit erop dat de Voorwaarde van een punt werd bijgewerkt. Wanneer het veld Voorwaarde wordt bijgehouden in de rapporten Dagboekvermeldingen, geven de waarden Nieuw en Oud getal het nummer weer dat aan de voorwaarde is gekoppeld in plaats van de naam ervan. Als een voorwaarde oorspronkelijk niet voor een taak of een kwestie wordt bepaald en u het later bijwerkt, zal de dagboekingang die de update vangt de Oude Waarde van het Aantal van het gebied van de Voorwaarde als -2.147.483.648 tonen.

## De voorwaarde automatisch bijwerken door de status bij te werken

Wanneer u een taak of kwestie toewijst en u klikt **eraan werken** , Start Taak of Start Uitgave of werk de status van de taak bij. De voorwaarde van de taak of uitgave wordt automatisch gewijzigd in de standaardvoorwaarde die is gekoppeld aan **Vloeiend**.

Zie de artikelen voor informatie over het gebruik van een aangepaste voorwaarde als een standaardvoorwaarde  [Een aangepaste voorwaarde instellen als standaard voor taken en problemen](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) en [Een aangepaste voorwaarde instellen als standaard voor projecten](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Zie voor informatie over het wijzigen van de taakstatus [Taakstatus bijwerken](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Voor informatie over het wijzigen van de status van de uitgave raadpleegt u [Uitgiftestatus bijwerken](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Voor informatie over het plaatsen van het Werk aan het knoop aan een Taak van het Begin of de knoop van de Uitgave van het Begin, zie [De knop Aan de werkbalk vervangen door de knop Start](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## De voorwaarde handmatig bijwerken

U moet aan een taak of de kwestie worden toegewezen of het hebben leidt toestemmingen aan het om de Voorwaarde op het te kunnen plaatsen.

U kunt de Voorwaarde van een taak of kwestie in een taak of een uitgiftenrapport of een lijst manueel bijwerken wanneer u het gebied van de Voorwaarde in de mening toont.

>[!NOTE]
>
>U kunt het systeem of de groepsbeheerder vragen om het veld Voorwaarde toe te voegen aan het deelvenster Samenvatting, zodat het in verschillende delen van Workfront eenvoudiger wordt om de voorwaarde bij te werken.
>
>Raadpleeg de volgende artikelen voor meer informatie:
>
>* [Overzicht van samenvattingen](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Home en overzicht aanpassen met een lay-outsjabloon](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

De voorwaarde van een taak of een kwestie manueel bijwerken:

1. Ga naar een lijst met taken of problemen waarvoor u beheerdersmachtigingen hebt. Zorg ervoor dat **Voorwaarde** wordt weergegeven in de lijstweergave.

1. Werk de **Voorwaarde** van de kwestie of de taak gealigneerd, door de bestaande voorwaarde te tweemaal te klikken en een nieuwe waarde van het drop-down menu te selecteren.

   ![](assets/condition-drop-down-values-in-task-list.png)

   >[!NOTE]
   >
   >De voorwaarden kunnen voor uw milieu worden aangepast, zodat kunt u meer dan drie opties voor Voorwaarde in uw milieu vinden. De namen van de Voorwaarden kunnen verschillen van de hierboven vermelde. Voor informatie over het aanpassen van Voorwaarden in Workfront raadpleegt u [Een aangepaste voorwaarde maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).


1. Druk **Enter** op uw toetsenbord of klik buiten het veld Voorwaarde om de nieuwe taak of uitgave op te slaan.

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p></li>   
     -->
