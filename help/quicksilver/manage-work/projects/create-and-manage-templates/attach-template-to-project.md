---
product-area: templates
navigation-topic: templates-navigation-topic
title: Een sjabloon aan een project koppelen
description: U kunt een malplaatje aan een project of tijdens de aanvankelijke creatiefase van het project of vastmaken nadat het is gecreeerd.
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---

# Een sjabloon aan een project koppelen

U kunt een malplaatje aan een project of tijdens de aanvankelijke creatiefase van het project of vastmaken nadat het is gecreeerd.

Voor meer informatie over het creëren van een project dat een malplaatje gebruikt, zie [ een project creëren gebruikend een malplaatje ](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Toegangsvereisten

U moet over de volgende opties beschikken om de in dit artikel beschreven stappen uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten bewerken </p> <p>Voor informatie over projecttoegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref"> toegang van de Verlening tot projecten </a>.</p> <p>Toegang tot sjablonen weergeven</p> <p>Voor informatie over malplaatjetoestemmingen, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref"> een malplaatje </a> delen. </p> <p>Voor informatie over malplaatjetoegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref"> Toegang van de Verlening tot malplaatjes </a>.</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het project beheren</p> <p>Voor informatie over projecttoestemmingen, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref"> een project in Adobe Workfront </a> delen. </p> <p>Machtigingen voor de sjabloon weergeven of hoger</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations when adding templates to projects</h2>
<p>(NOTE: moved this to an Overview article of its own) </p>
<p>Consider the following when adding templates to projects:</p>
<ul>
<li> <p>You can attach only active templates to projects. </p> </li>
<li> <p>You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your Adobe Workfront administrator <span>or a group administrator</span> has enabled this functionality in the Project&nbsp;Preferences area. For information about setting project preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> </li>
<li> <p>Unless you exclude specific template tasks from being added in the attachment process, all template tasks are added to the existing project. </p> </li>
<li> <p>Most template settings are added to the project. </p> </li>
<li> <p>Some settings from the template automatically transfer to the project, unless you specifically mark them to be excluded. </p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<span class="autonumber"><span><b>Example: </b></span></span>
<p>For example, these settings are added to the project:</p>
<ul>
<li>Start&nbsp;From field</li>
<li>Custom forms and the information on them</li>
<li>Queue Details </li>
<li>Financial settings </li>
</ul>
</div> </li>
</ul>
</div>
-->

## Een sjabloon aan een bestaand project koppelen {#attach-a-template-to-an-existing-project}

U kunt een malplaatje aan een project in Workfront van de projectpagina of van een projectlijst of rapport vastmaken.

1. Ga naar het project waar u een malplaatje wilt vastmaken en **Meer** pictogram ![ Meer pictogram ](assets/qs-more-icon-on-an-object.png) aan het recht van de projectnaam klikken

   ![ Meer dropdown ](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   of

   Ga naar een projectlijst of een rapport en selecteer dan een project **Meer** pictogram ![ Meer pictogram ](assets/qs-more-icon-on-an-object.png) bij de bovenkant van de lijst.

   ![ Meer uitgevouwen menu ](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)


1. Klik **Sjabloon** vastmaken.

   Het vak Sjabloon koppelen wordt weergegeven.

1. Begin de naam van het malplaatje te typen dat u op het **gebied van de Malplaatjes van het Onderzoek** wilt vastmaken, dan het klikken wanneer het vertoningen.in de lijst

   of

   Klik de naam van een malplaatje in het **Andere gebied van Malplaatjes**.

   Een voorbeeld van de sjabloon wordt rechts weergegeven met de volgende informatie over de sjabloon:

   * Duur
   * Eigenaar
   * Het aantal taken op hoofdniveau (bevat een lijst met de eerste drie taken op hoofdniveau)
   * Totaal aantal taken
   * Namen van bijgevoegde aangepaste formulieren

   ![ Band malplaatjedoos ](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. (Facultatief) klik het **pictogram van Favorieten ![ pictogram van Favorieten ](assets/favorites-icon-small.png) links van de malplaatjenaam om het als favoriet te merken.** Hierdoor wordt de sjabloon verplaatst naar de lijst Favorieten.

   ![ pictogram Favorieten op malplaatjelijst ](assets/favorites-icon-on-template-list-in-attach-template-box-nwe-350x79.png)

1. (Facultatief) klik het **pictogram van Favorieten ![ pictogram van Favorieten ](assets/favorites-icon-selected.png) opnieuw om het uit de lijst van Favorieten te verwijderen.**
1. Klik **aanpassen en verbinden**.

   ![ Band malplaatje ](assets/attach-template-large-box-nwe-350x262.png)

1. De informatie van de update in de volgende secties alvorens het malplaatje (of, klik **Malplaatje** op elk ogenblik vastmaken):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Sectie Taken</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">De geselecteerde sjabloontaken hieronder worden geïmporteerd in het project. Schakel de opties uit die u wilt uitsluiten. </td> 
      <td>Hef de selectie op van alle taken die u van de sjabloon wilt uitsluiten voordat u deze aan het project koppelt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Selecteer de projecttaak u als voorganger voor de taken in dit malplaatje wilt.</td> 
      <td> <p>Klik het gebied om een lijst van projecttaken te tonen. Selecteer welke projecttaak u gebeëindigd wilt alvorens de malplaatjetaken kunnen beginnen. Alternatief, kunt u deze stap en opstellingsverhoudingen binnen het project overslaan nadat het malplaatje in bijlage is. </p> <p> Selecteer het <strong> Type van Afhankelijkheid </strong>, <strong> Lag </strong> informatie, en of u wilt dat predecessor <strong> wordt gedwongen </strong> of niet. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Selecteer de projecttaak die u als ouder van de taken in dit malplaatje wilt.</td> 
      <td> Selecteer welke projecttaak u als oudertaak voor alle malplaatjetaken wilt aanwijzen. Als u geen selectie maakt, verschijnen alle malplaatjetaken aan het eind van uw huidige projecttaken. U kunt deze stap overslaan en taken verplaatsen in het project nadat de sjabloon is bijgevoegd.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Sectie Opties</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">De onderstaande geselecteerde items worden overgebracht naar het project. Schakel de opties uit die u wilt uitsluiten.</td> 
      <td> <p>Schakel de selectievakjes uit naast de gegevens die u uit de sjabloon wilt verwijderen voordat u deze aan het project koppelt. Deze informatie wordt niet overgebracht van het malplaatje aan het project. Voor meer informatie over elk gebied, zie <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref"> Overzicht van het vastmaken van een malplaatje aan een project </a>. </p> <p>Belangrijk: Als u de <strong> doos van de Eigenschappen van de Rij &amp; van de Opstelling van Kwesties </strong> controleert, beschrijven de Details van de Rij van het malplaatje die van het project. In dit geval, worden de Verpletterende Regels, de Onderwerpen van de Rij, en de Groepen van het Onderwerp van het malplaatje toegevoegd aan die van het project. <br> als het project opstelling als verzoekrij is en het malplaatje u aan het project vastmaakt niet opstelling als verzoekrij, wordt de rijinformatie van het project verwijderd als u de <strong> gecontroleerde doos van de Eigenschappen van de Rij en van de Opstelling van de Uitgave </strong> verlaat. <br> als u de <strong> Eigenschappen van de Rij en de doos van de Opstelling van de Uitgave </strong> schrapt, worden alle montages van de Opstelling van de Rij van het project bewaard en geen montages van de Opstelling van de Rij van het malplaatje zijn in bijlage. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Aangepaste Forms-sectie</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aangepaste Forms</td> 
      <td> <p>Als aangepaste formulieren aan de sjabloon zijn gekoppeld, worden de namen van de formulieren in het linkerdeelvenster weergegeven. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Werk de gegevens in de aangepaste formulieren bij. Deze informatie wordt overgedragen naar het project.

   >[!TIP]
   >
   >* Deze stap is verplicht wanneer de aangepaste formulieren op de sjabloon verplichte velden bevatten die leeg zijn.
   >* Als de gebieden van de malplaatjedouane vormen reeds op het project bestaan en informatie bevatten, behouden zij de informatie reeds over het project. U kunt deze niet bewerken tijdens het koppelen van de sjabloon.

1. Klik **Sjabloon vastmaken.**
1. Klik **annuleer gehechtheid** ophouden vastmakend het malplaatje.

   of

   Toestaan dat de bijlage klaar is om de sjabloon aan het project toe te voegen.

   Na het vastmaken van het malplaatje, kunt u het project uitgeven en om het even welke taken, informatie, of montages aanpassen zoals nodig.

1. (Facultatief) klik **Details van het Project**, dan **Overzicht** om de naam van het malplaatje te bekijken u in het **verhoudingen van het Project** gebied vastmaakte.

   >[!TIP]
   >
   >Als u meer dan één malplaatje aan het project vastmaakt, slechts toont het malplaatje u eerst in bijlage op dit gebied. Voor informatie, zie [ veelvoudige malplaatjes aan een bestaand project vastmaken en de informatie van het meningsmalplaatje ](#attach-multiple-templates-to-an-existing-project-and-view-template-information) sectie in dit artikel.

1. (Optioneel) Verwijder sjabloongegevens uit het project waar u de sjabloon hebt gekoppeld. Voor informatie, zie [ malplaatjeinformatie uit een project ](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md) verwijderen.

## Meerdere sjablonen koppelen aan een bestaand project en sjablooninformatie weergeven {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

U kunt veelvoudige malplaatjes (één tegelijkertijd) aan het zelfde project vastmaken, na de stappen die in de sectie [ worden beschreven een malplaatje aan een bestaand project ](#attach-a-template-to-an-existing-project) in dit artikel vastmaken. Dit voegt de taken en andere informatie van elk malplaatje aan het project toe.

>[!TIP]
>
>Wanneer u verscheidene malplaatjes aan een project vastmaakt, slechts toont één u eerst in bijlage in het gebied van de Details van het Project.

Om te begrijpen welke malplaatje op een project wordt toegepast:

1. Navigeer naar een project waaraan een sjabloon is gekoppeld.
1. Klik **Details van het Project** in het linkerpaneel.
1. Vind de naam van het malplaatje in bijlage aan het project op het **gebied van het Malplaatje** bij de bodem van de **sectie van het Overzicht** onder **verhoudingen van het Project**.

   ![ Info van het Malplaatje over project ](assets/nwe-template-info-on-project-350x356.png)


