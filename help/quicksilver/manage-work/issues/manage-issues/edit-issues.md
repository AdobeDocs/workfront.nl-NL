---
product-area: projects
navigation-topic: manage-issues
title: Problemen bewerken
description: U kunt informatie bewerken over uitgaven die u hebt gemaakt of die andere gebruikers hebben gemaakt als zij de problemen met u hebben gedeeld.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 1449374a-ab0d-4c98-83cd-4e511467633a
source-git-commit: 5b7a5aff0f8bdf7cf8429ac29b50c3beaf4bd3b4
workflow-type: tm+mt
source-wordcount: '2504'
ht-degree: 0%

---

# Problemen bewerken

U kunt informatie bewerken over uitgaven die u hebt gemaakt of die andere gebruikers hebben gemaakt als zij de problemen met u hebben gedeeld.

U kunt één uitgave bewerken of u kunt uitgaven in een lijst bewerken. Voor informatie over bewerkingsproblemen in een lijst raadpleegt u [Uitgaven in een lijst bewerken](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

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
   <td> <p>Aanvraag of hoger</p> <p>De vergunning van het overzicht of hoger om kwesties in de sectie van Kwesties van een taak of een project uit te geven</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau*</td> 
   <td> <p>Toegang tot problemen bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over toegang tot kwesties in uw Niveau van de Toegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Toegang verlenen tot kwesties</a>. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute-machtigingen voor een uitgave om de volgende velden in het gebied Details te bewerken: </p>
   <ul>
   <li>Beschrijving</li>
   <li>Status</li>
   <li>Ernst</li>
   </ul>
   <p>Rechten beheren voor een uitgave om alle velden in het gebied Details of in het vak Uitgave bewerken te bewerken</p> <p> Voor informatie over het verlenen van machtigingen voor uitgaven raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Een uitgave delen </a></p> <p>Voor informatie over het aanvragen van aanvullende machtigingen raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Beperkingen bij het bewerken van problemen

Er zijn enkele beperkingen die kunnen voorkomen dat u problemen kunt bewerken.

* U kunt geen kwesties uitgeven die in een Goedkeuringsproces zijn. U kunt de status van een probleem dat zich in afwachting van goedkeuring bevindt, alleen aanmelden of bijwerken.
* U kunt documenten aan kwesties op een project uitgeven en toevoegen dat een status van Voltooid heeft, Dead, of in afwachting van Goedkeuring slechts wanneer uw beheerder van Workfront of een groepsbeheerder deze functionaliteit op het gebied van de Voorkeur van het Project toeliet. Voor informatie over het instellen van projectvoorkeuren raadpleegt u [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Eén uitgave bewerken

U kunt een uitgave bewerken met de gebieden Probleem bewerken of Details van probleem. In de volgende stappen wordt het bewerken van een probleem beschreven in het venster Uitgave bewerken.

1. Ga naar de **Hoofdmenu**.
1. Klikken **Projecten** klikt u vervolgens op de naam van een project om het project te openen.
1. (Optioneel) Klik op **Taken** klikt u vervolgens op de naam van een taak om de taak te openen.
1. Klikken **Problemen** in het linkerdeelvenster.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. (Optioneel) Als u de beperkte informatie over een uitgave wilt bewerken, klikt u op **Probleemdetails** in het linkerdeelvenster.

   ![](assets/qs-issue-details-icon-highlighted-and-expanded-on-issue-350x206.png)

   >[!NOTE]
   >
   >Afhankelijk van de manier waarop uw Workfront-beheerder of groepsbeheerder uw lay-outsjabloon heeft gewijzigd, kunnen de velden in het gebied Details van uitgave opnieuw worden gerangschikt of niet worden weergegeven. Zie voor meer informatie [De weergave Details aanpassen met een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Ga als volgt te werk om de gegevens in de sectie Details te bewerken:

   1. (Optioneel) Klik op de knop **Alles samenvouwen** om alle gebieden samen te vouwen.
   1. (Optioneel en voorwaardelijk) Klik op het pictogram **pijl-rechts** ![](assets/right-pointing-arrow.png) naast elk gebied om het gebied uit te breiden u wilt uitgeven.
   1. (Optioneel) Als u een aangepast formulier wilt bijvoegen, typt u de naam van een formulier in het dialoogvenster **Aangepast formulier toevoegen** , selecteert u het veld wanneer het wordt weergegeven in de lijst en klikt u vervolgens op **Wijzigingen opslaan**.
   1. (Optioneel) Klik op de knop **Exporteren** pictogram ![](assets/export.png) als u het overzicht en de aangepaste formuliergegevens wilt exporteren naar een PDF-bestand, klikt u op **Exporteren**. Selecteer een van de volgende opties:

      * Alles selecteren (wordt alleen weergegeven als er ten minste één aangepast formulier is gekoppeld)
      * Overzicht
      * De naam van een of meerdere aangepaste formulieren

      Het PDF-bestand wordt naar de computer gedownload.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Zie voor meer informatie [Aangepaste formulieren en objectdetails exporteren](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

   Voor informatie over de velden die zichtbaar zijn in de sectie Details van uitgave, gaat u verder met het bewerken van het probleem in het venster Uitgave bewerken, zoals hieronder beschreven.

1. Als u alle informatie over een uitgave wilt bewerken, selecteert u een uitgave in een lijst en klikt u op **Bewerken** boven aan de lijst

   of

   Klik op de naam van een uitgave in een lijst en klik vervolgens op de knop **Meer** menu naast de naam van de uitgave, en **Bewerken.**

   De **Probleem bewerken** wordt weergegeven.

   >[!IMPORTANT]
   >
   >U moet over beheerdersmachtigingen voor het probleem beschikken om de koppeling Bewerken te kunnen zien.

   Alle uitgiftevelden zijn beschikbaar in het vak Uitgave bewerken en zijn gegroepeerd op de gebieden in het linkerdeelvenster.

1. Overweeg informatie op te geven in een van de volgende secties:

   * [Naam van uitgave](#issue-name)
   * [Overzicht](#overview)
   * [Toewijzingen](#assignments)
   * [Aangepaste Forms](#Custom%C2%A0F)
   * [Instellingen](#settings)

   >[!NOTE]
   >
   >Afhankelijk van de manier waarop uw Workfront-beheerder onze lay-outsjabloon instelt, kunnen de velden in het vak Probleem bewerken verschillen in uw omgeving. Zie voor meer informatie [De weergave Details aanpassen met een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
   >
   >De meeste velden in de onderstaande secties zijn ook toegankelijk vanuit het vak Nieuwe uitgave wanneer u een uitgave maakt. De secties waaronder de velden zich bevinden, komen niet overeen met het vak Nieuwe uitgave. Voor informatie over het maken van problemen raadpleegt u [Problemen maken](../../issues/manage-issues/create-issues.md).

### Naam van uitgave {#issue-name}

1. Bewerk een uitgave zoals hierboven beschreven.
1. Klikken **Naam van uitgave**.

   ![](assets/issue-name-section-edit-issue-box-nwe-350x127.png)

1. Werk de **Naam van uitgave** veld.
1. Klikken **Opslaan** of ga door met het bewerken van de volgende secties.

### Overzicht {#overview}

1. Bewerk een uitgave zoals hierboven beschreven.
1. Klikken **Overzicht**.

   ![](assets/overview-section-edit-issue-box-nwe-350x284.png)

1. Werk of herzie om het even welke gebieden in de volgende lijst bij:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td> <p>Voeg aanvullende informatie toe over het probleem.</p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader">Sectie Basisinformatie</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td> <p>Selecteer de status van de uitgave. Zie voor meer informatie over uitgiftestatussen <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Toegang krijgen tot de lijst met systeemuitgiftestatussen</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prioriteit</td> 
      <td> <p>Dit is een visuele vlag voor u die u toestaat om kwesties voorrang te geven.</p> <p>Selecteer een van de volgende opties:</p> 
       <ul> 
        <li> <p><strong>Geen</strong> </p> </li> 
        <li> <p><strong>Laag</strong> </p> </li> 
        <li> <p><strong>Normaal</strong> </p> </li> 
        <li> <p><strong>Hoog</strong> </p> </li> 
        <li> <p><strong>Dringend</strong> </p> </li> 
       </ul> <p>Afhankelijk van de projectvoorkeuren die door uw Workfront-beheerder zijn geselecteerd, kunnen de namen van prioriteiten voor u anders zijn. Voor meer informatie over het uitgeven van prioriteiten, zie <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Prioriteiten maken en aanpassen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ernst</td> 
      <td> <p>Dit is een visuele markering die aangeeft hoe ernstig het probleem is dat in het probleem wordt beschreven. Ernsten zijn specifiek voor problemen. Selecteer een van de volgende opties:</p> 
       <ul> 
        <li> <p style="font-weight: bold;">Cosmetisch</p> </li> 
        <li> <p style="font-weight: bold;">Verwardheid</p> </li> 
        <li> <p style="font-weight: bold;">Fout met tijdelijke oplossing</p> </li> 
        <li> <p style="font-weight: bold;">Fout zonder tijdelijke oplossing</p> </li> 
        <li> <p style="font-weight: bold;">Fatale fout</p> </li> 
       </ul> <p>Afhankelijk van de projectvoorkeuren die door uw Workfront-beheerder zijn geselecteerd, kunnen de namen van de bestandscontroles voor u anders zijn. Voor meer informatie over het bewerken van bestandsversies raadpleegt u <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md" class="MCXref xref">Uitgiftecontroles maken of aanpassen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>Typ een webkoppeling die betrekking heeft op de informatie over de uitgave.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type</td> 
      <td> <p>Volgens de Eigenschappen van de Rij die door uw projectmanager op het gebied van de Details van de Rij van het project worden geselecteerd, zou u het type van de kwestie kunnen specificeren. Selecteer een van de volgende opties in het dialoogvenster <b>Type</b> vervolgkeuzelijst: </p> 
       <ul> 
        <li> <p><strong>Foutrapport</strong> </p> </li> 
        <li> <p><strong>Volgorde wijzigen</strong> </p> </li> 
        <li> <p><strong>Probleem</strong> </p> </li> 
        <li> <p><strong>Verzoek</strong> </p> </li> 
       </ul> <p>Afhankelijk van de projectvoorkeuren die door uw Workfront-beheerder zijn geselecteerd, kunnen de namen van de typen problemen voor u verschillen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Primaire contactpersoon</td> 
      <td>Standaard is de primaire contactpersoon de maker van de uitgave. Als u dit wilt wijzigen, typt u de naam van een actieve gebruiker in Workfront en selecteert u deze in de lijst. Een kwestie kan slechts één Primaire Contact hebben.<br> Als u de primaire contactpersoon wijzigt, heeft de oorspronkelijke primaire contactpersoon nog steeds beheertoegang tot het probleem. U moet deze toegang uit het vakje van de Toegang van de Uitgave manueel verwijderen, wanneer het delen van een kwestie.

   <b>TIP</b>

   <p>Wanneer u een gebruiker van een primaire contactpersoon toevoegt, ziet u de avatar, de primaire rol van de gebruiker en hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen. Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt.</p>
      <p> De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md">Toegang verlenen aan gebruikers</a>.</p>


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Datum en tijd vastleggen</td> 
      <td> <p>Dit is de datum waarop de ontvanger van de uitgifte schat dat de uitgifte zal worden voltooid. Alleen toegewezen personen kunnen dit veld bewerken.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplande begindatum</td> 
      <td>Standaard is de geplande begindatum de datum en het tijdstip waarop de uitgave is gemaakt. U kunt de <strong>Geplande begindatum</strong> van de kwestie. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplande voltooiing Datum en tijd</td> 
      <td> Standaard is de geplande aanmaakdatum 24 uur na de standaardbegindatum. Standaard hebben uitgaven een Duur van 1 dag. U kunt de <strong>Geplande afsluitdatum</strong> van de kwestie.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Begindatum en -tijd</td> 
      <td>De werkelijke begindatum wordt automatisch ingevuld wanneer u de status van de uitgave wijzigt in <strong>In uitvoering</strong>. U kunt de <strong>Werkelijke begindatum</strong> van de kwestie. U kunt de datum desgewenst handmatig bijwerken. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werkelijke einddatum en -tijd</td> 
      <td>De datum van feitelijke voltooiing wordt automatisch ingevuld wanneer u de status van de uitgave wijzigt in <strong>Gesloten</strong> of<strong>Opgelost</strong>. U kunt de <strong>Werkelijke afsluitdatum</strong> voor de kwestie. U kunt de datum desgewenst handmatig bijwerken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Opgelost door</td> 
      <td> <p>Dit toont of de kwestie door een ander voorwerp wordt opgelost. U kunt selecteren of deze kwestie door een taak, een project, of een andere kwestie van het drop-down menu wordt opgelost, dan begin de naam van de taak, het project, of de kwestie te typen die de kwestie zal oplossen. Selecteer het wanneer het in de lijst verschijnt.</p>

   <b>OPMERKING</b>

   Wanneer u een object selecteert om een probleem op te lossen, is de status van het probleem gekoppeld aan de status van het object dat het probleem oplost en kan deze status niet worden gewijzigd. Zie voor meer informatie over het omzetten van objecten <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overzicht van Oplossende en Oplosbare objecten </a>.

   <b>TIP</b>

   Wanneer uw systeem of groepsbeheerder het veld &quot;Opgelost door&quot; toevoegt aan een aangepaste koptekst voor uitgaven, verandert het veld in &quot;Probleem oplossen&quot;, &quot;Taak oplossen&quot; of &quot;Project oplossen&quot; wanneer er een object is dat is gekoppeld aan de kwestie.

   U kunt dit veld niet bewerken wanneer het wordt weergegeven in de uitgiftheader. Voor meer informatie over het aanpassen van uitgiftekopballen, zie <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md">Objectkoppen aanpassen met een lay-outsjabloon </a>
   </td> 
     </tr>

   <tr> 
      <td role="rowheader">Probleem oplossen, Taak oplossen of Project oplossen</td> 
      <td>De gekoppelde naam van het probleem, de taak of het probleem dat het probleem verhelpt.  </td> 
     </tr> 
      <tr> 
      <td role="rowheader">Deze oplossingen</td> 
      <td>De gekoppelde naam van het probleem dat wordt voltooid wanneer het probleem dat u opent, is opgelost.  </td> 
     </tr>


   </tbody> 
   </table>





1. Klikken **Opslaan** of ga door met het bewerken van de volgende secties.

#### Toewijzingen {#assignments}

1. Bewerk de uitgave zoals hierboven beschreven.
1. Klikken **Toewijzingen** in het linkerdeelvenster.

   ![](assets/assignments-section-edit-issue-box-nwe-350x230.png)

1. Klikken **Personen, rollen en teams zoeken** en begint de naam van een gebruiker, een rol, of een team te typen die u aan de taak wilt toewijzen, dan het klikken of drukken binnengaan wanneer het op de lijst toont.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this is still called this; asked Anna to change it to "roles" and add a comma)</p>
   -->

   >[!NOTE]
   >
   >Als de naam van de gebruiker een speciaal teken bevat, moet u het speciale teken in het zoekveld opnemen.

   >[!TIP]
   >
   >U kunt meerdere gebruikers, taakrollen of teams toewijzen. U kunt alleen actieve gebruikers, taakrollen en teams toewijzen.
   >
   >
   >Als een gebruiker, een baanrol, of een team werden toegewezen alvorens zij werden gedeactiveerd, blijven zij toegewezen aan het het werkpunt. In dit geval raden we het volgende aan:
   >
   >* Wijs het werkitem opnieuw toe aan actieve bronnen.
   >* Koppel de gebruikers in een gedeactiveerd team aan een actief team en wijs het het werkpunt aan het actieve team opnieuw toe.

1. (Optioneel) Geef aan of een verkrijger de primaire verkrijger is in verband met de kwestie door de aanwijzer boven de naam van de verkrijger te houden en op **Primair maken**. Een team kan niet de primaire ontvanger van een kwestie zijn.
1. Werk de volgende velden bij:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Geplande uren</td> 
      <td> <p>Dit is de hoeveelheid tijd die het werkelijk nodig zou hebben om de taken van de Commissie af te ronden. Typ het aantal geplande uren voor de uitgave.<br></p> <p>Opmerking: als u de geplande uren van de uitgave wijzigt, blijft de geplande afwerkingsdatum ongewijzigd. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Rol van de gemachtigde</td> 
      <td> <p>Selecteer een rol in het menu <strong>Rol van de gemachtigde</strong> vervolgkeuzemenu wanneer u een persoon als ontvanger hebt geselecteerd. Dit is de rol die de verkrijger op dit punt kan vervullen. </p> <p><b>TIP</b>

   Alleen de functies die aan elke toegewezen persoon in het profiel zijn gekoppeld, worden weergegeven in het vervolgkeuzemenu.</p> </td>
   </tr> 
    </tbody> 
   </table>

1. Klikken **Opslaan** of ga door met het bewerken van de volgende secties.

### Aangepaste Forms

1. Bewerk een uitgave zoals hierboven beschreven.
1. Klikken **Aangepaste Forms**.

   ![](assets/custom-forms-section-edit-issue-box-nwe-350x132.png)

1. In de **Aangepast formulier toevoegen** selecteert u het aangepaste formulier of de formulieren die u aan de uitgave wilt koppelen. U moet aangepaste formulieren maken voordat u ze in dit veld kunt selecteren. Alleen actieve aangepaste formulieren worden in de lijst weergegeven. Zie voor meer informatie over het samenstellen van aangepaste formulieren [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). U kunt maximaal tien aangepaste formulieren toevoegen aan een uitgave.

1. (Voorwaardelijk) Als u een aangepast formulier aan de uitgave hebt gekoppeld, bewerkt u alle velden op het formulier. U moet alle vereiste velden opgeven voordat u de uitgave kunt opslaan.

   >[!NOTE]
   >
   >Afhankelijk van de manier waarop uw Workfront-beheerder de machtigingen voor de secties in uw aangepaste formulier instelt, kan niet iedereen dezelfde velden op een aangepast formulier weergeven of bewerken. De machtigingen voor het bewerken van velden in een sectie van een aangepast formulier zijn afhankelijk van de machtigingen die u hebt voor de uitgave zelf. Zie voor informatie over het instellen van machtigingen voor secties in een aangepast formulier [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). Zie voor informatie over het instellen van machtigingen voor uitgaven [Een uitgave delen](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

1. Klikken **Opslaan** of ga door met het bewerken van de volgende sectie.

### Instellingen {#settings}

1. Bewerk een uitgave zoals hierboven beschreven.
1. Klikken **Instellingen**.

   ![](assets/settings-section-edit-issue-box-nwe-350x240.png)

   Werk de volgende gegevens bij:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Goedkeuringsproces</td> 
      <td> 
       <div> 
       <p>Selecteer een goedkeuringsproces dat u met de kwestie wilt associëren. Uw Workfront-beheerder moet goedkeuringsprocessen op systeemniveau definiëren voordat u deze aan problemen kunt koppelen. Gebruikers met administratieve toegang tot goedkeuringsprocessen <span> U kunt ook groepsspecifieke goedkeuringsprocessen maken.</span>Ga voor meer informatie over het maken van goedkeuringsprocessen naar <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Een goedkeuringsproces voor werkitems maken</a>. </p> 
       <p>Houd rekening met het volgende wanneer u goedkeuringsprocessen toevoegt: </p> 
       <ul> 
       <li>Alleen actieve goedkeuringsprocessen worden in de lijst weergegeven. </li> 
       <li> <p>Systeemspecifieke en groepsspecifieke goedkeuringsprocessen worden in de lijst weergegeven. Een goedkeuringsproces verbonden aan een groep buiten die van het project toont niet in de lijst.</p> <p>Belangrijk: als de groep van het project verandert, wordt het groepsspecifieke goedkeuringsproces een goedkeuringsproces voor eenmalig gebruik. Voor meer informatie over hoe de veranderingen in de groep van het project of de veranderingen in het goedkeuringsproces goedkeuringsmontages beïnvloeden, zie <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">De invloed van wijzigingen in groep- en goedkeuringsproces op toegewezen goedkeuringsprocessen</a>. </p> </li> 
       <li> <p>U kunt standaardgoedkeuringsprocessen bepalen die automatisch aan kwesties moeten worden vastgemaakt wanneer het creëren van verzoekrijen of de Onderwerpen van de Rij. Voor informatie over het bijwerken van de Details van de Rij, zie <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Een aanvraagwachtrij maken</a>. Voor informatie over het creëren van de Onderwerpen van de Rij, zie <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Werkvoorraadonderwerpen maken</a>. </p> </li> 
       <li>Bij problemen met bulkbewerking bestaan de volgende scenario's: 
       <ul> 
       <li><p>Wanneer u meerdere problemen van dezelfde groep selecteert, worden zowel systeemspecifieke als groepsspecifieke goedkeuringsprocessen in dit veld weergegeven.</p></li> 
       <li><p>Wanneer u meerdere problemen selecteert uit verschillende groepen, worden alleen goedkeuringsprocessen op systeemniveau weergegeven in dit veld.</p></li> 
       <li><p>Als voor een van de problemen een goedkeuringsproces voor eenmalig gebruik is gekoppeld, wordt dit vervangen door het goedkeuringsproces op systeemniveau of groepsniveau dat u selecteert. </p></li> 
       </ul></li> 
       </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Herinneringsmeldingen</td> 
      <td> <p>Schakel het selectievakje in waarvoor meldingen voor herinneringen die u aan deze uitgave wilt toevoegen. Alle herinneringsmeldingen voor problemen worden weergegeven. Uw Workfront-beheerder moet Herinneringsmeldingen configureren voordat u deze op een uitgave kunt selecteren. Zie voor meer informatie over het configureren van Herinneringsmeldingen de informatie <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Herinneringsmeldingen instellen</a></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Opslaan.**

## Een probleem bewerken in de uitgaveheader (beperkt)

U kunt een beperkte hoeveelheid informatie in de uitgiftheader bewerken.

Uw systeem- of groepsbeheerder kan de velden die u in de uitgiftekop ziet, aanpassen. Zie voor meer informatie [Objectkoppen aanpassen met een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

![](assets/issue-header-350x19.png)

De volgende velden worden standaard opgenomen in de uitgiftheader:

* Naam van uitgave
* Percentage voltooid
* Toewijzingen
* Geplande voltooiing Datum en tijd
* Status
* Goedkeuringsbeslissingen nemen als u in een huidig goedkeuringsproces als fiatteur bent ingesteld
