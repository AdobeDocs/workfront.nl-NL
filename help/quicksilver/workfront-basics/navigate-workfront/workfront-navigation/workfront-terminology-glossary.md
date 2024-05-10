---
content-type: reference
navigation-topic: workfront-navigation
title: Verklarende woordenlijst [!DNL Adobe Workfront] terminologie
description: De [!DNL Adobe Workfront] woordenlijst bevat veelgebruikte termen in [!DNL Adobe Workfront]. You can use the glossary when you want to find the definition of concepts you see in the [!UICONTROL Workfront] interface, rapporten, of u probeert de betekenis van [!DNL Workfront] in de [!DNL Workfront] documentatie.
author: Alina
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: b57f5038746094dde4b98bd28361e730c28ba412
workflow-type: tm+mt
source-wordcount: '16482'
ht-degree: 0%

---


# Verklarende woordenlijst [!DNL Adobe Workfront] terminologie

<!--Audited: 12/2023-->

>[!IMPORTANT]
>
>Dit artikel moet worden gebruikt als een verwijzing naar de termen die u in het dialoogvenster [!DNL Adobe Workfront] in de [!DNL Workfront] documentatie, of wanneer over het algemeen het spreken over planning en het leiden van het werk. Deze gegevens worden momenteel bijgewerkt, waardoor deze tabel wellicht niet volledig is. We zullen deze disclaimer wegnemen wanneer we deze informatie volledig vinden.

De volgende tabel bevat een lijst met veelgebruikte termen in Adobe Workfront:

## A - C

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Objectnaam</strong></th> 
   <th><strong>Beschrijving</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Access Level]</td> 
   <td>Een gebruikersprofiel dat bepaalt hoe een gebruiker met verschillende objecten en gereedschappen in Workfront kan communiceren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Active Task]</td> 
   <td>Een onvolledige taak in een huidig project dat niet wordt verhinderd om door een voorgangertaak worden gewerkt en geen taakbeperking met een toekomstige geplande begindatum heeft. Met andere woorden, er kan vandaag aan gewerkt worden.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Activity]</td> 
   <td>In [!DNL Workfront Goals]Een activiteit is een voortgangsindicator voor een doel. Dit kan een voortgangsbalk zijn die u handmatig bijwerkt of een project dat aan het doel is gekoppeld. U kunt geen activiteiten weergeven in een rapport en u hebt geen toegang tot deze activiteiten via de [!DNL Workfront] API. Zie voor informatie over activiteiten <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Aan de slag met resultaten en activiteiten in Adobe Workfront Goals</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Cost]</td> 
   <td> <p>Voor taken en kwesties, is dit de kosten verbonden aan de daadwerkelijke die uren met betrekking tot de Kosten per uurtarief van het middel worden geregistreerd aan de taak of de kwestie worden toegewezen. Voor projecten is dit in totaal [!UICONTROL Actual Costs] van taken en problemen met het project. Zie voor meer informatie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Trackkosten</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Expense Cost]</td> 
   <td> <p>De som van de [!UICONTROL Actual Amounts] voor alle uitgaven die voor een project of een taak worden geregistreerd.</p> <b>VOORBEELD </b>
   <p>Als u een uitgave voor Taak 1 creeert en $600.00 in ingaat [!UICONTROL Actual Amount] in het veld [!UICONTROL Actual Expense Cost] hiervoor is $ 600.00 . </p> 
   <p>Voor een project: [!DNL Workfront] gebruikt de volgende formule om te berekenen [!UICONTROL Actual Expense Cost]:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Actual Hours]</td> 
   <td> <p>In een project, een taak, of een uitgifterapport, [!UICONTROL Actual Hours] zijn de som alle uren het programma geopend op het project, de taak, of de kwestie.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span> Indien van de [!UICONTROL Updates] tab voor Taak 1, klikt u op 'Logtijd' en voert u 25 uur in. De werkelijke uren van Taak 1 = 25 uur. </p> <p>[!DNL Workfront] berekeningen [!UICONTROL Actual Hours] voor bovenliggende taken of projecten met behulp van de volgende formules:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Labor Cost]</td> 
   <td> <p>De [!UICONTROL Actual Cost] in verband worden gebracht met de arbeid die in een taak of project wordt geïnvesteerd. </p> <p>Voor een taak: [!DNL Workfront] berekent de [!UICONTROL Actual Labor Cost] met behulp van de volgende formule:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Als de taak een [!UICONTROL Cost Type] van [!UICONTROL User Hourly], [!DNL Workfront] gebruikt de gebruikerstarief. Als de taak een [!UICONTROL Cost Type] van [!UICONTROL Role Hourly], [!DNL Workfront] gebruikt het taakroltarief om te berekenen [!UICONTROL Actual Labor Cost]. </p> <p>Voor een project: [!DNL Workfront] gebruikt de volgende formule om de [!UICONTROL Actual Labor Cost]:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Zie voor meer informatie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Trackkosten</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span>Als een gebruiker zich bijvoorbeeld 5 uur voor een taak aanmeldt met een [!UICONTROL User Hourly] [!UICONTROL Cost Type] en hun uurtarief is $100, [!UICONTROL Actual Labor Cost] is $500.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Revenue] </td> 
   <td> <p>De [!UICONTROL Actual Revenue] van een project of een taak het bedrag is dat verband houdt met de [!UICONTROL Actual Hours] van het project of de taak. </p> <p>Voor informatie over het bijhouden van inkomsten in [!DNL Workfront], zie <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overzicht van facturering en inkomsten</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Actual Start]</td> 
   <td>De tijdstempel wanneer een gebruiker een object wijzigt dat bezig is met werk dat aan hem of haar is toegewezen.</td> 
  </tr> 
  <!--<tr> 
 <td>A type of work process that is unplanned.</td> 
 -->
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Additional Schedules</td> 
    <td>An additional preset to be used for a new user group.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Agile] Methodologie</td> 
   <td>Een soort methodologie gebaseerd op de gezamenlijke ontwikkeling van behoeften en oplossingen met interfunctionele teams. Het stimuleert flexibiliteit en verandering op basis van een vaste tijdslijn.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Agile Team]</td> 
   <td>Verschilt van traditioneel team omdat zij hun toekomstig werk van een achterstand nemen en aan het binnen een bepaalde periode werken die wordt genoemd een [!UICONTROL Iteration].</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL All My Teams]</td> 
   <td> <p>Wanneer hiernaar wordt verwezen in [!UICONTROL filters], toont dit gebied of gebruikers die tot om het even welke teams behoren die de het programma geopende gebruiker tot behoort, of het werkpunten die aan om het even welke teams worden toegewezen die de het programma geopende gebruiker tot behoort. </p> <p>Wij adviseren gebruikend dit gebied in een filter om rapporten generischer te maken wanneer het delen van hen met andere gebruikers. Deze manier, kunt u slechts één rapport bouwen dat verschillende informatie afhankelijk van zal tonen wie het programma opent om het te bekijken, aangezien de informatie altijd voor de het programma geopende gebruiker wordt aangepast. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Allocation Date]</td> 
   <td> <p>U kunt dit gebied in de volgende types van rapporten vinden:</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Project] (Financiële gegevens)</li> 
     <li>[!UICONTROL Budgeted Hour]</li> 
    </ul> <p>Voor een<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL Project (Financial Data)] rapport: </p> 
    <ul> 
     <li>Dit rapport samenstellen wanneer wordt geprobeerd het te begrijpen <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> het bedrag van [!UICONTROL Planned Hours] die aan uw middelen wordt toegewezen.</li> 
     <li> <p>De [!UICONTROL Allocation Date] is de eerste dag (zondag) van een week waarin de toewijzing van een [!UICONTROL Job Role] om een taak te starten. Een resource ([!UICONTROL Job Role]) kan zo veel hebben [!UICONTROL Allocation Dates] zoals in weken gedurende de [!UICONTROL Duration] van de taken waaraan het wordt toegewezen. Als taken zich uitstrekken over meerdere maanden, kan de eerste dag van een maand ook een [!UICONTROL Allocation Date], indien het binnen de [!UICONTROL Duration] van de taak.</p> <p>U kunt bijvoorbeeld een [!UICONTROL Job Role] toegewezen aan een taak die zich over 3 weken uitstrekt en 90 [!UICONTROL Planned Hours]. Deze uren worden gelijkmatig verdeeld tijdens de duur van de taak, die elke dag 6 aanwijst [!UICONTROL Planned Hours] naar uw taakrol:</p> <p><em> [!UICONTROL Daily Planned Hours] = [!UICONTROL Total Planned Hours]/ Aantal [!UICONTROL Work Days] tijdens de [!UICONTROL Duration] van de taak </em> </p> <p>Er zijn dus drie [!UICONTROL Allocation Dates]elke zondag gedurende de [!UICONTROL Duration] , elk met een bepaald aantal [!UICONTROL Planned Hours] geassocieerd met hen.<br>Als de taak in het midden van de laatste week van een maand begint en twee weken na het begin van een nieuwe maand eindigt, zal de taak vier hebben [!UICONTROL Allocation Dates]: één voor elke zondag van elke week tijdens de [!UICONTROL Duration] en één voor de eerste dag van de nieuwe maand.</p> <p>Om deze informatie optimaal te gebruiken, adviseren wij dat u een <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> Rapport voor project (financiële gegevens) en een matrixgroep toevoegen voor [!UICONTROL Allocation Date]en groepeert de resultaten vervolgens wekelijks, maandelijks, driemaandelijks of jaarlijks voor de meest nauwkeurige gegevens.<br>Zie het artikel voor informatie over het maken van een matrixgroepering <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">Een matrixrapport maken</a>.</p> </li> 
    </ul> <p>Financiële informatie wordt ingevuld in [!UICONTROL Project (Financial Data)] alleen als de gegevens die ermee verband houden, jonger zijn dan 5 jaar. Als bijvoorbeeld in januari 2015 een functie werd toegewezen aan een taak en vandaag september 2021, een financieel gebied zoals [!UICONTROL Allocation Date] voor de rol job niet wordt gevuld in het dialoogvenster [!UICONTROL Project (Financial Data)] verslag. </p> 
    <div> 
     <p>Voor een [!UICONTROL Budgeted Hour] rapport:</p> 
     <ul> 
      <li>Dit rapport samenstellen wanneer u probeert te begrijpen hoeveel [!UICONTROL Budgeted Hours] dat aan uw middelen of aan uw projecten in de Planner van het Middel wordt toegewezen.</li> 
      <li> <p>De [!UICONTROL Allocation Date] is de eerste dag (een zondag) van de week waarvoor u de uren in de [!UICONTROL Resource Planner]. </p> <p><b>TIP</b></p> <p>Als een week zich over twee maanden uitstrekt, zal het twee rijen in het rapport produceren: één die aan de eerste dag van de week (Zondag van de eerste week die tijdens de eerste maand is) beantwoordt, en de tweede rij toont de eerste dag van de tweede maand. </p> <p>Als u bijvoorbeeld 8 uur begroot voor een gebruiker voor de week van 30 juni (zondag) - 6 juli (zaterdag), worden in de twee rijen een [!UICONTROL Allocation Date] van 30 juni en 1 juli. </p> </p> <p>Voor informatie over begrotingsmiddelen in het [!DNL Resource Planner], zie het artikel <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Begrotingsmiddelen in de [!DNL Resource Planner] met de [!UICONTROL Project] en [!UICONTROL Role] views</a>.</p> <p>Voor informatie over het samenstellen van een [!UICONTROL Budgeted Hour] rapport, zie <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Verslag: Budgeted Hour</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Announcements]</td> 
   <td> <p>Een manier om met gebruikersinformatie binnen het systeem te communiceren. Deze informatie komt vaak van [!DNL Workfront] naar de beheerder of van de beheerder naar de gebruiker. </p> <p>Zie voor meer informatie <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Aankondigingen verzenden</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL App Integration]</td> 
   <td>Een toepassing vertegenwoordigt doorgaans een aansluiting op een softwaretoepassing, maar kan ook speciale functies vertegenwoordigen die gegevens manipuleren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver Decision]</td> 
   <td> <p>In de [!UICONTROL Proof Approval] In dit veld worden goedkeuringsbesluiten voor proefdrukken weergegeven die niet meer actief zijn.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver stage]</td> 
   <td>In de [!UICONTROL Proof Approval report]In dit veld wordt informatie over een proefversie van het huidige werkgebied weergegeven.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval]</td> 
   <td> <p>Een bepaald het werkpunt, zoals een taak, een document, of een timesheet, kunnen vereisen dat een supervisor of een andere gebruiker weg op het het werkpunt ondertekent. Dit proces van het ondertekenen van weg wordt genoemd goedkeuring. </p> <p>Zie voor meer informatie <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Overzicht van goedkeuringsproces</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval date]</td> 
   <td>In de [!UICONTROL Proof Approval] rapport, toont dit gebied de datum een bewijs werd goedgekeurd.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver]</td> 
   <td>Een gebruiker of baanrol die op een bepaald het werkpunt moet ondertekenen, of de gebruiker die uuringangen op timesheets goedkeurt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assigned To]</td> 
   <td> <p>In een [!UICONTROL Task or Issue] rapport, toont dit gebied de Eigenaar van de taak of de kwestie, of [!UICONTROL Primary Assignee]. U kunt ook filteren of groeperen op dit veld.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment]</td> 
   <td>Een gebruiker, taakrol of team die is toegewezen aan een uitgave of een taak. Projecten, portfolio's of programma's kunnen geen toewijzingen hebben.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignments]</td> 
   <td> <p>In een [!UICONTROL Task] of [!UICONTROL Issue] rapport, toont dit gebied een lijst van alle entiteiten (gebruikers, baanrollen, teams) die aan de taak of de kwestie worden toegewezen. U kunt filteren op dit veld met de velden [!UICONTROL Assignment Users] en [!UICONTROL Assignment Roles]. U kunt filteren door het team dat aan de taak of kwestie wordt toegewezen gebruikend het gebied van het Team. U kunt een rapport niet groeperen door dit gebied.</p> <p>Werkitems die in het deelvenster [!UICONTROL Recycle Bin] zal in sommige rapporten blijven tonen die naar verwijzen [!UICONTROL Assignment] object waar [!DNL OR] filtermodifier wordt gebruikt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Roles]</td> 
   <td>
   <p>In een [!UICONTROL Task] of [!UICONTROL Issue] rapport, toont dit gebied informatie over de baanrollen die aan de taken of de kwesties worden toegewezen. Dit veld wordt weergegeven [!UICONTROL Primary Owners]en andere functies die zijn toegewezen aan taken of problemen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Status]</td> 
   <td> <p>In een taak-, taak- of uitgifterapport [!UICONTROL Assignment Status] toont of de gebruikers die aan een het werkpunt worden toegewezen hebben geklikt [!UICONTROL Work On It] of de [!UICONTROL Done] om het werk te accepteren of te voltooien. Het volgende [!UICONTROL Assignment Statuses] bestaan:</p> 
    <ul> 
     <li><b>[!UICONTROL Requested]</b>: de gebruiker is toegewezen aan de taak of uitgave, maar heeft niet op de knop [!UICONTROL Work On It] om er nog aan te werken.</li> 
     <li><b>[!UICONTROL Working]</b>: de gebruiker heeft op de knop [!UICONTROL Work On It] en werkt momenteel aan het item. </li> 
     <li><b>[!UICONTROL Done]</b>: de gebruiker heeft op de knop [!UICONTROL Done] en heeft hun werk aan het onderdeel voltooid. </li> 
    </ul> <p>Zie voor meer informatie <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[!UICONTROL Work On It] en [!UICONTROL Done] knopoverzicht</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Teams]</td> 
   <td>
   <p>In een [!UICONTROL task] of [!UICONTROL issue] rapport, toont dit gebied informatie over de teams die aan de taken of de kwesties worden toegewezen. Het veld wordt weergegeven [!UICONTROL Primary Owners], alsmede andere teams die zijn toegewezen aan taken of problemen. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Users]</td> 
   <td>
   <p>In een [!UICONTROL Task] of [!UICONTROL Issue] rapport, toont dit gebied informatie over de gebruikers die aan de taken of de kwesties worden toegewezen. Dit veld wordt weergegeven [!UICONTROL Primary Owners], alsmede andere gebruikers die zijn toegewezen aan taken of problemen. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attribute]</td> 
   <td>Een kenmerk is een kenmerk van een [!DNL Workfront] object.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Area]</td> 
   <td> <p>Audits zijn systeemberichten die een actie registreren die in Workfront gebeurde. De volgende soorten audits worden geregistreerd:</p> 
    <ul> 
     <li>[!UICONTROL Scope Change]</li> 
     <li>[!UICONTROL Attachment Action]</li> 
     <li>[!UICONTROL General Edit]</li> 
     <li>[!UICONTROL Status Change]</li> 
     <li>[!UICONTROL Note]</li> 
     <li>[!UICONTROL Combined Entry]</li> 
     <li>[!UICONTROL Error Entry]</li> 
     <li>[!UICONTROL Status Change]</li> 
     <li>[!UICONTROL Subscription Change]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Trail]</td> 
   <td>De verzameling notities die automatisch worden gegenereerd door gebeurtenissen die worden bijgehouden via de Opgenomen wijzigingen ([!UICONTROL Audit Areas]). Elke notitie registreert wie de actie heeft uitgevoerd, wat ze hebben gedaan en wanneer ze het hebben gedaan.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automatic And On Change]</td> 
   <td> <p>Een van de [!UICONTROL Project Update] typen. Dit zal de Geprojecteerde en Geplande chronologie van het Project opnieuw berekenen wanneer het niight herberekeningsproces loopt en wanneer om het even welke update aan het project of de taken binnen het Project wordt gemaakt. </p> <p>Zie voor meer informatie <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecteer het Type van projectupdate </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Beschikbaarheid</p></td> 
   <td> <p>Deze termijn wordt gebruikt met betrekking tot "gebruikersbeschikbaarheid"of "middelbeschikbaarheid"en het illustreert de hoeveelheid tijd dat het middel (gebruiker of baanrol) beschikbaar is om te werken. </p> 
   <p>Workfront berekent de beschikbaarheid van gebruikers in verschillende velden en afhankelijk van de instellingen van de voorkeuren voor het beheer van bronnen in uw systeem. Zie voor meer informatie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voorkeuren voor beheer van bronnen configureren</a>. </p>
   <p>Voor meer informatie over middelbeschikbaarheid, zie <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Aan de slag met Resource Management</a></p>
   Afwisselend, wordt de "capaciteit"ook gebruikt om naar middelbeschikbaarheid te verwijzen. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Automatic Only]</td> 
   <td> <p>Een van de [!UICONTROL Project Update] typen. Hiermee worden de geprojecteerde en geplande tijdlijnen opnieuw berekend wanneer het nibleke herberekeningsproces wordt uitgevoerd.</p> <p>Zie voor meer informatie <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecteer het Type van projectupdate</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>"Zaken zoals gebruikelijk"werk dat aan het runnen van de dagelijkse primaire bedrijfsdoelstellingen bijdraagt.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Backlog]</td> 
   <td>Het gebied in een flexibele omgeving waar nieuwe problemen worden bewaard totdat ze klaar zijn om te worden bewerkt.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Baseline]</td> 
   <td>Een bron van gegevens waarmee herhalingen in een flexibele omgeving worden gemeten.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Billable Expense]</td> 
   <td> <p>Een last die als factureerbaar aan de klant wordt gemerkt. Dit kan ofwel een geplande uitgave zijn, ofwel een werkelijke uitgave.</p> <p>De Geplande Billable Kosten van de Kosten en de Ware Facturable gebieden van de Kosten van de Kosten van de Uitgaven zijn beschikbaar voor u om aan meningen en rapporten toe te voegen. Ze worden niet weergegeven op de pagina's met project- of taakdetails.</p>
   <p>U kunt deze gebieden in de volgende types van rapporten vinden:</p>
   <ul>
   <li>Basislijn</li>
   <li>Sjabloon</li>
   <li>Project (financiële gegevens)</li>
   </ul>
   <p>Voor meer informatie over het merken van een uitgave als factureerbaar, zie <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Projectkosten beheren</a>.</p>
   </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Billing Record]</td> 
   <td> <p>Registreert de inkomsten, uren, of uitgaven die kunnen worden gefactureerd. Deze informatie kan worden gebruikt om facturen op te stellen in een extern boekhoudsysteem.</p> <p>Zie voor meer informatie <a href="../../../manage-work/projects/project-finances/create-billing-records.md">Factureringsrecords maken</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>Status van factureringsrecord</td> 
   <td> <p>In een factureringsrecord of een urenrapport geeft de status van een factureringsrecord aan of de factureringsrecord al dan niet is gefactureerd. U kunt een project niet verwijderen of tijd bewerken die aan een factureringsrecord is gekoppeld. Zie voor meer informatie <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Factureringsrecords maken</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Branding]</td> 
   <td><p>Het aanpassen van [!DNL Workfront] om de interface een verschijning te geven die uw bedrijf door uw kleuren en logo's weerspiegelt te gebruiken.</p><p><strong>OPMERKING</strong><br>Als uw organisatie is aangemeld bij [!DNL Adobe Experience Cloud], is branding niet beschikbaar.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Breadcrumbs]</td> 
   <td> <p>Het gebied boven aan de pagina dat de hiërarchische locatie aangeeft van de locatie van de gebruiker in de toepassing.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Zie voor meer informatie <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Overzicht van Broodkruimels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budget Status]</td> 
   <td> <p>Dit is een verouderd veld. Alle informatie die in dit veld wordt weergegeven, is gerelateerd aan een functie die [!DNL Workfront] is verwijderd en het veld kan niet worden bijgewerkt. </p> <p>Dit gebied toont of het project aan [!UICONTROL Capacity Planner] en of de begrotingsberekening voor de begroting is afgerond. De [!UICONTROL Capacity Planner] is verwijderd uit [!DNL Workfront]. </p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;not added to the capacity planner, its value is <i>Not Included</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;added to the Capacity Planner but is excluded from the budget calculation,&nbsp;the value is <i>Included but not Calculated</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is&nbsp;added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgeted Completion Date]</td> 
   <td> <p>Dit is een verouderd veld. Alle informatie die in dit veld wordt weergegeven, is gerelateerd aan een functie die [!DNL Workfront] is verwijderd. Dit veld kan niet worden bijgewerkt. </p>
   <p> Dit veld is nog steeds zichtbaar in [!UICONTROL project] en [!UICONTROL tasks] rapporten en lijsten.</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgeted Cost]</td>

