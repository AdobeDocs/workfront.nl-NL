---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Plan een automatische levering van rapporten
description: Plan een automatische levering van rapporten
author: Nolan
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 0%

---

# Plan een automatische levering van rapporten

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

U kunt rapporten plannen om automatisch aan gebruikers op een bepaald programma te leveren, of u kunt rapporten manueel één keer verzenden. Wanneer u een rapport van Adobe Workfront verzendt, ontvangt de gebruiker een e-mail met het Workfront-rapport in een aparte bijlage.

Zie voor meer informatie, waaronder groottebeperkingen die van invloed kunnen zijn op de levering van uw rapporten [Overzicht van levering rapporteren](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Toegangsvereisten

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

Voordat u begint, moet u een rapport maken. Ga voor meer informatie over het maken van rapporten naar [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Plan de levering van een rapport

Om een rapport voor automatische levering te plannen of een bestaande rapportlevering uit te geven of te schrappen: &#x200B;

1. Ga naar een rapport dat u voor levering wilt plannen.

   >[!NOTE]
   >
   >Rapportleveringen bevatten geen aanwijzingen. Als u gegevens in een rapportlevering wilt beperken, adviseren wij het toepassen van filters op het rapport dat u wilt verzenden.

1. Klikken **Handelingen rapporteren** vervolgens **Rapport verzenden**.

   De **Rapport verzenden** wordt weergegeven.

   >[!TIP]
   >
   >Als u een rapport op een bepaald moment handmatig wilt verzenden, gaat u naar het rapport en klikt u op **Handelingen rapporteren** > **Rapport verzenden** > **Nu verzenden**.

1. Selecteer **Herhalende leveringen** tab.
1. (Voorwaardelijk) om een bestaande herhalende rapportlevering te wijzigen, selecteer de rapportlevering in **Herhalende leveringen** sectie.
1. Geef de volgende informatie op:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Verzenden naar</p> </td> 
      <td> <p>Typ de naam van de gebruiker, groep, team of rol waarnaar u het rapport wilt verzenden en klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.</p> <p>of</p> <p>Geef het e-mailadres op van een persoon buiten het Workfront-systeem die toegang moet hebben tot het rapport.</p> <p>Herhaal dit proces om het rapport naar veelvoudige gebruikers, groepen, teams, of rollen te verzenden.</p> <p>Opmerking:  <p>Overweeg het volgende wanneer het toevoegen van de ontvangers van de rapportlevering:</p> 
        <ul> 
         <li>Als uw organisatie Workfront-berichten beperkt tot specifieke e-maildomeinen, kunt u rapporten alleen verzenden naar e-mailadressen die worden vermeld in de lijst van gewenste personen voor e-mail.<p>Voor informatie over hoe een beheerder van Workfront de e-maillijst van gewenste personen bijwerkt, zie de sectie <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">Uw e-maillijst van gewenste personen configureren</a>.</p></li> 
         <li> <p>Het toevoegen van een groot aantal gebruikers als ontvangers kan ertoe leiden dat de levering mislukt. Als u leveringsmislukkingen ervaart, kunt u veelvoudige rapportleveringen met kleinere groepen gebruikers plannen.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>E-mailonderwerp</p> </td> 
      <td> <p>Geef een onderwerp voor de e-mailmelding op.</p> <p>Standaard is het onderwerp van de e-mail:</p> <p><em>Workfront-rapport: [Naam van het rapport] [Datum]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>E-mailbericht</p> </td> 
      <td> <p>Geef een bericht op dat u in de e-mail wilt opnemen.</p> <p>Standaard is het e-mailbericht:</p> <p><em>Bijgevoegd is het [rapportfrequentie] rapport [Naam van het rapport] dat door Workfront op [Datum] wordt geproduceerd.</em> </p> <p>Opmerking: Voor rapporten die alleen als Excel-bestand worden geleverd, wordt het volgende bericht ook toegevoegd aan de e-mail: "Houd er rekening mee dat bij MS Excel-bestandstypen (XLS) een limiet geldt (65.530) voor het aantal hyperlinks dat door deze bestandstypen wordt ondersteund. Als u deze limieten overschrijdt, wordt het bestand niet geopend en wordt aangeraden het bestand opnieuw te verzenden zonder de hyperlinks. Gelieve te gaan terug naar de rapportplanner om hyperlinks te verwijderen en het rapport opnieuw te verzenden." "gelieve terug naar de rapportplanner"uitdrukking te gaan is een verbinding terug naar het rapport.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Dit rapport leveren met de toegangsrechten van</p> </td> 
      <td> <p>Typ de naam van een gebruiker die toegang heeft tot het rapport en klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst. De gebruikers die het rapport ontvangen zullen het zelfde niveau van toegang tot het rapport worden verleend zoals de gebruiker die u hier specificeert.<br> Zie voor meer informatie <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Een rapport uitvoeren en leveren met de toegangsrechten van een andere gebruiker</a>.</p> <p>Opmerking: Dit veld ondersteunt geen jokertekens. Bijvoorbeeld, die het vervangings$$User.ID gebruikt stelt niet het rapport met de toegangsrechten van de gebruiker in werking die het rapport ontvangt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Indeling</p> </td> 
      <td> <p>Selecteer het formaat u voor het geleverde rapport wilt:</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>Als u dit selecteert, kunt u de uitvoer opmaken met behulp van de extra <strong>Papierformaat</strong> en <strong>Afdrukstand</strong> opties die worden weergegeven.</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Inclusief koppelingen</p> </td> 
      <td> <p>Deze optie is alleen beschikbaar als <strong>MS Excel</strong> is geselecteerd in het dialoogvenster <strong>Indeling</strong> vervolgkeuzemenu. Als deze optie is ingeschakeld, worden alle hyperlinks opgenomen in het geëxporteerde Excel-document.</p> <p>Documenten die meer dan 65.530 koppelingen bevatten, kunnen niet worden geopend. Schakel deze optie uit als het geëxporteerde document meer dan 65.530 koppelingen bevat.</p> <p>Deze optie is standaard ingeschakeld.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Samenvatting</p> </td> 
      <td> <p>Toont een samenvatting van wanneer de levering zich herhaalt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Herhalen</p> </td> 
      <td> <p>Selecteer of het rapport dagelijks, wekelijks, maandelijks, of jaarlijks zou moeten worden geleverd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Herhaalt om de</p> </td> 
      <td> <p>Selecteer de frequentie waarmee u de levering wilt herhalen. De waarde die u voor deze optie selecteert, is gebaseerd op de optie die is geselecteerd in het dialoogvenster <strong>Herhalen</strong> vervolgkeuzelijst.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Tijd</p> </td> 
      <td> <p>Selecteer de tijd van de dag waarop de levering moet worden verzonden.</p> <p>Tip: Omdat de systeemladingen de tijden van de rapportlevering kunnen beïnvloeden, kan er een vertraging tussen de geplande tijd en de daadwerkelijke leveringstijd zijn. Als u een rapport nodig hebt dat tegen een specifieke tijd wordt geleverd, adviseren wij de levering voorafgaand aan de tijd te plannen dat het nodig is. Bijvoorbeeld, adviseren wij de levering een dag voorafgaand aan de datum te plannen wanneer het nodig is.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Herhaalt op</p> </td> 
      <td> <p>Deze optie is beschikbaar als de optie <strong>Herhalen</strong> optie is ingesteld op <strong>Wekelijks</strong> of <strong>Maandelijks</strong>:</p> 
       <ul> 
        <li> <p>Wanneer de <strong>Herhalen</strong> optie is ingesteld op <strong>Wekelijks</strong>: Selecteer de dagen van de week waarin de levering wordt verzonden.</p> </li> 
        <li> <p>Wanneer de <strong>Herhalen</strong> optie is ingesteld op <strong>Maandelijks</strong>: Selecteer of de levering wordt verzonden op de dag van de maand, de dag van de week, of de laatste dag van de maand (deze opties beïnvloeden de datum die u in selecteert <strong>Begint op</strong> veld).</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Begint op</p> </td> 
      <td>Selecteer de datum waarop de geplande levering moet beginnen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Eindigt op</p> </td> 
      <td>Selecteer een datum voor de geplande levering aan eind.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Nooit</p> </td> 
      <td>Selecteren <strong>Nooit</strong> als u wilt dat de geplande levering eindeloos duurt.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Opslaan** om de rapportlevering te bewaren.

   Het rapport wordt weergegeven in het dialoogvenster **Herhalende leveringen** in de **Rapport verzenden** ) en wordt op het geplande tijdstip verzonden.

   Zie de secties voor informatie over groottebeperkingen die de aflevering van rapporten kunnen beïnvloeden [Leveringslimieten rapporteren](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) en [Exportlimieten](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

1. (Optioneel) Een geplande levering verwijderen:

   1. In de **Herhalende leveringen** klikt u op de geplande levering en vervolgens klikt u op **Verwijderen**.
   1. Klikken **Verwijderen** ter bevestiging.

## Video doorlopen

Bekijk de volgende video om te leren hoe te om een rapportlevering te plannen. Deze video is opgenomen in Workfront Classic. De inhoud is echter ook van toepassing op de nieuwe Workfront-ervaring.

[ ![](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Additional information</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See also:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ" target="_blank">Learning Path for reports and dashboards</a> </li>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/basic-report-creation-program">Basic Report Creation Program for the new Workfront experience</a> </p>
  -->
