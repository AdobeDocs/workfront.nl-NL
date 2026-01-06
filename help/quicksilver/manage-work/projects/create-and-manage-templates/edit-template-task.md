---
product-area: templates
keywords: taak,standaardinstellingen,automatiseren,maken
navigation-topic: templates-navigation-topic
title: Sjabloontaak bewerken
description: Nadat u een sjabloon hebt gemaakt, kunt u informatie over de sjabloontaken bewerken. De informatie u op een malplaatjetaak bijwerkt wordt geassocieerd met projecttaken nadat u het malplaatje gebruikt om een project tot stand te brengen of u het malplaatje aan een project vastmaakt.
author: Alina
feature: Work Management
exl-id: 2df8522e-7eee-4440-be0f-f7483c5acdb0
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '4633'
ht-degree: 0%

---

# Sjabloontaken bewerken

<!--Audited: 11/2025-->

<!--take out production and preview references and new/ old experiences at release-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

Nadat u een sjabloon hebt gemaakt, kunt u de informatie van de sjabloontaken bewerken. De informatie u op een malplaatjetaak bijwerkt wordt geassocieerd met projecttaken nadat u het malplaatje gebruikt om een project tot stand te brengen of u het malplaatje aan een project vastmaakt.

Voor informatie over het creëren van een malplaatje, zie [ een projectmalplaatje ](../../../manage-work/projects/create-and-manage-templates/create-template.md) creëren.

U kunt één sjabloontaak tegelijk bewerken of sjabloontaken bulksgewijs bewerken.

>[!NOTE]
>
>U kunt sjabloontaken die tot verschillende sjablonen behoren, niet bulksgewijs bewerken. U kunt sjabloontaken alleen bewerken die tot dezelfde sjabloon behoren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p>
   <p>Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuratie op toegangsniveau</td> 
   <td> <p>Toegang tot sjablonen bewerken</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen </td> 
   <td> <p>Rechten voor een sjabloon beheren. </p> <p>U kunt een sjabloontaak niet delen. </p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Standard </p>
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Templates</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions </td> 
   <td> <p>Manage permissions for a template. </p> <p>You cannot share a template task. </p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Vereisten

Voordat u begint, moet u

* Maak een sjabloon.

  Voor informatie over het creëren van een malplaatje, zie [ een projectmalplaatje ](../../../manage-work/projects/create-and-manage-templates/create-template.md) creëren.

## Sjabloontaken bewerken

U kunt een sjabloontaak bewerken met de gebieden Sjabloontaak bewerken of Sjabloontaakdetails.

{{step1-to-templates}}

1. Klik op de naam van een sjabloon om deze te openen.
1. Klik **Taken van het Malplaatje** in het linkerpaneel.
1. Klik op de naam van een sjabloontaak in de lijst om de sjabloontaak te openen.
1. Ga als volgt te werk om beperkte informatie over de sjabloontaak te bewerken:
   1. (Facultatief) klik **Updates** in het linkerpaneel om updates aan de malplaatjetaak toe te voegen. De de taakupdates van het malplaatje brengen niet naar projecttaken over wanneer het malplaatje wordt gebruikt om een project tot stand te brengen.
   1. (Facultatief) klik **Documenten** in het linkerpaneel om documenten aan de malplaatjetaak toe te voegen. De documenten zullen naar de projecttaken overbrengen wanneer u het malplaatje gebruikt om het project tot stand te brengen.
   1. (Voorwaardelijk) om beperkte informatie over een malplaatjetaak uit te geven, klik **Details van de Taak van het Malplaatje** in het linkerpaneel, dan ga naar de gebieden van de sectie van Details om informatie voor elk gebied uit te geven.
   1. (Optioneel) Voer een van de volgende handelingen uit:
      * Klik **samenvouwen alle** pictogram ![ samenvouwen al pictogram ](assets/collapse-all-icon.png) om alle gebieden samen te vouwen.
      * Klik het **uitgeven** pictogram ![ geeft pictogram ](assets/edit-icon.png) uit, dan selecteren van om het even welke gebieden hieronder, of klik **geef allen** uit om informatie op alle gebieden uit te geven:

         * Overzicht
         * Aangepaste Forms
De namen van douaneformulieren worden alleen weergegeven als er aangepaste formulieren aan de sjabloontaak zijn gekoppeld.
         * Financiën

        >[!TIP]
        >
        >Voor informatie over alle velden die in het gebied Details worden weergegeven, gaat u verder met het bewerken van alle velden via het vak Sjabloontaak bewerken, zoals hieronder wordt beschreven.

   1. (Facultatief) klik de **Subtasks** sectie in het linkerpaneel om kinderen voor de malplaatjetaak toe te voegen. Het toevoegen van subtaken voor malplaatjetaken is gelijkaardig aan het toevoegen van subtasks van de projecttaak. Voor informatie, zie de sectie &quot;subtasks van de taak subtasks sectie&quot;in artikel [ tot subtasks ](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md) leiden.
   1. (Facultatief) klik **Uitgaven** in het linkerpaneel, en voeg uitgaven aan de malplaatjetaken toe. De de taakuitgaven van het malplaatje overdracht aan toekomstige projecttaken, wanneer het malplaatje wordt gebruikt om een project tot stand te brengen.
   1. (Facultatief) klik **goedkeurt** in het linkerpaneel om goedkeuringen tot stand te brengen of globale of groep-vlakke goedkeuringen aan de malplaatjetaken vast te maken. De goedkeuringen worden overgedragen naar toekomstige projecttaken.
   1. (Facultatief) klik de **sectie van Predecessors** in het linkerpaneel om predecessors voor de malplaatjetaken toe te voegen. Het toevoegen van predecessors van de malplaatjetaak is gelijkaardig aan het toevoegen van predecessors van de projecttaak. Voor informatie, zie [ een voorgangersverhouding creëren gebruikend het gebied van Voorgangers ](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).

