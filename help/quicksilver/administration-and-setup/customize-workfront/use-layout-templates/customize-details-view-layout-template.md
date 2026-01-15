---
title: De weergave Details aanpassen met een lay-outsjabloon
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Workfront-beheerder kunt u een lay-outsjabloon gebruiken om te bepalen welke informatie wordt weergegeven wanneer een gebruiker de sectie Details in het linkerdeelvenster selecteert terwijl een taak, uitgave, document, programma of portfolio wordt weergegeven.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: c037b4f9e5530d8dd796bed25021f7073f16061f
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 0%

---

# De weergave Details aanpassen met een lay-outsjabloon

Als beheerder van Adobe Workfront, kunt u een lay-outmalplaatje gebruiken om te bepalen welke informatie verschijnt wanneer een gebruiker het pictogram van Details ![ pictogram van Details ](assets/project-details-icon.png) in het linkerpaneel klikt terwijl het bekijken van een taak, een kwestie, een document, een programma, of een portefeuille.

U kunt ook de volgorde wijzigen van de gegevens waarin deze gegevens worden weergegeven. Voor alle taken die uw gebruikers bijvoorbeeld zien, kunt u de gegevens van Aangepaste Forms boven aan de weergave Details plaatsen voor alle taken die uw gebruikers zien.

Voor informatie over het creëren van lay-outmalplaatjes, zie [ lay-outmalplaatjes ](../use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.

Voor informatie over lay-outmalplaatjes voor groepen, zie [ tot stand brengen en wijzigen de lay-outmalplaatjes van een groep ](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nadat u een lay-outmalplaatje hebt gevormd, moet u het aan gebruikers voor veranderingen toewijzen u aanbracht om aan anderen zichtbaar te zijn. Voor informatie over het toewijzen van een lay-outmalplaatje aan gebruikers, zie [ gebruikers aan een lay-outmalplaatje ](../use-layout-templates/assign-users-to-layout-template.md) toewijzen.

De wijzigingen die u aanbrengt in de weergave Details voor een object, bepalen ook de beschikbaarheid en volgorde van velden die gebruikers in de volgende gebieden zien:


* &quot;Object maken&quot;-vakken, zoals Taak maken

  ![ Nieuwe taakdialoog ](assets/new-task-dialog.png)


* Schermen &quot;Object bewerken&quot; tijdens het bewerken van een object, zoals Taak bewerken, Probleem bewerken en Project bewerken

  ![ geef taakscherm ](assets/edit-task-screen.png) uit


* &quot;Objecten bewerken&quot; wordt weergegeven in schermen wanneer objecten bulksgewijs worden bewerkt. Momenteel wordt dit ondersteund voor het bulksgewijs bewerken van projecten.

  ![ pas uitgeeft projecten ](assets/customize-edit-projects-in-bulk-box-with-layout-template.png) aan


* Samenvattings paneel ![ Samenvattings paneel ](assets/summary-panel-icon.png) voor lijsten van taken en kwesties

  ![ Samenvattingsgebied ](assets/summary-area.png)

  >[!NOTE]
  >
  >Wijzigingen in de lay-outsjablonen zijn alleen van invloed op de volgorde en beschikbaarheid van velden in het deelvenster Samenvatting voor de taken en uitgaven die zijn toegewezen aan de aangemelde gebruiker.

* Conversievakken, zoals de kwestie van de Bekeerling aan taak of zet kwestie in projectvakjes om.

  ![ Bekeerling kwestie aan taakdoos ](assets/convert-issue-to-task-box.png)

Voor informatie over lay-outmalplaatjes voor groepen, zie [ tot stand brengen en wijzigen de lay-outmalplaatjes van een groep ](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>Om deze stappen op systeemniveau uit te voeren, hebt u het toegangsniveau van de Beheerder van het Systeem nodig.</p>
        <p>Om hen voor een groep uit te voeren, moet u een manager van die groep zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aanpassen wat gebruikers zien in de weergave Details

1. Begin werkend aan een lay-outmalplaatje, zoals die in [ wordt beschreven creeer en beheer lay-outmalplaatjes ](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klik de benedenpijl ![ onderaan pijl ](assets/dropdown-arrow-12x12.png) onder **aanpassen welke gebruikers** zien, dan klikken **Project**, **Taak**, **Uitgave**, **Programma**, of **Portfolio.**<!--, or billing record-->
1. In de **sectie van Details**, doe om het even welke volgend om aan te passen wat de gebruikers in de mening van Details zien:

   * Sleep om het even welke sectiekopballen ![ pictogram van de Beweging ](assets/move-icon---dots.png) om hun orde te veranderen.
   * Laat of maak opties onder de diverse gebieden (zoals **Overzicht**, **Financiën**, en **Douane Forms**) toe onbruikbaar om hen te tonen of te verbergen.

     Als u alle velden in een van deze secties verbergt, wordt de volledige sectie verborgen.

     Alle velden zijn standaard ingeschakeld. U kunt selecteren of ontruimen **alle** controledoos op een gebied selecteren om alle gebieden in dat gebied te tonen of te verbergen.

     ![ mening van Details in lay-outmalplaatje ](assets/layout-template-details-view-updated-save-buttons.png)

1. Blijf het lay-outmalplaatje aanpassen. U kunt **klikken** op elk ogenblik van toepassing zijn om uw vooruitgang te bewaren.

   of

   Als u wordt gebeëindigd aanpassend, klik **sparen en sluit**.