<td> <p>Dit zijn de kosten verbonden aan het begroten van middelen voor een project. </p>
   <p>Het veld wordt weergegeven in de volgende gebieden van [!DNL Workfront] onder de volgende namen:</p>
   <ul>
   <li><strong>[!UICONTROL Budgeted Cost]</strong>: in de [!UICONTROL Business Case Summary] deelvenster</li>
   <li><strong>[!UICONTROL Cost]</strong>: in de [!UICONTROL Utilization] gebieden wanneer het bekijken van informatie door [!UICONTROL Cost]</li>
   <li><strong>[!UICONTROL Project Budgeted Cost]</strong>: in lijsten en rapporten</li>
   </ul>   
    <p>De [!UICONTROL Budgeted Cost] voor het project wordt de volgende formule gebruikt:</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Meer informatie over berekenen [!UICONTROL Budgeted Cost] en diverse namen voor dit concept te begrijpen in [!DNL Workfront], zie <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">De begrote projectkosten berekenen</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Budgeted Hours]</td> 
   <td> <p>De uren die zijn begroot voor de middelen voor het werk dat zij aan projecten moeten voltooien. Dit veld heeft betrekking op de in de [!UICONTROL Resource Budgeting] gebied van de [!UICONTROL Business Case] (of in de [!UICONTROL Resource Planner]) voor het project of voor de projectmiddelen.</p> <p>Zie voor meer informatie <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Begrijpen [!UICONTROL Budgeted Labor Cost] en [!UICONTROL Budgeted Hours] voor projecten</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Voor informatie over het in de begroting opnemen van gebruikers in [!DNL Resource Planner], zie het artikel <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Begrotingsmiddelen in de [!DNL Resource Planner] met de [!UICONTROL Project] en [!UICONTROL Role] views</a>. </p> 
    <p>De in de [!UICONTROL Resource Budgeting] gebied van de [!UICONTROL Business Case] of de [!UICONTROL Resource Planner] worden weergegeven in de volgende gebieden: [!DNL Workfront] en onder de volgende namen:</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>[!UICONTROL Budgeted Hours] weergavenaam</strong></td> 
        <td><strong>Gebieden van [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Hours]</td> 
        <td>[!UICONTROL Resource Budgeting] gebied van de [!UICONTROL Business Case]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Resource Planner] bekeken door [!UICONTROL Hours]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Budgeted Hours]</td> 
        <td> <p>Gebruiksrapport [!UICONTROL Hours] weergave</p> <p>Voor meer informatie over de [!UICONTROL Utilization] rapport, zie het artikel <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Overzicht van de [!UICONTROL Resource Utilization] verslag</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. Hours]</td> 
        <td> <p>[!UICONTROL Budgeted Hour] verslag</p><p>De [!UICONTROL Budgeted Hour] -object in het rapport Boedgeted Hour verwijst naar informatie die betrekking heeft op een vervangen hulpmiddel voor middelenbeheer. Alleen de "[!UICONTROL Bud. Hours]" in dit verslag wordt verwezen naar de in de [!UICONTROL Resource Planner] of de [!UICONTROL Resource Budgeting] gebied van het project [!UICONTROL Business Case]. </p> <p>Raadpleeg het artikel voor meer informatie over het maken van een rapport <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Een aangepast rapport maken</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Resource Planner Budgeted Hours] </td> 
        <td> <p>Gevonden in de volgende rapporten:</p>
        <ul>
        <li>[!UICONTROL Project] verslag
        <li>[!UICONTROL Project (Financial Data)] verslag
        <li>[!UICONTROL Task] verslag
        <li>[!UICONTROL Issue] verslag
        <li>[!UICONTROL Budgeted Hour] verslag</li>
        </ul>
         <p>Raadpleeg het artikel voor meer informatie over het maken van een rapport <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Een aangepast rapport maken</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Elke andere vermelding van [!UICONTROL Budgeted Hours] in [!DNL Adobe Workfront] verwijst naar uren die zijn gebudgetteerd met vervangen functies die uit Workfront zijn verwijderd. Dit zijn alleen-weergeven velden en werken niet bij met de huidige informatie wanneer u de huidige bronnen in de begroting opneemt. </p>
    <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the&nbsp;Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy&nbsp;Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy&nbsp;Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial&nbsp;Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul> --> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgeted Labor Cost]</td> 
   <td> <p>Dit is de kosten verbonden aan de uren die u, als Manager van het Middel, begroting voor uw baanrollen voor het werk dat zij aan projecten moeten voltooien. </p> <p>De [!UICONTROL Budgeted Labor Cost] in een projectverslag wordt de volgende formule gebruikt:</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Dit veld kan naar het volgende verwijzen:</p> 
    <ul> 
     <li> <p>De arbeidskosten in de [!UICONTROL Resource Budgeting] gebied van de [!UICONTROL Business Case] of in de [!UICONTROL Resource Planner] die worden geassocieerd met de kosten van baanrollen op een project. Voor informatie over het berekenen van de [!UICONTROL Budgeted Labor Cost], zie het artikel <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Understand Budgeted Labor Cost] en [!UICONTROL Budgeted Hours] voor projecten</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>De arbeidskosten in de [!UICONTROL Resource Budgeting] gebied van de [!UICONTROL Business Case] die de [!UICONTROL People Costs] geraamd in een initiatief dat verband houdt met het project van het [!DNL Scenario Planner] wanneer u de Planner van het Scenario gebruikt om uw projectmiddelen te begroten. Zie voor informatie over initiatieven <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Overzicht van initiatieven in het scenario Planner</a>. </p> <p>De [!DNL Scenario Planner] vereist een aanvullende licentie. Voor informatie over de [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">De [!DNL Scenario Planner] overzicht</a>. </p> </li> 
     <p>Deze wordt in de volgende gebieden onder de volgende namen weergegeven:</p>
   <ul>
   <li><strong>[!UICONTROL Budgeted Labor Cost]</strong>: in de [!UICONTROL Resource Budgeting] gebied van de [!UICONTROL Business Case].
   <li><strong>[!UICONTROL Budgeted Cost]</strong>: in de [!UICONTROL Utilization] verslag [!UICONTROL Cost] weergave
   <p>Zie voor meer informatie <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Informatie over bronnengebruik weergeven </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: in de [!DNL Resource Planner] Project of [!DNL Role] weergaven, wanneer weergeven op kosten
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: in de volgende verslagen: 
   <ul>
    <li>[!UICONTROL Project] verslag</li>
    <li>[!UICONTROL Project (Financial Data)] verslag</li>
    <li>[!UICONTROL Task] verslag</li>
    <li>[!UICONTROL Issue] verslag</li>
    <li>[!UICONTROL Budgeted Hour] verslag</li> 
    </ul>
    <p>Raadpleeg het artikel voor meer informatie over het maken van een rapport <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Een aangepast rapport maken</a>.</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in&nbsp;Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;.&nbsp;</p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Budgeted Start Date]</td> 
  <td> <p>Dit is een verouderd veld. Alle informatie die in dit veld wordt weergegeven, is gerelateerd aan een functie die [!DNL Workfront] is verwijderd. Dit veld kan niet worden bijgewerkt.</p>
  <p>Deze gebieden zijn verwijderd uit [!DNL Workfront]. </p> 
  <p>Het veld is nog steeds zichtbaar in [!UICONTROL project] en [!UICONTROL task] rapporten en lijsten.</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Burndown Chart]</td> 
   <td>Een lijngrafiek die een visuele vertegenwoordiging van voltooide en resterende werk verstrekt.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case]</td> 
   <td> <p>Een hulpmiddel dat wordt gebruikt om te beoordelen of een project van [!UICONTROL Idea] status aan de [!UICONTROL Planning] status. Met andere woorden: [!UICONTROL business case] helpt de organisatie te beslissen of het de moeite waard is het project te lanceren en te voltooien, met name wanneer zij projecten vergelijkt met andere projecten in een portfolio.</p> <p>Zie voor meer informatie <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Een [!UICONTROL Business Case] voor een project </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case Budgeted Hours]</td> 
   <td> <p>Dit is een verouderd veld. Alle informatie die in dit veld wordt weergegeven, is gerelateerd aan een functie die [!DNL Workfront] is verwijderd. Dit veld kan niet worden bijgewerkt.</p> <p>Dit veld is nog zichtbaar in project en [!UICONTROL task] lijsten en rapporten. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Assignment]</td> 
   <td> <p>Een van de taken [!UICONTROL Duration Types] . Dit zal het percentage van een 8-uurs het werkdag berekenen dat de gebruiker die aan de taak wordt toegewezen aan de taak zal worden toegewezen, gebaseerd op [!UICONTROL Duration] van de taak en de [!UICONTROL Work Required].</p> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overzicht van taak [!UICONTROL Duration] en [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Work]</td> 
   <td> <p>Een van de taken [!UICONTROL Duration Types]. Hiermee wordt het [!UICONTROL Work Required] over een taak, gezien de [!UICONTROL Duration] en de gebruiker [!UICONTROL Assignment] percentages (die gebaseerd zijn op een werkdag van 8 uur).</p> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overzicht van taak [!UICONTROL Duration] en [!UICONTROL Duration Type]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar]</td> 
   <td> <p>Er zijn twee soorten kalenders in [!DNL Workfront]: de [!UICONTROL Home Calendar] en kalenderverslagen.</p> <p>De [!UICONTROL Home Calendar] is een persoonlijke kalender die een gebruiker in staat stelt zijn werkbelasting te beheren op basis van de beschikbare uren in [!DNL Workfront]. De gebruikers kunnen hun ook integreren [!UICONTROL Home Calendar] with [!DNL Outlook] ([!DNL Google] en [!DNL Microsoft] toekomstige integratie). </p> <p>Voor meer informatie over de [!UICONTROL Home Calendar], zie <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">[!UICONTROL Home Calendar] weergave</a>.</p> <p>Een kalenderrapport is een dynamisch rapport waarin gebruikers de datum en andere belangrijke details van een gebeurtenis kunnen bekijken, met inbegrip van de vervaldatum, de status van het werk, en de gebruiker aan wie de gebeurtenis wordt toegewezen.</p> <p> Voor meer informatie over kalenderrapporten, zie <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">Overzicht van kalenderrapporten</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Can Start]</td> 
   <td> <p>In dit veld wordt aangegeven of een taak gereed is om te worden bewerkt. Als het begin klaar is om te worden bewerkt aan de [!UICONTROL Can Start] veld op de taak is ingesteld op [!UICONTROL True]. </p> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">"[!UICONTROL Can Start]" overzicht voor taken</a>.</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    --> <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.&nbsp;</li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.&nbsp;</li> 
     </ul>
    --> 
    <!--
     <p>For information about task predecessors, see <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p>
    --> <!--
     <p>Tip: If the Dependency Type between a task and its predecessors is Start-Start, the predecessor must start before the predecessor relationship is considered resolved and the successor tasks can start. For information about dependency types, see <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>. </p>
    --> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Capacity</td> 
    <td>The total availability (measure in either hours or FTE) of a designated user, resource pool, team, rob role, or company.</td> 
   </tr>
  -->

<tr> 
   <td> <p>Capaciteit</p> </td> 
   <td> <p>De beschikbare tijd van een bron wanneer zij aan het werk kunnen worden toegewezen. Zie "Beschikbaarheid". </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Category]</p> </td> 
   <td> <p>Een categorie is een aangepast formulier. U kunt rapporten voor dit voorwerp bouwen en u kunt het in andere objecten rapporten tonen, eveneens. Niet alle objecten kunnen een aangepast formulier of een aangepaste categorie hebben. De volgende objecten kunnen een aangepast formulier hebben: <br></p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Document]</li> 
     <li>[!UICONTROL Expense]</li> 
     <li>[!UICONTROL Program]</li> 
     <li>[!UICONTROL User]</li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Category Name]</td> 
   <td> <p>Als een kolom wordt toegevoegd aan de weergave van een van de volgende objecten, wordt een lijst weergegeven met alle aangepaste formulieren die aan deze objecten zijn gekoppeld:</p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]<br></li> 
     <li>[!UICONTROL Issue]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL Document]<br></li> 
     <li>[!UICONTROL Expense]<br></li> 
     <li>[!UICONTROL Program]<br></li> 
     <li>[!UICONTROL User]<br></li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Management]</td> 
   <td>Een praktijkgebied concentreerde zich op het bepalen van, het begrip van, en het aanpassen van gepland werk aan veranderingen in werkingsgebied, programma, kosten, en middelfactoren.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Order]</td> 
   <td>Een type van kwestie tegen een project dat een gevraagde verandering in het overeengekomen werkingsgebied schetst.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Only]</td> 
   <td>Een van de projecten [!UICONTROL Update Types]. Alleen updates [!UICONTROL Project Projected] en [!UICONTROL Planned] de termijnen wanneer de Updates aan taken worden gemaakt of uitgeeft worden uitgevoerd op het project of de taken.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Order]</td> 
   <td> <p>Een van de [!UICONTROL Issue] typen, waarbij doorgaans wordt aangegeven dat een ongeplande hoeveelheid werk moet worden verricht voordat het project kan worden voltooid.</p> <p>Voor meer informatie over [!UICONTROL Issue] typen, raadpleegt u de sectie "Standaarduitgavetypen" in het artikel <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">Standaardobjecttypen aanpassen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Child Task]</td> 
   <td>Een taak die [!UICONTROL Subtask] van een [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Children]</td> 
   <td>De verzameling van [!UICONTROL Subtasks] een [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] en [!UICONTROL Training]</td> 
   <td>Leermodules, certificeringen, standaarden of een praktijkgemeenschap.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit]</td> 
   <td>Een communicatiemiddel voor gebruikers om verwachtingen ten aanzien van te plaatsen taak te leveren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit Date]</td> 
   <td>Een communicatiemiddel voor gebruiker om verwachtingen rond taak te plaatsen te leveren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Communication] en [!UICONTROL Reporting]</td> 
   <td>Normen om de uitzonderingen en de gezondheid van een project, programma, of portefeuille te herzien</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Company]</td> 
   <td> <p>A [!UICONTROL Company] is een organisatorische eenheid in [!DNL Workfront]. </p> 
   <p> U kunt een gebruiker of een project met één bedrijf associëren. Zie voor meer informatie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">Bedrijven maken en bewerken</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion date]</td> 
   <td> <p>De datum waarop een project, een taak of een uitgave moet worden voltooid. Er zijn verschillende typen [!UICONTROL Completion dates] in [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL Actual Completion Date]. Zie voor meer informatie <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">Overzicht van het project [!UICONTROL Actual Completion Date] </a>.</li> 
     <li>[!UICONTROL Planned Completion Date]. Zie voor meer informatie <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Het project instellen [!UICONTROL Planned Completion Date]</a> en <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Overzicht van de taak [!UICONTROL Planned Completion Date]</a>.</li> 
     <li>[!UICONTROL Projected Completion Date]. Zie voor meer informatie <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Overzicht van de [!UICONTROL Projected Completion Date] voor projecten, taken en kwesties</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Day]</td> 
   <td>De dag in verhouding tot het begin van de [!UICONTROL Template], dat [!UICONTROL Template Task] of [!UICONTROL Template] moet volledig zijn.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Mode]</td> 
   <td> <p>Dit geeft aan hoe een project wordt gemarkeerd als [!UICONTROL Complete]. Deze kan twee waarden hebben:</p> 
    <ul> 
     <li>[!UICONTROL Manual]: Een gebruiker moet de projectstatus wijzigen in [!UICONTROL Complete].</li> 
     <li>[!UICONTROL Automatic]: De projectstatus wordt automatisch gewijzigd in [!UICONTROL Complete] wanneer alle taken in het project 100% voltooid zijn en alle problemen zijn afgesloten.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition]</td> 
   <td> <p>Dit is een visuele weergave van de voortgang van een taak, kwestie of project.</p> <p>Voor projecten kan de voorwaarde handmatig worden ingesteld door de eigenaar van het project of automatisch worden ingesteld door [!DNL Workfront], op basis van de stand van de voortgang van het project. </p> <p>De mogelijke waarden voor de projectvoorwaarde zijn:</p> 
    <ul> 
     <li>[!UICONTROL On Target]</li> 
     <li>[!UICONTROL At Risk]</li> 
     <li>[!UICONTROL In Trouble]</li> 
    </ul> <p>Zie het artikel voor meer informatie over projectvoorwaarden <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Overzicht van [!UICONTROL Project Condition] en [!UICONTROL Condition Type]</a>.</p>
     <p>U kunt taak en uitgiftevoorwaarden met een aantal associëren dat in rapporten kan tonen. In de onderstaande lijsten staan de standaardnamen en -nummers voor taken en uitgaven. Uw systeembeheerder kan de namen van voorwaarden bijwerken en zij kunnen nieuwe voorwaarden met verschillende aantallen toevoegen. Nadat een getal aan een voorwaarde is gekoppeld, kan het niet worden bewerkt.  </p> 
     <p>Voor taken wordt de voorwaarde handmatig ingesteld door de eigenaar van de taak. De mogelijke waarden voor de taakvoorwaarde zijn:</p> 
    <ul> 
     <li>[!UICONTROL Going Smoothly] (0)<br></li> 
     <li> [!UICONTROL Some Concerns] (1)<br></li> 
     <li>[!UICONTROL Major Roadblocks] (2)</li> 
    </ul> <p>Raadpleeg het artikel voor meer informatie over taakvoorwaarden <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Bijwerken [!UICONTROL Condition] voor taken en problemen</a>.</p> <p>Voor uitgaven wordt de voorwaarde handmatig ingesteld door de eigenaar van de uitgave. De mogelijke waarden voor de uitgiftevoorwaarde zijn:<br></p> 
    <ul> 
     <li>[!UICONTROL Going Smoothly] (0)<br></li> 
     <li>[!UICONTROL Some Concerns] (1)<br></li> 
     <li>[!UICONTROL Major Roadblocks] (2)</li> 
    </ul> 
   <p><b>OPMERKING</b></p>
    <p>Wanneer de [!UICONTROL Condition] veld wordt bijgehouden in [!UICONTROL Journal Entry] de [!UICONTROL New] en [!UICONTROL Old Number Values] Geef het nummer weer dat aan de voorwaarde is gekoppeld in plaats van de naam ervan. Als een voorwaarde oorspronkelijk niet voor een taak of een kwestie wordt bepaald en u het later bijwerkt, zal de dagboekingang die de update vangt tonen [!UICONTROL Old Number Value] van de [!UICONTROL Condition] veld als -2,147,483,648. Zie ook "[!UICONTROL New Number Value]", "[!UICONTROL Old Number Value]", en "[!UICONTROL Journal Entry]" in dit artikel. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition Update]</td> 
   <td> <p>Dit gebied toont de huidige staat van taken, projecten of kwesties. Deze optie toont de meest recente updates die de eigenaars van taken, projecten of problemen hebben verstrekt in [!UICONTROL Update Status] en de nieuwe voorwaarde.</p> <p>Opmerkingen die zijn gemaakt bij updates van voorwaarden worden niet weergegeven in het dialoogvenster [!UICONTROL Condition Update] kolom; alleen de hoofdupdate wordt weergegeven.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Date]</td> 
   <td> <p>Als u een [!UICONTROL Task Constraint] die gekoppeld is aan een specifieke datum, zoals [!UICONTROL Must Start On], dan wordt die specifieke datum [!UICONTROL Constraint Date] van de taak.</p> <p>De volgende taakbeperkingen werken de [!UICONTROL Constraint Date] veld:</p> 
    <ul> 
     <li>[!UICONTROL Must Start On]</li> 
     <li>[!UICONTROL Must Finish On]</li> 
     <li>[!UICONTROL Start No Later Than]</li> 
     <li>[!UICONTROL Start No Earlier Than]</li> 
    </ul> <p><b>TIP</b></p>   
     <ul> 
      <li> <p>Een taak met een [!UICONTROL Constraint] van [!UICONTROL Fixed Dates] heeft geen [!UICONTROL Constraint Date]. </p> </li> 
      <li> <p> [!UICONTROL Constraint Date] kan alleen worden weergegeven in een rapport of aangepaste weergave.</p> </li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Day]</td> 
   <td> <p>Als u een Restrictie van de Taak in een malplaatjetaak gebruikt die aan een specifieke dag, zoals moet op beginnen is, dan wordt die specifieke dag de Dag van de Beperking van de malplaatjetaak.</p> <p>De volgende taakbeperkingen werken de [!UICONTROL Constraint Day] veld:</p> 
    <ul> 
     <li>[!UICONTROL Must Start On]</li> 
     <li>[!UICONTROL Must Finish On]</li> 
     <li>[!UICONTROL Start No Later Than]</li> 
     <li>[!UICONTROL Start No Earlier Than]</li> 
    </ul> <p><b>TIP</b></p> <p>  [!UICONTROL Constraint Day] kan alleen worden weergegeven in een rapport of aangepaste weergave. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Type]</td> 
   <td> <p>De planningsneiging van een taak. Bijvoorbeeld: [!UICONTROL As Soon as Possible] een taak zo spoedig mogelijk zal beginnen, en [!UICONTROL Finish No Later Than] zal een taak plannen die door [!UICONTROL Constraint Date] en later.</p> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[!UICONTROL Task Constraint] overzicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contextual Menu]</td> 
   <td>Een menu, dat zich aan de linkerkant van het scherm bevindt, waarop de items worden gewijzigd in de correlatie met de actieve inhoud. Wanneer een gebruiker bijvoorbeeld een project bekijkt, [!UICONTROL Contextual Menu] koppelingen naar projectgerelateerde informatie en tools weergeven.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converted Issue Originator]</td> 
   <td>Een gebied in een project of taakrapport dat informatie over de gebruiker toont die is [!UICONTROL Primary Contact] van een kwestie wanneer de kwestie in een project of een taak wordt omgezet. Het veld wordt ook weergegeven in het dialoogvenster [!UICONTROL Project Details]  op de plaats waar de naam van de [!UICONTROL Primary Contact] van de omgezette emissie. Zie ook "[!UICONTROL Primary Contact]" in dit artikel.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Cost]</td> 
   <td> <p>Het geldbedrag dat u moet uitgeven wanneer het voltooien van een project, een taak, of een kwestie. </p> <p>U kunt verschillende soorten arbeidskosten, uitgaven, risico's volgen die met het project verband houden.Voor informatie over het volgen van kosten in [!DNL Workfront] zie <a href="../../../manage-work/projects/project-finances/track-costs.md">Trackkosten</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cost Type]</td> 
   <td>Voor een taak [!UICONTROL Cost Type] bepaalt hoe de taak kosten zal opleveren. Enkele voorbeelden zijn [!UICONTROL Fixed Hourly], [!UICONTROL User Hourly], en [!UICONTROL User Hourly plus Fixed]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cross-Project Dependencies]</td> 
   <td> <p>Een taak van één project is afhankelijk van een taak van een verschillend project.</p> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">Predecessors voor meerdere projecten maken</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custom Data]</td> 
   <td> <p>Gegevens die uniek zijn voor een organisatie. Organisaties kunnen de [!DNL Workfront] door aangepaste formulieren en aangepaste velden te maken. Deze douaneinformatie kan rapportering voor KPIs, controle, en vraagmengeling drijven. </p> <p>[!UICONTROL Custom Data] kan worden gekoppeld aan:</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Iterations]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Data Type]</td> 
   <td>De optie om op te geven of een [!UICONTROL Custom Data] Veld wordt in de database opgeslagen als tekst, een datum, een getal of valuta.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Display Type]</td> 
   <td>Het weergavetype van een aangepast veld. Voorbeelden zijn [!UICONTROL Drop-Down], [!UICONTROL Text Field], [!UICONTROL Text Area], [!UICONTROL Radio Buttons], enz.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Field]</td> 
   <td>Voor de gegevens van de Douane die de gebruiker toestaan om uit verscheidene opties te selecteren, zijn dit de waarden waarvan een gebruiker kan selecteren. Aangepaste opties zijn alleen geldig op [!UICONTROL Drop-Down], [!UICONTROL Multi-Select Drop-Down], [!UICONTROL Radio Buttons], en [!UICONTROL Checkboxes].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Form Label]</td> 
   <td>Wanneer u een Type aangepaste weergave gebruikt met aangepaste opties, is dit de tekst voor de gebruikersinterface die wordt weergegeven in het vervolgkeuzemenu, de selectievakjes of de keuzerondjes voor die aangepaste optie.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Value]</td> 
   <td>Wanneer u een aangepast veld gebruikt met aangepaste opties, is dit de waarde die in de database voor een bepaalde optie wordt opgeslagen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom View]</td> 
   <td>Een definitie van de gegevensvelden of kolommen die worden weergegeven voor elk object in een lijst.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Customer]</td> 
   <td>Een organisatie die een instantie van Workfront gebruikt.</td> 
  </tr> 
 </tbody> 
