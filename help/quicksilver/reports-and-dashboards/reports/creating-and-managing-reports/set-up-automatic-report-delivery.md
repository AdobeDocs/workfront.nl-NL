---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Plan een automatische levering van rapporten
description: Plan een automatische levering van rapporten
author: Courtney
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 62f56486ccc590921b7dc8227d46cdede84df32d
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 0%

---

# Plan een automatische levering van rapporten

<!-- Audited: 4/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

U kunt rapporten plannen om automatisch aan gebruikers op een bepaald programma te leveren, of u kunt rapporten manueel één keer verzenden. Wanneer u een rapport van Adobe Workfront verzendt, ontvangt de gebruiker een e-mail met het Workfront-rapport in een aparte bijlage.

Voor meer informatie, met inbegrip van groottebeperkingen die de levering van uw rapporten kunnen beïnvloeden, zie [ de leveringsoverzicht van het Rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td role="rowheader">Adobe Workfront-licentie</td> 
      <td> 
      <p>Nieuw: Standaard</p>
      <p>of</p>

<p>Huidig: Plan</p>

</td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat u begint, moet u een rapport maken. Meer leren over het creëren van rapporten, zie [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

## Een rapportlevering plannen


Een rapport plannen voor automatische levering: &#x200B;

{{step1-to-reports}}

>[!NOTE]
>
>Rapportleveringen bevatten geen aanwijzingen. Als u gegevens in een rapportlevering wilt beperken, adviseren wij het toepassen van filters op het rapport dat u wilt verzenden.

1. Voor de **pagina van Rapporten**, selecteer een rapport.
1. Bij de bovenkant van het scherm, klik **Acties van het Rapport**, dan **verzend Rapport** van de drop-down die verschijnt. Het **verzendt de dialoogvakje van het Rapport**.

   >[!TIP]
   >
   >Om een rapport te verzenden manueel op om het even welk bepaald tijdstip, ga naar het rapport, dan klik **de Acties van het Rapport** > **verzenden Rapport** > **verzenden nu**.

1. Selecteer de **Herhalende Leveringen** tabel.
1. (Voorwaardelijk) om een bestaande herhalende rapportlevering te wijzigen, selecteer de rapportlevering in de **Herhalende Leveringen** sectie op de rechterkant van de dialoogdoos.
1. Geef de volgende informatie op:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Verzenden naar</p> </td> 
      <td> <p>Typ de naam van de gebruiker, groep, team of rol waarnaar u het rapport wilt verzenden en klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.</p> <p>of</p> <p>Voer het e-mailadres in van een persoon buiten het Workfront-systeem die u toegang tot het rapport wilt hebben.</p> <p>Herhaal dit proces om het rapport naar veelvoudige gebruikers, groepen, teams, of rollen te verzenden.</p> <p>Opmerking:  <p>Overweeg het volgende wanneer het toevoegen van de ontvangers van de rapportlevering:</p> 
        <ul> 
         <li><p>Als uw organisatie Workfront-meldingen beperkt tot specifieke e-maildomeinen, kunt u rapporten alleen verzenden naar e-mailadressen die worden vermeld in de lijst van gewenste personen voor e-mail.</p> <p>Bijvoorbeeld, wanneer een gebruiker als rapportontvanger wordt geplaatst en een e-mailadres heeft dat eerder werd toegelaten, en de lijst van gewenste personen wordt bijgewerkt om e-mails niet meer aan dat domein te leveren, zal de gebruiker niet meer geleverde rapporten ontvangen.</p><p>Voor informatie over hoe een beheerder van Workfront de e-maillijst van gewenste personen bijwerkt, zie de sectie <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref"> uw e-maillijst van gewenste personen </a> vormen.</p></li> 
         <li> <p>Het toevoegen van een groot aantal gebruikers als ontvangers kan ertoe leiden dat de levering mislukt. Als u leveringsmislukkingen ervaart, kunt u veelvoudige rapportleveringen met kleinere groepen gebruikers plannen.</p> </li> 
        </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>E-mailonderwerp</p> </td> 
      <td> <p>Voer een onderwerp voor de e-mailmelding in.</p> <p>Standaard is het onderwerp van de e-mail:</p> <p><em> het Rapport van Workfront: [Naam van het rapport] [Datum] </em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>E-mailbericht</p> </td> 
      <td> <p>Voer een bericht in dat u in de e-mail wilt opnemen.</p> <p>Standaard is het e-mailbericht:</p> <p><em> in bijlage is het [rapportfrequentie] rapport [Naam van het rapport] door Workfront op [Datum] wordt geproduceerd.</em> </p> <p>Opmerking: voor rapporten die alleen worden geleverd als Excel-bestand, wordt het volgende bericht ook toegevoegd aan de e-mail: "Houd er rekening mee dat er bij MS Excel (XLS)-bestandstypen een limiet geldt (65.530) voor het aantal hyperlinks dat door deze bestandstypen wordt ondersteund. Als u deze limieten overschrijdt, wordt het bestand niet geopend en wordt aangeraden het bestand opnieuw te verzenden zonder de hyperlinks. Gelieve te gaan terug naar de rapportplanner om hyperlinks te verwijderen en het rapport opnieuw te verzenden." "gelieve terug naar de rapportplanner"uitdrukking te gaan is een verbinding terug naar het rapport.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Dit rapport leveren met de toegangsrechten van</p> </td> 
      <td> <p>Typ de naam van een gebruiker die toegang heeft tot het rapport en klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst. De gebruikers die het rapport ontvangen zullen het zelfde niveau van toegang tot het rapport worden verleend zoals de gebruiker die u hier specificeert.<br> voor meer informatie, zie <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref"> Looppas en lever een rapport met de toegangsrechten van een andere gebruiker </a>.</p> <p>Opmerking: dit veld ondersteunt geen jokertekens. Bijvoorbeeld, stelt het gebruiken van het vervangings{</em> 0}$$User.ID niet het rapport met de toegangsrechten van de gebruiker in werking die het rapport ontvangt.<em></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Indeling</p> </td> 
      <td> <p>Selecteer het formaat u voor het geleverde rapport wilt:</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>Als u PDF selecteert, kunt u de output formatteren gebruikend de extra <strong> Opties van de Grootte van het Papier </strong> en <strong> van de Richtlijn </strong> die tonen.</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Inclusief koppelingen</p> </td> 
      <td> <p>Deze optie is beschikbaar slechts wanneer <strong> MS Excel </strong> in het <strong> Formaat </strong> drop-down menu wordt geselecteerd. Als deze optie is ingeschakeld, worden alle hyperlinks opgenomen in het geëxporteerde Excel-document.</p> <p>Documenten die meer dan 65.530 koppelingen bevatten, kunnen niet worden geopend. Schakel deze optie uit als het geëxporteerde document meer dan 65.530 koppelingen bevat.</p> <p>Deze optie is standaard ingeschakeld.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Samenvatting</p> </td> 
      <td> <p>Toont een samenvatting van wanneer de levering zich herhaalt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Herhalingen</p> </td> 
      <td> <p>Selecteer of het rapport dagelijks, wekelijks, maandelijks, of jaarlijks zou moeten worden geleverd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Herhaalt om de</p> </td> 
      <td> <p>Selecteer de frequentie waarmee u de levering wilt herhalen. De waarde u voor deze optie selecteert is gebaseerd op de optie die in <strong> wordt geselecteerd herhaalt </strong> drop-down lijst.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Tijd</p> </td> 
      <td> <p>Selecteer de tijd van de dag waarop de levering moet worden verzonden.</p> <p>Tip: Omdat systeembelastingen de leveringstijden van het rapport kunnen beïnvloeden, kan er een vertraging van maximaal 24 uren tussen de geplande tijd en de daadwerkelijke leveringstijd zijn. Als u een rapport nodig hebt dat tegen een specifieke tijd wordt geleverd, adviseren wij de levering voorafgaand aan de tijd te plannen dat het nodig is. Over het algemeen raden we aan de levering ten minste een dag vóór de datum te plannen waarop deze nodig is.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Herhaalt op</p> </td> 
      <td> <p>Deze optie is beschikbaar wanneer de <strong> herhaalt </strong> optie aan of <strong> Wekelijks </strong> of <strong> Maandelijks </strong> wordt geplaatst:</p> 
       <ul> 
        <li> <p>Wanneer <strong> </strong> optie herhaalt wordt geplaatst aan <strong> Wekelijks </strong>: Selecteer de dagen van de week dat de levering wordt verzonden.</p> </li> 
        <li> <p>Wanneer <strong> herhaalt </strong> optie aan <strong> wordt geplaatst Maandelijks </strong>: Selecteer of de levering op de dag van de maand, de dag van de week, of laatste dag van de maand (deze opties hefboomwerking de datum die u op <strong> selecteert begint op </strong> gebied) wordt verzonden.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Begint op</p> </td> 
      <td>Selecteer de datum waarop de geplande levering moet beginnen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Eindigt op</p> </td> 
      <td>Selecteer een datum waarop de geplande levering moet worden beëindigd.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Nooit</p> </td> 
      <td>Selecteer <strong> nooit </strong> als u de geplande levering wilt voor onbepaalde tijd duren.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **sparen** om de rapportlevering te bewaren. De rapportvertoningen in de **Herhalende Leveringen** sectie van **verzenden het de dialoogvakje van het Rapport** en zullen op de geplande tijd verzenden.

   Voor informatie over groottebeperkingen die de levering van uw rapporten kunnen beïnvloeden, zie de de leveringsgrenzen van het sectierapport [ ](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) en [ de grenzen van de Uitvoer ](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

>[!IMPORTANT]
>
>Geplande rapporten zijn onderworpen aan een interne tijdslimiet wanneer zij voor levering worden verwerkt. Als een rapport langer duurt dan de te verzenden limiet, ontvangt u een melding en wordt het rapport niet meer bezorgd, ongeacht de resterende geplande leveringen. Om het rapport verder te verzenden, probeer eerst de grootte van het rapport door filters en meningen te verminderen, dan creeer een nieuwe geplande levering.
>
>Als u een gepland rapport gebruikt om Workfront-gegevens te analyseren met een BI-programma, raden we u aan in plaats daarvan Workfront Data Connect te gebruiken. Voor meer informatie, zie [ de Gegevens van Workfront verbinden overzicht ](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md).

## Een geplande rapportlevering verwijderen

Om een geplande rapportlevering te schrappen: &#x200B;

{{step1-to-reports}}

1. Voor de **pagina van Rapporten**, selecteer een rapport.

1. Bij de bovenkant van het scherm, klik **Acties van het Rapport**, dan **verzend Rapport** van de drop-down die verschijnt. Het **verzendt de dialoogvakje van het Rapport**.

1. Selecteer de **Herhalende Leveringen** tabel.
1. In de **Herhalende Leveringen** sectie op de rechterkant van de dialoogdoos, klik de geplande levering u wilt schrappen.
1. In de **Herhalende Leveringen** detailsectie, klik **Schrapping**.

1. Klik **Schrapping** om te bevestigen.

<!--## Video walk-through

View the following video to learn how to schedule a report delivery. This video was recorded in Workfront Classic. However, the content also applies to the new Workfront experience.

[ ![Video walkthrough of report delivery](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)


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
