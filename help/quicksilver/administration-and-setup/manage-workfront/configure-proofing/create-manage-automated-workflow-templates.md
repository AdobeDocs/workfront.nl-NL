---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Geautomatiseerde workflowsjablonen maken en beheren
description: Als beheerder van Adobe Workfront, als het proces van het inhoudsherzicht van uw organisatie vaak wordt herhaald of de inhoud vaak door de zelfde mensen wordt herzien, kunt u Geautomatiseerde malplaatjes van het Werkschema tot stand brengen die die recensenten met proefrollen en berichtmontages bevatten die u specificeert. Een Geautomatiseerde malplaatje van het Werkschema kan eenvoudig met slechts één of twee recensenten of complex met vele stadia en gebiedsdelen zijn.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '2075'
ht-degree: 0%

---

# Geautomatiseerde workflowsjablonen maken en beheren

<!-- Audited: 2/2024 -->

Als beheerder van Adobe Workfront, als het proces van het inhoudsherzicht van uw organisatie vaak wordt herhaald of de inhoud vaak door de zelfde mensen wordt herzien, kunt u Geautomatiseerde malplaatjes van het Werkschema tot stand brengen die die recensenten met proefrollen en berichtmontages bevatten die u specificeert. Een Geautomatiseerde malplaatje van het Werkschema kan eenvoudig met slechts één of twee recensenten of complex met vele stadia en gebiedsdelen zijn.

Geautomatiseerde werkstroomsjablonen maken het eenvoudig om een proefdruk te maken met behulp van een geautomatiseerde workflow. Wanneer een gebruiker een proef creeert, kiezen zij eenvoudig het malplaatje zij nodig hebben.

U kunt op elk gewenst moment eenvoudig elke automatische werkstroomsjabloon wijzigen, zodat revisoren en fasen kunnen worden toegevoegd of verwijderd. Proefmakers die de sjabloon gebruiken, kunnen revisoren toevoegen of verwijderen voor de proefdruk.

Overweeg het volgende wanneer u een Geautomatiseerde malplaatje van het Werkschema gebruikt:

1. De instellingen van een automatische werkstroomsjabloon bepalen wat u kunt doen met de geautomatiseerde workflow voor een proefdruk. Als de knop Een werkgebied toevoegen bijvoorbeeld is uitgeschakeld in de sjabloon, is deze niet zichtbaar wanneer u werkt met de instellingen voor Geautomatiseerde workflow voor de proefdruk.
1. Wanneer een persoon wordt toegevoegd aan een werkgebied in een Geautomatiseerde malplaatje van het Werkschema, maar ook reeds als recensent op het bewijs aanwezig is, verwijdert het toepassen van het malplaatje de recensent uit het stadium. Als u geen andere revisor aan het werkgebied toevoegt, wordt u in een bericht gevraagd er een toe te voegen.
1. Uw vermogen om een Geautomatiseerde malplaatje van het Werkschema te wijzigen hangt van de malplaatjemontages af die door de beheerder van Workfront worden gevormd, zoals die in wordt beschreven. Als de mogelijkheid om de sjabloon te wijzigen is uitgeschakeld, kan alleen de eigenaar van de sjabloon deze wijzigen.