</table>

## D - F

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objectnaam</th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Dashboards]</td> 
   <td> <p> U kunt dit gebied in een rapport of een mening van het voorwerp van het Rapport toevoegen, om de dashboards te tonen waarop het rapport in een lijst wordt vermeld. </p> <p> U kunt dit veld gebruiken om te filteren op rapporten die ook op een specifiek dashboard worden weergegeven. </p> <p> Voor meer informatie over het omvatten van dashboardinformatie over rapportobjecten rapporten, zie "Begrijpen welke Rapporten op Dashboards"sectie in het artikel worden vermeld <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">Rapporten openen en ordenen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data Type]</td> 
   <td>Zie "[!UICONTROL Custom Data Type]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Days Late]</td> 
   <td> <p>In dit veld wordt een datumverschil weergegeven tussen [!UICONTROL Planned Start] en [!UICONTROL Today] als de [!UICONTROL Actual Completion Date] ontbreekt.</p> <p>Geeft ook een datumverschil weer tussen [!UICONTROL Actual Completion] en [!UICONTROL Planned Completion], wanneer [!UICONTROL Actual Completion Date] aanwezig is.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Default Schedule]</td> 
   <td> <p>Aanpasbare standaardwerkuren die moeten worden toegewezen aan gebruikers en projecten binnen een organisatie. </p> <p>Planningen worden gebruikt om de geplande, start- en voltooiingsdatums te berekenen van taken die aan gebruikers zijn toegewezen.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Deliverable]</td> 
   <td>Kwantificeerbare goederen of diensten die bij de voltooiing van een project moeten worden geleverd.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Demand Management]</td> 
   <td>Scores en prioritering van de innameprocessen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Department Goals]</td> 
   <td>Doelen uniek aan een specifieke afdeling die zich op het verbeteren van operationele metriek binnen de afdeling richt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency]</td> 
   <td>Het verband tussen twee taken die één taak vereisen om status vóór de andere taak te veranderen kan status ook veranderen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency Type]</td> 
   <td> <p>Het type van het plannen van verhouding tussen een taak en zijn voorganger(s). Eén voorbeeld is [!UICONTROL Finish-Start], waarvoor de eerste taak moet zijn voltooid voordat de tweede taak kan worden gestart.</p> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overzicht van typen taakafhankelijkheid</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document]</td> 
   <td>Elk bestand dat is gekoppeld aan een object binnen [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document Version]</td> 
   <td> <p>Telkens wanneer hetzelfde document naar hetzelfde object wordt geüpload, wordt er een versienummer aan toegewezen. Gebruikers kunnen verschillende opties voor een vorige versie van een document weergeven en wijzigen.</p> <p>Zie voor meer informatie <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">Documentversies beheren</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration]</td> 
   <td> <p>De tijd die is toegewezen voor het voltooien van een taakprobleem of project (zoals bepaald door het aantal dagen tussen de [!UICONTROL Planned Start] en de geplande voltooiing).</p> 
    <ul> 
     <li>Voor taken, is de Duur een editable gebied als het Type van Duur van de taak niet Eenvoudig is. Als het Type van Duur van de taak Eenvoudig is, of als de Beperking van de Taak Vaste Datums is, is de Duur een berekening die door Workfront wordt uitgevoerd.</li> 
     <li>Voor kwesties, is de Duur altijd een editable gebied en het zou een schatting van een aantal dagen moeten vertegenwoordigen die de kwestie zouden vereisen om worden opgelost.</li> 
     <li>Voor projecten is de duur een berekening die wordt uitgevoerd door [!DNL Workfront] en geeft het het verschil in dagen weer tussen het geplande begin van de eerste taak en het [!UICONTROL Planned Completion] van de meest recente taak van het project.</li> 
    </ul> <p>Voor meer informatie over het verschil tussen [!UICONTROL Duration] en [!UICONTROL Planned Duration] zie het artikel voor taken <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">Verschil tussen [!UICONTROL Planned Duration] en [!UICONTROL Duration] voor taken</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration in Minutes]</td> 
   <td>In dit veld wordt dezelfde informatie weergegeven als in het dialoogvenster [!UICONTROL Duration] in minuten in plaats van dagen. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Duration per Occurrence]</td> 
   <td> <p>Dit wordt weergegeven in het dialoogvenster [!UICONTROL Task Details] en de [!UICONTROL Edit Task] de vakjes van een ouder van terugkomende taken. Het toont de duur van elke terugkomende taak. Voor informatie over het creëren van terugkomende taken, zie <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Herhalende taken maken</a>. </p> <p> <span>De duur die in individuele terugkerende taken wordt gewijzigd toont niet de waarde die op dit gebied wordt vermeld.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Duration Type]</td> 
   <td> <p>Een taakgebied dat erop wijst hoe het werk dat wordt vereist om de taak te voltooien aan de wijzers over de taakduur wordt toegewezen. Het vertegenwoordigt de relatie tussen de [!UICONTROL Duration] van de taak [!UICONTROL Work Required]en de hoeveelheid tijd, of [!UICONTROL Allocation], moeten de toegewezen middelen aan de taak besteden om deze te voltooien. </p> <p>Dit veld wordt weergegeven op het tabblad [!UICONTROL Details] taaktabblad. </p> <p>De opties voor het Type van Duur van een taak zijn:</p> 
    <ul> 
     <li>[!UICONTROL Calculated assignment]</li> 
     <li>[!UICONTROL Calculated Work]</li> 
     <li>[!UICONTROL Effort Driven]</li> 
     <li>[!UICONTROL Simple]</li> 
    </ul> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overzicht van taak [!UICONTROL Duration] en [!UICONTROL Duration Type]</a>.</p> 
    —&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Duration Unit]</td> 
   <td>De eenheid die wordt gebruikt om tijd in een machtsonderzoek te meten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Effort Driven]</td> 
   <td>De verhouding tussen het aantal gebruikers en de hoeveelheid tijd de taak zal vergen om te voltooien. Terwijl u meer gebruikers toevoegt, neemt de totale tijd die voor de taak is gepland af, maar blijft de duur van de taak ongewijzigd. Als een taak bijvoorbeeld een vat pinda's schuurt, wordt de geplande tijd verkort als u meer mensen toevoegt, maar blijft de tijdsduur per dag ongewijzigd.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Elapsed Time]</td> 
   <td> <p>[!UICONTROL Elapsed time] is een tijdseenheid voor een taak [!UICONTROL Duration]. De tijd tussen [!UICONTROL Planned Start Date] en de [!UICONTROL Planned Completion Date] van een taak die vakantie, weekends, en onderbreking omvat. Met andere woorden, de verstreken tijd is de doorloop van kalenderdagen. </p> <p>[!DNL Workfront] ondersteunt de volgende verstreken tijdeenheden voor de taakduur:</p> 
    <ul> 
     <li> <p>[!UICONTROL Elapsed Minutes]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Hours]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Days]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Weeks]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Months]</p> </li> 
    </ul> <p>Voor meer informatie over taakduur, met inbegrip van verstreken tijd, zie <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overzicht van taak [!UICONTROL Duration] en [!UICONTROL Duration Type]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL End Date]</td> 
   <td> <p> In een [!UICONTROL Rate] rapport, dit is de datum waarop een nieuw factureringspercentage voor een baanrol op projectniveau eindigt. De uren verbonden aan het project die vóór deze datum zijn worden vermenigvuldigd met dit het factureringspercentage om de opbrengst op het project te berekenen. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Engagement]</td> 
   <td>De [!UICONTROL Work Performance Indicator] (WPI) die aangeeft wanneer het engagement en het geloof in de taak, het project, het team of de organisatie afneemt. Dit geeft aan dat je moet optreden om dat geloof en engagement nieuw leven in te blazen. WPI zou worden gemeten door de eenvoudige vragen te stellen: "Heb je begrepen wat van je werd verwacht? Heeft het werk dat u hebt toegewezen een verschil gemaakt met de organisatie? Heb je geweldig werk gedaan?"</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Enterprise Goals]</td> 
   <td>Interfunctionele doelstellingen die tot de metriek van de bedrijfsdoelstellingen bijdragen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event]</td> 
   <td>Elke wijziging in een project of taak.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event Handler]</td> 
   <td>Geautomatiseerde taken die plaatsvinden wanneer gebeurtenissen plaatsvinden. Een veelvoorkomend voorbeeld is een geautomatiseerd e-mailbericht.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event notification]</td> 
   <td>E-mail die wordt gegenereerd op basis van een gebeurtenishandler.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Expenses]</td> 
   <td>Niet-arbeidskosten voor taken of projecten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External]</td> 
   <td> <p>Dit is doorgaans een licentietype of een gebruiker met een dergelijke licentie. Een gebruiker met een dergelijk licentietype kan alleen informatie in het systeem controleren. Zij kunnen niet actief aan het werk deelnemen.</p> <p>Zie voor meer informatie <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] overzicht van licenties</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External System]</td> 
   <td>Alle diensten of software die buiten het aangewezen registratiesysteem worden opgeslagen en beheerd.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Field]</td> 
   <td><p>Alle Workfront-objecten of de bijbehorende informatie, zoals deze in de database worden weergegeven. </p>
   <p>"Project", "user" en "hour" zijn bijvoorbeeld zowel Workfront-objecten als velden. "Naam", "status", "eigenaar" en "begindatum" zijn Workfront-velden die zijn gekoppeld aan de bovenstaande objecten. </p>

<p>Wanneer u naar objecten verwijst, kunnen de termen "objecten" en "velden" door elkaar worden gebruikt.</p>
   <p>In het bereik van rapportage verwijzen de "velden" naar de objecten of de informatie over het object dat u wilt vastleggen in het rapport.</p>

<p><b>OPMERKING</b></p>

<p>Bij meer tekstrapportage verwijzen velden naar de objecten of hun informatie zoals deze wordt weergegeven in de database.</p>
   <p>Soms is de naam die u in de gebruikersinterface ziet anders dan de naam van het veld in de database. 'issue' is bijvoorbeeld de naam van het object in de Workfront-interface, maar 'opTask' is de naam van het object (of het veld) in de Workfront-database. </p> 
   <p> Het is belangrijk om het gebied te gebruiken zoals het in het gegevensbestand wanneer het schrijven van een tekst-wijze rapport, mening, filter, of groepering verschijnt, of wanneer het creëren van een berekend gebied.</p>

<p>Zie voor meer informatie <a href="../../../wf-api/general/api-explorer.md">API Explorer</a> en <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">Overzicht van de tekstmodus</a>.</p>

<p>Workfront wordt standaard geleverd met een set velden die zowel objecten als hun gegevens definiëren. U kunt ook aangepaste velden maken om objecten te definiëren, maar u kunt geen aangepaste objecten maken.</p> 
   </td> 
  </tr>

<tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>Één van de belangrijkste bouwstenen van een rapport of een lijstelement dat bepaalt welke informatievertoningen op het scherm. Zie voor meer informatie over rapportelementen <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementen rapporteren: filters, weergaven en groepen</a>.</p> <p>De filter bepaalt de resultaten die in een rapport of op een [!DNL Workfront] , zoals projecten, taken of problemen.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>Procedure voor het beheren van de loonkosten, kosten en inkomstengegevens in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fixed Cost]</td> 
   <td>U kunt een vast bedrag van kosten voor een project bepalen. Dit maakt deel uit van het [!UICONTROL Planned Cost] van het project dat het bedrag vertegenwoordigt dat u nodig hebt om het project te voltooien. Voor informatie over kosten raadpleegt u <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Trackkosten</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fixed Revenue]</td> 
   <td>U kunt een vast bedrag van opbrengst voor een project bepalen. Dit maakt deel uit van het [!UICONTROL Planned Revenue] van het project dat de hoeveelheid geld vertegenwoordigt die u zou kunnen verkrijgen als u het project voltooit. Zie voor informatie over inkomsten <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overzicht van facturering en inkomsten</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Flags]</td> 
   <td> <p> Dit is hetzelfde veld als [!UICONTROL Status Icons], maar deze optie is alleen beschikbaar voor de volgende weergaven: </p> 
    <ul> 
     <li> [!UICONTROL Templates] </li> 
     <li> [!UICONTROL Expenses] </li> 
    </ul> <p> Zie het artikel voor meer informatie <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Ingebouwde statuspictogrammen in weergaven</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>Mappen worden gebruikt om documenten of rapporten te ordenen die aan een object zijn gekoppeld.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (voltijdequivalent)</td> 
   <td>Dit is het Voltijdequivalent dat op de hoeveelheid tijd wijst dat een middel voor het werk beschikbaar is. 
   De [!UICONTROL FTE] wordt weergegeven in de volgende gebieden: 
  <ul>
   <li> Gebruikersprofiel, bij het bewerken of maken van de gebruiker </li>
   <li> [!UICONTROL Resource Planner] </li>
   <li> [!UICONTROL Scenario Planner] (aanvullende licentie vereist voor de Workfront Scenario Planner) </li>
   <li> Gebruikerslijsten en -rapporten </li> </ul>

<p>De [!UICONTROL FTE] moet een decimaal getal zijn tot en met 1, en mag niet 0 zijn. </p>
   <p> An [!UICONTROL FTE] van 1 (dit is de standaardwaarde voor [!UICONTROL FTE] veld, zoals gedefinieerd in hun profiel) betekent dat een bron (gebruiker of rol) het volledige aantal uren werkt, op basis van het schema dat de beschikbaarheid ervan berekent. </p>
   <p>Uw Workfront-beheerder bepaalt welk schema wordt gebruikt om de beschikbaarheid van de gebruiker te bepalen.  </p>
   <ul>
   <li> Wanneer de [!UICONTROL Default Schedule] wordt gebruikt, gebruikt Workfront de [!UICONTROL FTE] van de gebruiker in hun profiel wordt gevonden om beschikbaarheid te berekenen. </li>
   <li> Wanneer het Programma van de Gebruiker wordt gebruikt, gebruikt Workfront de tijd van de gebruiker weg, [!UICONTROL Work Time] waarde, en [!UICONTROL Default Schedule]-uren om de gebruikersgegevens te berekenen [!UICONTROL FTE]. </li> </ul>

<p>Zie voor meer informatie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voorkeuren voor beheer van bronnen configureren</a>.  </p>
   <p>Voor meer informatie over het maken van programma's in [!DNL Workfront], zie <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Een schema maken</a>. </p>

<p><b>OPMERKING</b></p>
   <p>Voor alle berekeningen in de [!UICONTROL Scenario Planner], Workfront gebruikt de volgende waarde: 1 [!UICONTROL FTE] = 8 uur.</p>
   <p>Zie voor meer informatie <a href="../../../scenario-planner/get-started-with-scenario-planning.md">Aan de slag met de [!UICONTROL Scenario Planner]</a>. </p>
   </td> </tr> 
   </tbody> 
   </table>

<!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Task field used by the planner to set how the work required is allocated to the assignees across the duration.</p>
<!--
FTE
The designated full time equivalency for users. A full-time user should have 100% FTE and part-time user should have a percentage that equals their working hours. 
-->

