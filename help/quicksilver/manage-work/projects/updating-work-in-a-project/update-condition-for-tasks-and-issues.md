---
product-area: projects
navigation-topic: update-work-in-a-project
title: Voorwaarde voor bijwerken voor taken en problemen
description: De voorwaarde van een taak of een kwestie is een vlag die op het wordt geplaatst om erop te wijzen hoe het gaat. Dit is anders dan de status van het werkitem, die de huidige fase van de ontwikkeling van het item aangeeft.
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 0%

---

# Voorwaarde voor bijwerken voor taken en problemen

De voorwaarde van een taak of een kwestie is een vlag die op het wordt geplaatst om erop te wijzen hoe het gaat. Dit is anders dan de status van het werkitem, die de huidige fase van de ontwikkeling van het item aangeeft.

U kunt de voorwaarde van een taak of een kwestie of automatisch of manueel plaatsen.

De Adobe Workfront-beheerder kan aangepaste voorwaarden voor uw omgeving maken, zoals beschreven in [Een aangepaste voorwaarde maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)

<!--You can manually update the Condition of a task or issue if you are assigned to it or if you have permissions to it, as described in the [Access requirements](#access-requirements) section of this article.-->

## Toegangsvereisten {#access-requirements}

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the current licenses:
   <ul><li><p>Standard for tasks</p></li>
   <li><p>Contributor or higher for issues</p></li></ul>


   For legacy licenses:
   <ul><li><p>Work or higher for tasks</p></li>
   <li><p>Request or higher for issues</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
    <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Werk of hoger voor taken</p>
   <p>Aanvraag of hoger voor problemen</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten weergeven of vergroten</p> <p>Toegang tot taken en problemen bewerken </p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor taken en uitgaven om hun voorwaarde weer te geven</p>
   <p>Machtigingen beheren voor taken en uitgaven om de voorwaarde bij te werken</p>
    <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## De voorwaarde van taken en problemen opzoeken

De voorwaarden worden weergegeven als een vlag die is gekoppeld aan taken of problemen. Ze kunnen ook worden gekoppeld aan een getal dat in rapporten kan worden weergegeven in plaats van aan het label. Zie voor meer informatie over het koppelen van voorwaarden aan getallen [Een aangepaste voorwaarde maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

U kunt de voorwaarde van taken en kwesties op de volgende gebieden de plaats bepalen:

* Het gebied van de Updates van de taak en van de kwestie, binnen van een update, wanneer u aan de taak of de kwestie wordt toegewezen.
* Hiermee worden rapporten en lijsten weergegeven wanneer u het veld Voorwaarde weergeeft in een weergave of Groepering.

>[!NOTE]
>
>Wanneer het woord &quot;voorwaarde&quot;op het gebied van de Naam van het Gebied van een rapport van de Ingang van het Dagboek toont, wijst dit erop dat de Voorwaarde van een punt werd bijgewerkt. Wanneer het veld Voorwaarde wordt bijgehouden in de rapporten Dagboekvermeldingen, geven de waarden Nieuw en Oud getal het nummer weer dat aan de voorwaarde is gekoppeld in plaats van de naam ervan. Als een voorwaarde oorspronkelijk niet voor een taak of een kwestie wordt bepaald en u het later bijwerkt, zal de dagboekingang die de update vangt de Oude Waarde van het Aantal van het gebied van de Voorwaarde als -2.147.483.648 tonen.

## De voorwaarde automatisch bijwerken door de status bij te werken

Wanneer u een taak of kwestie toewijst en u klikt **eraan werken** , Start Taak of Start Uitgave of werk de status van de taak bij. De voorwaarde van de taak of uitgave wordt automatisch gewijzigd in de standaardvoorwaarde die is gekoppeld aan **Vloeiend gaan**.

Zie de artikelen voor informatie over het gebruik van een aangepaste voorwaarde als een standaardvoorwaarde  [Een aangepaste voorwaarde instellen als standaard voor taken en problemen](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) en [Een aangepaste voorwaarde instellen als standaard voor projecten](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Voor informatie over het wijzigen van de taakstatus raadpleegt u [Taakstatus bijwerken](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

Voor informatie over het wijzigen van de status van de uitgave raadpleegt u [Uitgiftestatus bijwerken](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

Voor informatie over het plaatsen van het Werk aan het knoop aan een Taak van het Begin of de knoop van de Uitgave van het Begin, zie [De knop Aan de werkbalk vervangen door de knop Start](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## De voorwaarde handmatig bijwerken

U moet aan een taak of de kwestie worden toegewezen of het hebben leidt toestemmingen aan het om de Voorwaarde op het te kunnen plaatsen.

Het bijwerken van de voorwaarde van een taak of kwestie verschilt afhankelijk van of u aan het wordt toegewezen of niet:

* U kunt de Voorwaarde op het lusje van Updates of in een lijst van taken of kwesties bijwerken als u aan hen wordt toegewezen.
* U kunt de voorwaarde alleen bijwerken in een lijst met taken of problemen als u deze niet hebt toegewezen, maar over beheermachtigingen beschikt. In dit geval kunt u de voorwaarde niet bijwerken op het tabblad Update van de taak of uitgave.

De voorwaarde van een taak of een kwestie manueel plaatsen:

1. Ga naar een taak of kwestie aan u wordt toegewezen waarvoor u de Voorwaarde wilt plaatsen die.

   of

   Ga naar een lijst met taken of problemen waarvoor u beheerdersmachtigingen hebt, maar die niet aan u zijn toegewezen.

1. Wijzig de voorwaarde van de uitgave of taak als volgt:

   * Als u aan de taak of de kwestie bent toegewezen en beheerderstoestemmingen aan het hebt, op **Updates** tabblad, klikt u op **Een nieuwe update starten**, selecteert u de **Voorwaarde** die het beste aansluit bij de uitvoering van de taak, typt u de reden voor het wijzigen van de voorwaarde in het dialoogvenster **Een nieuwe update starten** gebied (optioneel) en klik vervolgens op **Bijwerken**.

      ![](assets/change-condition-update-comment-350x141.png)

      >[!NOTE]
      >
      >De voorwaarden kunnen voor uw milieu worden aangepast, zodat kunt u meer dan drie opties voor Voorwaarde in uw milieu vinden. De namen van de Voorwaarden kunnen verschillen van de hierboven vermelde. Voor informatie over het aanpassen van Voorwaarden in Workfront raadpleegt u [Een aangepaste voorwaarde maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

      Voor informatie over de extra functionaliteit die beschikbaar is wanneer het bijwerken van een het werkpunt, zie [Werk bijwerken](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p></li>   
     -->