Voor informatie over Geautomatiseerde Werkstromen, zie [ Geautomatiseerd overzicht van het Werkschema ](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Nieuw: alle</p><p>Huidig: Pro of hoger</p><p>Verouderd: Premium of Selecteren</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref"> Toegang tot het proefdrukken van functionaliteit in Workfront </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Nieuw: Standaard</p><p>Huidig: Werk of Plan</p> <p>Verouderd: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Beheerder moet zijn geselecteerd in het machtigingsprofiel voor proefdrukken. </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een automatische werkstroomsjabloon maken

{{step1-to-proofing}}

1. Klik **Werkschema&#39;s** in het linkerpaneel.
1. Op het **lusje van het Werkschema**, klik **Nieuw** > **Nieuw malplaatje**.

1. In de **sectie van Details**, specificeer de volgende informatie:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sjabloonnaam</td> 
      <td>(Vereist) Typ een naam voor de sjabloon. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eigenaar van sjabloon</td> 
      <td>U kunt de Workfront-beheerder of de Workfront Proof-beheerder selecteren die de sjabloon zal beheren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sjabloongroep</td> 
      <td> <p> Als de geautomatiseerde workflows van uw organisatie zijn ingedeeld in groepen, kunt u de naam van de groep selecteren. Zie <a href="#create-automated-workflow-template-groups" class="MCXref xref"> de Geautomatiseerde groepen van het malplaatje van het Werkschema </a> later in dit artikel voor meer informatie creëren.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Tijdzone sjabloon </td> 
      <td> <p>De standaardtijdzone voor de sjabloon is de tijdzone waarin u werkt. Als de tijdzone van de makers en revisoren van de proefdrukken die de sjabloon zullen gebruiken anders is, kunt u deze hier wijzigen om ervoor te zorgen dat de tijdslimieten van het werkgebied op de juiste tijden voor deze gebruikers worden ingesteld. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Toestaan</td> 
      <td> <p>U kunt de werkgebiedactiviteiten selecteren die beschikbaar zijn voor de persoon die proefdrukken maakt met de sjabloon.</p> 
      <p><b> WAARSCHUWING </b>: Als u niet de opties selecteert voeg een stadium toe en voeg mensen aan stadia toe, noch zal de malplaatjeeigenaar noch de eigenaar van om het even welke proef gebruikend dit malplaatje een stadium kunnen toevoegen of de proef delen. 
      </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. In de **sectie van Staven**, vorm elk stadium van het Geautomatiseerde malplaatje van het Werkschema.

   U kunt meerdere fasen toevoegen en er tussenin maken.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Naam</td> 
      <td> <p>De naam van het werkgebied wordt weergegeven in het geautomatiseerde workflowdiagram boven aan de sectie Workflow, op de pagina Proefgegevens en in de e-mailmeldingen die naar revisoren worden verzonden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werkgebied activeren</td> 
      <td> <p>Geef op of het werkgebied automatisch of handmatig wordt geactiveerd. Voor het eerste stadium, kunt u <strong> op proefverwezenlijking </strong> selecteren, <strong> op een specifieke datum en tijd </strong>, of <strong> manueel </strong>.</p> <p>De andere opties worden beschikbaar wanneer u een tweede werkgebied toevoegt, omdat u een hoofdwerkgebied moet selecteren. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Termijn berekend op basis van</td> 
      <td> <p>Geef op hoe de deadline moet worden berekend:</p> 
       <ul> 
        <li> <p><strong> creatie van het Bewijs </strong>: In de drop-down lijst onder <strong> Deadline (+ werkdagen) </strong>, selecteer het aantal bedrijfsdagen u aan de datum van de proefverwezenlijking wilt toevoegen om een termijn op de proef automatisch te plaatsen.</p> </li> 
        <li><strong> wanneer het stadium </strong> begint: In de drop-down lijst onder <strong> Deadline (+ bedrijfsdagen) </strong>, selecteer het aantal bedrijfsdagen u aan de datum van de werkgebiedactivering wilt toevoegen om een termijn op de proef automatisch te plaatsen.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werkgebied vergrendelen</td> 
      <td>Geef op of u het werkgebied wilt vergrendelen voor opmerkingen. U kunt een werkgebied handmatig of automatisch vergrendelen wanneer het volgende werkgebied wordt gestart of wanneer alle beslissingen in het bovenliggende werkgebied worden genomen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Primaire beslisser</td> 
      <td> <p>De beschikbare besluitvormers worden pas in de lijst weergegeven nadat u de controleurs aan het werkgebied hebt toegevoegd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Slechts één besluit vereist</td> 
      <td>Het evaluatieproces voor de fase zal worden afgerond zodra een van de besluitvormers zijn besluit indient. Voor meer informatie, zie <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref"> de Montages van het Bewijs in Workfront Proof </a> vormen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Privéstadium</td> 
      <td>Hiermee verbergt u opmerkingen en beslissingen van personen die niet aan het werkgebied zijn toegevoegd of die geen Workfront-beheerder zijn. Voor meer informatie, zie <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref"> Geautomatiseerd overzicht van het Werkschema </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dit werkgebied niet verwijderen</td> 
      <td> <p>Maakt het werkgebied verplicht.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Als de proefdrukken die deze sjabloon zullen gebruiken altijd naar dezelfde personen in het werkgebied worden verzonden, voegt u ze hier toe zodat gebruikers ze niet hoeven toe te voegen telkens wanneer ze een proefdruk maken.

   Kies de Rol van elke persoon **** op de proeven die dit malplaatje en het **E-mailalarm** zullen gebruiken u de gebruiker wilt ontvangen wanneer het werken aan proeven die dit malplaatje gebruiken.

   Voor informatie over rollen op een proef, zie [ standaard het proef rollen ](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) vormen. Voor informatie over proefe-mailalarm, zie sectie [ proefdrukgebreken voor een gebruiker ](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) in het artikel [ vormen e-mailberichtmontages in Workfront Proof ](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Elke gebruiker kan slechts aan één stadium worden toegevoegd. U kunt zoveel gebruikers toevoegen als u aan een werkgebied wilt.

   >[!TIP]
   >
   >U kunt de namen van revisoren slepen en neerzetten tussen de fasen in het stappendiagram. De beschikbare stadia worden in blauw gemarkeerd.

1. Herhaal de twee vorige stappen voor alle andere stappen die u aan de sjabloon wilt toevoegen.

   Bij de bovenkant van de **sectie van het Werkschema**, kunt u een diagram van het Geautomatiseerde Werkschema zien u opstelling. Aangezien u stadia blijft toevoegen, verschijnen zij op het diagram met lijnen die de gebiedsdelen tussen hen tonen. U kunt op een werkgebied in het diagram klikken om de instellingen voor dat werkgebied weer te geven.

   Als u niet het diagram moet zien, kunt u **Diagram van de Verbergen** klikken.

1. In het **malplaatje van het Aandeel met** sectie, klik een optie (als het malplaatje niet reeds met de volledige organisatie wordt gedeeld) om te specificeren wie het zal kunnen gebruiken.

   Standaard worden nieuwe automatische workflowsjablonen gedeeld met iedereen in uw organisatie.

1. Klik **creëren**.

## Een automatische werkstroomsjabloon wijzigen

Als Workfront Proof-beheerder kunt u een automatische werkstroomsjabloon wijzigen. Uw wijzigingen worden automatisch opgeslagen wanneer u ze aanbrengt.

{{step1-to-proofing}}

1. Klik **Werkschema&#39;s** in het linkerpaneel.
1. In de **malplaatjes van het Werkschema** lijst die verschijnt, klik het malplaatje u wilt wijzigen.
1. In de **sectie van Details**, specificeer de volgende informatie:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sjabloonnaam</td> 
      <td>(Vereist) Typ een naam voor de sjabloon. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eigenaar van sjabloon</td> 
      <td>U kunt de Workfront-beheerder of de Workfront Proof-beheerder selecteren die de sjabloon zal beheren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sjabloongroep</td> 
      <td> <p> Als de geautomatiseerde workflows van uw organisatie zijn ingedeeld in groepen, kunt u de naam van de groep selecteren. Zie <a href="#create-automated-workflow-template-groups" class="MCXref xref"> de Geautomatiseerde groepen van het malplaatje van het Werkschema </a> later in dit artikel voor meer informatie creëren.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tijdzone sjabloon </td> 
      <td> <p>De standaardtijdzone voor de sjabloon is de tijdzone waarin u werkt. Als de tijdzone van de makers en revisoren van de proefdrukken die de sjabloon zullen gebruiken anders is, kunt u deze hier wijzigen om ervoor te zorgen dat de tijdslimieten van het werkgebied op de juiste tijden voor deze gebruikers worden ingesteld. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Toestaan</td> 
      <td> <p>Selecteer de werkgebiedactiviteiten die beschikbaar moeten zijn voor diegenen die proefdrukken maken met de sjabloon. </p> <p><b> WAARSCHUWING </b>: Als u niet de opties selecteert voeg een stadium toe en voeg mensen aan stadia toe, noch zal de malplaatjeeigenaar noch de eigenaar van om het even welke proef gebruikend dit malplaatje een stadium kunnen toevoegen of de proef delen.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. In de **sectie van het Werkschema**, verander de naam van om het even welk stadium en breid het montages ![](assets/arrow-button.png) uit om het even welke noodzakelijke veranderingen aan te brengen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Termijn berekend op basis van</td> 
      <td> <p>Geef op hoe de deadline moet worden berekend:</p> 
       <ul> 
        <li> <p><strong> Deadline die van proefverwezenlijking </strong> wordt berekend: In de <strong> plaats de drop-down lijst van de einddatum van het werkgebied </strong>, selecteer het aantal bedrijfsdagen u aan de datum van de proefverwezenlijking wilt toevoegen om een termijn op de proef automatisch te plaatsen.</p> </li> 
        <li><strong> Deadline die van werkgebiedactivering </strong> wordt berekend: In <strong> plaats de 3} drop-down lijst van de werkgebieddeadline {, selecteer het aantal bedrijfsdagen u aan de datum van de werkgebiedactivering wilt toevoegen om een termijn op de proef automatisch te plaatsen.</strong></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werkgebied activeren</td> 
      <td> <p>Geef op of het werkgebied automatisch of handmatig wordt geactiveerd. Voor het eerste stadium, kunt u <strong> op proefverwezenlijking </strong> selecteren, <strong> op een specifieke datum en tijd </strong>, of <strong> manueel </strong>.</p> <p>De andere opties worden beschikbaar wanneer u een tweede werkgebied toevoegt, omdat u een hoofdwerkgebied moet selecteren. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werkgebied vergrendelen</td> 
      <td>Geef op of u het werkgebied wilt vergrendelen voor opmerkingen. U kunt een werkgebied handmatig of automatisch vergrendelen wanneer het volgende werkgebied wordt gestart of wanneer alle beslissingen in het bovenliggende werkgebied worden genomen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Besluit</td> 
      <td>Beëindigt de fase de eerste keer dat een van de besluitvormers zijn besluit indient. Voor meer informatie, zie <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref"> de Montages van het Bewijs in Workfront Proof </a> vormen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Privacy</td> 
      <td>Hiermee verbergt u opmerkingen en beslissingen van personen die niet aan het werkgebied zijn toegevoegd of die geen toezichthouder of hoger in de account zijn. Voor meer informatie, zie <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref"> Geautomatiseerd overzicht van het Werkschema </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werkgebied verwijderen</td> 
      <td>Maakt het werkgebied verplicht.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Meer <img src="assets/more-icon.png"></td> 
      <td>Revisoren toevoegen aan het werkgebied of het werkgebied verwijderen.<p>Als elk van uw proefdrukken naar dezelfde personen in een bepaald werkgebied wordt verzonden, kunt u hun namen hier opgeven, zodat u ze niet telkens opnieuw hoeft toe te voegen wanneer u een proefdruk maakt. Het type en selecteert de naam van een gebruiker u aan het stadium wilt toevoegen, dan hun <strong> Rol </strong> op de proef en <strong> e-mailalarm </strong> montages toevoegen u voor de gebruiker wilt. Voor informatie over het proefdrukken van rollen, zie <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref"> standaard het proefdrukken rollen </a> vormen. Voor informatie over proefe-mailalarm, zie sectie <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref"> proefdrukgebreken voor een gebruiker </a> in het artikel <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref"> vormen e-mailberichtmontages in Workfront Proof </a>.</p><p>U kunt zoveel gebruikers toevoegen als u wilt in een werkgebied</p><p>Tip: u kunt de namen van revisoren slepen en neerzetten tussen de stappen in het stappendiagram. De beschikbare stadia worden in blauw gemarkeerd.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Herhaal de stap voor alle andere stappen die u aan de sjabloon wilt toevoegen.

   Bij de bovenkant van de **sectie van het Werkschema**, kunt u een diagram van het Geautomatiseerde Werkschema zien u opstelling. Aangezien u stadia blijft toevoegen, verschijnen zij op het diagram met lijnen die de gebiedsdelen tussen hen tonen. U kunt op een werkgebied in het diagram klikken om de instellingen voor dat werkgebied weer te geven.

   Als u niet het diagram moet zien, kunt u **Diagram van de Verbergen** klikken.

1. In **Gedeeld met** sectie, als u een gebruiker wilt schrappen, klik de Meer ![](assets/more-icon.png) knoop aan het recht, dan klik **verwijderen**.

## Geautomatiseerde workflowsjabloongroepen maken {#create-automated-workflow-template-groups}

Als Workfront-beheerder kunt u alle sjablonen voor geautomatiseerde workflow in de account van uw organisatie weergeven en beheren. Het kan handig zijn om sjablonen in groepen in te delen.

Een automatische sjabloongroep voor werkstromen maken:

{{step1-to-proofing}}

1. Klik **Werkschema&#39;s** in het linkerpaneel.
1. Op het **lusje van het Werkschema**, klik **Nieuw** > **Nieuwe malplaatjegroep**.
1. Typ een beschrijvende naam voor de nieuwe malplaatjegroep, dan druk **gaat** binnen.

U kunt de sjablonen tussen groepen verplaatsen door te slepen en neer te zetten.

## Geautomatiseerde workflowsjablonen beheren

{{step1-to-proofing}}

1. In het linkerpaneel in Workfront Proof, klik **Werkschema&#39;s**.
1. Op de **pagina van Werkschema&#39;s** die verschijnt, doe om het even welke volgend:

   * Een nieuwe sjabloon toevoegen
   * Een nieuwe sjabloongroep toevoegen
   * Een of meer sjabloongroepen verwijderen
   * De details van een sjabloon openen
   * Sleep een sjabloon naar een andere sjabloongroep