## G - I

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objectnaam</th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Gantt Chart]</td> 
   <td> <p>Een visuele tijdlijn van het project dateert in een kalenderweergave op basis van de geplande of geplande datums aangezien de taken van het project op dit moment gepland zijn.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal]</td> 
   <td><p>Er zijn twee concepten van doelstellingen in [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>Projectdoelen</b>: Een reeks bedrijfsdoelstellingen die door de relevante belanghebbenden van een project zijn overeengekomen. De doelstellingen van het project maken deel uit van het BedrijfsGeval van een project. </p> <p>U kunt projectdoelstellingen niet in lijsten of rapporten tonen maar u kunt tot hen door API toegang hebben. </p> <p>Voor informatie over de projectdoelstellingen van het BedrijfsGeval, zie <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">Zakelijke hoofddoelen maken </a>. </p> </li> 
     <li> <p><b>Strategische doelstellingen</b>: Een strategisch doel is een doel dat u kunt creëren om uw werkstrategie voor een specifieke periode te plannen. U kunt deze typen doelen maken met [!DNL Workfront Goals]. Uw organisatie moet een extra licentie aanschaffen en u moet toegang hebben tot deze functie om strategische doelen te kunnen maken. [!DNL Workfront Goals] alleen beschikbaar zijn met een extra licentie.</p> 
     <p>Zie voor meer informatie <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] overzicht </a>. </p> 
     <p>U kunt strategische doelstellingen in een doel of een projectrapport tonen en tot hen toegang hebben door API. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal Hierarchy]</td> 
   <td> <p>In [!UICONTROL Goal] en [!UICONTROL Project] rapporten, is dit een inzamelingsgebied dat de doelstellingen in de hiërarchie toont dat een strategisch doel tot behoort wanneer het aan andere doelstellingen richt. De doelen worden gescheiden door een ▸ scheidingsteken. </p> <p>Alleen de ouders van het doel en het doel tonen op dit gebied. Onderliggende doelen worden niet weergegeven. </p> <p>Voor informatie over het uitlijnen van doelen in [!DNL Workfront Goals], zie <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">Overzicht van uitlijning van doelstellingen in [!DNL Workfront Goals]</a>. </p> 
   <p>Dit veld is alleen zichtbaar als uw organisatie een aankoop heeft gedaan [!DNL Workfront Goals]. Voor informatie over het beheer van strategische doelen met [!DNL Workfront Goals], zie <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] overzicht </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal Success Score]</td> 
   <td> In een [!UICONTROL Project report] dit gebied wordt gebruikt om naar project-vlakke doelstellingen te verwijzen verbonden aan [!UICONTROL Business] Case. Dit is momenteel een verouderd veld en is niet gekoppeld aan functionaliteit.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Goals] </td> 
   <td> <p>In een [!UICONTROL Project] rapport, is dit een inzamelingsgebied dat alle strategische doelstellingen toont die met een project worden geassocieerd. De doelen worden gescheiden door komma's.</p> <p>Dit veld is alleen zichtbaar als uw organisatie een aankoop heeft gedaan [!DNL Workfront Goals]. Voor informatie over het beheer van strategische doelen met [!DNL Workfront Goals], zie <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] overzicht</a>. Voor meer informatie over strategische doelstellingen en projectdoelstellingen in [!DNL Workfront], zie "[!UICONTROL Goal]" in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global Interface Preferences]</td> 
   <td>Interfacemontages die alle gebruikers beïnvloeden. [!UICONTROL Global Interface Preferences] kan door [!UICONTROL User Interface Preferences].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Group]</td> 
   <td> <p>Een verzameling gebruikers (mogelijk van dezelfde afdeling of bedrijfseenheid) die toegang hebben tot dezelfde objecten. Naast gebruikers, kunnen de groepen met portefeuilles, programma's, projecten worden geassocieerd,<span> projectsjablonen,</span> bedrijven, teams, programma's, lay-outmalplaatjes, en timesheet profielen.</p> <p>U kunt objecten ook machtigingen per groep geven. Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Overzicht van groepen</a>.</p> <p>In een lijst of rapport met objecten van een van de volgende typen kunt u de opdracht [!UICONTROL Group] veld om aan te geven welke objecten van dat type aan een bepaalde groep zijn gekoppeld: gebruiker, portfolio, programma, project, <span>projectsjabloon</span>, bedrijf, team, schema, lay-outsjabloon of tijdbladprofiel.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Group Administrator]</td> 
   <td> <p>Gebruikers die de objecten, toegang en gebruikers van bepaalde gebruikersgroepen beheren.</p> <p> In een [!UICONTROL Group] rapport, toont dit gebied de namen van de gebruikers aangewezen als [!UICONTROL Group Administrators] in de groep. Zie voor meer informatie over groepsbeheerders <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Groepbeheerders</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group with Administration Access]</td> 
   <td> <p> In een [!UICONTROL Layout Template], [!UICONTROL Timesheet Profile], of [!UICONTROL Schedule report], toont dit gebied de Groepen waarvan de Beheerders van de Groep toegang hebben om het malplaatje te wijzigen. U kunt dit rapport ook filteren op dit veld. </p> <p> Zie voor meer informatie <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Lay-outsjablonen maken en beheren</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Grouping]</td> 
   <td> <p>A reporting element used to categorize information in a list by a common criterium.</p> <p>Zie voor meer informatie de "[!UICONTROL Groupings]" in het artikel <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementen rapporteren: filters, weergaven en groepen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Handoff Date]</td> 
   <td> <p>De datum waarop een taak beschikbaar wordt voor het werk. De [!UICONTROL Handoff Date] is een berekening en kan niet handmatig worden ingesteld. <br>Voor meer informatie over de [!UICONTROL Handoff Date], zie het artikel <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[!UICONTROL Task Handoff Date] overzicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help Desk]</td> 
   <td>Een alternatieve naam om de [!UICONTROL Requests] gebied van [!DNL Workfront]. U kunt de [!UICONTROL Requests] gebied om klantensteunkaartjes, projectverzoeken, helpdeskkaartjes, enz. te verwerken.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Owner]</td> 
   <td>In een [!UICONTROL Hour] het [!UICONTROL Owner] is de gebruiker aan wie de uren worden toegeschreven. Dit is anders dan de gebruiker die de tijd registreert. Deze twee entiteiten kunnen soms twee verschillende gebruikers zijn. <br>Raadpleeg het artikel voor meer informatie over de logtijd voor een andere gebruiker <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Logtijd</a>.</td> 
  </tr>

<tr> 
   <td>Uur</td> 
   <td> <p>An attribute set by Workfront for the Actual Hours that users log for tasks, issues, or projects. </p>

Uur-items kunnen een van de volgende statussen in Workfront hebben:
<ul>
   <li><b>Verzonden</b>: de uren zijn het programma geopend op een project, een taak, of een kwestie. Ze maken deel uit van een factureringsrecord of worden nog niet toegevoegd aan een factureringsrecord.</li>
   <li><b>Goedgekeurd</b>: de uren zijn geregistreerd en zijn goedgekeurd door de eigenaar van het project. Ze maken deel uit van een factureringsrecord of worden nog niet toegevoegd aan een factureringsrecord.</li> 
   <li><b>Niet goedgekeurd</b>: de uren zijn geregistreerd en verworpen door de eigenaar van het project. Ze maken deel uit van een factureringsrecord of worden nog niet toegevoegd aan een factureringsrecord.</li>
   <li><b>Gefactureerd</b>: de uren zijn geregistreerd, toegevoegd aan een factureringsrecord en de status van de factureringsrecord is gemarkeerd als Met factuur. Zij hoefden niet te worden goedgekeurd door de eigenaar van het project.</li>
   <li><b>Gefactureerd en goedgekeurd</b>: de uren zijn geregistreerd, goedgekeurd door de eigenaar van het project en de status van de factureringsrecord is gemarkeerd als Met factuur.</li>
   </ul>


<p>Wanneer de uren deel van een facturerings verslag uitmaken, wijst de Status van het Uur erop of de uren zijn goedgekeurd of als het het FactureringsVerslag van hen tot behoren in rekening is gebracht. De Status van het uur van een ureningang is slechts zichtbaar in een uurlijst of een rapport. </p>

<p>Zie de sectie "Uren toevoegen aan factureringsrecords" in het artikel voor meer informatie over het toevoegen van uren aan factureringsrecords. <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >Factureringsrecords maken</a>.</p>

<p>Voor meer informatie over het goedkeuren van tijd over projecten, zie <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >Tijd vereisen om te worden goedgekeurd voor een project</a>.</p>

<p><b>TIP</b></p>

<p>De algemene uren die niet direct op het werkpunten worden geregistreerd tonen geen Status van het Uur. </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Hour Type]</td> 
   <td> <p>An attribute that can be set for Actual Hours that users log for tasks, issues, or projects. Dit is ook een attribuut voor de geregistreerde uren die niet direct met het werk verbonden zijn, zoals [!UICONTROL Vacation] en [!UICONTROL Time Off].</p> <p>Zie voor meer informatie <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Uurtypen beheren</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>De id is een alfanumerieke indicator die aan elk object in [!DNL Workfront]. Elk object in de [!DNL Workfront] database. U kunt de id van elk object weergeven in een rapport of een lijst voor elk object. </p> <p><b>TIP</b></p>   <p>U kunt de id ook weergeven in de URL van de objectpagina. De id van een project kan er bijvoorbeeld ongeveer zo uitzien als het getal dat in de volgende URL wordt vermeld, wanneer u de [!UICONTROL Project Details] pagina:</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Individual Goals]</td> 
   <td>Individuele doelstellingen die bijdragen tot de metriek van de teamdoelstellingen, maar niet met betrekking tot persoonlijke of carrièreontwikkeling.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Inherited Access]</td> 
   <td>Functie voor delen waarmee toegang kan worden doorgegeven van object naar een ander object. Bijvoorbeeld, erven de de erfenistoegang van de projectgebruiker in programma en portefeuillerecords wordt bepaald.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>In de [!DNL Workfront Scenario Planner], kunt u een plan opsplitsen in verschillende initiatieven om het beheer van het plan te vergemakkelijken. <span>U kunt een [!UICONTROL Initiative] rapport en u kunt tot [!UICONTROL Initiative] informatie in een [!UICONTROL Project] verslag.</span></p> <p>De [!DNL Scenario Planner] vereist een aanvullende licentie. Voor informatie over de [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">De [!DNL Scenario Planner] overzicht</a>. </p> <p>De [!DNL Initiative] het rapport is niet zichtbaar in uw [!DNL Workfront] -instantie tenzij uw bedrijf een [!DNL Workfront Scenario Planner] licentie. U hebt geen toegang tot [!UICONTROL Initiatives] via de API.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role]</span> </td> 
   <td> <p><span>De [!UICONTROL Initiative Job Role] het rapporttype toont informatie over de baanrollen verbonden aan een planinitiatief in [!DNL Workfront Scenario Planner].</span> </p> <p>De [!DNL Scenario Planner] vereist een aanvullende licentie. Voor informatie over de [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md">De [!DNL Scenario Planner] overzicht</a>. </p> <p><span>Dit rapporttype is niet zichtbaar in uw [!DNL Workfront] -instantie tenzij uw bedrijf een [!DNL Workfront Scenario Planner] licentie.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role Hours]</span> </td> 
   <td> <p><span> In een [!UICONTROL Initiative Job Role] rapport, dit toont het aantal uren verbonden aan een baanrol in een initiatief.</span> </p> <p>De [!DNL Scenario Planner] vereist een aanvullende licentie. Voor informatie over de [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md">De [!DNL Scenario Planner] overzicht</a>. </p> <p>Dit veld en de [!UICONTROL Initiative Job Role] rapporttype is niet zichtbaar in uw [!DNL Workfront] -instantie tenzij uw bedrijf een [!DNL Workfront Scenario Planner] licentie.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role Count]</td> 
   <td> <p>In een [!UICONTROL Initiative Job Role] rapport, toont dit het aantal specifieke baanrollen verbonden aan een initiatief.</p> <p>De [!DNL Scenario Planner] vereist een aanvullende licentie. Voor informatie over de [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md">De [!DNL Scenario Planner] overzicht</a>. </p> <p>Dit veld en de [!UICONTROL Initiative Job Role] rapporttype is niet zichtbaar in uw [!DNL Workfront] -instantie tenzij uw bedrijf een [!DNL Workfront Scenario Planner] licentie.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Last Published Date]</td> 
   <td> <p>Een veld in een [!UICONTROL Initiative], [!UICONTROL Initiative Job Role], en [!UICONTROL Project] een rapport met de datum waarop een planinitiatief voor het laatst naar een project is gepubliceerd. U kunt initiatieven publiceren om projecten tot stand te brengen of projecten bij te werken met betrekking tot de initiatieven.</p> <p>De [!DNL Scenario Planner] vereist een aanvullende licentie. Voor informatie over de [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md">De [!DNL Scenario Planner] overzicht</a>. </p> <p><span>Zie voor informatie over publicatieinitiatieven</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">Publiceer scenario's om projecten in te stellen en bij te werken [!DNL Workfront Scenario Planner]</a>. Dit veld is niet zichtbaar in uw [!DNL Workfront] -instantie tenzij uw bedrijf een [!DNL Workfront Scenario Planner] licentie.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Inline Search]</td> 
   <td>Tijdens het invullen van een formulier is een zoekopdracht uitgevoerd om mogelijke gegevens voor een bepaald veld te zoeken.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interface Setup]</td> 
   <td>Het gebied van de toepassing dat het bepalen van de Weergaven van de Douane, Filters, Groepen, Controles van de Lijst, enz. toestaat.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Is Company Goal]</p></td> 
   <td> <p>In [!DNL goal reports], wordt een "[!UICONTROL True]/ [!UICONTROL False]" waarde voor elk strategisch doel om aan te geven of uw organisatie aan het doel is toegewezen als eigenaar. </p> 
   <p>Dit veld is alleen zichtbaar als uw organisatie een aankoop heeft gedaan [!DNL Workfront Goals]. Voor informatie over het beheer van strategische doelen met [!DNL Workfront Goals], zie <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] overzicht </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue]</td> 
   <td> <p>Een niet-gepland het werkpunt dat gewoonlijk wijst op een probleem verhinderend de voltooiing van een taak of een project. Het wordt getrigeerd en geëvalueerd voor verdere werkzaamheden</p> <p>An [!UICONTROL Issue] kan ook een [!UICONTROL Help Desk] verzoek. [!UICONTROL Change Orders], [!UICONTROL Requests], en [!UICONTROL Bugs] ook [!UICONTROL Issues].</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Management]</td> 
   <td> <p>Het proces en de regels die de definitie van uitgiftetypen en het verpletteren, triage, of verkeersproces verbonden aan elk type bepalen.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Owner]</td> 
   <td>Het team dat of de gebruikers die verantwoordelijk zijn voor het triggeren en voltooien van een probleem.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iteration]</td> 
   <td>Een periode waarin een team een vooraf bepaalde reeks te leveren items produceert.</td> 
  </tr> 
 </tbody> 
</table>

## J - L

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objectnaam</th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Job Role]</td> 
   <td> <p>Wordt gebruikt om de dagelijkse functies en verantwoordelijkheden van een gebruiker te identificeren. De rollen van de baan kunnen aan de werkpunten worden toegewezen om de vereiste vaardigheid te identificeren nodig om een het werkproces te voltooien zonder het aan een specifieke gebruiker toe te wijzen. </p> <p>Een gebruiker kan meerdere rollen hebben. Voorbeelden zijn Grafische ontwerper of Consultant.</p> <p>Zie voor meer informatie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Taakrollen maken en beheren</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Journal Entry]</p> </td> 
   <td> <p>Een te rapporteren object dat u informatie geeft over systeemupdates voor bijgehouden velden die in het dialoogvenster [!UICONTROL Updates] gebied met projecten, taken, problemen en andere objecten.</p> <p>Zie voor meer informatie <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Verslag over de [!UICONTROL Updates] gebied</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kanban Flag]</td> 
   <td> <p>In een [!UICONTROL Task] Rapport of [!UICONTROL Issue] Rapport, de [!UICONTROL Kanban Flag] in het veld wordt de vlagstatus weergegeven die is ingesteld in het artikel in het [!UICONTROL Kanban board]. Mogelijke waarden zijn [!UICONTROL On Track], [!UICONTROL Ready to Pull], en [!UICONTROL Is Blocked].</p> <p>Voor meer informatie over het instellen van de vlagstatus in artikelen op het tabblad [!UICONTROL Kanban story board], zie het artikel <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">Markeringen gebruiken voor artikelen op de [!UICONTROL Kanban board]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI's</td> 
   <td>Een meetbare waarde die aantoont hoe effectief een bedrijf belangrijke bedrijfsdoelstellingen bereikt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>Hoeveelheid tijd die na de taak van de voorganger moet overgaan [!UICONTROL Planned Completion Date] is overgegaan tot de afhankelijke taak kan beginnen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag Types]</td> 
   <td> <p>De methode voor de berekening van [!UICONTROL Lag]. Het kan zijn:</p> 
    <ul> 
     <li>[!UICONTROL Days] (werkdagen)</li> 
     <li>[!UICONTROL Calendar Days] (feestdagen negeren)</li> 
     <li>[!UICONTROL Percent]</li> 
     <li>[!UICONTROL Day of Week]</li> 
    </ul> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">Overzicht van typen labels</a>.</p> </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Large Thumbnail]</td> 
   <td> <p> In een [!UICONTROL Document] weergegeven in een miniatuur. </p> <p>Selecteren <strong>[!UICONTROL Large Thumbnail]</strong> om een miniatuur van 400 pixels breed in het rapport weer te geven.</p> <p>De grootte van de miniatuur wordt aangepast wanneer u de breedte van de kolom in een lijst of rapport wijzigt.</p> <p>Zie ook "[!UICONTROL Thumbnail]" in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last 10 Viewers]</td> 
   <td> <p>In een rapportlijst, toont dit gebied de namen van maximaal 10 gebruikers die het rapport onlangs hebben bekeken.<br>Raadpleeg het artikel voor meer informatie over het gebruik in rapportlijsten <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Rapportgebruik weergeven</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Condition Note]</td> 
   <td> <p>In dit veld wordt de laatste update weergegeven die de eigenaar van het object voor een object heeft ingevoerd. Dit is de meest recente activiteit of interactie van de eigenaar van een object.</p> <p>De [!DNL Last Condition Note] is leeg als de notitietekst van de laatste notitie van een object is verwijderd. Wanneer een nieuwe notitie op het object wordt ingevoerd, wordt deze de laatste notitie en wordt deze opnieuw weergegeven in de kolom. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Finance Update Date]</td> 
   <td>In een [!UICONTROL project] in dit veld worden de datum en het tijdstip van de laatste berekening en bijwerking van de projectfinanciering vermeld . Voor informatie over projectfinanciën, zie <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">Overzicht van de projectfinanciën</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Note]</td> 
   <td> <p>In dit veld wordt de laatste update weergegeven die een gebruiker voor een object heeft ingevoerd. Dit is de meest recente activiteit of interactie op een voorwerp.</p> <p>De [!UICONTROL Last Note] is leeg als de tekst van de laatste notitie van een object is verwijderd. Wanneer een nieuwe notitie op het object wordt ingevoerd, wordt deze de laatste notitie en wordt deze opnieuw weergegeven in de kolom.</p>
   <p>Wanneer dit veld wordt toegevoegd aan een [!UICONTROL Task] rapporteren, eventuele updates die over onderliggende objecten blijven bestaan, zoals problemen, subtaken, documenten, enz. — van de taak wordt niet weergegeven in deze kolom.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Viewed By]</td> 
   <td> <p>In een rapportlijst, toont dit gebied informatie over de gebruiker die het rapport het laatst bekeken.<br>Raadpleeg het artikel voor meer informatie over het gebruik in rapportlijsten <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Rapportgebruik weergeven</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Viewed Date]</td> 
   <td> <p>In een rapportlijst, toont dit gebied de datum waarop het rapport het laatst werd getoond.<br>Raadpleeg het artikel voor meer informatie over het gebruik in rapportlijsten <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Rapportgebruik weergeven</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Layout Template]</td> 
   <td>Gedefinieerd door de systeembeheerder of groepsbeheerder om de tabbladen en rapporten te identificeren die worden weergegeven in de werkruimte van een bepaalde gebruiker.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Layout Type]</td> 
   <td>In combinatie met [!UICONTROL Custom Views]de [!UICONTROL Layout Type] geeft het type van [!UICONTROL Custom View]. Momenteel is alleen de lijst beschikbaar. In de toekomst [!UICONTROL Detail] (de [!UICONTROL Detail] (weergave van een object) kan beschikbaar komen.</td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Cost</i>. </p> </td> 
  </tr>
  --> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Hours</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Hours</i>. </p> <p>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        This field shows the number of hours budgeted for the project in the Legacy Resource Estimates area of the Business Case or in the Capacity Planner. 
       <br>If there&nbsp;are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.&nbsp; 
     </p> </td> </tr> -->
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.&nbsp;</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;&nbsp;</p>
    --> </td> 
  </tr> 
  <tr> 
   <!-- <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection&nbsp;of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Library Task]</td> 
   <td>Een malplaatje voor één enkele taak die wordt gebruikt om verenigbare noemende van [!UICONTROL Tasks] en [!UICONTROL Template Tasks] in de toepassing.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Type]</td> 
   <td>Het type vergunning dat aan een [!UICONTROL Access Level]. Het is ofwel [!UICONTROL Full User], [!UICONTROL Limited User], of [!UICONTROL Requester].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Plan]</td> 
   <td> <p>In een [!UICONTROL Group] bekijken of rapporteren, toont dit gebied het maximumaantal [!UICONTROL Plan] licenties die kunnen worden toegewezen aan gebruikers die de desbetreffende groep als hun [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Work]</td> 
   <td> <p>In een [!UICONTROL Group] bekijken of rapporteren, toont dit gebied het maximumaantal [!UICONTROL Work] licenties die kunnen worden toegewezen aan gebruikers die de desbetreffende groep als hun [!UICONTROL Home Group].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limited User]</td> 
   <td>Een licentietype dat het maken van een [!DNL Access Level] die alleen-weergeven rechten bevat, met de mogelijkheid om problemen te verzenden, notities in te voeren en documenten te uploaden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL List Controls]</td> 
   <td> <p>Een deel van [!UICONTROL Interface Setup] waarmee u aangepaste filters, weergaven en groepen kunt koppelen aan individuele gebruikers of aan alle gebruikers.</p> </td> 
  </tr> 
 </tbody> 
</table>

