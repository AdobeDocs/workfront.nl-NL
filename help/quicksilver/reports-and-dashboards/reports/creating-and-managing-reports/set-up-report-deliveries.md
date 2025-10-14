---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Overzicht van levering rapporteren
description: Overzicht van levering rapporteren
author: Nolan
feature: Reports and Dashboards
exl-id: 1637df59-ca1d-4cf6-b83d-2b27936cdb96
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1534'
ht-degree: 0%

---

# Overzicht van levering rapporteren

<!-- Audited: 11/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is linked to the UI in the Send Report box inside the Preview sandbox. If you change title, log bug for Dev to fix the link) </p>
-->

U kunt rapporten plannen die automatisch aan gebruikers op een bepaald programma worden geleverd, of u kunt rapporten verzenden in één keer, manueel. Wanneer u een rapport van Adobe Workfront verzendt, ontvangt de gebruiker een e-mail met het Workfront-rapport in een aparte bijlage.

Voor informatie over vestiging een rapport voor levering, zie het artikel [&#x200B; Plan een automatische rapportlevering &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

U kunt geen rapporten voor levering plannen, noch hen manueel in de milieu van de Sandbox van de Voorproef leveren. Voor meer informatie over de zandbak van de Voorproef, zie het artikel [&#x200B; het Milieu van de Voorproef van Adobe Workfront Sandbox &#x200B;](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).\
Voor meer informatie over het leveren van rapporten in het milieu van Sandbox van de Voorproef, zie het artikel [&#x200B; een rapport in het milieu van Sandbox van de Voorproef verzenden &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/send-report-preview-sandbox-environment.md).

## Leveringslimieten rapporteren

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."])</p>
-->

Overweeg het volgende wanneer het plannen van rapporten voor levering:

* U kunt tot 10 herhaalde rapportleveringen voor om het even welk bepaald rapport plannen.
* U kunt een rapport plannen dat slechts moet worden geleverd als u de schepper van het rapport bent. Als u een rapport moet verzenden dat u niet hebt gemaakt, kunt u het handmatig verzenden.

## Exportlimieten

Er zijn verscheidene groottegrenzen die beïnvloeden hoe de rapporten in Workfront tonen en hoe zij door een handuitvoer, een geleverd rapport, of door API uitvoeren:

* **10MB dossiergrootte:** de groottelimiet van het Dossier voor om het even welk uitgevoerd rapport dat voor levering wordt gepland. Als een geëxporteerd bestand dat is gekoppeld aan een e-mailbericht groter is dan 5 MB, wordt een koppeling waarnaar het bestand kan worden gedownload per e-mail verzonden in plaats van het bijgevoegde geëxporteerde rapport.

  >[!NOTE]
  >
  >Excel .xlsx-bestanden die groter zijn dan 10 MB, genereren geen e-mail. U kunt het rapport handmatig naar deze indeling exporteren. Voor informatie over het uitvoeren van rapporten, zie [&#x200B; gegevens van de Uitvoer &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* **50.000 rijen:** het aantal rijen van gegevens toegestaan in een rapportuitvoer voor .pdf en Van het Lusje Gescheiden dossiers.

  Voor de dossiers van Excel .xls, is deze grens **65.000 rijen**.

  Voor de dossiers van Excel .xlsx, is deze grens **100.000 rijen**.

  Deze grenzen sluiten de kolomrubrieken, evenals rijen voor groepen in het rapport uit. Bijvoorbeeld, als u 6 groeperingen in een rapport hebt, en 50.000 rijen van gegevens, zal het uitgevoerde dossier 50.000 rijen hebben.

  Als uw rapport meer punten dan deze grenzen heeft, ontvangt u een fout dat de uitvoer en de levering van het rapport niet succesvol zijn. Verlaag het aantal items dat u op het scherm ziet tot een getal dat kleiner is dan of gelijk is aan deze limiet om de resultaten te kunnen leveren. Als u alle gegevens wilt exporteren, is het raadzaam filters te gebruiken om kleinere hoeveelheden gegevens te verkrijgen en vervolgens meerdere exportbewerkingen uit te voeren. Voor meer informatie, zie [&#x200B; Overzicht van Filters &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

  Deze grenswaarden gelden voor:

   * Een handmatige export van een rapport.
   * Een gepland rapport.
   * Een export via een API-integratie.
   * Gegevens geëxporteerd via een trap-start.

     Voor meer informatie over het uitvoeren van gegevens via schop-begin, zie de artikel [&#x200B; gegevens van de Uitvoer van Adobe Workfront via Kick-Begarts &#x200B;](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

     >[!NOTE]
     >
     >U kunt 50.000 rijen exporteren in een startbestand, maar alleen naar een Excel-bestand.

   * Gebruiksinformatie voor een project exporteren.

     Voor meer informatie over het uitvoeren van gebruiksinformatie voor een project, zie [&#x200B; Overzicht van het rapport van het Gebruik van het Middel &#x200B;](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* **65.530 hyperlinks:** dit is een grens die door Excel op documenten wordt opgelegd die meer dan 65.530 hyperlinks bevatten. Deze documenten kunnen niet worden geopend wanneer ze handmatig worden geëxporteerd of in een bezorgd rapport worden verzonden. Een Excel-document kan slechts 200 rijen gegevens bevatten, maar als het document meer dan 65.530 koppelingen bevat, wordt het document niet geopend. Deze limiet geldt alleen voor Excel-bestanden en niet voor de andere ondersteunde indelingen.
* **256 kolommen**: Dit is een grens die door Excel op documenten wordt opgelegd die meer dan 256 kolommen bevatten. Deze documenten kunnen niet handmatig worden geëxporteerd of in een bezorgd rapport worden verzonden. Deze limiet geldt alleen voor Excel-bestanden en niet voor de andere ondersteunde indelingen.

Als u probeert gegevens te exporteren die de limiet overschrijden, ontvangt u mogelijk niet alle verwachte gegevens in de exportbewerking. In plaats daarvan wordt een gewijzigd verslag binnen de limiet opgesteld.

Bovendien worden rapporten die langer dan 60 minuten duren, gestopt.

Neem contact op met de technische ondersteuning van Workfront als u problemen hebt met uw limiet.

## Tijdstempels op geleverde rapporten begrijpen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Note about if this is delivered at a time based on the user's time zone settings?)</p>
-->

Wanneer u een rapport in een e-mail ontvangt, komen het tijdstempel en de tijdnotatie in het rapport mogelijk niet overeen met die in Workfront als u het rapport tegelijkertijd in Workfront moest bekijken.

Overweeg het volgende:

* Wanneer u een rapport weergeeft in de browser, komen het tijdstempel en de notatie in het rapport overeen met de landinstelling en de tijdzone van de browser, zoals gedefinieerd in de instellingen van de browser.
* Wanneer het rapport in een e-mail wordt geleverd, wordt het rapport geleverd met de tijdstempel en notatie die overeenkomen met de landinstelling en tijdzone van de gebruiker zoals deze zijn opgegeven in uw Workfront-profiel.\
  Voor meer informatie over de Plaats van de Gebruiker en de Streek van de Tijd in Workfront, zie het artikel [&#x200B; uitgeven het profiel van een gebruiker &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Rapporten met een speciale weergave {#reports-with-a-special-view}

Als u een speciale weergave toepast op een rapport, wordt de speciale weergave weergegeven op het tabblad Details van het rapport in Workfront.

Wanneer u de levering plant van een rapport dat een speciale mening heeft, wordt het lusje van Details geleverd in de gehechtheid van verzonden e-mail, in plaats van de speciale mening.

De volgende opmerkingen worden beschouwd als speciale weergaven:

* Mijlpaal van een projectrapport
* Gantt-weergave op een project- of taakrapport
* Rapporten met een Grafiek als standaardlusje

>[!NOTE]
>
>Als er ook een lusje van de Matrijs op het rapport naast het standaardlusje met een speciale mening is, wordt het rapport geleverd aangezien het op het lusje van de Matrijs toont.

Voor meer informatie over hoe te om een speciale mening op een rapport toe te passen, zie het artikel [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

## Het geleverde bestand gebruiken

Wanneer u een rapport van Workfront verzendt, ontvangt de gebruiker een e-mail met het rapport in een afzonderlijke bijlage.

* [&#x200B; Onderwerpregel, gehechtheidsnaam, en rapporttitel &#x200B;](#subject-line-attachment-name-and-report-title)
* [&#x200B; Tijdstempels &#x200B;](#timestamps)
* [&#x200B; Branding &#x200B;](#branding)
* [&#x200B; Formatterend &#x200B;](#formatting)
* [Koppelingen](#links)

### Onderwerpregel, naam van bijlage en rapporttitel {#subject-line-attachment-name-and-report-title}

Voor meer informatie over de onderwerpregel van het geleverde rapport e-mail, zie [&#x200B; Plan een automatische rapportlevering &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

De naam van het in bijlage rapport is: *The_Name_Of_The_Report* die door het uitgevoerde dossierformaat wordt gevolgd.

Als u het geleverde rapport wilt opmaken als PDF- of HTML-bestand, krijgt u de volgende titel van het rapport:

*De Naam van het Rapport.*

Rapporten die gepland zijn voor levering in Excel, Excel (.xlsx), of formaat TSV hebben geen titel.

>[!NOTE]
>
>Als het rapport een beschrijving bevat, wordt het opgenomen in het geëxporteerde bestand als het bestand is opgemaakt als een PDF- of HTML-bestand.

### Tijdstempels {#timestamps}

Een tijdstempel wordt alleen weergegeven in het bijgevoegde bestand als de indeling van het bestand .pdf is. De tijdstempel bevindt zich in de voettekst van het bijgevoegde bestand.

De tijdstempel bevat:

* Datum
* Tijd
* Tijdzone waarop het rapport is verzonden

### Branding {#branding}

Als uw Workfront-beheerder aangepaste branding heeft toegevoegd aan uw Workfront-exemplaar, bevatten de rapporten die in .pdf-indeling worden verzonden ook uw persoonlijke logo.

Rapporten die in alle andere indelingen worden verzonden, kunnen niet worden gepersonaliseerd met uw logo.

Voor meer informatie over branding uw instantie van Workfront, zie het artikel [&#x200B; merk uw instantie van Adobe Workfront &#x200B;](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### Opmaak {#formatting}

U ontvangt altijd het lusje van Details van een rapport wanneer een rapport wordt verzonden of voor een levering gepland, tenzij het rapport een speciale mening heeft.

Als uw rapport een speciale opmaak heeft in de webtoepassing, moet het rapport worden geleverd met de speciale opmaak wanneer de tabbladen Details en Matrix alleen worden geleverd voor .pdf- en Excel-bestanden.

Het filter, de weergave of de groepering van het rapport worden niet opgenomen in het geleverde bestand. De beschrijving van het rapport wordt alleen opgenomen wanneer u het rapport verzendt als een PDF-bestand.

Voor meer informatie over het ontvangen van rapporten met een speciale mening, zie de artikel [&#x200B; Rapporten met een speciale mening &#x200B;](#reports-with-a-special-view).\
Voor meer informatie over het selecteren van het standaardlusje van een rapport en over het speciale formatteren, zie [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

### Koppelingen {#links}

Als u een rapport verzendt van Workfront naar PDF of Excel, blijven werkkoppelingen in het oorspronkelijke document actief in het verzonden bestand. Koppelingen kunnen verwijzen naar elk object in Workfront dat koppelingen ondersteunt.

De naam van het rapport in het e-mailbericht is ook een koppeling.

## Rapport over geplande rapporten

U kunt zien of een rapport is gevormd om te worden geleverd door het volgende te creëren:

* **Mening A** voor het voorwerp van het Rapport in een lijst of een rapport voor rapporten: Creeer een mening op een lijst van rapporten of in een rapport voor rapporten, en voeg de volgende kolom aan de mening toe:\
  *Geplande rapportnaam.\
  *The de namen van alle leveringen die voor dat rapport worden gepland zijn vermeld in de kolom in een bulleted lijst.\
  ![&#x200B; scheduled_reports_info_in_view.png &#x200B;](assets/scheduled-reports-info-in-view-350x294.png)

* **de Filter van A** voor het voorwerp van het Rapport: Creeer een filter op een lijst van rapporten of in een rapport over rapporten met de volgende verklaring: *Geplande identiteitskaart van het Rapport is niet leeg*.\
  Hiermee worden alleen rapporten weergegeven die in uw lijst of rapport zijn gepland.\
  ![&#x200B; Gepland rapportfilter &#x200B;](assets/qs-scheduled-report-filter-350x101.png)\
  Voor meer informatie over het creëren van rapporten, zie [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren. Voor informatie bij het creëren van een rapport over rapporten, zie [&#x200B; een rapport over het melden van activiteiten &#x200B;](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md) creëren.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Scheduling a Repeating Report Delivery</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can schedule up to 10 repeating report deliveries for any given report.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can schedule a report to be delivered only if you are the creator of the report. If you need to send a report that you did not create, you can send it on a manual basis.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To schedule a report for automatic delivery or to edit an existing report delivery: ​</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report for which you want to schedule delivery. </li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then <strong>Send Report</strong>.<br> The <strong>Send Report</strong> dialog box is displayed.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the <strong>Repeating Deliveries</strong> tab.<br><img src="assets/report-delivery-schedule-350x169.png" alt="" style="width: 350;height: 169;"></li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Conditional) To modify an existing repeating report delivery, select the report delivery in the <strong>Repeating Deliveries</strong> section.</li>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Specify the following information:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Send to:</strong> Begin typing the name of the user, group, team, or role who you want to send the report to, then click the name when it appears in the drop-down list.<br>Or<br>Specify the email address of a person external to the Workfront system who you want to have access to the report.<br> Repeat this process to send the report to multiple users, groups, teams, or roles.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Subject:</strong> Specify a subject for the email notification.<br> By default, the email subject is: <em>Workfront Report: <Name of the report> Date of the Export</em>.<strong></strong></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Message:</strong> Specify a message to include in the email.<br>By default, the email message is: <em>Attached is the <report frequency> report <Name of the report> generated by Workfront on <Date>.</em><br>
   <note type="note">
   For reports delivered as an Excel file only, the following message is also added to the email: "Please be aware that with MS Excel (XLS) file types, there is a limit (65,530) on the number of hyperlinks these file types support. If you exceed those limits, your file will not open and it is recommended to resend without the hyperlinks. Please go back to the report scheduler to remove hyperlinks and resend the report." The "please go back to the report scheduler" phrase is a link back to the report. 
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Deliver this report with the Access Rights of:</strong> Begin typing the name of a user who has access to the report, then click the name when it appears in the drop-down list. Users who receive the report will be granted the same level of access to the report as the user that you specify here.<br> For more information, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Run and deliver a report with the access rights of another user</a>
   <note type="note">
   This field does not support wildcards. For example, using the wildcard $$User.ID does not run the report with the access rights of the user who is receiving the report.
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Format:</strong> Select in which of the following formats you want the report to be delivered:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> HTML</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">PDF</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS Excel</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS Excel (.xlsx)</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">TSV  </li>
   </ul></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Include Links:</strong> This option is available only when <strong>MS Excel</strong> is selected in the <strong>Format</strong> drop-down menu. When this option is enabled, any hyperlinks are included in the exported Excel document. <br>Documents that contain more than 65,530 links cannot be opened. If the exported document will contain more than 65,530 links, deselect this option.<br>This option is enabled by default. </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Summary:</strong> Displays a summary of when the delivery repeats.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats:</strong> Select whether the report should be delivered daily, weekly, monthly, or yearly.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats Every:</strong> Select the frequency with which you want the delivery to repeat. The value you select for this option is based on the option that is selected in the <strong>Repeats</strong> drop-down list.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Time:</strong> Select the time of day for the delivery to be sent.</li>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats On:</strong> This option is available when the <strong>Repeats</strong> option is set to either <strong>Weekly</strong> or <strong>Monthly</strong>.</p>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the <strong>Repeats</strong> option is set to <strong>Weekly</strong>: Select the days of the week that the delivery is sent.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the <strong>Repeats</strong> option is set to <strong>Monthly</strong>: Select whether the delivery is sent on the day of the month, day of the week, or last day of the month (these options leverage the date that you select in the <strong>Starts On</strong> field).</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Starts On:</strong> Select the date for the scheduled delivery to begin.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Ends On:</strong> Select a date for the scheduled delivery to end. <br>Or</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Never</strong> if you want the scheduled delivery to last indefinitely.</li>
   -->

<!--
   <li value="6" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save</strong> to save the report delivery.<br> The report is saved in the <strong>Repeating Deliveries</strong> section (in the <strong>Send Report</strong> dialog box).<br> The report will be sent at the schedule time<br>Or<br>To manually send the report, click <strong>Send Now</strong>.<br>For more information about sending the report instantly or manually, see .</li>
   -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a Scheduled Report Delivery</h2>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to the report with the delivery you want to delete.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then <strong>Send Report</strong>. </li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Repeating Deliveries</strong>. </li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the name of the scheduled delivery you want to delete, then click <strong>Delete</strong>. The report is no longer set up for the scheduled delivery. </li>
   -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Sending a Report Manually, on a One-Time Basis</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can manually send a report that has been previously scheduled, or you can create a single-use report delivery.​</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a title="Setting Up Report Deliveries" href="#sending-a-scheduled-report-now" class="MCXref xref">Sending a Scheduled Report Now</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a title="Setting Up Report Deliveries" href="#sending-a-report-one-time-only" class="MCXref xref">Sending a Report (One Time Only)</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="sending-a-scheduled-report-now">Sending a Scheduled Report Now</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">After a scheduled report has been set up, you can manually send the report rather than waiting until the scheduled time.</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report that you want to send now.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then <strong>Send Report</strong>.<br> The Send Report dialog box is displayed.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>Repeating Deliveries</strong> tab.</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Repeating Deliveries</strong> section, select the report delivery that was previously created.<br><img src="assets/report-delivery-schedule-send-350x160.png" alt="" style="width: 350;height: 160;"></li>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Send Now</strong>.<br> The report is sent to all users identified in the scheduled delivery.</li>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="sending-a-report-one-time-only">Sending a Report (One Time Only)</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can manually send a report at any time. When you send a report in this way, delivery information (such as the users you are sending to and the email subject) are not saved. If you want to create a report delivery that you can save for later use, create a repeating scheduled report. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To send a report to users (one time only):</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report that you want to send now.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then <strong>Send Report</strong>.<br> The <strong>Send Report</strong> dialog box is displayed.<br><img src="assets/report-delivery-sendnow-350x351.png" alt="" style="width: 350;height: 351;"></li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">On the <strong>Send Now</strong> tab, specify the following information:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Send to:</strong> Begin typing the name of the user, group, team, or role who you want to send the report to, then click the name when it appears in the drop-down list. Or, specify the email address of a person external to the Workfront system who you want to have access to the report.<br> Repeat this process to send the report to multiple users, groups, teams, or roles.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Subject:</strong> Specify a subject for the email notification.<br> By default, the email subject is: <em>Workfront Report: <Name of the report> Date of the Export</em>.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Message:</strong> Specify a message to include in the email.<br>By default, the email message is: <em>Attached is the <report frequency> report <Name of the report> generated by Workfront on <Date>.</em><br>
   <note type="note">
   For reports delivered as an Excel file only, the following message is also added to the email: "Please be aware that with MS Excel (XLS) file types, there is a limit (65,530) on the number of hyperlinks these file types support. If you exceed those limits, your file will not open and it is recommended to resend without the hyperlinks. Please go back to the report scheduler to remove hyperlinks and resend the report." The "please go back to the report scheduler" phrase is a link back to the report. 
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Deliver this report with the Access Rights of:</strong> Begin typing the name of a user who has access to the report, then click the name when it appears in the drop-down list. Users who receive the report will be granted the same level of access to the report as the user that you specify here.<br> For more information, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Run and deliver a report with the access rights of another user</a>.
   <note type="note">
   This field does not support wildcards. For example, using the wildcard $$User.ID does not run the report with the access rights of the user who is receiving the report.
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Format:</strong> Select in which of the following formats you want the report to be delivered:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> HTML</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">PDF</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS Excel</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS Excel (.xlsx)</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">TSV</li>
   </ul></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Include Links:</strong> This option is available only when <strong>MS Excel</strong> is selected in the <strong>Format</strong> drop-down menu. When this option is enabled, any hyperlinks are included in the exported Excel document. <br>Documents that contain more than 65,000 links cannot be opened. If the exported document will contain more than 65,000 links, deselect this option.<br>This option is enabled by default.</li>
   </ul></li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Send Now</strong>.<br> The report is sent to all users that you identified.<br> Or<br> Click <strong>Make Repeating Delivery</strong> if you want to set up a scheduled delivery with this same information, then complete the additional information regarding the frequency of when the report is sent.</li>
   -->