1. (Facultatief) om verscheidene malplaatjetaken in bulk uit te geven, selecteer veelvoudige malplaatjetaken, dan klik **uitgeven** bij de bovenkant van de malplaatjelijst.
1. (Voorwaardelijk) om alle informatie over de malplaatjetaak of over verscheidene taken tezelfdertijd uit te geven, klik om hen van een lijst te selecteren, dan **uitgeeft** pictogram ![ pictogram ](assets/edit-icon.png) bij de bovenkant van de lijst uit te geven.

   **geeft de Taak van het Malplaatje** vakvertoningen in de nieuwe ervaring uit.

   ![ Nieuwe ervaring voor geeft de Taak van het Malplaatje uit ](assets/edit-template-task-box-unshimmed.png)

   >[!TIP]
   >
   >U kunt een malplaatjetaak in een lijst ook selecteren, dan **** aan het recht van de naam van de malplaatjetaak in de kopbal uitgeven, om **te openen geeft de Taak van het Malplaatje** vakje uit.

   Ga verder het uitgeven van de malplaatjetaak zoals die in [ wordt beschreven een malplaatjetaak gebruikend de nieuwe ervaring ](#edit-a-template-task-using-the-new-experience) sectie in dit artikel uitgeven.

1. (Facultatief) klik **Schakelaar terug naar oude ervaring** bij de bodem van **geef de Taak van het Malplaatje** doos uit om **te openen geef de Taak van het Malplaatje** doos in de oude ervaring uit.

   ![ geef malplaatjetaak ](assets/edit-template-tasks-box-classic-350x356.png) uit

1. Overweeg informatie op te geven in een van de volgende secties:

   * [Overzicht](#overview)
   * [Financiën](#finance)
   * [Instellingen](#settings)
   * [Toewijzingen](#assignments)
   * [Aangepaste Forms](#custom-forms)
   * [Opmerking](#comment)

1. Ga verder het uitgeven van de malplaatjetaak zoals die in [ wordt beschreven een malplaatjetaak gebruikend de oude ervaring ](#edit-a-template-task-using-the-old-experience) sectie in dit artikel.

### Een sjabloontaak bewerken met oude ervaring

#### Overzicht {#overview}

1. Beginnen met het bewerken van een sjabloontaak zoals hierboven beschreven.
1. Klik **Overzicht**.

   ![ geef_task_overview.png uit ](assets/edit-task-overview-350x438.png)

1. Werk een van de volgende items bij:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> Naam </strong> </td> 
      <td>Geef een naam op voor de sjabloontaak. Dit veld wordt niet weergegeven wanneer sjabloontaken bulksgewijs worden bewerkt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Beschrijving </strong> </td> 
      <td>Voeg aanvullende informatie toe over de sjabloontaak.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> URL </strong> </td> 
      <td>Geef een webkoppeling op die betrekking heeft op de informatie over de sjabloontaak.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Prioriteit </strong> </td> 
      <td> <p>Dit is een visuele vlag voor u die u toestaat om aan uw malplaatjetaken voorrang te geven. </p> <p>Selecteer een van de volgende opties:</p> 
       <ul> 
        <li> <p><strong> niets </strong> </p> </li> 
        <li> <p><strong> Laag </strong> </p> </li> 
        <li> <p> <b> Normaal </b></p> </li> 
        <li> <p><b> Hoog </b> </p> </li> 
        <li> <p><b> Dringend </b> </p> </li> 
       </ul> <p>Afhankelijk van de projectvoorkeuren die door uw Workfront-beheerder zijn geselecteerd, kunnen de namen van prioriteiten voor u anders zijn. Voor meer informatie over het uitgeven van prioriteiten, zie <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref"> prioriteiten </a> creëren en aanpassen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Type van Duur </strong> </td> 
      <td> <p>De toekomstige die taak van dit malplaatje wordt gecreeerd zal dit Type van Duur hebben. <br> het Type van Duur identificeert het verband tussen het volgende:</p> <p>- aantal aan een taak toegewezen middelen</p> <p>- de totale inspanning die nodig is om de taak te voltooien</p> <p>- de totale duur van de taak. </p> <p>De Types van Duur laten u toe om verenigbare middeltaken te plaatsen die op de behoeften van de taak worden gebaseerd. Voor meer informatie over het Type van Duur van een taak, zie <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref"> Overzicht van het Type van Duur en van de Duur van de Taak </a>.</p> <p>Selecteer een van de volgende opties:</p> 
       <ul> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;"> Berekende Taak </span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;"> Berekend Werk </span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;"> Gedreven inspanning </span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;"> Eenvoudig </span> <br> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Duur </strong> </td> 
      <td> <p>Geef de duur van de toekomstige taken op in minuten, uren, dagen, weken of maanden. Voor de toekomstige taak die met deze sjabloon wordt gemaakt, wordt de hier opgegeven Duur gebruikt.</p> <p>Workfront meet standaard Duur in dagen. Dit is de hoeveelheid tijd die u toestaat voor de taak om onvolledig te blijven, alvorens het moet worden voltooid. U kunt niet de Duur van een taak specificeren wanneer het <strong> Type van Duur </strong> van de taak <strong> Eenvoudig </strong> is, of wanneer de <strong> Beperking van de Taak </strong> <strong> Vaste Datums </strong> is.</p> <p><b>BELANGRIJK</b></p> <p>De duur is typisch de hoeveelheid tijd tussen de Geplande Begin en de Geplande Datums van de Voltooiing van een malplaatjetaak, en daarom, beïnvloedt het de chronologie van het malplaatje. Hiermee bepaalt u de tijdlijn van het toekomstige project dat op basis van de sjabloon wordt gemaakt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Geplande Uren </strong> </td> 
      <td> <p>Geef het aantal geplande uren voor de toekomstige taak op voor het project dat met deze sjabloon is gemaakt. Dit is de hoeveelheid werkelijke tijd die nodig is om de taken af te ronden. U kunt het aantal Geplande Uren voor een taak slechts specificeren wanneer het <strong> Type van Duur </strong> aan <strong> Berekende Toewijzing </strong> wordt geplaatst. </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong> Beperking van de Taak </strong> </td> 
      <td> <p>De taak op het project dat van dit malplaatje wordt gecreeerd zal deze beperking hebben. De Beperkingen van de taak identificeren wanneer een taak moet worden voltooid. </p> <p>Selecteer een van de volgende opties:</p> 
       <ul> 
        <li><strong> Vaste Datums </strong>. Specificeer a <strong> Geplande Begin </strong> en a <strong> Geplande Datum van de Voltooiing.</strong></li> 
        <li><strong> moet </strong> beginnen. Specificeer a <strong> Geplande Datum van het Begin.</strong></li> 
        <li><strong> moet op </strong> beëindigen. Specificeer a <strong> Geplande Datum van de Voltooiing </strong>.</li> 
        <li><strong> zo spoedig mogelijk </strong> </li> 
        <li><strong> zo laat mogelijk </strong> </li> 
        <li style="font-weight: bold;"><strong> vroegst Beschikbare Tijd </strong> </li> 
        <li style="font-weight: bold;"><strong> Laatste Beschikbare Tijd </strong> </li> 
        <li>Begin niet later dan. Specificeer a <strong> Geplande Datum van het Begin </strong>.</li> 
        <li><strong> Begin niet vroeger dan </strong>. Specificeer a <strong> Geplande Datum van het Begin </strong>.</li> 
        <li><strong> beëindigt niet later dan </strong>. Specificeer a <strong> Geplande Datum van de Voltooiing </strong>.</li> 
        <li><strong> beëindigt geen vroeger dan </strong>. Specificeer a <strong> Geplande Datum van de Voltooiing </strong>.</li> 
       </ul> <p>Voor meer informatie over de Beperking van de Taak, zie <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref"> Overzicht van de Beperking van de Taak </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;"> Dag van het Begin </span> <span style="font-weight: normal;"> (Facultatieve en voorwaardelijke) </span> </td> 
      <td> <p> U kunt de Dag van het Begin van een malplaatjetaak specificeren slechts wanneer de Beperking van de Taak één van het volgende is:</p> 
       <ul> 
        <li>Moet beginnen op</li> 
        <li>Niet eerder starten dan</li> 
        <li>Niet later starten dan</li> 
        <li>Vaste datums</li> 
       </ul> <p>Dit komt overeen met de datum binnen de tijdlijn van het toekomstige project waarop de taak zal starten. Voor alle andere beperkingen berekent Workfront de Begindag op basis van de afhankelijkheid van een voorganger tussen de taken. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Dag van de Voltooiing </strong> <span style="font-weight: normal;"> (Facultatieve en voorwaardelijke) </span> </td> 
      <td> <p> U kunt de Dag van de Voltooiing van een malplaatjetaak slechts specificeren wanneer de Beperking van de Taak één van het volgende is:</p> 
       <ul style="list-style-type: circle;"> 
        <li>Moet worden voltooid op</li> 
        <li>Niet eerder voltooien dan</li> 
        <li>Uiterlijk op</li> 
        <li>Vaste datums</li> 
       </ul> <p>Dit komt overeen met de datum binnen de tijdlijn van het toekomstige project waarop de taak wordt voltooid. Voor alle andere beperkingen, berekent Workfront de Dag van de Voltooiing die op Duur en voorgangsafhankelijkheid wordt gebaseerd. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Ga door met het bewerken van de volgende secties, afhankelijk van de gegevens die u wilt wijzigen.

   of

   Klik **sparen Veranderingen**.

#### Financiën {#finance}

1. Beginnen met het bewerken van een sjabloontaak zoals hierboven beschreven.
1. Klik **Financiën**.

   ![ edit_task_finance.png ](assets/edit-task-finance-350x216.png)

1. Werk een van de volgende items bij:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> Type van Kosten </strong> </td> 
      <td> <p>Geef het type kosten voor de toekomstige taak op. Dit gaat bepalen hoe de Kosten op de taak, gebaseerd op het aantal uren op de taken wordt berekend. </p> <p>Selecteer een van de volgende opties:</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span> Geen Kosten </span> </p> </li> 
        <li> <p style="font-weight: normal;"><span> Vaste Uur </span> </p> </li> 
        <li> <p style="font-weight: normal;"><span> Uur van de Gebruiker </span> </p> </li> 
        <li> <p style="font-weight: normal;"><span> Rol Uur </span> </p> </li> 
       </ul> <p>Voor meer informatie over het volgen van kosten, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref"> Kosten van het Spoor </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Type van Inkomsten </strong> </td> 
      <td> <p>Geef het type inkomsten voor de toekomstige taak op. Dit gaat bepalen hoe de Inkomsten op de taak worden berekend, gebaseerd op het aantal uren op de taken.</p> <p style="font-weight: normal;">Selecteer een van de volgende opties: </p> 
       <ul> 
        <li> <p style="font-weight: normal;">Niet opblaasbaar</p> </li> 
        <li> <p style="font-weight: normal;">Uur gebruiker</p> </li> 
        <li> <p style="font-weight: normal;">Rol Uur</p> </li> 
        <li> <p style="font-weight: normal;">Vast uurwerk</p> </li> 
        <li> <p style="font-weight: normal;">Uur gebruiker met lampvoet</p> </li> 
        <li> <p style="font-weight: normal;">Rol Uur met lampvoet</p> </li> 
        <li> <p style="font-weight: normal;">Uur plus vaste kosten gebruiker</p> </li> 
        <li> <p style="font-weight: normal;">Rol Uur plus vast</p> </li> 
        <li> <p style="font-weight: normal;">Vaste inkomsten</p> </li> 
       </ul> <p>Voor meer informatie over het volgen van opbrengst, zie <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref"> Overzicht van Facturering en Ontvangsten </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Ga door met het bewerken van de volgende secties, afhankelijk van de gegevens die u wilt wijzigen.

   of

   Klik **sparen Veranderingen**.

#### Instellingen {#settings}

1. Beginnen met het bewerken van een sjabloontaak zoals hierboven beschreven.
1. Klik **Montages**.

   ![ geef de montages van de malplaatjetaak ](assets/edit-template-tasks-settings-classic-350x231.png) uit

1. Werk een van de volgende items bij:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Mijlsteen</b></p></strong> </td> 
      <td> <p>Kies een mijlpaal die u aan de geselecteerde sjabloontaak wilt koppelen.</p>

   <p><b>BELANGRIJK</b></p>
   <p>U moet een milestone-pad aan een sjabloon koppelen, zodat dit veld kan worden weergegeven. Voor meer informatie, zie <a href="../create-and-manage-templates/edit-templates.md"> projectmalplaatjes </a> uitgeven.</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong> het Volgen Wijze </strong> </td> 
      <td> <p>Geef op hoe de voortgangsstatus van de toekomstige taak wordt bijgehouden. </p> <p>Selecteer een van de volgende opties:</p> 
       <ul> 
        <li> <p><strong> Gebruiker moet </strong> bijwerken </p> </li> 
        <li> <p><strong> veronderstel op Tijd </strong> </p> </li> 
        <li> <p><strong> negeer Late Waarschuwingen </strong> </p> </li> 
        <li> <p><strong> Autocomplete </strong> </p> </li> 
        <li> <p><strong> Predecessor </strong> </p> </li> 
       </ul> <p>Voor meer informatie over de het Volgen Wijze op taken, zie <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref"> het Volgen van de Taak overzicht van de Wijze </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Proces van de Goedkeuring </strong> </td> 
      <td> <p>Selecteer het goedkeuringsproces u met de malplaatjetaak wilt associëren. Uw Workfront-beheerder moet processen voor taakgoedkeuring op systeemniveau definiëren voordat u deze aan sjabloontaken kunt koppelen. <span> de gebruiker van A met administratieve toegang tot de processen van de Goedkeuring kan tot groep-specifieke goedkeuringsprocessen ook leiden.</span> voor meer informatie over het creëren van goedkeuringsprocessen, zie <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref"> een goedkeuringsproces voor het werkpunten </a> creëren.</p> <p>Houd rekening met het volgende wanneer u goedkeuringsprocessen toevoegt: </p> 
       <ul> 
       <li>Alleen actieve goedkeuringsprocessen worden in de lijst weergegeven. </li> 
       <li> <p>Systeemspecifieke en groepsspecifieke goedkeuringsprocessen worden in de lijst weergegeven. Goedkeuringsprocessen die aan een andere groep dan die van de sjabloon zijn gekoppeld, worden niet in de lijst weergegeven.</p> <p>Belangrijk: als de groep die aan de sjabloon is gekoppeld, verandert het groepsspecifieke goedkeuringsproces in een goedkeuringsproces voor één gebruik. Voor meer informatie over hoe de veranderingen in de groep van het project of de veranderingen in het goedkeuringsproces goedkeuringsmontages beïnvloeden, zie <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref"> hoe de groep en de veranderingen van het goedkeuringsproces aangewezen goedkeuringsprocessen </a> beïnvloeden. </p> </li> 
       <li> <p>Als u een goedkeuringsproces voor eenmalig gebruik hebt toegevoegd, wordt dit weergegeven als "&lt;Custom&gt;" in dit veld. Voor informatie, zie <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref"> een nieuw of bestaand goedkeuringsproces met het werk </a> associëren. </p> <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will be valid only for Classic when they edit the Edit Template box in NWE)</p>--> </li> 
       <li> <p>Bij het bulkbewerken van sjabloontaken bestaan de volgende scenario's:</p> 
       <ul> 
       <li> <p>Wanneer u sjabloontaken selecteert uit dezelfde sjabloongroep, worden zowel op systeemniveau als op groepsniveau goedkeuringsprocessen weergegeven in dit veld.</p> </li> 
       <li> <p>Wanneer u sjabloontaken selecteert uit verschillende sjabloongroepen, worden alleen goedkeuringsprocessen op systeemniveau weergegeven in dit veld.</p> </li> 
       <li> <p>Wanneer om het even welke malplaatjetaken een enig-gebruiks goedkeuringsproces in bijlage hebben, wordt het vervangen door het systeem-niveau <span> of groep-vlakke goedkeuringsproces </span> u selecteert. </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Meldingen van de Herinnering </strong> </td> 
      <td> <p>Selecteer welke herinneringsberichten u aan de malplaatjetaak wilt vastmaken. Zij zullen aan de toekomstige taken op het project worden vastgemaakt dat van dit malplaatje wordt gecreeerd. Uw systeembeheerder moet Meldingen van de Herinnering vormen alvorens u hen op een taak kunt selecteren. Voor meer informatie over het vormen van de Meldingen van de Herinnering, zie <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref"> de herinneringsberichten van de Opstelling </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Ga door met het bewerken van de volgende secties, afhankelijk van de gegevens die u wilt wijzigen.

   of

   Klik **sparen Veranderingen**.

#### Toewijzingen {#assignments}

1. Beginnen met het bewerken van een sjabloontaak zoals hierboven beschreven.
1. Klik **Taken**.

   ![ toewijzingen_edit_tasks.png ](assets/assignments-edit-tasks-350x87.png)

1. Klik **toevoegen Ontvanger** om een nieuwe ontvanger aan de malplaatjetaak toe te voegen. U kunt gebruikers, rollen, of teams aan een taak toewijzen. U kunt meerdere toewijzingen aan een taak toewijzen. De toekomstige taken zullen de zelfde middelen hebben die aan het wanneer gecreeerd van deze malplaatjetaak worden toegewezen.
1. (Facultatief) als u veelvoudige wijzers hebt, selecteer het **Keuzerondje van de Eigenaar** om op te wijzen welke gebruiker of rol als de Eigenaar van de Taak of Primaire Ontvanger wordt beschouwd. Workfront markeert de eerste gebruiker of de baanrol die u aan een malplaatjetaak als Eigenaar of Primaire Ontvanger toewijst.
1. (Voorwaardelijk en facultatief) als uw **Type van Duur** **Berekend Werk** of **Gedreven inspanning** is, specificeer **Toewijzing %** (toewijzingspercentage) voor elke toegewezen persoon. Dit is de hoeveelheid tijd van het programma van de toegewezen persoon die zij aan deze taak kunnen uitgeven. Als het toewijzingspercentage voor een toegewezen persoon wordt gewijzigd, veranderen de geplande uren van een taak.
1. (Voorwaardelijk en facultatief) als uw **Type van Duur** **Eenvoudig** is, specificeer de **Uren** van elke toegewezen persoon

   of

   Specificeer het totale aantal **Geplande Uren** voor de malplaatjetaak. Dit verdeelt de totale uren gelijkelijk over alle toegewezen personen.

1. (Voorwaardelijk en facultatief) als uw **Type van Duur** Eenvoudig is, specificeer de **Duur** van de malplaatjetaak in dagen. Dit wordt de duur van de taak die op basis van deze sjabloon wordt gemaakt.
1. (Facultatief) selecteer een rol van het **drop-down menu van de Rol van 0} toewijzen.** Dit is de rol die de ontvanger kan vervullen bij deze toekomstige taak. Alleen de functies die aan elke toegewezen persoon in het profiel zijn gekoppeld, worden weergegeven in het vervolgkeuzemenu.
1. (Optioneel) Ga door met het bewerken van de volgende secties, afhankelijk van de gegevens die u wilt wijzigen.

   of

   Klik **sparen Veranderingen**.

#### Aangepaste Forms {#custom-forms}

U kunt aangepaste formulieren definiëren die automatisch aan taken worden gekoppeld wanneer de taken aan een project worden toegevoegd. Voor informatie over vestiging het project om de vormen van de standaardtaakdouane te omvatten, zie de &quot;sectie van Taken&quot;in het artikel [ projecten ](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

U kunt ook aangepaste formulieren toevoegen aan de toekomstige taken van een project wanneer het project wordt gemaakt op basis van een sjabloon, door de aangepaste formulieren toe te voegen aan de sjabloontaken.

1. Beginnen met het bewerken van een sjabloontaak zoals hierboven beschreven.
1. Klik **Aangepaste Forms**.

   ![ custom_forms_edit_task.png ](assets/custom-forms-edit-task-350x136.png)

1. Selecteer het aangepaste formulier of de formulieren die u aan de sjabloontaak wilt koppelen.

   U moet aangepaste formulieren maken voordat u ze in dit veld kunt selecteren.
Alleen actieve aangepaste formulieren worden in de lijst weergegeven.
Voor meer informatie over de bouw van douaneformulieren, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.
U kunt maximaal tien aangepaste formulieren toevoegen aan een sjabloontaak.
De formulieren worden automatisch toegevoegd aan de taken die op basis van de sjabloon worden gemaakt.
1. (Voorwaardelijk en optioneel) Als u een aangepast formulier aan de sjabloontaak hebt gekoppeld, bewerkt u alle velden op het formulier. U moet alle vereiste velden opgeven voordat u de sjabloontaak kunt opslaan.

   >[!NOTE]
   >
   >Afhankelijk van de manier waarop uw Workfront-beheerder de machtigingen voor de secties in uw aangepaste formulier instelt, kan niet iedereen dezelfde velden op een aangepast formulier weergeven of bewerken. De machtigingen voor het bewerken van velden in een sectie van een aangepast formulier zijn afhankelijk van de machtigingen die u hebt voor de sjabloontaak of de toekomstige taak.\
   >Voor informatie over het plaatsen van toestemmingen op secties van een douanevorm, zie [ een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md) delen.\
   >Voor informatie over het plaatsen van taaktoestemmingen, zie [ een taak ](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md) delen.\
   >Voor informatie over het plaatsen van malplaatjetoestemmingen, zie [ een malplaatje ](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md) delen.

1. (Optioneel) Ga door met het bewerken van de volgende sectie, afhankelijk van de informatie die u wilt wijzigen.

   of

   Klik **sparen Veranderingen**.

#### Opmerking {#comment}

1. Beginnen met het bewerken van een sjabloontaak zoals hierboven beschreven.
1. Klik **Commentaar**.

   ![ comment_edit_task.png ](assets/comment-edit-task-350x138.png)

1. Geef een opmerking op die u in de updatestream van de sjabloontaak wilt weergeven in het beschikbare veld. Deze opmerking is zichtbaar voor iedereen met Weergavetoegang tot de sjabloon en de sjabloontaak en met toegang tot weergavenotities.
1. Klik **sparen Veranderingen**.

   Wanneer u of een andere gebruiker een project van dit malplaatje creeert, worden alle montages u op malplaatjetaken toepaste de montages voor de projecttaken.

### Een sjabloontaak bewerken met de nieuwe ervaring

Na het openen van **geef de doos van de Taak van het Malplaatje** in de nieuwe ervaring uit, denk na specificerend informatie in om het even welke volgende secties:

* [Naam sjabloontaak](#template-task-name)
* [Overzicht](#overview-1)
* [Toewijzingen](#assignments-1)
* [Financiën](#finance-1)
* [Aangepaste Forms](#custom-forms-1)
* [Instellingen](#settings-1)
* [Opmerking](#comment-1)

#### Naam sjabloontaak

>[!TIP]
>
>De sectie Naam sjabloontaak is niet beschikbaar wanneer u sjabloontaken bulksgewijs bewerkt.


1. Beginnen met het bewerken van een sjabloontaak zoals hierboven beschreven.
1. In het Edit vakje van de Taak van het Malplaatje, klik {de Naam van de Taak van het 0} Malplaatje **en voeg een naam voor de malplaatjetaak toe.**

   Deze weergave is niet beschikbaar als u sjabloontaken bulksgewijs bewerkt.

1. (Optioneel) Ga door met het bewerken van de volgende secties, afhankelijk van de gegevens die u wilt wijzigen.

   of

   Klik **sparen**.

#### Overzicht {#overview-1}

1. Beginnen met het bewerken van een sjabloontaak zoals hierboven beschreven.
1. In **geef de Taak van het Malplaatje** vakje uit, klik **Overzicht** in het linkerpaneel.

   ![ de taak van het Malplaatje geeft overzichtssectie uit ](assets/template-task-edit-overview.png)

1. Werk een van de volgende items bij:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> Beschrijving </strong> </td> 
      <td>Voeg aanvullende informatie toe over de sjabloontaak.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Prioriteit </strong> </td> 
      <td> <p>Dit is een visuele vlag voor u die u toestaat om aan uw malplaatjetaken voorrang te geven. </p> <p>Selecteer een van de volgende opties:</p> 
       <ul> 
        <li> <p><strong> niets </strong> </p> </li> 
        <li> <p><strong> Laag </strong> </p> </li> 
        <li> <p> <b> Normaal </b></p> </li> 
        <li> <p><b> Hoog </b> </p> </li> 
        <li> <p><b> Dringend </b> </p> </li> 
       </ul> <p>Afhankelijk van de projectvoorkeuren die door uw Workfront-beheerder zijn geselecteerd, kunnen de namen van prioriteiten voor u anders zijn. Voor meer informatie over het uitgeven van prioriteiten, zie <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref"> prioriteiten </a> creëren en aanpassen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Beperking van de Taak </strong> </td> 
      <td> <p>De taak op het project dat van dit malplaatje wordt gecreeerd zal deze beperking hebben. De Beperkingen van de taak identificeren wanneer een taak moet worden voltooid. </p> <p>Selecteer een van de volgende opties:</p> 
       <ul> 
        <li><strong> Vaste Datums </strong>. Specificeer a <strong> Geplande Begin </strong> en a <strong> Geplande Datum van de Voltooiing.</strong></li> 
        <li><strong> moet </strong> beginnen. Specificeer a <strong> Geplande Datum van het Begin.</strong></li> 
        <li><strong> moet op </strong> beëindigen. Specificeer a <strong> Geplande Datum van de Voltooiing </strong>.</li> 
        <li><strong> zo spoedig mogelijk </strong> </li> 
        <li><strong> zo laat mogelijk </strong> </li> 
        <li style="font-weight: bold;"><strong> vroegst Beschikbare Tijd </strong> </li> 
        <li style="font-weight: bold;"><strong> Laatste Beschikbare Tijd </strong> </li> 
        <li>Begin niet later dan. Specificeer a <strong> Geplande Datum van het Begin </strong>.</li> 
        <li><strong> Begin niet vroeger dan </strong>. Specificeer a <strong> Geplande Datum van het Begin </strong>.</li> 
        <li><strong> beëindigt niet later dan </strong>. Specificeer a <strong> Geplande Datum van de Voltooiing </strong>.</li> 
        <li><strong> beëindigt geen vroeger dan </strong>. Specificeer a <strong> Geplande Datum van de Voltooiing </strong>.</li> 
       </ul> <p>Voor meer informatie over de Beperking van de Taak, zie <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref"> Overzicht van de Beperking van de Taak </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;"> Dag van het Begin </span> <span style="font-weight: normal;"> (Facultatieve en voorwaardelijke) </span> </td> 
      <td> <p> U kunt de Dag van het Begin van een malplaatjetaak specificeren slechts wanneer de Beperking van de Taak één van het volgende is:</p> 
       <ul> 
        <li>Moet beginnen op</li> 
        <li>Niet eerder starten dan</li> 
        <li>Niet later starten dan</li> 
        <li>Vaste datums</li> 
       </ul> <p>Dit komt overeen met de datum binnen de tijdlijn van het toekomstige project waarop de taak zal starten. Voor alle andere beperkingen berekent Workfront de Begindag op basis van de afhankelijkheid van een voorganger tussen de taken. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Dag van de Voltooiing </strong> <span style="font-weight: normal;"> (Facultatieve en voorwaardelijke) </span> </td> 
      <td> <p> U kunt de Dag van de Voltooiing van een malplaatjetaak slechts specificeren wanneer de Beperking van de Taak één van het volgende is:</p> 
       <ul style="list-style-type: circle;"> 
        <li>Moet worden voltooid op</li> 
        <li>Niet eerder voltooien dan</li> 
        <li>Uiterlijk op</li> 
        <li>Vaste datums</li> 
       </ul> <p>Dit komt overeen met de datum binnen de tijdlijn van het toekomstige project waarop de taak wordt voltooid. Voor alle andere beperkingen, berekent Workfront de Dag van de Voltooiing die op Duur en voorgangsafhankelijkheid wordt gebaseerd. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> URL </strong> </td> 
      <td>Geef een webkoppeling op die betrekking heeft op de informatie over de sjabloontaak.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong> de Werkinspanning van het Werk </strong> </td> 
      <td>Kies een van de volgende opties:
      <ul><li>Klein</li>
      <li>Medium</li>
      <li>Groot</li></ul>

   <p><b>BELANGRIJK</b></p>
      <p>Het gebied van de Werkinspanning van het Werk toont wanneer het uitgeven van een malplaatjetaak slechts wanneer u de <b> Werkinspanning van het Gebruik selecteert om taak Geplande Uren </b> automatisch te berekenen die wanneer het uitgeven van het malplaatje plaatsen.</p>

   </td> 
     </tr> 
     </tbody> 
   </table>

1. (Optioneel) Ga door met het bewerken van de volgende secties, afhankelijk van de gegevens die u wilt wijzigen.

   of

   Klik **sparen**.

#### Toewijzingen {#assignments-1}

1. Beginnen met het bewerken van een sjabloontaak zoals hierboven beschreven.
1. In **geef de Taak van het Malplaatje** vakje uit, klik **Toewijzingen** in het linkerpaneel.

   ![ de taak van het Malplaatje geeft taken uit ](assets/template-task-edit-assignments.png)

1. In de **mensen van het Onderzoek, de rol, of het teamgebied**, begin de naam van een ontvanger te typen, dan het te selecteren wanneer het in de lijst toont

   of

   Klik **toewijzen aan me** om de malplaatjetaak aan zich toe te wijzen.
1. U kunt overwegen de volgende gegevens bij te werken:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody>

   <tr> 
         <td role="rowheader"><strong> Type van Duur </strong> </td> 
         <td> <p>De toekomstige die taak van dit malplaatje wordt gecreeerd zal dit Type van Duur hebben. <br> het Type van Duur identificeert het verband tussen het volgende:</p> 
         <ul>
         <li><p>Aantal middelen die aan een taak worden toegewezen</p> </li>
         <li><p>De totale vereiste inspanning om de taak te voltooien</p></li> 
         <li><p>De totale duur van de taak </p></li></ul> <p>Gebruikend de Types van Duur, kunt u verenigbare middeltaken plaatsen die op de behoeften van de taak worden gebaseerd. Voor meer informatie over het Type van Duur van een taak, zie <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref"> Overzicht van het Type van Duur en van de Duur van de Taak </a>.</p> <p>Selecteer een van de volgende opties:</p> 
         <ul> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;"> Berekende Taak </span> </p> </li> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;"> Berekend Werk </span> </p> </li> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;"> Gedreven inspanning </span> </p> </li> 
         <li> <p style="font-weight: bold;"><span style="font-weight: normal;"> Eenvoudig </span> <br> </p> </li> 
         </ul> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong> Duur </strong> </td> 
         <td> <p>Geef de duur van de toekomstige taken op in minuten, uren, dagen, weken of maanden. Voor de toekomstige taak die met deze sjabloon wordt gemaakt, wordt de hier opgegeven Duur gebruikt.</p> <p>Workfront meet standaard Duur in dagen. Dit is de hoeveelheid tijd die u toestaat voor de taak om onvolledig te blijven, alvorens het moet worden voltooid. U kunt niet de Duur van een taak specificeren wanneer het <strong> Type van Duur </strong> van de taak <strong> Eenvoudig </strong> is, of wanneer de <strong> Beperking van de Taak </strong> <strong> Vaste Datums </strong> is.</p> <p><b>BELANGRIJK</b></p> <p>De duur is typisch de hoeveelheid tijd tussen de Geplande Begin en de Geplande Datums van de Voltooiing van een malplaatjetaak, en daarom, beïnvloedt het de chronologie van het malplaatje. Hiermee bepaalt u de tijdlijn van het toekomstige project dat op basis van de sjabloon wordt gemaakt. </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong> Geplande Uren </strong> </td> 
         <td> <p>Geef het aantal geplande uren voor de toekomstige taak op voor het project dat met deze sjabloon is gemaakt. Dit is de hoeveelheid werkelijke tijd die nodig is om de taken af te ronden. U kunt het aantal Geplande Uren voor een taak slechts specificeren wanneer het <strong> Type van Duur </strong> aan <strong> Berekende Toewijzing </strong> wordt geplaatst. </p> </td> 
      </tr> 
   </tbody> 
      </table>

1. (Optioneel) Ga door met het bewerken van de volgende secties, afhankelijk van de gegevens die u wilt wijzigen.

   of

   Klik **sparen**.

#### Financiën {#finance-1}

1. Beginnen met het bewerken van een sjabloontaak zoals hierboven beschreven.
1. In **geef de Taak van het Malplaatje** vakje uit, klik **Financiën** in het linkerpaneel.

   ![ de taak van het Malplaatje geeft financieringssectie uit ](assets/template-task-edit-finance.png)

1. Werk een van de volgende items bij:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> Type van Kosten </strong> </td> 
      <td> <p>Geef het type kosten voor de toekomstige taak op. Dit gaat bepalen hoe de Kosten op de taak, gebaseerd op het aantal uren op de taken wordt berekend. </p> <p>Selecteer een van de volgende opties:</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span> Geen Kosten </span> </p> </li> 
        <li> <p style="font-weight: normal;"><span> Vaste Uur </span> </p> </li> 
        <li> <p style="font-weight: normal;"><span> Uur van de Gebruiker </span> </p> </li> 
        <li> <p style="font-weight: normal;"><span> Rol Uur </span> </p> </li> 
       </ul> <p>Voor meer informatie over het volgen van kosten, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref"> Kosten van het Spoor </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Type van Inkomsten </strong> </td> 
      <td> <p>Geef het type inkomsten voor de toekomstige taak op. Dit gaat bepalen hoe de Inkomsten op de taak worden berekend, gebaseerd op het aantal uren op de taken.</p> <p style="font-weight: normal;">Selecteer een van de volgende opties: </p> 
       <ul> 
        <li> <p style="font-weight: normal;">Niet opblaasbaar</p> </li> 
        <li> <p style="font-weight: normal;">Uur gebruiker</p> </li> 
        <li> <p style="font-weight: normal;">Rol Uur</p> </li> 
        <li> <p style="font-weight: normal;">Vast uurwerk</p> </li> 
        <li> <p style="font-weight: normal;">Uur gebruiker met lampvoet</p> </li> 
        <li> <p style="font-weight: normal;">Rol Uur met lampvoet</p> </li> 
        <li> <p style="font-weight: normal;">Uur plus vaste kosten gebruiker</p> </li> 
        <li> <p style="font-weight: normal;">Rol Uur plus vast</p> </li> 
        <li> <p style="font-weight: normal;">Vaste inkomsten</p> </li> 
       </ul> <p>Voor meer informatie over het volgen van opbrengst, zie <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref"> Overzicht van Facturering en Ontvangsten </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Ga door met het bewerken van de volgende secties, afhankelijk van de gegevens die u wilt wijzigen.

   of

   Klik **sparen**.

#### Aangepaste Forms {#custom-forms-1}

U kunt aangepaste formulieren definiëren die automatisch aan taken worden gekoppeld wanneer de taken aan een project worden toegevoegd. Voor informatie over vestiging het project om de vormen van de standaardtaakdouane te omvatten, zie de &quot;sectie van Taken&quot;in het artikel [ projecten ](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

U kunt ook aangepaste formulieren toevoegen aan de toekomstige taken van een project wanneer het project wordt gemaakt op basis van een sjabloon, door de aangepaste formulieren toe te voegen aan de sjabloontaken.

1. Beginnen met het bewerken van een sjabloontaak zoals hierboven beschreven.
1. In **geef de Taak van het Malplaatje** vakje uit, klik **Douane Forms** in het linkerpaneel.

   ![ de taak van het Malplaatje geeft de sectie van douaneformulieren uit ](assets/template-task-edit-custom-forms.png)

1. Selecteer het aangepaste formulier of de formulieren die u aan de sjabloontaak wilt koppelen.

   U moet aangepaste formulieren maken voordat u ze in dit veld kunt selecteren.
Alleen actieve aangepaste formulieren worden in de lijst weergegeven.

   Voor meer informatie over de bouw van douaneformulieren, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

   U kunt maximaal tien aangepaste formulieren toevoegen aan een sjabloontaak.
De formulieren worden automatisch toegevoegd aan de taken die op basis van de sjabloon worden gemaakt.
1. (Voorwaardelijk en optioneel) Als u een aangepast formulier aan de sjabloontaak hebt gekoppeld, bewerkt u alle velden op het formulier. U moet alle vereiste velden opgeven voordat u de sjabloontaak kunt opslaan.

   >[!NOTE]
   >
   >Afhankelijk van de manier waarop uw Workfront-beheerder de machtigingen voor de secties in uw aangepaste formulier instelt, kan niet iedereen dezelfde velden op een aangepast formulier weergeven of bewerken. De machtigingen voor het bewerken van velden in een sectie van een aangepast formulier zijn afhankelijk van de machtigingen die u hebt voor de sjabloontaak of de toekomstige taak.\
   >Voor informatie over het plaatsen van toestemmingen op secties van een douanevorm, zie [ een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md) delen.\
   >Voor informatie over het plaatsen van taaktoestemmingen, zie [ een taak ](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md) delen.\
   >Voor informatie over het plaatsen van malplaatjetoestemmingen, zie [ een malplaatje ](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md) delen.

1. (Optioneel) Ga door met het bewerken van de volgende sectie, afhankelijk van de informatie die u wilt wijzigen.

   of

   Klik **sparen**.

#### Instellingen {#settings-1}

1. Beginnen met het bewerken van een sjabloontaak zoals hierboven beschreven.
1. In **geef de Taakdoos van het Malplaatje uit**, klik **Montages** in het linkerpaneel.

   ![ de taak van het Malplaatje geeft montagessectie uit ](assets/template-task-edit-settings.png)

1. Werk een van de volgende items bij:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Mijlsteen</b></p></strong> </td> 
      <td> <p>Kies een mijlpaal die u aan de geselecteerde sjabloontaak wilt koppelen.</p>

   <p><b>BELANGRIJK</b></p>
   <p>U moet een milestone-pad aan een sjabloon koppelen, zodat dit veld kan worden weergegeven. Voor meer informatie, zie <a href="../create-and-manage-templates/edit-templates.md"> projectmalplaatjes </a> uitgeven.</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong> het Volgen Wijze </strong> </td> 
      <td> <p>Geef op hoe de voortgangsstatus van de toekomstige taak wordt bijgehouden. </p> <p>Selecteer een van de volgende opties:</p> 
       <ul> 
        <li> <p><strong> Gebruiker moet </strong> bijwerken </p> </li> 
        <li> <p><strong> veronderstel op Tijd </strong> </p> </li> 
        <li> <p><strong> negeer Late Waarschuwingen </strong> </p> </li> 
        <li> <p><strong> Autocomplete </strong> </p> </li> 
        <li> <p><strong> Predecessor </strong> </p> </li> 
       </ul> <p>Voor meer informatie over de het Volgen Wijze op taken, zie <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref"> het Volgen van de Taak overzicht van de Wijze </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Meldingen van de Herinnering </strong> </td> 
      <td> <p>Selecteer welke herinneringsberichten u aan de malplaatjetaak wilt vastmaken. Zij zullen aan de toekomstige taken op het project worden vastgemaakt dat van dit malplaatje wordt gecreeerd. Uw systeembeheerder moet Meldingen van de Herinnering vormen alvorens u hen op een taak kunt selecteren. Voor meer informatie over het vormen van de Meldingen van de Herinnering, zie <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref"> de herinneringsberichten van de Opstelling </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Proces van de Goedkeuring </strong> </td> 
      <td> <p>Selecteer het goedkeuringsproces u met de malplaatjetaak wilt associëren. Uw Workfront-beheerder moet processen voor taakgoedkeuring op systeemniveau definiëren voordat u deze aan sjabloontaken kunt koppelen. <span> de gebruiker van A met administratieve toegang tot de processen van de Goedkeuring kan tot groep-specifieke goedkeuringsprocessen ook leiden.</span> voor meer informatie over het creëren van goedkeuringsprocessen, zie <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref"> een goedkeuringsproces voor het werkpunten </a> creëren.</p> <p>Houd rekening met het volgende wanneer u goedkeuringsprocessen toevoegt: </p> 
       <ul> 
       <li>Alleen actieve goedkeuringsprocessen worden in de lijst weergegeven. </li> 
       <li> <p>Systeemspecifieke en groepsspecifieke goedkeuringsprocessen worden in de lijst weergegeven. Goedkeuringsprocessen die aan een andere groep dan die van de sjabloon zijn gekoppeld, worden niet in de lijst weergegeven.</p> <p>Belangrijk: als de groep die aan de sjabloon is gekoppeld, verandert het groepsspecifieke goedkeuringsproces in een goedkeuringsproces voor één gebruik. Voor meer informatie over hoe de veranderingen in de groep van het project of de veranderingen in het goedkeuringsproces goedkeuringsmontages beïnvloeden, zie <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref"> hoe de groep en de veranderingen van het goedkeuringsproces aangewezen goedkeuringsprocessen </a> beïnvloeden. </p> </li> 
       <li> <p>Als u een goedkeuringsproces voor eenmalig gebruik hebt toegevoegd, wordt dit weergegeven als "&lt;Custom&gt;" in dit veld. Voor informatie, zie <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref"> een nieuw of bestaand goedkeuringsproces met het werk </a> associëren. </p>  </li> 
       <li> <p>Bij het bulkbewerken van sjabloontaken bestaan de volgende scenario's:</p> 
       <ul> 
       <li> <p>Wanneer u sjabloontaken selecteert uit dezelfde sjabloongroep, worden zowel op systeemniveau als op groepsniveau goedkeuringsprocessen weergegeven in dit veld.</p> </li> 
       <li> <p>Wanneer u sjabloontaken selecteert uit verschillende sjabloongroepen, worden alleen goedkeuringsprocessen op systeemniveau weergegeven in dit veld.</p> </li> 
       <li> <p>Wanneer om het even welke malplaatjetaken een enig-gebruiks goedkeuringsproces in bijlage hebben, wordt het vervangen door het systeem-niveau <span> of groep-vlakke goedkeuringsproces </span> u selecteert. </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr>

   </tbody> 
   </table>

1. (Optioneel) Ga door met het bewerken van de volgende secties, afhankelijk van de gegevens die u wilt wijzigen.

   of

   Klik **sparen**.

#### Opmerking {#comment-1}

1. Beginnen met het bewerken van een sjabloontaak zoals hierboven beschreven.
1. In **geef de Taak van het Malplaatje** vakje uit, klik **Commentaar** in het linkerpaneel.

   ![ de taak van het Malplaatje geeft sectie van de Commentaar uit ](assets/template-task-edit-comment.png)

1. In **voeg een update aan het gebied van de malplaatjetaak** toe, specificeer een commentaar dat u in de updatestroom van de malplaatjetaak op het beschikbare gebied wilt tonen. Deze opmerking is zichtbaar voor iedereen met Weergavetoegang tot de sjabloon en de sjabloontaak en met toegang tot weergavenotities.
1. Klik **sparen**.

   Wanneer u of een andere gebruiker een project van dit malplaatje creeert, worden alle montages u op malplaatjetaken toepaste de montages voor de projecttaken.