## M - O

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objectnaam</th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Manual Only]</td> 
   <td> <p>Een van een [!UICONTROL Project]s [!UICONTROL Update Types]. Deze instelling staat [!UICONTROL Project Projected] en [!UICONTROL Planned] tijdlijnen die alleen moeten worden bijgewerkt wanneer "[!UICONTROL Recalculated Timelines]" is aangeklikt. Projecten die op deze manier worden ingesteld, worden tijdens het nachtelijke herberekeningsproces genegeerd en wanneer het project of de taken in het project worden bijgewerkt.</p> <p>Zie voor meer informatie <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecteer het project [!UICONTROL Update Type] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>Dit verwijst naar de momenteel aangemelde gebruiker. </p> <p>Wij adviseren gebruikend dit gebied in een filter om rapporten generischer te maken wanneer het delen van hen met andere gebruikers. Deze manier, kunt u slechts één rapport bouwen dat verschillende informatie afhankelijk van zal tonen wie het programma opent om het te bekijken, aangezien de informatie altijd voor de het programma geopende gebruiker wordt aangepast. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Max Users]</td> 
   <td> <p>Dit is een verouderd veld. Alle informatie die in dit veld wordt weergegeven, is gerelateerd aan een functie die [!DNL Workfront] is verwijderd en het veld kan niet worden bijgewerkt. </p> <p>In eerdere versies van [!DNL Workfront]kunt u dit veld bijwerken wanneer u een taakrol maakt of bewerkt. Het toonde het totale aantal gebruikers die met een rol op elk project kunnen worden geassocieerd. De waarde nul is toegestaan voor een onbeperkt aantal gebruikers dat aan een project kan worden toegewezen. </p>Het veld is in sommige rapporten en lijsten nog steeds zichtbaar, maar de weergegeven informatie kan niet worden bijgewerkt. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone]</td> 
   <td> <p>Een teller die u met een taak kunt associëren om erop te wijzen dat een zeer belangrijk punt in het project is bereikt wanneer de taak wordt voltooid. In het algemeen kunt u mijlpalen gebruiken om een belangrijke gebeurtenis weer te geven, zoals de voltooiing van een fase van het project of een reeks kritieke activiteiten. [!UICONTROL Milestones] zijn doorgaans gekoppeld aan bovenliggende taken. U moet de mijlpalen creëren alvorens u hen aan taken kunt vastmaken. Voor informatie over mijlpalen raadpleegt u <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">Een milestone-pad maken</a> en <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">Mijlpalen koppelen aan taken</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Milestone Path]</td> 
   <td>Een verzameling van [!UICONTROL milestones]. [!UICONTROL Milestone Paths] worden gebruikt voor projecten om projecten met bepaalde soorten [!UICONTROL Milestones] van projecten met een andere reeks [!UICONTROL Milestones].</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone Task]</td> 
   <td>Een taak die is gemarkeerd om een te meten te melden gebeurtenis aan te geven.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Module]</td> 
   <td>Eén stap binnen een scenario in [!DNL Workfront Fusion] die een bepaalde functie uitvoert op basis van de bijbehorende app.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Primary Role]</td> 
   <td> <p>Wanneer in filters naar dit wordt verwezen, worden gebruikers met dezelfde instelling weergegeven [!UICONTROL Primary Role] als het programma geopende gebruiker, of het werkpunten die aan [!UICONTROL Primary Role] van de aangemelde gebruiker.</p> <p>Wij adviseren gebruikend dit gebied in een filter om rapporten generischer te maken wanneer het delen van hen met andere gebruikers. Deze manier, kunt u slechts één rapport bouwen dat verschillende informatie afhankelijk van zal tonen wie het programma opent om het te bekijken, aangezien de informatie altijd voor de het programma geopende gebruiker wordt aangepast. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Home Team]</td> 
   <td> <p>Wanneer hiernaar wordt verwezen in filters, wordt in dit veld een van de gebruikers weergegeven die bij het [!UICONTROL Home Team] van de aangemelde gebruiker of de aan de [!UICONTROL Home Team] van de aangemelde gebruiker. </p> <p>Wij adviseren gebruikend dit gebied in een filter om rapporten generischer te maken wanneer het delen van hen met andere gebruikers. Deze manier, kunt u slechts één rapport bouwen dat verschillende informatie afhankelijk van zal tonen wie het programma opent om het te bekijken, aangezien de informatie altijd voor de het programma geopende gebruiker wordt aangepast. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Naming convention]</td> 
   <td>Een voor de hele organisatie geldende set regels die gegevens gebruiken om namen van projecten, taken en te leveren items te maken.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Native Integration]</td> 
   <td>Een integratie waarvoor geen handmatige codering of API-configuratie vereist is. Wordt ook wel 'out-of-the-box'-integratie genoemd.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Navigation Menu]</td> 
   <td>Het middelste bovenste deelvenster van de toepassing dat koppelingen bevat naar de hoofdgebieden van [!UICONTROL Workfront].</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL New Number Value]</td> 
   <td>In een [!UICONTROL Journal Entry] rapport, toont dit de bijgewerkte waarde van een gebied dat vervangt [!UICONTROL Old Number Value].
   Zie voor meer informatie "[!UICONTROL Old Number Value]" in dit artikel.</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Non-Billable Expense]</td> 
   <td> <p>Een last die niet als factureerbaar aan de klant wordt gemerkt. Dit kan ofwel een geplande uitgave zijn, ofwel een werkelijke uitgave.</p> <p>De geplande niet-factureerbare de Kosten van de Kosten en de Ware niet-factureerbare gebieden van de Kosten van de Kosten zijn beschikbaar voor u om aan meningen en rapporten toe te voegen. Ze worden niet weergegeven op de pagina's met project- of taakdetails.</p>
   <p>U kunt deze gebieden in de volgende types van rapporten vinden:</p>
   <ul>
   <li>Basislijn</li>
   <li>Sjabloon</li>
   <li>Project (financiële gegevens)</li>
   </ul>
   <p>Voor meer informatie over het merken van een uitgave als factureerbaar, zie <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md">Projectkosten beheren</a>.</p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Non Work Day]</td> 
   <td>Een dag die niet wordt toegewezen aan het uitvoeren van een opdracht. Dit is meestal een feestdag, vakantie of weekend. De term wordt weergegeven in de API-verkenner. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note]</td> 
   <td>Een opmerking of update die is aangebracht op een [!DNL Workfront] object.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note Text]</td> 
   <td> <p>Hiermee wordt de tekst weergegeven van een update die een gebruiker heeft ingevoerd voor een willekeurig object. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Number of Linked Goals]</td> 
   <td> <p>In een [!UICONTROL Project] dit is het aantal strategische doelstellingen dat aan het project is gekoppeld . Voor informatie over het associëren van projecten met strategische doelstellingen, zie <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Projecten toevoegen aan doelen in  [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>Voor informatie over strategische doelstellingen, zie ook "[!UICONTROL Goal]" in dit artikel.</p> 
   <p>Dit veld is alleen zichtbaar als uw organisatie een aankoop heeft gedaan [!DNL Workfront Goals]. Voor informatie over het beheer van strategische doelen met [!DNL Workfront Goals], zie <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">Projecten toevoegen aan doelen in [!UICONTROL Adobe Workfront Goals]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object]</td> 
   <td> <p>De informatie die u in [!DNL Adobe Workfront] wordt voorgesteld door voorwerpen die in [!DNL Workfront] database. De objecten zijn de drijvende kracht achter de informatie in Workfront. Voorbeelden van objecten zijn:</p> 
    <ul> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Groups]</li> 
     <li>[!UICONTROL Teams]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Custom forms]</li>
     <li>[!UICONTROL Custom fields]</li>  
     <li>[!UICONTROL Hours]</li> 
     <li>[!UICONTROL Billing Rates]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Template tasks]</li>

<p><b>OPMERKING</b></p>
  <p>Dit is geen uitgebreide lijst. </p>

