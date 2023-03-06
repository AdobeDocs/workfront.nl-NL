---
title: De weergave Details aanpassen met een lay-outsjabloon
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Workfront-beheerder kunt u een lay-outsjabloon gebruiken om te bepalen welke informatie wordt weergegeven wanneer een gebruiker de sectie Details in het linkerdeelvenster selecteert terwijl een taak, uitgave, document, programma of portfolio wordt weergegeven.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: 78de23b4d5814e5e2ead6bb61a80bba7bd2aed33
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# De weergave Details aanpassen met een lay-outsjabloon

<!-- drafted for bulk editing proejcts: 
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

Als Adobe Workfront-beheerder kunt u een lay-outsjabloon gebruiken om te bepalen welke informatie wordt weergegeven wanneer een gebruiker op het pictogram Details klikt ![](assets/project-details-icon.png) in het linkerdeelvenster wanneer u een taak, uitgave, document, programma of portfolio bekijkt.

<!--
or billing record
-->

U kunt ook de volgorde wijzigen van de gegevens waarin deze gegevens worden weergegeven. Voor alle taken die uw gebruikers bijvoorbeeld zien, kunt u de gegevens van Aangepaste Forms boven aan de weergave Details plaatsen voor alle taken die uw gebruikers zien.

De wijzigingen die u aanbrengt in de weergave Details voor een object, bepalen ook de beschikbaarheid en volgorde van velden die gebruikers in de volgende gebieden zien:

* &quot;Nieuw object&quot;-vakken, zoals Nieuwe taak en Nieuw probleem

   ![](assets/new-task-dialog.png)

* Schermen &quot;Object bewerken&quot;, zoals Taak bewerken, Probleem bewerken en Project bewerken

   ![](assets/edit-task-screen.png)

<!--drafted for bulk editing proejcts - make this bullet live and in yellow at Preview: 

* <span class="preview">"Edit objects" screens when editing projects in bulk, like Edit Projects</span>

  <span>![](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)</span>
  -->

* Samenvatting ![](assets/summary-panel-icon.png) deelvenster voor lijsten met taken en problemen

   ![](assets/summary-area.png)

   >[!NOTE]
   >
   >Wijzigingen in de lay-outsjablonen zijn alleen van invloed op de volgorde en beschikbaarheid van velden in het deelvenster Samenvatting voor de taken en uitgaven die zijn toegewezen aan de aangemelde gebruiker.

* Conversievakken, zoals de kwestie van de Bekeerling aan taak of zet kwestie in projectvakjes om.

   ![Uitgave converteren naar taakvak](assets/convert-issue-to-task-box.png)

Voor informatie over lay-outsjablonen voor groepen raadpleegt u [De lay-outsjablonen van een groep maken en wijzigen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Om deze stappen op systeemniveau uit te voeren, hebt u het toegangsniveau van de Beheerder van het Systeem nodig.
Om hen voor een groep uit te voeren, moet u een manager van die groep zijn</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Aanpassen wat gebruikers zien in de weergave Details

1. Beginnen met het werken aan een lay-outsjabloon, zoals beschreven in [Lay-outsjablonen maken en beheren](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klik op de pijl omlaag ![](assets/dropdown-arrow-12x12.png) krachtens **Aanpassen wat gebruikers zien** en klik vervolgens op **Project**, **Taak**, **Probleem**, **Programma**, of **Portfolio.**
<!--
, or billing record
-->

1. In de **Details** in, voert u een van de volgende handelingen uit om aan te passen wat gebruikers zien in de weergave Details:

   * Alle sectiekoppen slepen ![](assets/move-icon---dots.png) om hun orde te veranderen.
   * Opties in- of uitschakelen onder **Overzicht** en **Aangepaste Forms** om ze te tonen of te verbergen.

      Als u alle velden in een van deze secties verbergt, wordt de volledige sectie verborgen.

      Alle velden zijn standaard ingeschakeld.

1. Blijf het lay-outmalplaatje aanpassen.

   of

   Als u klaar bent met het aanpassen, klikt u op **Opslaan**.

   >[!TIP]
   >
   >U kunt op elk gewenst moment op Opslaan klikken om de voortgang op te slaan en de sjabloon later blijven wijzigen.