</ul> <p>Zie voor meer informatie <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Objecten begrijpen in [!UICONTROL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object Types]</td> 
   <td>Als u een rapport of lijst maakt met al uw aangepaste formulieren, kunt u dit veld gebruiken als weergave of filter om te zien welke objecttypen aan elk formulier zijn gekoppeld. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Old Number Value]</td> 
   <td>In een [!UICONTROL Journal Entry] rapport, toont dit de originele waarde van een gebied alvorens het werd bijgewerkt. Wanneer de waarde van een veld is bijgewerkt, wordt deze weergegeven als de [!UICONTROL New Number Value] in een [!UICONTROL Journal Entry] verslag. Zie ook "[!UICONTROL New Number Value]".</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL On Change Only]</td> 
   <td> <p>Een van de [!UICONTROL Project Update] Typen. Als deze optie is geselecteerd, wordt [!UICONTROL Project Projected] en [!UICONTROL Planned] tijdlijnen worden alleen bijgewerkt wanneer het project of een taak in het project wordt bijgewerkt of gewijzigd. Het werkt het project niet elke nacht bij.</p> <p>Zie voor meer informatie <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecteer het Type van projectupdate </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Op Task]</td> 
   <td> <p>De naam voor [!UICONTROL Issue] in de [!DNL Workfront] database, gebruikt in tekstmodusrapporten of berekende aangepaste gegevens.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Open]</td> 
   <td>Een kwestie of een taak die niet volledig is, maar aan wordt gewerkt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Org Chart]</td> 
   <td>Kort voor organisatieschema. Dit is een grafiek die de hiërarchie van een organisatie toont. Het staat ook op het Tab-tabblad [!UICONTROL User] detailscherm dat het plaatsen van toont en toestaat [!UICONTROL User]s [!UICONTROL Company] en [!UICONTROL Reporting] relaties.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organizational Setup]</td> 
   <td>Deze definitie [!UICONTROL Companies], [!UICONTROL Groups], en [!UICONTROL Security Profiles] voor uw organisatie.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Other Groups]</td> 
   <td> <p>In een rapport of een mening die van gebruikers een lijst maakt, toont dit gebied alle groepen waar elke gebruiker een lid is. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency]</span> </td> 
   <td> 
    <div> 
     <p>In een [!UICONTROL Job Role] rapport : dit is de valuta die gekoppeld is aan een functie . Het is een opheffing van de [!UICONTROL Base Currency] , zoals vastgesteld in [!UICONTROL Setup] door de [!DNL Workfront] beheerder. </p> 
     <p>Zie voor meer informatie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Taakrollen maken en beheren</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Billing/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>In een [!UICONTROL Job Role] rapport, dit is het facturerings per uurtarief van de baanrol gebruikend geselecteerde [!UICONTROL Override Currency] van de functie.</p> 
     <p> Zie voor meer informatie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Taakrollen maken en beheren</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Cost/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>In een [!UICONTROL Job Role] rapport, dit is het tarief van de kosten per uur van de baanrol gebruikend geselecteerde [!UICONTROL Override Currency] van de functie. </p> 
     <p>Zie voor meer informatie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Taakrollen maken en beheren</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Owner]</td> 
   <td>De gebruiker die verantwoordelijk is voor de voltooiing van het opgegeven object.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Owner Type]</span> </td> 
   <td> 
    <div> 
     <p>In een [!UICONTROL Goal] rapport, toont dit het type van eigenaar dat aan een strategisch doel wordt toegewezen. Het volgende is de types van doeleigenaar:</p> 
     <ul> 
      <li> <p>[!UICONTROL User]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL Group]</p> </li> 
     </ul> 
     <p>Er wordt geen waarde in dit veld weergegeven wanneer de eigenaar van het doel uw organisatie is. </p> 
     <p>Hiervoor is een aanvullende licentie vereist. Voor informatie over [!DNL Workfront Goals], zie <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] overzicht</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## P - R

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objectnaam</th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Parameter]</td> 
   <td> <p>A [!UICONTROL parameter] is een aangepast veld. U kunt een rapport maken voor alle parameters of aangepaste velden in uw systeem. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent]</td> 
   <td>In een rapport bevat dit veld informatie over het bovenliggende element van het object. In een [!UICONTROL issue] rapport, zou het informatie over de taak of het project kunnen tonen dat de kwestie onder het programma wordt geopend; in een taakrapport, zou het informatie over de directe oudertaak of over het project kunnen tonen. Meer informatie over de objecten waarin bovenliggende elementen kunnen staan [!DNL Workfront], zie de sectie "Interdependentie en hiërarchie van objecten" in het artikel <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Objecten begrijpen in [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent Lag]</td> 
   <td>De hoeveelheid tijd die tussen moet overgaan [!UICONTROL Parent Task] en de [!UICONTROL Subtask] Start.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent Task]</td> 
   <td>Ook bekend als a [!UICONTROL Summary Task]. Dit is een taak met subtaken (ook wel [!UICONTROL Children Tasks]). De [!UICONTROL Duration], [!UICONTROL Work Required], en [!UICONTROL Percent Complete] van de Ouderlijke Taak wordt berekend van Subtaken.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Part-Time Resources]</td> 
   <td>Een gebruiker met licentie die minder capaciteit heeft dan het standaardschema dat in het systeem is gedefinieerd.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percent Complete]</td> 
   <td> <p>Een project, een taak, of een probleemgebied dat toont welk percentage van het werk verbonden aan de taak, het project, of de kwestie wordt voltooid.</p> <p>U kunt dit veld handmatig bijwerken voor problemen en werktaken. </p> <p>Voor projecten en oudertaken, is dit gebied een roll-up van alle het werk taken en u kunt niet het manueel bijwerken. </p> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">Project [!UICONTROL Percent Complete] overzicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permission]</td> 
   <td> <p>Rechten die aan een gebruiker op een voorwerp worden verleend, typisch gegeven zodat kunnen zij het werk aan het punt voltooien of het punt bekijken. U kunt machtigingen verlenen aan:</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Custom Forms]</li> 
     <li>[!UICONTROL Views]</li> 
     <li>[!UICONTROL Filters]</li> 
     <li>[!UICONTROL Groupings]</li> 
    </ul> <p>Zie voor meer informatie <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overzicht van het delen van machtigingen voor objecten</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]</td> 
   <td> <p>Dit is een volledig licentietype in het dialoogvenster [!DNL Workfront] systeem. Gebruikers moeten dit doen om toegang te krijgen tot alle functies in [!DNL Workfront].</p> <p>Zie voor meer informatie <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] overzicht van licenties</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan] (in de [!DNL Scenario Planner])</td> 
   <td> <p>Een plan is het belangrijkste voorwerp wanneer het werken met [!DNL Workfront] Scenario Planner. U kunt de strategie voor de nabije en lange toekomst van uw bedrijf schetsen en elk resultaat op hoog niveau identificeren en het als plan toevoegen aan [!DNL Workfront] Scenario Planner. </p> <p>U kunt niet weergeven [!DNL Scenario Planner] de plannen in een rapport en u kunt niet tot hen door [!DNL Workfront] API. </p> <p>De [!DNL Scenario Planner] vereist een aanvullende licentie. Voor informatie over de [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md">De [!DNL Scenario Planner] overzicht</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned]</td> 
   <td> <p>Het tijdkader waarbinnen iets gepland is voor te komen. Wanneer u projecten, taken of kwesties binnen creeert [!DNL Workfront], stelt u de geplande begin- en einddatums vast, evenals het geplande tijdsbestek waarin deze plaatsvinden. Deze waarden geven uw oorspronkelijke intentie weer of schatten hoe lang het duurt voordat een object is voltooid. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Benefit]</td> 
   <td>Dit is een handmatige vermelding voor de projectmanager om te schatten of de voltooiing van een project de organisatie enig geldelijk voordeel zou opleveren. Het opgeven van deze waarde kan onderdeel zijn van het samenstellen van een [!UICONTROL Business Case] voor het project. U moet [!UICONTROL Manage] bevoegdheden aan het project om deze waarde bij te werken.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Planned Budgeted Hours]</td> 
   <td> <p>In een [!UICONTROL Budgeted Hour] rapport, dit toont het aantal uren die voor projecten of [!UICONTROL Job Roles] in de [!UICONTROL Resource Planner]. </p> <p>Voor informatie over budgettaire projecten of rollen in de [!UICONTROL Resource Planner], zie het artikel <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Begrotingsmiddelen in de [!UICONTROL Resource Planner] met de [!UICONTROL Project] en [!UICONTROL Role] views</a>. Voor informatie over de [!UICONTROL Budgeted Hours] rapport, zie het artikel <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Verslag: Budgeted Hour</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Completion Date]</td> 
   <td> <p>U kunt de [!UICONTROL Planned Completion Date] naar de gewenste datum. Als u de instelling [!UICONTROL Planned Completion Date], [!DNL Workfront] wordt automatisch ingesteld. Als deze optie automatisch wordt ingesteld, [!UICONTROL Planned Completion Date] is: [!UICONTROL Planned Start Date] + [!UICONTROL Duration]</p> <p>Raadpleeg de volgende artikelen voor meer informatie:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Overzicht van de taak [!UICONTROL Planned Completion Date]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">Het project instellen [!UICONTROL Planned Completion Date]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Cost]</td> 
   <td> <p>Een totaal van [!UICONTROL Planned Labor Cost] en de [!UICONTROL Planned Expense Cost] van het project. Hieronder vallen niet de [!UICONTROL Planned Risk Cost] over het project.  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration]</td> 
   <td> <p>Een taak [!UICONTROL Planned Duration] is meestal hetzelfde als de taak [!UICONTROL Duration]. Dit is het verschil in dagen tussen de [!UICONTROL Planned Start] en de [!UICONTROL Planned Completion Dates] van de taak. </p> <p>Als de taak een [!UICONTROL Duration] Type [!UICONTROL Effort Driven]de [!UICONTROL Planned Duration] kan verschillen van [!UICONTROL Duration] van de taak, gebaseerd op hoeveel middelen u aan de taak toewijst. </p> <p>Bijvoorbeeld als een taak met een [!UICONTROL Duration] Type [!UICONTROL Effort Driven] heeft een [!UICONTROL Duration] van 3 dagen en u wijst één middel met een full-time programma aan de taak toe, [!UICONTROL Planned Duration] is ook drie dagen. Als u drie middelen met een full-time programma aan de zelfde taak toewijst, [!UICONTROL Duration] blijft 3 dagen, maar de [!UICONTROL Planned Duration] wordt 1 dag. De [!UICONTROL Planned Duration] wijzigt ook de [!UICONTROL Planned Start] en [!UICONTROL Planned Completion] datum van de taak , om de nieuwe [!UICONTROL Planned Duration]. Hierdoor wordt ook de tijdlijn van het project beïnvloed. </p> <p>Voor meer informatie over het verschil tussen [!UICONTROL Duration] en [!UICONTROL Planned Duration] zie het artikel voor taken <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">Verschil tussen [!UICONTROL Planned Duration] en [!UICONTROL Duration] voor taken</a>.</p> <p>Projecten en problemen hebben geen [!UICONTROL Planned Duration]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration Minutes]</td> 
   <td> <p>De [!UICONTROL Planned Duration Minutes] van een project of een kwestie [!UICONTROL Duration] van het project of de uitgifte in minuten. </p> <p>Taken hebben geen [!UICONTROL Planned Duration Minutes] veld. </p> <p>[!UICONTROL Template Tasks] een [!UICONTROL Planned Duration Minutes] veld dat de [!UICONTROL Planned Duration] van de taak in minuten. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Expense Cost]</td> 
   <td> <p>De som van de [!UICONTROL Planned Amounts] voor alle uitgaven die voor een project of een taak worden geregistreerd.</p> <p><b>VOORBEELD</b></p>
   <p>Als u een uitgave voor Taak 1 creeert en $600.00 in ingaat [!UICONTROL Planned Amount] in het veld [!UICONTROL Planned Expense Cost] hiervoor is $ 600.00 . </p> 
   <p>Voor een project: [!DNL Workfront] gebruikt de volgende formule om te berekenen [!UICONTROL Planned Expense Cost]:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Hours]</td> 
   <td> <p>Dit veld wordt weergegeven in het dialoogvenster [!UICONTROL projects], [!UICONTROL tasks], en geeft gebieden, rapporten voor projecten, taken, of kwesties, en middelen beheersinstrumenten zoals [!UICONTROL Resource Planner], [!UICONTROL Workload Balancer] en de [!UICONTROL Utilization] verslag. </p> <p>Het toont het aantal uren dat de Eigenaar van het Project schat dat elke taak of kwestie zou moeten voltooien. Voor projecten is het doorgaans een opsomming van de [!UICONTROL Planned Hours] van de taken in het project. </p> <p>De [!UICONTROL Planned Hours] in het veld kan andere informatie worden weergegeven, afhankelijk van waar u deze weergeeft. Voor informatie over geplande uren raadpleegt u <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Overzicht van geplande uren</a>.</p> <p>Geplande uren worden in minuten opgeslagen in de [!DNL Workfront] database. Zorg er bij het schrijven van berekeningen met dit veld voor dat de uren als minuten worden weergegeven.<br></p> <p>Door gebrek, worden de Geplande Uren gelijkelijk verdeeld over alle dagen binnen de duur van een het werkpunt en ook voor alle middelen die aan de taak worden toegewezen. Gebruikers kunnen het dagelijkse aantal geplande uren voor een werkartikel of de individuele geplande uren voor elke toegewezen persoon bijwerken.</p> <p>Het bijwerken van dit gebied verschilt voor projecten, taken, en kwesties: </p> 
    <ul> 
     <li> <p>Voor uitgaven kunt u dit veld handmatig bijwerken. De geplande uren van de uitgave worden niet toegevoegd aan het Geplande Uren van het Project. </p> <p><b>TIP</b></p> <p>In een uitgiftenrapport wordt een van de [!UICONTROL Planned Hours] velden worden vervangen door [!UICONTROL Work] veld. In het veld wordt het aantal geplande uren weergegeven. Zie voor meer informatie het onderwerp "Werk" of "[!UICONTROL Work]"- velden in deze tabel. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>Voor taken kunt u dit veld handmatig bijwerken wanneer de [!UICONTROL Duration Type] van de taak [!UICONTROL Calculated Assignment] of [!UICONTROL Simple]. Dit veld wordt berekend door [!DNL Workfront] wanneer de [!UICONTROL Duration Type] van de taak [!UICONTROL Calculated Work] of [!UICONTROL Effort Driven].<br>Voor informatie over [!UICONTROL Task Duration], zie het artikel <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overzicht van taak [!UICONTROL Duration] en [!UICONTROL Duration Type]</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Voor projecten [!DNL Workfront] Berekent de Geplande Uren door alle Geplande Uren van alle taken op het project toe te voegen. </p> </li> 
    </ul> <p><b>TIP</b></p> <p>U kunt [!UICONTROL Planned Hours] in [!UICONTROL project], [!UICONTROL task], of [!UICONTROL issues] rapporten ook door tekstwijze te gebruiken en van verwijzingen te voorzien extra gebieden. Zie voor meer informatie de "<code>work</code>", "[!UICONTROL Work]", en "<code>workRequiredExpression</code>"- velden in deze tabel. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Labor Cost]</td> 
   <td> 
    <p>Voor een taak, het uurtarief van de gebruiker of de rol vermenigvuldigd met het aantal uren die aan de gebruiker of de rol worden toegewezen.</p> <p>Voor een project is het een totaal van [!UICONTROL Planned Labor Costs] van alle taken.</p> <p>Of het tarief van de gebruiker of de rol wordt gebruikt hangt van het Type van Kosten af dat voor de bepaalde taak wordt geselecteerd. </p> <p>Zie voor meer informatie <a href="../../../manage-work/projects/project-finances/track-costs.md">Trackkosten</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Revenue]</td> 
   <td> <p>Taken en projecten kunnen een waarde weergeven voor [!UICONTROL Planned Revenue] in [!DNL Workfront]. [!UICONTROL Planned Revenue] staat voor het bedrag van de aan de [!UICONTROL Planned Hours] van de projecttaken. Voor projecten kan het ook de [!UICONTROL Fixed Revenue] van het project. </p> <p>Voor taken, is dit de opbrengst verbonden aan [!UICONTROL Planned Hours] van taken. De geplande uren van alle taken lopen tot de geplande uren van het project om bij te dragen tot de berekening van het project [!UICONTROL Planned Hours]. </p> 
   <p>[!DNL Workfront] berekeningen [!UICONTROL Planned Revenue] voor taken en projecten met behulp van de volgende formules:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>Het project [!UICONTROL Planned Revenue] die worden weergegeven in het dialoogvenster [!UICONTROL Project Details] het gebied en de projectverslagen verschillen van de geplande inkomsten die in het [!UICONTROL Utilization] verslag. </p> <p>De [!UICONTROL Planned Revenue] in de [!UICONTROL Project Details] het gebied weerspiegelt de taakontvangsten evenals de Vaste Ontvangsten van het project. De [!UICONTROL Planned Revenue] in de [!UICONTROL Utilization Report] displays [!UICONTROL Planned Revenue] alleen gekoppeld aan de taken in het project. </p> 
     <p><b>VOORBEELD</b></p>  
      <p>Als het project 1 taak met 10 uren heeft, die aan een Consultant met $20 uurtarief wordt toegewezen, en het project heeft $100 [!UICONTROL Fixed Revenue]de [!UICONTROL Utilization] rapport geeft $200 weer voor [!UICONTROL Planned Revenue] (de [!UICONTROL Planned Revenue] gekoppeld aan de uren op de taak). De [!UICONTROL Project Details] wordt $300 weergegeven (de [!UICONTROL Planned Revenue] uit de taak en de vaste inkomsten voor het project.) </p> 
    <p>Voor informatie over het bijhouden van inkomsten in [!DNL Workfront] zie <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">Overzicht van facturering en inkomsten</a>. </p> 
    <p>Voor informatie over [!UICONTROL Planned Revenue] in de [!UICONTROL Utilization report], zie <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Informatie over bronnengebruik weergeven </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Risk Cost]</td> 
   <td> <p>Het totaal van [!UICONTROL Potential Cost] van alle risico's voor het project waarbij rekening wordt gehouden met de waarschijnlijkheid dat het project zich voordoet. Dit bedrag is niet opgenomen in het [!UICONTROL Planned Cost] van het project.</p> <p>De [!UICONTROL Planned Risk Cost] van een project wordt berekend aan de hand van de volgende formule:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Profile]</td> 
   <td>Een beheerder-bepaalde inzameling van Lusjes en Portaalsecties die op de [!DNL Workfront] Toepassing [!UICONTROL Home] en andere dashboards.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Section]</td> 
   <td>Eén component van een tabblad op een dashboard of een portalpagina. Gewoonlijk één enkel Rapport, Grafiek, Kalender, of lijst van zeer belangrijke informatie.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Tab]</td> 
   <td>Een lusje op een Portaal of een Dashboard dat tot drie Portaalsecties bevat.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>Een verzameling projecten met verenigende kenmerken. Deze projecten concurreren doorgaans met dezelfde middelen, hetzelfde budget of dezelfde tijd. U kunt Portfolio's in Programma's verdelen en de projecten met de Programma's associëren alvorens zij aan een Portfolio worden toegevoegd.</p> <p>Zie voor meer informatie over portfolio's <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Overzicht van Portfolio's in [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Management]</td> 
   <td>Een praktijkgebied dat gericht is op het beheer van een collectie of verwante programma's en projectinspanningen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Optimizer]</td> 
   <td>A [!DNL Workfront] hulpmiddel bij het beoordelen en prioriteren van projecten binnen een portfolio.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Owner]</td> 
   <td>De belanghebbende die verantwoordelijk is voor de prioritering en de begroting van een portefeuille.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Potential Risk Cost]</td> 
   <td>Dit is een projectgebied dat u in lijsten en rapporten kunt de plaats bepalen. Het toont de potentiële kosten voor de risico's verbonden aan het project, als zij voorkomen. Zie voor meer informatie <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Mogelijke risicokosten berekenen </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Predecessor]</td> 
   <td> <p>Een taak die vóór de voltooiing van een afhankelijke taak moet worden voltooid. Ook een taak die als een taak is gemarkeerd [!UICONTROL Dependency] voor een andere taak. De voorgangers staan de planner toe om opeenvolging-gebiedingslogica te plaatsen, zoals om een taak te beginnen nadat een andere taak eindigt.</p> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overzicht van voorgangers van taken</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Company]</td> 
   <td>Het bedrijf tot wie de gebruiker behoort zoals aangewezen in hun gebruikersmontages. Bedrijven kunnen ook met projecten worden geassocieerd.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Contact]</td> 
   <td><p>De [!UICONTROL Primary Contact] is de maker van een uitgifte en wordt automatisch aangewezen door [!DNL Workfront] wanneer de persoon de kwestie creeert. U kunt dit veld handmatig bijwerken als u [!DNL Manage] machtigingen voor de uitgave. Een kwestie kan slechts één Primaire Contact hebben.</p> 
   <p>Als u de primaire contactpersoon wijzigt, heeft de gebruiker die oorspronkelijk als de primaire contactpersoon was aangewezen, nog [!UICONTROL Manage] toegang tot het probleem.</p>
   <p>Wanneer het omzetten van een kwestie in een taak of een project, de gebruiker die als [!UICONTROL Primary Contact] van de uitgifte [!UICONTROL Converted Issue Originator] van het project of de taak. Als de [!UICONTROL Primary Contact] van de uitgave wordt bijgewerkt nadat de uitgave is omgezet, [!UICONTROL Converted Issue Originator] wordt behouden als de [!UICONTROL Primary Contact] van de kwestie op het moment dat de omzetting plaatsvond. Zie ook "[!UICONTROL Converted Issue Originator]" in dit artikel.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Priority]</td> 
   <td>Een waarde die aan een taak, kwestie of een project kan worden toegewezen om aan te wijzen hoe belangrijk het is. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Private]</td> 
   <td>Op een [!UICONTROL Note] of [!UICONTROL Document]maakt u dat object verborgen voor de meeste viewers. Voor een Privé Rij van het Verzoek van de Hulp, slechts kunnen de gebruikers op het Team van het Project kwesties aan die rij (of project) door voorleggen [!UICONTROL Requests] gebied.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profile]</td> 
   <td>Alle informatie over een gebruikersaccount.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Program]</td> 
   <td> <p>Een subset binnen een portefeuille, waar soortgelijke projecten kunnen worden gegroepeerd om een welomschreven voordeel te behalen.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Management]</td> 
   <td>Beheer van afhankelijkheden, risico's, problemen, vereisten en oplossingen voor meerdere projecten om het programma gezond te houden en het vastgestelde programmavoordeel te behalen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Owner]</td> 
   <td>De belanghebbende die verantwoordelijk is voor het toezicht op en de organisatie van activiteiten om ervoor te zorgen dat de projectdoelstellingen in overeenstemming zijn met de bedrijfsdoelstellingen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Progress]</span> </td> 
   <td> <p>In een [!UICONTROL Goal] rapport, toont dit het percentage van hoe dicht een strategisch doel aan voltooiing is. Het percentage van de voortgang wordt weergegeven als een getal. Voor informatie over strategische doelstellingen, zie ook "[!UICONTROL Goal]" in deze tabel.</p> <p>Dit veld is alleen zichtbaar als uw organisatie een aankoop heeft gedaan [!DNL Workfront] Doelen. Voor informatie over het beheer van strategische doelen met [!DNL Workfront Goals], zie <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> Projecten toevoegen aan doelen in [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Progress Status]</td> 
   <td> <p>In een project, een Taak, en een rapport van het Doel, toont dit gebied de Status van de Voortgang van projecten, taken, of strategische doelstellingen. Raadpleeg de volgende artikelen voor meer informatie:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">Overzicht van voortgang van project</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Overzicht van status voortgang taak</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">Overzicht van voortgang en toestand van het doel in [!DNL Adobe Workfront Goals]</a> </p>
     <p>De [!UICONTROL Goal] en de [!UICONTROL Progress Status] for [!DNL goals] het veld is alleen zichtbaar als uw organisatie heeft aangeschaft [!DNL Workfront Goals]. Voor informatie over strategische doelstellingen in [!DNL Workfront Goals], zie <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] overzicht</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Project]</td> 
   <td> <p>Een groot deel van de werkzaamheden moet binnen een bepaald tijdsbestek worden voltooid en moet een specifiek budget en een bepaald aantal middelen gebruiken. Om het beheersbaar te maken, verdeelt u het project in een reeks taken. Als u alle taken uitvoert, wordt het project voltooid. Voor informatie over het plannen van een project, zie <a href="../../../manage-work/projects/planning-a-project/plan-project.md">Een projectoverzicht plannen</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Assignment Planned Hours]</td> 
   <td> <p>In een [!UICONTROL Initiative Job Role] rapport, dit toont het aantal van [!UICONTROL Planned Hours] gekoppeld aan een taakrol die is toegewezen aan taken of problemen in het project. Dit veld en de [!UICONTROL Initiative Job Role] rapporttype wordt niet weergegeven in uw [!DNL Workfront] -instantie tenzij uw bedrijf een [!DNL Workfront Scenario Planner] licentie. Voor informatie over de [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md">De [!DNL Workfront Scenario Planner] overzicht</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Details]</td> 
   <td>De details van de huidige status van een project.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Budgeted Cost]</td> 
   <td> <p> Dit is het [!UICONTROL Budgeted Cost] van een project zoals het in lijsten en rapporten toont.</p><p>Zie ook "[!UICONTROL Budgeted Cost]" in dit artikel.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Project Management]</td> 
   <td>Een reeks beleid dat de drempels voor projectverwezenlijking, categorisering, en het noemen van de projecten beheerst.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Project Overhead]</td> 
   <td>In een [!UICONTROL Hour] rapport, is dit gebied gereserveerd voor financiële informatie verbonden aan de uren die met het uurtype worden geregistreerd [!UICONTROL Project Time]. De projecten kunnen hun eigen het Factureren Tarieven hebben en als een uur rechtstreeks op een project wordt geregistreerd, dan zullen die tarieven in berekeningen worden gebruikt. Op basis van de projectinstellingen kunnen projecten ook verschillende valuta's hebben en kan er voor die uren een valutaomrekening plaatsvinden. De [!UICONTROL Project Overhead] object staat [!DNL Workfront] om die informatie te krijgen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Owner]</td> 
   <td>De gebruiker verantwoordelijk voor het beheren van het bereik, de tijdlijn en de toewijzingen van een project. De standaardfiatteur voor wijzigingsorders, financiële wijzigingen en te leveren items.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Planning]</td> 
   <td>Processen om het projectschema te ontwikkelen en te handhaven.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Sponsor]</td> 
   <td>Een profiel van een aangewezen belanghebbende waaraan elk van uw gebruikers zou moeten betrekking hebben. In [!DNL Workfront], worden deze aangeduid als [!UICONTROL Access Levels]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Teams]</td> 
   <td> <p>De inzameling van gebruikers of rollen die aan een project worden toegewezen</p> <p>Zie voor meer informatie <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">Overzicht van het projectteam</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project tracking]</td> 
   <td>De gegevens die worden gebruikt om de gezondheid en de reikwijdte van een project te meten</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projected]</td> 
   <td> <p>Een schatting van de tijdstempel van wanneer het werk zal worden voltooid op basis van de geplande uren en het percentage dat een taak, uitgave of project voltooid zal zijn.</p> <p>Dit heeft betrekking op datums of de [!UICONTROL Duration] van taken, kwesties, of projecten. Doorgaans worden datums en tijdsduur aangegeven die meer gelden voor het leven van de onderdelen van het werk, nadat een deel van het werk al is voltooid of enige tijd is verstreken. </p> <p>Bijvoorbeeld de [!UICONTROL Projected Completion Date] van een taak is de datum waarop [!DNL Workfront] verwacht dat deze taak zal worden voltooid op basis van hoeveel werk er tot dusverre is verricht , hoeveel mensen er zijn toegewezen en hoeveel tijd er is verstreken sinds de begindatum .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Deadline]</td> 
   <td> <p>In rapporten die de [!UICONTROL Document Version] object (zoals [!UICONTROL Document Version] verslag en [!UICONTROL Proof Approval] rapport). In dit veld wordt de dag van de week, de datum, het tijdstip en het jaar van de proeftijdslimiet weergegeven.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Decision]</td> 
   <td> <p>In rapporten die de [!UICONTROL Document Version] object (zoals [!UICONTROL Document Version] verslag en [!UICONTROL Proof Approval] rapport), toont dit gebied de beslissingsstatus van het bewijs (hangende, vereiste of goedgekeurde veranderingen)</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Name]</td> 
   <td> <p>In rapporten die de [!UICONTROL Document Version] object (zoals [!UICONTROL Document Version] verslag en [!UICONTROL Proof Approval] (rapport). In dit veld wordt de proefdruknaam weergegeven.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Pages]</td> 
   <td> <p>In rapporten die de [!UICONTROL Document Version] object (zoals [!UICONTROL Document Version] verslag en [!UICONTROL Proof Approval] (rapport), toont dit gebied het aantal pagina's inbegrepen in de proef.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Progress]</td> 
   <td> <p>In rapporten die de [!UICONTROL Document Version] object (zoals [!UICONTROL Document Version] verslag en [!UICONTROL Proof Approval] rapport), wordt de status van de voortgang van het bewijs weergegeven ([!UICONTROL Sent], [!UICONTROL Opened], [!UICONTROL Commented], [!UICONTROL Decision Made]).</p> <p>Zie voor meer informatie <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">Voortgangsoverzicht proefdrukken</a> in <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">Voortgang van proefdrukken en statusoverzicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proofing]</td> 
   <td>Een revisieproces waarbij een of meer gebruikers de inhoud markeren en opmerkingen plaatsen die moet worden gewijzigd in een afbeelding, een tekstdocument, een video of interactieve webinhoud.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>Op een [!UICONTROL Note] of [!UICONTROL Document]maakt deze optie dat object toegankelijk voor andere gebruikers of zelfs voor personen van buiten [!DNL Workfront]. Voor een [!UICONTROL Help Request Queue], [!UICONTROL Public] betekent dat alle gebruikers die problemen kunnen indienen bij een project, problemen kunnen indienen via de [!UICONTROL Requests] gebied.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Quality]</td> 
   <td>De perceptie van de arbeidskwaliteit binnen de organisatie.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue]</td> 
   <td>Ook genoemd de Rij van de Helpdesk of [!UICONTROL Help Request Queue]. Dit is een project dat is gepubliceerd naar de [!UICONTROL Requests] zodat gebruikers problemen kunnen indienen. Gewoonlijk worden de rijen gecreeerd voor bepaalde onderwerpen, zoals [!UICONTROL Bugs], [!UICONTROL Project Requests], enz.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Properties]</td> 
   <td>Deze instellingen definiëren de regels voor het indienen van uitgaven voor een project dat wordt gepubliceerd naar de [!UICONTROL Requests] gebied.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Topic]</td> 
   <td> <p>Een eigenschap op een [!UICONTROL Help Request Queue] Hiermee kunnen gebruikers die een uitgave verzenden een onderwerp selecteren. Onderwerpen kunnen:</p> 
    <ul> 
     <li>Aan een aangepast gegevensformulier worden gekoppeld.</li> 
     <li>Wijs de kwestie automatisch aan een gebruiker toe, rol, of team door de Verpletterende Regel die op het geselecteerde Onderwerp wordt geplaatst.</li> 
     <li>Verplaats de kwestie naar een verschillend project of rij door de verpletterende regel die op het geselecteerde onderwerp wordt geplaatst.</li> 
    </ul> <p>Zie voor meer informatie <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Werkvoorraadonderwerpen maken</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rank]</td> 
   <td> <p>In een [!UICONTROL Access Level] rapport, kunt u manueel wijzen op [!UICONTROL Rank] van de [!UICONTROL Access Level]. Dit helpt u als [!DNL Workfront] beheerder, om het niveau van ingewikkeldheid verbonden aan elk Niveau van de Toegang visueel te identificeren. U kunt bijvoorbeeld lagere getallen opgeven voor complexere ([!UICONTROL Plan]-level) Toegangsniveaus, en hogere aantallen voor minder complex ([!UICONTROL Requester]-level) Toegangsniveaus. U kunt de standaardtoegangsniveaus niet rangschikken. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ready]</td> 
   <td> <p>Dit gebied op een taakrapport wijst erop of [!UICONTROL Agile] taak is gemarkeerd als [!UICONTROL Ready] op de achtergrond. Deze markering geldt alleen voor [!UICONTROL Agile] taken, die taken zijn die zijn toegewezen aan een [!UICONTROL Agile] team. </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Recurrence Frequency]</td> 
   <td> <p>Een veld dat wordt weergegeven in het dialoogvenster [!UICONTROL Task Details] of de [!UICONTROL Edit Task] van een bovenliggende map van terugkerende taken. Het is de frequentie waarmee de taken in de herhaling voorkomen. Voor informatie over het creëren van terugkomende taken, zie <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">Herhalende taken maken</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reference Number]</td> 
   <td> <p>Projecten, taken en problemen worden automatisch gekoppeld aan een uniek referentienummer wanneer ze worden gemaakt. U kunt de [!UICONTROL Reference Number] in de [!UICONTROL Details] pagina met projecten, taken of problemen, of in een lijst of rapport. </p> <p><b>TIP</b><p><br>U kunt verwijzen naar referentienummers wanneer twee items dezelfde naam hebben, omdat referentienummers altijd uniek zijn. </p> <p>[!DNL Workfront] genereert automatisch opeenvolgende referentienummers op systeemniveau. Elk project, elke taak, of elke kwestie krijgt het volgende beschikbare aantal in de opeenvolging. <br></p> <p>Als gebruiker A bijvoorbeeld een taak maakt, [!DNL Workfront] zou de taak automatisch het Aantal van de Verwijzing 100 kunnen toewijzen. Als Gebruiker B een kwestie onmiddellijk daarna creeert, [!DNL Workfront] wijst het nummer 101 toe aan de uitgave. U kunt referentienummers niet handmatig bewerken. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rejection Issue]</td> 
   <td>In een project of een taakrapport, is dit de kwestie die wordt gecreeerd wanneer de goedkeuring voor het project of de taak wordt verworpen. Zie het artikel voor informatie over afwijzingskwesties <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Een goedkeuringsproces voor werkitems maken</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Remaining Risk Cost]</td> 
   <td> <p>Een projectgebied dat het verschil tussen toont [!UICONTROL Planned Risk Cost] van een project en het totaal van [!UICONTROL Actual Costs] van alle risico's voor het project. </p> <p>De [!UICONTROL Remaining Risk Cost] voor een project wordt berekend aan de hand van de volgende formule:</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Replanning]</td> 
   <td>De datums van een project wijzigen om problemen te verhelpen of te verhelpen. Een project dat bijvoorbeeld al enkele maanden in de wachtstand staat, moet opnieuw worden gepland om nauwkeurige data te weerspiegelen. Dit is een handmatige bewerking waarbij de data van het project of die van de taken worden aangepast. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Report]</td> 
   <td>Een grafiek of tabel met informatie over een gegeven tabel [!DNL Workfront] object en de bijbehorende kenmerken.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request]</td> 
   <td> <p>Een type kwestie die in één enkele gecentraliseerde rij wordt getrigeerd en niet aan een voortdurende het werkinspanning verwant is.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request Queue]</td> 
   <td>De achterstand van kwesties die door een verkeer en triageproces worden beheerd.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Request velocity]</td> 
   <td>De totale werkcyclustijd die nodig is om in te nemen en een aanvraag in te vullen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requester]</td> 
   <td>Doorgaans een licentietype. Een gebruiker met een vergunning van de Vraag kan verzoeken om nieuw werk indienen om in het systeem voor te komen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reserved Time]</td> 
   <td>De dagen die op de Persoonlijke Tijd van een gebruiker worden gespecificeerd, erop wijzend dat de gebruiker niet voor het werk beschikbaar zal zijn. Zie "[!UICONTROL Non Work Days]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Issue]</td> 
   <td> <p>Gebruik dit veld in weergaven of filters in een uitgifterapport om te verwijzen naar het probleem dat het probleem verhelpt. </p> <p>Voor informatie over het weergeven van het omzetten van objecten in rapporten raadpleegt u <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">De informatie van Objecten van de mening Oplosbaar en van het Oplossen in een rapport</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overzicht van Oplossende en Oplosbare objecten </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Project]</td> 
   <td> <p>In een probleemrapport gebruikt u dit veld in weergaven of filters om te verwijzen naar het project dat het probleem verhelpt. </p> <p>Voor informatie over het weergeven van het omzetten van objecten in rapporten raadpleegt u <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">De informatie van Objecten van de mening Oplosbaar en van het Oplossen in een rapport</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overzicht van Oplossende en Oplosbare objecten </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Task]</td> 
   <td> <p>Gebruik dit veld in weergaven of filters in een probleemrapport om te verwijzen naar de taak die het probleem verhelpt. </p> <p>Voor informatie over het weergeven van het omzetten van objecten in rapporten raadpleegt u <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">De informatie van Objecten van de mening Oplosbaar en van het Oplossen in een rapport</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overzicht van Oplossende en Oplosbare objecten </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource]</td> 
   <td>Gebruikers of rollen in [!DNL Workfront] en worden toegewezen aan projectteams, -taken en -problemen. Zij zijn verantwoordelijk voor de voltooiing van het werk verbonden aan projecten, taken, of kwesties. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Resource Management]</td> 
   <td> <p>[!UICONTROL Resource Management] is een reeks bedrijfsinstrumenten waarmee u het gebruik van uw middelen nauwkeurig kunt voorspellen op basis van hun beschikbaarheid, zodat het werk dat moet worden gedaan op tijd en op budget wordt voltooid. </p> <p>Met de hulpmiddelen van het Beheer van het Middel kunt u capaciteit op lange termijn en kortetermijnplanningsbehoeften voor uw middelen plannen. </p> <p>Voor informatie over Resource Management in [!DNL Workfront], zie <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">Aan de slag met Resource Management</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager IDs]</td> 
   <td><p>In een projectrapport, kunt u deze optie gebruiken wanneer het creëren van een filter om een specifieke middelmanager te vinden. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Managers]</td> 
   <td> <p>In een projectrapport of lijstmening, is dit een informatiegebied dat gebruikers toont die worden aangewezen om middelbeheersactiviteiten op het project uit te voeren.  Wanneer u "[!UICONTROL Resource Managers]" in een rapport, wordt een lijst van middelmanagers getoond, met elke middelmanager op het project dat door een komma wordt gescheiden. U kunt maximaal 30 middelmanagers op een bepaald project aanwijzen.</p> <p>Zie het artikel voor meer informatie <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">Bronbeheerders aanwijzen voor een project of sjabloon </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Resource Planner Budgeted Hours] </td> 
   <td>De voor het project begrote uren en de bijbehorende middelen in het [!UICONTROL Resource Planner]. Zie ook "[!UICONTROL Budgeted Hours]" in dit artikel. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Resource Planner] </td> 
   <td>Geavanceerd [!DNL Workfront] hulpmiddel dat u middelen over projecten, baanrollen, of gebruikers laat bekijken en beheren. Zie voor meer informatie <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Overzicht van de bronnenplanner</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Planner Budgeted Labor Cost]</td> 
   <td> <p>Dit zijn de kosten verbonden aan de uren die voor de rollen van de projectbaan gebruikend de Planner van het Middel in de begroting worden opgenomen. </p> <p>Zie ook "Budgeted Labour Cost" in dit artikel. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Resource Pools]</td> 
   <td> <p>Brongroepen zijn verzamelingen van gebruikers die aan een project kunnen worden gekoppeld. De gebruikers in dezelfde bronnenpool behoren gewoonlijk tot dezelfde afdeling, hebben vergelijkbare of aanvullende vaardigheden of worden gefinancierd uit hetzelfde budget. U kunt veelvoudige Pools van het Middel aan een project of aan een gebruiker associëren. Een bronnenpool kan uitsluitend aan een project worden toegewezen of door meerdere projecten worden gedeeld.</p> 
   <p>Voor meer informatie over middelpools, zie <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Overzicht van bronnenpools </a>.</p> 
   <p>In projectrapporten, tonen de Pools van het Middel alle pools verbonden aan een project. Dit object kan niet in een groep worden gebruikt.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Utilization]</td> 
   <td>Een rapport met het aantal uren dat beschikbaar is tijdens een bepaalde periode en het aantal uren dat is gepland voor elke gebruiker in het rapport. Dit wordt ook berekend in [!UICONTROL Average Hours Per Day] en een toewijzingspercentage.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Result]</td> 
   <td>In [!DNL Workfront Goals]Een resultaat is een voortgangsindicator voor een doel. Dit kan een getal, een percentage of een valutabedrag zijn dat u handmatig bijwerkt. U kunt geen resultaten in een rapport tonen en u kunt niet tot hen door [!DNL Workfront] API. Zie voor informatie over activiteiten <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Aan de slag met resultaten en activiteiten in Adobe Workfront Goals</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Revenue]</td> 
   <td>Een factureerbare hoeveelheid voor de taak of het project. Het bedrag kan per uur, vast of een combinatie van beide zijn.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Revenue Type]</td> 
   <td>Het type inkomsten bepaalt hoe de taak inkomsten zal genereren. Enkele voorbeelden zijn [!UICONTROL Fixed Hourly], [!UICONTROL Role Hourly], en [!UICONTROL Role Hourly w/Cap]. Voor informatie over het bijhouden van inkomsten in [!DNL Workfront] zie <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overzicht van facturering en inkomsten</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>Doorgaans een licentietype. Een gebruiker met een [!UICONTROL Reviewer] De vergunning heeft de capaciteit om het werkpunten in het systeem te herzien en goed te keuren.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk]</td> 
   <td> <p>Dit kan verwijzen naar de volgende concepten in [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>Een gebied op een project dat erop wijst hoe riskant een project kan zijn. U kunt de uitvoering van uw projecten prioriteren op basis van het risiconiveau. Projecten kunnen de volgende risiconiveaus hebben:</p> <p>- [!UICONTROL Very Low]</p> <p>- [!UICONTROL Low]</p> <p>- [!UICONTROL Medium]</p> <p>- [!UICONTROL High]</p> <p>- [!UICONTROL Very High]</p> <p>De risiconiveaus die u aangeeft voor een project kunnen niet worden aangepast. </p> <p> Zie de sectie Projectinstellingen in het artikel voor informatie over het bijwerken van het risico van een project <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Projecten bewerken</a>. U kunt het risicogebied van een project in rapporten tonen. </p> </li> 
     <li> <p>Een gebeurtenis die tijdens de duur van een project kan voorkomen die een potentiële invloed op de kosten, het werkingsgebied, of het programma van het project identificeert. U bepaalt potentiële risico's aan een project en associeert een waarschijnlijkheid dat zij of kosten voorkomen aangezien u het BedrijfsGeval van het project bouwt. Voor informatie over het toevoegen van risico's aan het BedrijfsGeval van het project, zie "tot stand brengen en risico's op projecten uitgeven". </p> <p>U kunt geen risico's weergeven die zijn gedefinieerd in het dialoogvenster [!UICONTROL Business Case] in verslagen. U kunt slechts verscheidene soorten Kosten van het Risico in rapporten en lijsten tonen. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Cost]</td> 
   <td> <p>De kosten in verband met de risico's voor een project. Hier volgt een overzicht van de risicokosten voor projecten die u in rapporten kunt weergeven:</p> 
    <ul> 
     <li> <p>[!UICONTROL Actual Cost]: een veld met een risico dat de werkelijke kosten van het risico toont. Naast rapporten en lijsten kunt u het vinden in [!UICONTROL Edit Risk] bij het bewerken of maken van een risico. </p> <p>Voor project-, taak- of uitgaven raadpleegt u "[!UICONTROL Actual Cost]" in dit artikel. </p> </li> 
     <li> <p>[!UICONTROL Planned Risk Cost]: een veld op het project dat een totaal van alle [!UICONTROL Potential Risk Costs] voor het project. Zie ook "[!UICONTROL Planned Risk Cost]" in dit artikel. </p> <p>Voor informatie over de Mogelijke Kosten van het Risico, zie <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Mogelijke risicokosten berekenen </a>. </p> </li> 
     <li> <p>[!UICONTROL Remaining Risk Cost]: een veld op het project waarin het verschil tussen het totaal van de [!UICONTROL Actual Costs] van alle risico's en de [!UICONTROL Planned Risk Cost]. Zie ook "Resterende risicokosten" in dit artikel. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Management]</td> 
   <td>Processen om risico te identificeren, te verlichten en te controleren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td>Zie "[!UICONTROL Job Role]" in dit artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing]</td> 
   <td>Automatisch toewijzend of bewegend een kwestie, gewoonlijk toe te schrijven aan een Onderwerp van de Rij of door als StandaardRoute (het Verpletteren van Regel) voor de rij te zijn.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing Rule]</td> 
   <td>Het plaatsen op projecten en rijonderwerpen die automatisch een kwestie aan een gebruiker, een rol, of een team toewijst, of de kwestie naar een ander project of een rijonderwerp verplaatst. Het verpletteren van Regels wordt over het algemeen gebruikt met de Queues van het Verzoek van de Hulp om inkomende kwesties automatisch toe te wijzen.</td> 
  </tr> 
 </tbody> 
</table>

## S - U

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objectnaam</th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Saved Search]</td> 
   <td>Een zoekopdracht waarvoor de zoekcriteria zijn opgeslagen. Met Opgeslagen zoekopdrachten kunt u eenvoudig weer dezelfde zoekopdracht uitvoeren zonder dat u de zoekcriteria opnieuw hoeft in te voeren.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Scenario] (in [!DNL Workfront Fusion]) </td> 
   <td> <p>Een scenario bestaat uit een reeks stappen (modules) die aangeven hoe gegevens moeten worden overgebracht en getransformeerd tussen apps/services.</p> <p>Voor informatie over scenario's in [!DNL Workfront Fusion], zie <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] scenario-overzicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scenario] (in de [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>In de [!DNL Scenario Planner], is een scenario een exemplaar van een plan. </p> <p>De [!DNL Scenario Planner] vereist een aanvullende licentie. Voor informatie over de [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">De [!DNL Scenario Planner] overzicht</a>. </p> <p>Voor informatie over het creëren van scenario's, zie <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">Plan-scenario's maken en vergelijken in het dialoogvenster [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule]</td> 
   <td>Het wekelijkse werkschema, met inbegrip van werktijden, gecombineerd met Dagen uit (zoals Vakantiedagen) en uitzonderingsdagen (zoals een zaterdag werkdag). U kunt programma's met projecten en gebruikers associëren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule Exemption]</td> 
   <td>Ook bekend als a [!UICONTROL Modified Shift]. Dagen die gepland zijn in tegenstelling tot de normale wekelijkse arbeidstijden zoals bepaald in het schema. Een zaterdag die gepland is om te werken, zou bijvoorbeeld een [!UICONTROL Schedule Exemption].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scheduled Report]</td> 
   <td> <p>Wanneer u een rapport van rapporten bouwt, kunt u informatie over de programma's van het rapport tonen, als het rapport voor levering gebruikend gepland is [!UICONTROL Scheduled Report] veld. Dit gebied toont veelvoudige waarden, voor elk programma van elk rapport, in een bulleted lijst. Zie het artikel voor meer informatie over het plannen van rapporten <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Overzicht van levering rapporteren</a>.</p> <p>Omdat in dit veld meerdere waarden worden weergegeven, kan het niet worden gebruikt in een groep. U hebt alleen toegang tot dit bestand in een filter of weergave. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scope Change]</td> 
   <td>An [!UICONTROL Audit Trail] dat, als actief, een nota op om het even welk ogenblik produceert een verandering in het Toepassingsgebied van een project of een taak, zoals als [!UICONTROL Task Duration] of de [!UICONTROL Predecessors] worden gewijzigd.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section]</td> 
   <td>Een gebied op het scherm met een eigen koptekst dat is gemaakt om de aangepaste gegevens voor weergavedoeleinden in te delen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section Break]</td> 
   <td>Een tussenruimte of rand tussen secties.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Security]</td> 
   <td>De instellingen waarmee een gebruiker kan communiceren met bepaalde objecten in het systeem en niet met andere. Zie ook "[!UICONTROL Access Levels]" in dit artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Setup]</td> 
   <td>Het gebied waar beheerders systeemconfiguraties en voorkeuren kunnen instellen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severity]</td> 
   <td> <p>[!UICONTROL Severity] geeft aan hoe waarschijnlijk een punt de voltooiing van de werkzaamheden zal beïnvloeden. Bijvoorbeeld een probleem met hoge [!UICONTROL Severity] kan de voltooiing van een taak volledig blokkeren, maar een kwestie met laag [!UICONTROL Severity] kan slechts cosmetisch zijn.</p> <p>Zie voor meer informatie <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> Ernst van probleem bijwerken</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severities]</td> 
   <td>Zie "[!UICONTROL Severity]" in dit artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sharing]</td> 
   <td>De handeling waarmee andere gebruikers een bepaald item kunnen weergeven of bewerken in [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Slack Date]</td> 
   <td>In een taakweergave of rapport [!UICONTROL Slack Date] geeft de exacte datum weer waarop een taak beslist invloed kan hebben op de [!UICONTROL Completion Date] van het project. Voor informatie over de [!UICONTROL Slack Date] van een taak, zie <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">Overzicht van Datum Slack taak</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Smart Assignments]</td> 
   <td> <p>Bij het toewijzen van taken of problemen aan gebruikers [!DNL Workfront] doet aanbevelingen ([!UICONTROL Smart Assignments]) over wie de beste gebruikers het werk moeten voltooien, op basis van de tijd die zij hebben om het te voltooien en hun relatie met het project.</p> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">Overzicht van slimme toewijzingen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>Geeft het bovenliggende object van een ander object aan. Een document dat bijvoorbeeld is gekoppeld aan een taak, heeft de naam van de taak in het dialoogvenster [!UICONTROL Source] veld van een [!UICONTROL Document] rapport of mening; een kwestie die onder een project wordt geregistreerd heeft de naam van het project in [!UICONTROL Source] veld van een Issue report of view. </p> 
   <p>In de volgende rapporten wordt een kolom Bron weergegeven waarin u informatie over het bovenliggende object kunt weergeven:</p>
  <ul><li>Problemen melden</li>
    <li>Uur-rapporten</li>
    <li>Documentrapporten </li>
    </ul>
   <p>Als de gebruikers geen toestemmingen aan het oudervoorwerp van een kwestie, een uur, of een document hebben, toont de Bronkolom van het rapport leeg, zelfs wanneer het rapport aan vertoning wordt gevormd, of met de toegangsrechten van een andere gebruiker moet worden geleverd. </p>
   <p> Om informatie over het oudervoorwerp in het rapport te tonen, adviseren wij toevoegend een kolom voor het oudervoorwerp waar u de naam van de ouder kunt tonen. </p>
    <p>Bijvoorbeeld, kunt u om het even welke volgend aan een rapport met een Bronkolom toevoegen: </p>
    <ul><li>De kolommen van de Naam van het Project, van de Naam van de Taak, of van de Naam van de Uitgave aan een document of uurrapport.</li>
    <li>De kolommen van de Naam van het Project of van de Naam van de Taak aan een probleemrapport. </li> </ul>
    Zie voor meer informatie <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">Een rapport uitvoeren en leveren met de toegangsrechten van een andere gebruiker</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Start Date]</td> 
   <td> <p>De datum waarop het werk aan een item moet worden gestart. Er zijn verschillende begindatums in [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL Planned]</li> 
     <li>[!UICONTROL Actual]</li> 
     <li>[!UICONTROL Projected] </li> 
    </ul> <p>In een [!UICONTROL Rate report]Dit is de datum waarop een nieuw factureringspercentage voor een functie op projectniveau begint. De uren verbonden aan het project die na deze datum zijn worden vermenigvuldigd met dit het factureringspercentage om de opbrengst op het project te berekenen. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td> <p>Een indicator die wordt gebruikt om een werkschemapositie van een het werkpunt of van een strategisch doel te signaleren.</p> <p>Voor projecten [!UICONTROL Status] is het plaatsen op het project dat erop wijst of het project is:</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL On Hold] </li> 
     <li>[!UICONTROL Complete] </li> 
     <li>[!UICONTROL Dead]</li> 
    </ul> <p>Voor meer informatie over de Status van een project, zie <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">Heb toegang tot de lijst van de statussen van het systeemproject</a>.</p>
    <p>Voor taken [!UICONTROL Status] is een instelling op de taak die aangeeft of de taak:</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Complete]</li> 
    </ul> <p>Zie voor meer informatie over taakstatus <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">De lijst met taakstatussen van het systeem openen</a></p> <p>Voor problemen wordt de [!UICONTROL Status] is een instelling voor het probleem die aangeeft of dit probleem:</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Awaiting Feedback]</li> 
     <li>[!UICONTROL On Hold]</li> 
     <li>[!UICONTROL Resolved]</li> 
     <li>[!UICONTROL Won't Resolve]</li> 
     <li>[!UICONTROL Cannot Duplicate]</li> 
     <li>[!UICONTROL Verified Complete]</li> 
     <li>[!UICONTROL Reopened]</li> 
    </ul> <p>Zie voor meer informatie over uitgiftestatussen <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Toegang krijgen tot de lijst met systeemuitgiftestatussen</a>.</p> 
    <p>Voor strategische doelstellingen [!UICONTROL Status] is het plaatsen op het doel dat erop wijst of het doel is:</p> 
     <ul> 
      <li>[!UICONTROL Active]</li> 
      <li>[!UICONTROL Draft]</li> 
      <li>[!UICONTROL Inactive]</li> 
      <li>[!UICONTROL Closed]</li> 
     </ul> 
     <p>Zie voor meer informatie over strategische doelstellingen ook "[!UICONTROL Goal]" of "[!UICONTROL Goals]" in dit artikel. </p> 
     <p>Voor strategische doelen is dit veld alleen zichtbaar als uw organisatie een aankoop heeft gedaan [!DNL Workfront Goals]. Voor informatie over het beheer van strategische doelen met [!DNL Workfront Goals], zie <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] overzicht</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Change]</td> 
   <td>An [!UICONTROL Audit Trail]. Een nota wordt geproduceerd wanneer een gebruiker de Status van het project, de taak, of de kwestie verandert.</td> 
  </tr> 
  <tr> 
   <td>Statuspictogrammen</td> 
   <td> <p>U kunt de ingebouwde [!UICONTROL Status Icons] veld als kolom in uw weergaven om de zichtbaarheid van belangrijke punten van uw objecten te verbeteren, zoals:</p> 
    <ul> 
     <li>Een object bevat documenten</li> 
     <li>Een object is gekoppeld aan een goedkeuringsproces</li> 
     <li>Aan een object zijn aanvullende notities gekoppeld</li> 
     <li>Een last is factureerbaar of terugbetaalbaar </li> 
     <li>Een taak bevindt zich op een kritiek pad</li> 
     <li>Een gebruiker behoort tot een bedrijf, een team, of is gevestigd in een verschillende tijdzone </li> 
    </ul> <p>U kunt de [!UICONTROL Status Icons] in de weergaven van de volgende objecten: </p> 
    <ul> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Template Tasks]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Users]</li> 
    </ul> <p>Zie voor meer informatie <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Ingebouwde statuspictogrammen in weergaven</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Update]</td> 
   <td> <p>In een project-, taak- of uitgifterapport wordt in dit veld de meest recente statusupdate weergegeven die objecteigenaars hebben geleverd in de map '[!UICONTROL Updates]". Voor projecten betekent dit dat opmerkingen van de eigenaar van het project, en voor taken en kwesties, dat de opmerkingen van de ondertekenaars zijn.</p> 
   <p> Opmerkingen bij het bijwerken van de status van een object worden niet weergegeven in het dialoogvenster [!UICONTROL Status Update] kolom.</p> <p>Als u de optie '[!UICONTROL New],' '[!UICONTROL In Process],' en '[!UICONTROL Complete]' statussen, gebruik de [!UICONTROL Status] kolom.</p> <p>Raadpleeg het artikel voor meer informatie over statussen <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Taakstatus bijwerken</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Statuses]</td> 
   <td>Zie "[!UICONTROL Status]" in dit artikel.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>Een grafiek die de status van artikelen (taken in de 'agile'-methodologie) en hoe ze vorderen naar voltooiing.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Hours]</td> 
   <td>Een maateenheid die wordt gebruikt om de moeilijkheid of de ingewikkeldheid van een Verhaal te meten. Gegraveerde teams kunnen kiezen of ze Uren of Punten gebruiken.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Points]</td> 
   <td>Een maateenheid die wordt gebruikt om de moeilijkheid of de ingewikkeldheid van een Verhaal te meten. Gegraveerde teams kunnen kiezen of ze Uren of Punten gebruiken.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategic]</td> 
   <td>Werk op lange termijn dat de organisatie of de werking van de organisatie verandert.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Strategic Alignment]</td> 
   <td>Het meten en het richten van bedrijfsdoelstellingen over portefeuilles en programma's.</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>Dit wordt gebruikt in rapportkolommen wanneer het gebruiken van de interface van de Wijze van de Tekst. </p>
   <p>De <code>[!UICONTROL stretch]</code> wordt gebruikt om aan te geven welke kolommen extra ruimte innemen die niet nodig is voor de weergave. De breedte van de gebruikersinterface van de werkruimte voor een standaardgebruiker is ongeveer 850 pixels. Dit betekent dat als u een weergave hebt met vier kolommen (elk 150 pixels), uw weergave 600 van 850 pixels in beslag neemt. Er zijn 250 extra pixel in UI die aan de kolommen zullen worden toegevoegd die een rekbaarheidspercentage hebben verstrekt. </p>
   <p>Het uitrekken van een kolom wordt afgedwongen wanneer u de extra coderegel gebruikt: <code>[!UICONTROL usewidths=true]</code> voor ten minste een van de kolommen in de weergave. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Subscribers]</td> 
   <td> <p>Gebruikers die zich abonneren op projecten, taken of problemen.</p> <p>Wanneer u dit gebied in een rapport gebruikt, toont een lijst van abonnees, met elke abonnee die door een komma wordt gescheiden.</p> <p>Zie het artikel voor meer informatie <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Abonneren op objecten in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Summary Task]</td> 
   <td>Zie "[!UICONTROL Parent Task]" in dit artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subtask]</td> 
   <td>Een onderliggende taak die zich onder een bovenliggende taak bevindt.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL System Governance]</td> 
   <td>Een reeks beleidsregels die wijzigingen en onderhoud van een systeem regelt.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL System Integration]</td> 
   <td>Het proces waarbij verschillende computersystemen en softwaretoepassingen fysiek of functioneel met elkaar worden verbonden om als een gecoördineerd geheel te fungeren.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task]</td> 
   <td> <p>Een activiteit die als stap naar het bereiken van een definitief doel (het voltooien van het Project) moet worden uitgevoerd.</p> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">Overzicht van taken</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Attribute]</td> 
   <td>Andere velden of objecten die zijn gekoppeld aan een taak en die bepaalde details over de taak aangeven. Enkele voorbeelden zijn [!UICONTROL Planned Completion Date] en [!UICONTROL Status].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Constraint]</td> 
   <td>Zie "[!UICONTROL Constraint Type]" en "[!UICONTROL Constraint Date]".</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Management]</td> 
   <td>Een reeks beleid dat de drempels voor taakverwezenlijking, toewijzing, sluiting, en zichtbaarheid beheerst.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Owner]</td> 
   <td>Het team of de gebruiker die verantwoordelijk is voor de raming van de inspanning en de voltooiing van de taak</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Team]</td> 
   <td> <p>Een inzameling van gebruikers die aan gelijkaardige doelstellingen of bedrijfsdoelstellingen werken. Deze gebruikers kunnen collectief aan een het werkpunt worden toegewezen door het team aan het het werkpunt toe te wijzen.</p> <p>Zie voor meer informatie over teams <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Teams overzicht</a>.</p> <p>Projecten kunnen een [!UICONTROL Project Team], dat alle gebruikers of rollen bevat verbonden aan het werk aan het project.</p> <p>Zie voor meer informatie over projectteams <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Overzicht van het projectteam</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Template]</td> 
   <td> <p>De malplaatjes van het project zijn generische overzichten van uw meest herhaalbare projecten. U kunt taken, rijonderwerpen, douaneformulieren bepalen, documenten of goedkeuringen vastmaken wanneer u een projectmalplaatje creeert om u tijd te besparen wanneer u een nieuw project moet creëren. </p> <p>U kunt malplaatjes aan bestaande projecten vastmaken, of u kunt hen gebruiken om nieuwe projecten te bouwen. Alle informatie die op het malplaatje wordt gespecificeerd brengt naar de projecten over die gebruikend het worden gecreeerd. </p> <p>Zie voor meer informatie over sjablonen <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">Overzicht van de projectsjabloon</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Template Task]</td> 
   <td>Een taak die deel uitmaakt van een sjabloon. De Taken van het malplaatje worden Taken in het project dat door het malplaatje wordt gecreeerd te gebruiken.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>A [!UICONTROL Note] en de verzameling van antwoorden die betrekking hebben op een bepaald onderwerp.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thumbnail]</td> 
   <td> <p> In een [!UICONTROL Document] weergegeven in een miniatuur. </p> <p> Selecteren <strong>[!UICONTROL Thumbnail]</strong>  om een miniatuur van 33 tot 66 pixels breed in het rapport weer te geven. </p> <p>De grootte van de miniatuur wordt aangepast wanneer u de breedte van de kolom in een lijst of rapport wijzigt.</p> <p>Zie ook "[!UICONTROL Large Thumbnail]" in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time Off]</td> 
   <td>U kunt een [!UICONTROL Time Off] rapporteren om te bekijken wanneer gebruikers time-off in hun profiel hebben aangegeven. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet]</td> 
   <td> <p>Een tijdschema dat gebruikers toestaat om daadwerkelijke uren in te gaan dat zij het werken aan projecten, taken, of kwesties, of uren besteedden zij aan andere activiteiten niet verwant met het werk, zoals vergaderingen of opleiding. Naast het ingaan van de hoeveelheid tijd u het werken besteedde, kunt u ook erop wijzen of de tijd werk-verwant is of het aan overheadtijd door de Types van Uur te gebruiken om uw tijdingangen te bepalen is. Voor informatie over timesheets raadpleegt u <a href="../../../timesheets/timesheets/timesheets-overview.md">Overzicht van tijdbladen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet Profile]</td> 
   <td> <p>A [!UICONTROL Timesheet Profile] is een sjabloon die [!DNL Workfront] gebruiken om automatisch tijdbladen te creëren voor de gebruikers verbonden aan hen. </p> <p>U kunt een aantal montages vormen die op elk timesheet zullen van toepassing zijn aangezien het wordt gecreeerd. Enkele van deze instellingen zijn: hoe vaak het tijdspad moet worden gemaakt (wekelijks, om de week, tweemaal per maand of maandelijks), de startdag van het tijdspad, de fiatteurs van het tijdspad, de beschikbare [!UICONTROL Hour Types] dat gebruikers aan geregistreerde uren kunnen associëren.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL Top Parent ID] </td> 
   <td> <p>Met dit veld kunt u gegevens over een groep op hoofdniveau en de bijbehorende subgroepen in een lijst of rapport identificeren en filteren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Top Parent Name] </td> 
   <td> <p>Met dit veld kunt u gegevens identificeren over een groep op hoofdniveau en de bijbehorende subgroepen in een [!UICONTROL View] voor een lijst of rapport.</p> <p>U kunt dit ook doen met de [!UICONTROL Top Parent ID] veld.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total Hours]</td> 
   <td> <p>In een [!UICONTROL project report]In dit veld wordt de afgeronde som van alle uren van het project weergegeven, de laatste keer dat de projectfinanciering werd berekend. [!UICONTROL Actual Hours] wijzen op de nauwkeurige uren het programma worden geopend op het project. De [!UICONTROL Actual Hours] moet overeenkomen met de [!UICONTROL Total Hours]. Als de [!UICONTROL Total Hours] lijkt aanzienlijk te verschillen van de [!UICONTROL Actual Hours] in het veld moet u de financiën voor het project opnieuw berekenen.</p> <p>Zie het artikel voor meer informatie over het opnieuw berekenen van projectfinanciën <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">Projectfinanciën opnieuw berekenen</a>.</p> <p>In een tijdsplaat [!UICONTROL Standard] bekijken, verwijst dit gebied naar de totale uren die voor punten voor de data worden geregistreerd die op timesheet worden getoond. De [!UICONTROL Total Hours] het gebied voor timesheets in deze ingebouwde mening verwijst naar "[!UICONTROL hoursDuration]" veld dat het verschil in uren tussen de begin- en einddatum van het tijdblad dynamisch berekent. Dit wordt gebruikt om de [!UICONTROL Total Hours] in rood als de gebruiker meer tijd dan de beschikbare uren in het tijdspad van timesheet registreert. Zie voor meer informatie <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">Totale uren weergeven op het tijdblad</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tracking Mode]</td> 
   <td> <p>An attribute of a task. Hiermee bepaalt u hoe en wanneer de geprojecteerde tijdlijnen worden bijgewerkt voor een taak. Bijvoorbeeld:</p> 
    <ul> 
     <li>[!UICONTROL User Must Update] vereist dat een taak handmatig wordt bijgewerkt. Anders wordt het [!UICONTROL Behind Schedule]vervolgens [!UICONTROL Late].</li> 
     <li>[!UICONTROL Auto Complete] automatisch een taak zal voltooien op de vervaldatum, of [!UICONTROL Planned Completion Date], is verstreken.</li> 
    </ul> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">Overzicht van de modus Taken bijhouden</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Trigger]</td> 
   <td>Een gebeurtenis die een scenario start.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trouble Task]</td> 
   <td>Een onvolledige taak met een voorwaarde van [!UICONTROL Late], [!UICONTROL Behind Schedule], of [!UICONTROL At Risk].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unassigned Task]</td> 
   <td>Een taak die niet aan om het even welke Gebruiker, Rol, of Team wordt toegewezen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Update Type]</td> 
   <td> <p>Een instelling voor een project die bepaalt wanneer de projectietijdlijn van het project opnieuw wordt berekend. De [!UICONTROL Update Type] kan de volgende waarden hebben:</p> 
    <ul> 
     <li>[!UICONTROL Automatic and On Change]</li> 
     <li>[!UICONTROL Automatic Only]</li> 
     <li>[!UICONTROL Manual Only] </li> 
    </ul> <p>Zie voor meer informatie <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Selecteer het Type van projectupdate </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User]</td> 
   <td>Een account gemaakt in [!DNL Workfront] om een persoon toe te staan om zich aan te melden en met het systeem in wisselwerking te staan.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL User Delegation]</p> </td> 
   <td> <p>Een te rapporteren object dat u het volgende vertelt:</p> 
    <ul> 
     <li>Welke gebruikers taak, kwestie, en projectgoedkeuringen hebben gedelegeerd</li> 
     <li>Welke gebruikers taak, kwestie en projectgoedkeuringen hebben gehad die aan hen worden gedelegeerd</li> 
     <li>Wanneer deze delegaties beginnen en eindigen</li> 
    </ul> <p>Zie voor meer informatie <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">Een gebruikersdelegatierapport maken</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface]</td> 
   <td>Alle visuele en interactieve aspecten van de [!DNL Workfront] toepassing.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface Preferences]</td> 
   <td>[!UICONTROL User Interface Setup]. [!DNL Workfront] beheerders kunnen deze instellingen wijzigen om aspecten van de gebruikersinterface aan te passen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Utilization]</td> 
   <td>De beschikbaarheid voor een gebruiker of een rol die op het toegewezen programma, PTO, en huidige werkbelasting wordt gebaseerd.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Utilization]</td> 
   <td> <p>Een onderzoek dat met een rapport wordt gecombineerd dat toont hoe de Gebruikers (Middelen) worden toegewezen of over-toegewezen. Zie "[!UICONTROL Resource Utilization]" in dit artikel.</p> </td> 
  </tr> 
 </tbody> 
</table>

## V - Z

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Objectnaam</th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Velocity]</td> 
   <td>Een maat van de totale werkcyclustijd (hoe lang het duurt om een werk te voltooien) en hoe vaak het werk in de oorspronkelijk toegezegde tijd (werk-aan-bewijs verhouding) wordt gedaan.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL View]</td> 
   <td> <p>De meningen verwijzen naar een rapporterend element dat u toestaat om de kolommen in een rapport of in een lijst van voorwerpen te wijzigen.</p> 
   <p> De mening verwijst ook naar het recht van een gebruiker om informatie over een voorwerp slechts te bekijken, volgens hun toegangsniveau of op een toestemmingendelend niveau op dat voorwerp.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL View Icons]</td> 
   <td> <p> Dit is hetzelfde veld als statuspictogrammen, maar het is alleen beschikbaar voor de volgende weergaven: </p> 
    <ul> 
     <li> [!UICONTROL Documents] </li> 
    </ul> <p> Zie het artikel voor meer informatie <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">Ingebouwde statuspictogrammen in weergaven</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Month]</td> 
   <td> <p>In een rapportlijst, toont het het aantal tijden het rapport tijdens de laatste maand is bekeken.<br>Raadpleeg het artikel voor meer informatie over het gebruik in rapportlijsten <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Rapportgebruik weergeven</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Quarter]</td> 
   <td>In een rapportlijst, toont het het aantal tijden het rapport tijdens het laatste kwartaal is bekeken.<br>Raadpleeg het artikel voor meer informatie over het gebruik in rapportlijsten <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >Rapportgebruik weergeven</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Year]</td> 
   <td>In een rapportlijst, toont het het aantal tijden het rapport tijdens het laatste jaar is bekeken.<br>Raadpleeg het artikel voor meer informatie over het gebruik in rapportlijsten <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Rapportgebruik weergeven</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Month]</td> 
   <td> <p>In een rapportlijst, toont het het aantal tijden het rapport tijdens deze maand is bekeken.<br>Raadpleeg het artikel voor meer informatie over het gebruik in rapportlijsten <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Rapportgebruik weergeven</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Quarter]</td> 
   <td>In een rapportlijst, toont het het aantal tijden het rapport tijdens dit kwartaal is bekeken.<br>Raadpleeg het artikel voor meer informatie over het gebruik in rapportlijsten <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">Rapportgebruik weergeven</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Year]</td> 
   <td>In een rapportlijst, toont het het aantal tijden het rapport tijdens dit jaar is bekeken.<br>Raadpleeg het artikel voor meer informatie over het gebruik in rapportlijsten <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">Rapportgebruik weergeven</a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> In een rapport, wanneer het gebruiken van [!UICONTROL Text Mode] -interface, de coderegel waarin u de breedte van elke kolom kunt opgeven in pixels. Workfront biedt een aanbevolen breedte voor elk veld, maar afhankelijk van het type veld en de indeling kunt u de breedte aanpassen.
U moet de extra <code>[!UICONTROL usewidths=true]</code> coderegel om de voor de kolom opgegeven breedte af te dwingen. 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>In een project, een taak, of een uitgifterapport, die de volgende verklaring op tekstwijze gebruiken toont de Geplande Uren van het project, de taak, of de kwestie:</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>Zie voor informatie over het gebruik van de tekstmodus <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Overzicht van syntaxis in tekstmodus</a>. </p> 
   <p><b>TIP</b> 
   <p>In een uitgiftenrapport voegt u een van de opties [!UICONTROL Planned Hours] velden voegen de <code>work </code>aan het rapport. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work]</td> 
   <td> <p>Een van de twee primaire licentietypen. Dit heeft minder toegang dan [!UICONTROL Plan], maar kan updates in het systeem maken en uitvoeren. Een gebruiker met een werkvergunning heeft meer mogelijkheden dan een [!UICONTROL External], [!UICONTROL Reviewer], of [!UICONTROL Requester] vergunninghouder.</p> <p>Zie voor meer informatie <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] overzicht van licenties</a>.</p> <p>Het werk kan betrekking hebben op het aantal [!UICONTROL Planned Hours] voor een project, taak of kwestie. Zie voor meer informatie de "[!UICONTROL work]" in deze tabel. </p> <p><b>TIP</b></p> <p> In een uitgiftenrapport voegt u een van de opties [!UICONTROL Planned Hours] velden voegen de <code>work </code>aan het rapport. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Breakdown Structure]</td> 
   <td>Een hiërarchische structuur van de taken die door het projectteam moeten worden uitgevoerd die op de ouder/kindverhouding wordt gebaseerd.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Work Effort] </td> 
   <td> 
    <p>Een projectmanager zou kunnen besluiten om dit gebied in plaats van te gebruiken [!UICONTROL Planned Hours] een raming te maken van de inspanningen die nodig zijn om een taak te voltooien. Dit veld is alleen zichtbaar als aan de volgende voorwaarden is voldaan:</p> 
     <ul> 
      <li> <p>De taak heeft een [!UICONTROL Simple Duration Type]. </p> <p><b>TIP</b></p> <p> Als u de taak bijwerkt [!UICONTROL Duration Type] bij elk ander type, wordt dit veld verborgen. </p> </li> 
      <li>De projectmanager heeft de [!UICONTROL Use Work Effort] taak automatisch berekenen [!UICONTROL Planned Hours] veld op het project. </li> 
     </ul> 
     <p>Voor informatie over het gebruik [!UICONTROL Work Effort] in plaats van [!UICONTROL Planned Hours] om de taakinspanning te ramen , zie <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Overzicht van de werkprestaties</a>. </p> 
     <p>U kunt dit veld weergeven in taakrapporten en lijsten.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Work Item]</td> 
   <td> <p>In dit veld wordt verwezen naar taken of problemen in [!DNL Workfront]. </p> <p>De [!UICONTROL Work Item] het rapport toont informatie voor zowel taken als kwesties. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management mix]</td> 
   <td>A [!UICONTROL Work Performance Indicator] (WPI) van het deel van het werk dat wordt toegewezen om uw zaken in werking te stellen tegenover verandering uw zaken. Met Mix WPI kunt u op organisatorisch niveau begrijpen of er op uw strategie een werkelijke werktoewijzing is toegepast.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Resource]</td> 
   <td>Een aanwijzing van een persoon in het systeem die in aanmerking komt voor werk of tracktijd.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Role and Responsibilities]</td> 
   <td>De eigenaars en belanghebbenden definiëren voor het beheer van het bereik, de uitvoering en de goedkeuringen van de aangewezen uitgave, taak, project, programma of portfolio.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management SLA]</td> 
   <td>Een kwantificeerbare maatstaf waarover alle belanghebbenden overeenstemming hebben bereikt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Stakeholder]</td> 
   <td>Een verzameling gebruikers met een gevestigd belang in de resultaten van een werkverzoek.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management touchpoints]</td> 
   <td>Gedigitaliseerde verslagen van communicatie tussen belanghebbenden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Performance Indicators] </td> 
   <td> <p>Mix-verhouding, capaciteit, snelheid, kwaliteit en betrokkenheid.</p> <p>WPI is een gemeenschappelijk acroniem voor [!UICONTROL Work Performance Indicator].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Process]</td> 
   <td> <p>De methode waarin het werk wordt ontvangen, voorrang gegeven, en uitgevoerd. De manier waarop u het werk uitvoert wordt typisch genoemd "het werkschema"of "projectplan"(een lijst van taken met data, voorgangersverhoudingen, etc.). </p> <p>Voorbeelden van een werkproces kunnen de productie van één enkel actief of de levering van een campagne met meerdere activa zijn. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Workflow template]</td> 
   <td>In de [!UICONTROL Proof Approval] rapport, toont dit gebied om het even welke werkschemamalplaatjes in bijlage aan een proef. Als er geen sjablonen zijn gekoppeld, is de kolom leeg.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Work Time]</td> 
   <td>

<p>Vertegenwoordigt het percentage van het Voltijdequivalent ([!UICONTROL FTE]) tijd dat de gebruiker beschikbaar is voor daadwerkelijk werk, exclusief overhead. [!UICONTROL Work Time] moet een decimaal getal zijn tot en met 1, en mag niet 0 zijn. Een beschikbaarheid van 20% voor werkelijk werk zou bijvoorbeeld 0,2 zijn.</p>
   </p>De standaardinstelling van het veld is 1. Dit geeft aan dat een gebruiker de gehele waarde doorgeeft [!UICONTROL FTE] op concrete, projectgerelateerde werkzaamheden.  </p>
   <p>Het systeem gebruikt dit aantal om de beschikbaarheid van de gebruiker voor daadwerkelijke, op project betrekking hebbende werk te berekenen. </p>
   <p> De uitzonderingen van het programma en de onderbreking van het programma zouden ook de gebruikerscapaciteit kunnen beïnvloeden. </p>
   <p>Voor meer informatie over het maken van planningen in Workfront raadpleegt u <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">Een schema maken</a>. </p>
    <p>Workfront berekent de beschikbaarheid van een gebruiker op basis van de voorkeuren voor het beheer van bronnen in het dialoogvenster [!UICONTROL Setup] gebied. Zie voor meer informatie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">Voorkeuren voor beheer van bronnen configureren</a>. </p> 
   <p>U kunt de [!UICONTROL Work Time] van een gebruiker wanneer u de gebruiker bewerkt of maakt. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">Gebruikersprofiel bewerken</a></p> 
   <b>TIP</b> 
   <p>Stel de [!UICONTROL Work Time] waarde aan 1 om erop te wijzen dat de gebruiker voor project-verwant werk hun volledig-tijdequivalent beschikbaar is.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Working time]</td> 
   <td>In de documentatie van Workfront, wordt deze term gebruikt om de tijd te beschrijven die aan het werk, volgens een programma wordt toegewezen.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>In een project, een taak, of een uitgeven rapport, die de volgende verklaring op tekstwijze gebruikt toont het aantal Geplande Uren van het project, de taak, of de kwestie die door het woord "Uren"wordt gevolgd:</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>Zie voor informatie over het gebruik van de tekstmodus <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Overzicht van syntaxis in tekstmodus</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
