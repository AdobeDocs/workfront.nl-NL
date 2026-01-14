---
content-type: reference
navigation-topic: workfront-navigation
title: Verklarende woordenlijst van  [!DNL Adobe Workfront]  terminologie
description: De  [!DNL Adobe Workfront]  verklarende woordenlijst lijsten algemeen gebruikte termijnen in  [!DNL Adobe Workfront]. You can use the glossary when you want to find the definition of concepts you see in the [!UICONTROL Workfront]  interface, rapporten, of u probeert om de betekenis van  [!DNL Workfront]  concepten te begrijpen die in de  [!DNL Workfront]  documentatie worden bepaald.
author: Alina
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 8f7249e08268a8cb784d4c0ecc8c534542fa80cf
workflow-type: tm+mt
source-wordcount: '17893'
ht-degree: 0%

---


# Verklarende woordenlijst van de terminologie van [!DNL Adobe Workfront]

<!--Audited: 12/2023-->

>[!IMPORTANT]
>
>Dit artikel moet worden gebruikt als een verwijzing naar de termen die u kunt tegenkomen in de [!DNL Adobe Workfront] -toepassing, in de [!DNL Workfront] -documentatie of wanneer u het over het algemeen hebt over het plannen en beheren van werk. Deze gegevens worden momenteel bijgewerkt, waardoor deze tabel wellicht niet volledig is. We zullen deze disclaimer wegnemen wanneer we deze informatie volledig vinden.

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
   <td>In [!DNL Workfront Goals] is een activiteit een voortgangsindicator voor een doel. Dit kan een voortgangsbalk zijn die u handmatig bijwerkt of een project dat aan het doel is gekoppeld. U kunt geen activiteiten weergeven in een rapport en u hebt geen toegang tot deze activiteiten via de API van [!DNL Workfront] . Voor informatie over activiteiten, zie <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref"> begonnen worden met resultaten en activiteiten in de Doelen van Adobe Workfront </a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Cost]</td> 
   <td> <p>Voor taken en kwesties, is dit de kosten verbonden aan de daadwerkelijke die uren met betrekking tot de Kosten per uurtarief van het middel worden geregistreerd aan de taak of de kwestie worden toegewezen. Voor projecten is dit een totaal van alle [!UICONTROL Actual Costs] taken en problemen in het project. Voor informatie, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref"> kosten van het Spoor </a>.</p>

<p>[!UICONTROL Actual Cost] berekeningen houden rekening met [!UICONTROL Legacy Actual Hours] . Voor informatie, zie "[!UICONTROL Actual Hours]"of "[!UICONTROL Legacy Actual Hours]"in deze lijst. </p>   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Expense Cost]</td> 
   <td> <p>De som van [!UICONTROL Actual Amounts] voor alle uitgaven die voor een project of een taak worden geregistreerd.</p> <b> VOORBEELD </b>
   <p>Als u een uitgave voor Taak 1 creeert en $600.00 op het [!UICONTROL Actual Amount] gebied ingaat, is [!UICONTROL Actual Expense Cost] voor deze taak $600.00. </p> 
   <p>Voor een project gebruikt [!DNL Workfront] de volgende formule om te berekenen [!UICONTROL Actual Expense Cost] :</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Actual Hours]</td> 
   <td> <p>In een project, een taak, of een probleemrapport, [!UICONTROL Actual Hours] is de som alle uren het programma geopend op het project, de taak, of de kwestie na Mei 2021.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b> Voorbeeld: </b></span></span> Als van het [!UICONTROL Updates] lusje voor Taak 1, u "Tijd van het Logboek"klikt en 25 uren ingaat, de Werkelijke Uren van Taak 1 = 25 uren. </p> <p>[!DNL Workfront] berekent [!UICONTROL Actual Hours] voor bovenliggende taken of projecten met de volgende formules:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project + [!UICONTROL Actual Hours] logged on issues in the project</code>  </p> </li> 
    </ul> 
   <p>Zie ook <strong>[!UICONTROL Legacy Actual Hours]</strong> .
    <p>Voor meer informatie, zie <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md"> Ware Uren van de Mening </a>.</p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Labor Cost]</td> 
   <td> <p>De [!UICONTROL Actual Cost] die gekoppeld is aan de arbeid die in een taak of project wordt geïnvesteerd. </p> <p>Voor een taak berekent [!DNL Workfront] de [!UICONTROL Actual Labor Cost] met behulp van de volgende formule:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>Als de taak een [!UICONTROL Cost Type] van [!UICONTROL User Hourly] heeft, gebruikt [!DNL Workfront] de gebruikerstarief. Als de taak een [!UICONTROL Cost Type] van [!UICONTROL Role Hourly] heeft, gebruikt [!DNL Workfront] de taakrolsnelheid om te berekenen [!UICONTROL Actual Labor Cost] . </p> <p>Voor een project gebruikt [!DNL Workfront] de volgende formule om [!UICONTROL Actual Labor Cost] te berekenen:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>Voor meer informatie, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref"> kosten van het Spoor </a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b> Voorbeeld: </b></span></span> bijvoorbeeld, als een gebruiker 5 uren voor een taak met a [!UICONTROL User Hourly] [!UICONTROL Cost Type] het programma opent en hun uurtarief $100 is, is [!UICONTROL Actual Labor Cost] $500.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Revenue] </td> 
   <td> <p>De waarde [!UICONTROL Actual Revenue] van een project of taak is de hoeveelheid geld die is gekoppeld aan de [!UICONTROL Actual Hours] van het project of de taak. </p> <p>Voor informatie over het volgen van opbrengst in [!DNL Workfront], zie <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref"> Overzicht van Facturering en Ontvangsten </a>. </p> </td> 
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
   <td>Verschillend van een traditioneel team omdat ze hun toekomstige werk van een achterstand nemen en er binnen een bepaalde periode aan werken die een [!UICONTROL Iteration] wordt genoemd.</td> 
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
    </ul> <p>Voor een <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL Project (Financial Data)] rapport: </p> 
    <ul> 
     <li>Stel dit rapport samen wanneer u probeert te begrijpen hoeveel <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> aan uw bronnen is toegewezen. [!UICONTROL Planned Hours]</li> 
     <li> <p>[!UICONTROL Allocation Date] is de eerste dag (zondag) van een week waarin de toewijzing van een [!UICONTROL Job Role] aan een taak begint. Een resource ([!UICONTROL Job Role]) kan net zoveel [!UICONTROL Allocation Dates] hebben als weken tijdens [!UICONTROL Duration] van de taken waaraan deze is toegewezen. Als taken zich over meerdere maanden uitstrekken, kan de eerste dag van een maand ook een [!UICONTROL Allocation Date] worden, als deze binnen de [!UICONTROL Duration] van de taak valt.</p> <p>U kunt bijvoorbeeld een [!UICONTROL Job Role] toewijzen aan een taak die zich over 3 weken uitstrekt en die 90 [!UICONTROL Planned Hours] heeft. Deze uren worden gelijkmatig verdeeld tijdens de duur van de taak, die elke dag 6 [!UICONTROL Planned Hours] aan uw baanrol toewijst:</p> <p><em> [!UICONTROL Daily Planned Hours] = [!UICONTROL Total Planned Hours]/ Aantal [!UICONTROL Work Days] tijdens [!UICONTROL Duration] van de taak </em> </p> <p>Dit heeft tot gevolg dat er drie [!UICONTROL Allocation Dates] zijn, één voor elke zondag van elke week tijdens [!UICONTROL Duration] van de taak, elk met een bepaald aantal [!UICONTROL Planned Hours] dat eraan is gekoppeld.<br> als de taak in het midden van de laatste week van een maand begint en twee weken na het begin van een nieuwe maand beëindigt, zal de taak vier [!UICONTROL Allocation Dates] hebben: voor elke Zondag van elke week tijdens [!UICONTROL Duration] van de taak, en voor de eerste dag van de nieuwe maand.</p> <p>Als u deze informatie optimaal wilt gebruiken, raden we u aan een <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> Project (Financial Data)-rapport op te stellen en een matrix-groepering voor [!UICONTROL Allocation Date] toe te voegen. Vervolgens groepeert u de resultaten wekelijks, maandelijks, driemaandelijks of jaarlijks voor de meest nauwkeurige gegevens.<br> voor informatie over de bouw van een matrixgroepering, zie het artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref"> een matrixrapport </a> creëren.</p> </li> 
    </ul> <p>Financiële informatie wordt alleen in [!UICONTROL Project (Financial Data)] -rapporten ingevuld als de bijbehorende gegevens jonger zijn dan 5 jaar. Als bijvoorbeeld in januari 2015 een functie werd toegewezen aan een taak en vandaag september 2021, wordt een financieel veld als [!UICONTROL Allocation Date] voor de functie niet ingevuld in het [!UICONTROL Project (Financial Data)] -rapport. </p> 
    <div> 
     <p>Voor een [!UICONTROL Budgeted Hour] -rapport:</p> 
     <ul> 
      <li>Bouw dit rapport samen wanneer u probeert te begrijpen hoeveel [!UICONTROL Budgeted Hours] is toegewezen aan uw bronnen of aan uw projecten in de functie voor middelenplanning.</li> 
      <li> <p>De [!UICONTROL Allocation Date] is de eerste dag (een zondag) van de week waarvoor u de uren in de [!UICONTROL Resource Planner] in de begroting hebt opgenomen. </p> <p><b>TIP</b></p> <p>Als een week zich over twee maanden uitstrekt, zal het twee rijen in het rapport produceren: één die aan de eerste dag van de week (Zondag van de eerste week die tijdens de eerste maand is) beantwoordt, en de tweede rij toont de eerste dag van de tweede maand. </p> <p>Als u bijvoorbeeld 8 uur begroot voor een gebruiker voor de week van 30 juni (zondag) - 6 juli (zaterdag), wordt in de twee rijen een [!UICONTROL Allocation Date] van 30 juni en 1 juli weergegeven. </p> </p> <p>Voor informatie over het opnemen van middelen in [!DNL Resource Planner], zie de middelen van de artikel <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref"> Begroting in [!DNL Resource Planner] gebruikend [!UICONTROL Project] en [!UICONTROL Role] meningen </a>.</p> <p>Voor informatie over de bouw van a [!UICONTROL Budgeted Hour] rapport, zie <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref"> Rapport: Beoogde Uur </a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Announcements]</td> 
   <td> <p>Een manier om met gebruikersinformatie binnen het systeem te communiceren. Deze informatie komt vaak van [!DNL Workfront] aan de Beheerder of van de Beheerder aan de gebruiker. </p> <p>Voor meer informatie, zie <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref"> aankondigingen </a> verzenden</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL App Integration]</td> 
   <td>Een toepassing vertegenwoordigt doorgaans een aansluiting op een softwaretoepassing, maar kan ook speciale functies vertegenwoordigen die gegevens manipuleren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver Decision]</td> 
   <td> <p>In het [!UICONTROL Proof Approval] -rapport worden in dit veld goedkeuringsbesluiten voor proefdrukken weergegeven die niet meer actief zijn.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver stage]</td> 
   <td>In het [!UICONTROL Proof Approval report] veld wordt informatie over een proefdruk van het huidige werkgebied weergegeven.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval]</td> 
   <td> <p>Een bepaald het werkpunt, zoals een taak, een document, of een timesheet, kunnen vereisen dat een supervisor of een andere gebruiker weg op het het werkpunt ondertekent. Dit proces van het ondertekenen van weg wordt genoemd goedkeuring. </p> <p>Voor meer informatie, zie <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref"> overzicht van het proces van de Goedkeuring </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval date]</td> 
   <td>In het [!UICONTROL Proof Approval] -rapport wordt in dit veld de datum weergegeven waarop een proefdruk is goedgekeurd.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver]</td> 
   <td>Een gebruiker of baanrol die op een bepaald het werkpunt moet ondertekenen, of de gebruiker die uuringangen op timesheets goedkeurt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assigned To]</td> 
   <td> <p>In een [!UICONTROL Task or Issue] -rapport wordt in dit veld de eigenaar van de taak of het probleem of de [!UICONTROL Primary Assignee] weergegeven. U kunt ook filteren of groeperen op dit veld.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment]</td> 
   <td>Een gebruiker, taakrol of team die is toegewezen aan een uitgave of een taak. Projecten, portfolio's of programma's kunnen geen toewijzingen hebben.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignments]</td> 
   <td> <p>In een [!UICONTROL Task] - of [!UICONTROL Issue] -rapport wordt in dit veld een lijst weergegeven met alle entiteiten (gebruikers, taakrollen, teams) die aan de taak of uitgave zijn toegewezen. U kunt filteren op dit veld met de velden [!UICONTROL Assignment Users] en [!UICONTROL Assignment Roles] . U kunt filteren door het team dat aan de taak of kwestie wordt toegewezen gebruikend het gebied van het Team. U kunt een rapport niet groeperen door dit gebied.</p> <p>Werkitems die in de [!UICONTROL Recycle Bin] zijn geplaatst, worden ook in bepaalde rapporten weergegeven die naar het [!UICONTROL Assignment] -object verwijzen waar een filtermodifier [!DNL OR] wordt gebruikt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Roles]</td> 
   <td>
   <p>In een [!UICONTROL Task] - of [!UICONTROL Issue] -rapport wordt in dit veld informatie weergegeven over de taakrollen die zijn toegewezen aan de taken of problemen. In dit veld wordt [!UICONTROL Primary Owners] weergegeven, evenals andere taakrollen die zijn toegewezen aan taken of problemen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Status]</td> 
   <td> <p>In een taak-, taak- of uitgifterapport geeft [!UICONTROL Assignment Status] aan of de gebruikers die aan een werkitem zijn toegewezen op de knop [!UICONTROL Work On It] of [!UICONTROL Done] hebben geklikt om het werk te accepteren of te voltooien. Het volgende [!UICONTROL Assignment Statuses] bestaat:</p> 
    <ul> 
     <li><b>[!UICONTROL Requested]</b>: de gebruiker is toegewezen aan de taak of uitgave, maar heeft nog niet op de knop [!UICONTROL Work On It] geklikt om eraan te werken.</li> 
     <li><b>[!UICONTROL Working]</b>: de gebruiker heeft op de knop [!UICONTROL Work On It] geklikt en werkt momenteel aan het item. </li> 
     <li><b>[!UICONTROL Done]</b>: de gebruiker heeft op de knop [!UICONTROL Done] geklikt en de bewerking voor het item voltooid. </li> 
    </ul> <p>Zie <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[!UICONTROL Work On It] en [!UICONTROL Done] knopoverzicht </a> voor meer informatie. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Teams]</td> 
   <td>
   <p>In een [!UICONTROL task] - of [!UICONTROL issue] -rapport wordt in dit veld informatie weergegeven over de teams die zijn toegewezen aan de taken of problemen. Het veld wordt weergegeven [!UICONTROL Primary Owners] en andere teams die zijn toegewezen aan taken of problemen. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Users]</td> 
   <td>
   <p>In een [!UICONTROL Task] - of [!UICONTROL Issue] -rapport wordt in dit veld informatie weergegeven over de gebruikers die zijn toegewezen aan de taken of problemen. In dit veld wordt [!UICONTROL Primary Owners] weergegeven, evenals andere gebruikers die zijn toegewezen aan taken of problemen. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attribute]</td> 
   <td>Een kenmerk is een eigenschap van een [!DNL Workfront] -object.</td> 
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
   <td>De inzameling van nota's automatisch die door gebeurtenissen worden geproduceerd die door de Opgenomen Veranderingen ([!UICONTROL Audit Areas]) worden gevolgd. Elke notitie registreert wie de actie heeft uitgevoerd, wat ze hebben gedaan en wanneer ze het hebben gedaan.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automatic And On Change]</td> 
   <td> <p>Een van de [!UICONTROL Project Update] -typen. Dit zal de Geprojecteerde en Geplande chronologie van het Project opnieuw berekenen wanneer het niight herberekeningsproces loopt en wanneer om het even welke update aan het project of de taken binnen het Project wordt gemaakt. </p> <p>Voor meer informatie, zie <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref"> het Type van projectupdate selecteren </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>Beschikbaarheid</p></td> 
   <td> <p>Deze termijn wordt gebruikt met betrekking tot "gebruikersbeschikbaarheid"of "middelbeschikbaarheid"en het illustreert de hoeveelheid tijd dat het middel (gebruiker of baanrol) beschikbaar is om te werken. </p> 
   <p>Workfront berekent de beschikbaarheid van gebruikers in verschillende velden en afhankelijk van de instellingen van de voorkeuren voor het beheer van bronnen in uw systeem. Voor meer informatie, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md"> de voorkeur van het Beheer van het Middel </a> vormen. </p>
   <p>Voor meer informatie over middelbeschikbaarheid, zie <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md"> begonnen worden met het Beheer van het Middel </a></p>
   Afwisselend, wordt de "capaciteit"ook gebruikt om naar middelbeschikbaarheid te verwijzen. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Automatic Only]</td> 
   <td> <p>Een van de [!UICONTROL Project Update] -typen. Hiermee worden de geprojecteerde en geplande tijdlijnen opnieuw berekend wanneer het nibleke herberekeningsproces wordt uitgevoerd.</p> <p>Voor meer informatie, zie <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref"> het Type van projectupdate </a> selecteren.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>"Zaken zoals gebruikelijk"werk dat aan het runnen van de dagelijkse primaire bedrijfsdoelstellingen bijdraagt.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Backlog]</td> 
   <td>Het gebied in een flexibel milieu waar nieuwe kwesties worden bewaard tot zij klaar zijn om aan te worden gewerkt.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Baseline]</td> 
   <td>Een bron van gegevens om herhalingen tegen in een milieu van het Agile te meten.</td> 
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
   <p>Voor meer informatie over het merken van een uitgave als factureerbaar, zie <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md"> projectuitgaven beheren </a>.</p>
   </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Billing Record]</td> 
   <td> <p>Registreert de inkomsten, uren, of uitgaven die kunnen worden gefactureerd. Deze informatie kan worden gebruikt om facturen op te stellen in een extern boekhoudsysteem.</p> <p>Voor meer informatie, zie <a href="../../../manage-work/projects/project-finances/create-billing-records.md"> het factureren verslagen </a> creëren. </p> 
   </td> 
  </tr>

<tr> 
   <td>Status van factureringsrecord</td> 
   <td> <p>In een factureringsrecord of een urenrapport geeft de status van een factureringsrecord aan of de factureringsrecord al dan niet is gefactureerd. U kunt een project niet verwijderen of tijd bewerken die aan een factureringsrecord is gekoppeld. Voor meer informatie, zie <a href="../../../manage-work/projects/project-finances/create-billing-records.md" > het factureren verslagen </a> creëren.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Branding]</td> 
   <td><p>Het aanpassen van [!DNL Workfront] om de interface een verschijning te geven die uw bedrijf door uw kleuren en logo's weerspiegelt te gebruiken.</p><p><strong> NOTA </strong><br> als uw organisatie aan [!DNL Adobe Experience Cloud] is genegeerd, is het brandmerken niet beschikbaar.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Breadcrumbs]</td> 
   <td> <p>Het gebied boven aan de pagina dat de hiërarchische locatie aangeeft van de locatie van de gebruiker in de toepassing.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Voor meer informatie, zie <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref"> Overzicht van Broodkruimels </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budget Status]</td> 
   <td> <p>Dit is een verouderd veld. Alle informatie die in dit veld wordt weergegeven, is gerelateerd aan een functie die door [!DNL Workfront] is verwijderd en het veld kan niet worden bijgewerkt. </p> <p>In dit veld wordt aangegeven of het project aan de [!UICONTROL Capacity Planner] is toegevoegd en of de budgetberekening voor het project is voltooid. [!UICONTROL Capacity Planner] is verwijderd uit [!DNL Workfront] . </p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is  not added to the capacity planner, its value is <i>Not Included</i>.  </li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is  added to the Capacity Planner but is excluded from the budget calculation,  the value is <i>Included but not Calculated</i>.  </li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is  added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Breakdown]</td> 
   <td> <p>In de Planning van Workfront, kunt u verbonden verslagen in de chronologiemening van een verslag tonen door de eigenschap van de Onderbreking te gebruiken. </p>
   <p>Door records op te delen op basis van hun verbindingen kunt u de tijdlijnen van andere verbonden records weergeven en begrijpen hoe deze de prestaties en deadlines van uw records kunnen beïnvloeden. </p>
   <p>Verbonden records worden onder hun respectievelijke record genest weergegeven. </p>
   <p>Voor informatie, zie <a href="/help/quicksilver/planning/views/manage-the-timeline-view.md"> de chronologiemening </a> leiden. </p>
   </td> 
    </tr>

<tr> 
   <td>[!UICONTROL Budgeted Completion Date]</td> 
   <td> <p>Dit is een verouderd veld. Alle informatie die in dit veld wordt weergegeven, is gerelateerd aan een functie die door [!DNL Workfront] is verwijderd. Dit veld kan niet worden bijgewerkt. </p>
   <p> Dit veld is nog steeds zichtbaar in [!UICONTROL project] -rapporten en -lijsten.</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgeted Cost]</td>

<td> <p>Dit zijn de kosten verbonden aan het begroten van middelen voor een project. </p>
   <p>Het veld wordt weergegeven in de volgende gebieden van [!DNL Workfront] onder de volgende namen:</p>
   <ul>
   <li><strong>[!UICONTROL Budgeted Cost]</strong>: in het deelvenster [!UICONTROL Business Case Summary]</li>
   <li><strong>[!UICONTROL Cost]</strong>: in de [!UICONTROL Utilization] -gebieden als u informatie bekijkt op [!UICONTROL Cost]</li>
   <li><strong>[!UICONTROL Project Budgeted Cost]</strong>: in lijsten en rapporten</li>
   </ul>   
    <p>[!UICONTROL Budgeted Cost] voor het project wordt berekend met behulp van de volgende formule:</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>Voor meer informatie over het berekenen van [!UICONTROL Budgeted Cost] en om diverse namen voor dit concept in [!DNL Workfront] te begrijpen, zie <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref"> Gemaakte Kosten van het Project berekenen </a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Budgeted Hours]</td> 
   <td> <p>De uren die zijn begroot voor de middelen voor het werk dat zij aan projecten moeten voltooien. Dit veld verwijst naar de uren die zijn begroot in het [!UICONTROL Resource Budgeting] -gebied van [!UICONTROL Business Case] (of in het [!UICONTROL Resource Planner] ) voor het project of voor de projectbronnen.</p> <p>Voor meer informatie, zie <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref"> Begrijp [!UICONTROL Budgeted Labor Cost] en [!UICONTROL Budgeted Hours] voor projecten </a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> Voor informatie over het in de begroting opnemen van Gebruikers in [!DNL Resource Planner], zie de artikel <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref"> middelen van de Begroting in [!DNL Resource Planner] gebruikend [!UICONTROL Project] en [!UICONTROL Role] meningen </a>. </p> 
    <p>De uren die in het [!UICONTROL Resource Budgeting] gebied van [!UICONTROL Business Case] of [!UICONTROL Resource Planner] worden begroot tonen in de volgende gebieden van [!DNL Workfront] en onder de volgende namen:</p> 
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
        <td> <p>Gebruiksrapport [!UICONTROL Hours] weergave</p> <p>Voor meer informatie over het [!UICONTROL Utilization] rapport, zie het artikel <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref"> Overzicht van het [!UICONTROL Resource Utilization] rapport </a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. Hours]</td> 
        <td> <p>[!UICONTROL Budgeted Hour] verslag</p><p>Het [!UICONTROL Budgeted Hour] -object in het rapport Boedgeted Hour verwijst naar informatie met betrekking tot een afgekeurd hulpmiddel voor middelenbeheer. Alleen het veld "[!UICONTROL Bud. Hours]" in dit rapport verwijst naar de in de begroting opgenomen uren in het [!UICONTROL Resource Planner] - of [!UICONTROL Resource Budgeting] -gebied van het project [!UICONTROL Business Case] . </p> <p>Voor meer informatie over het creëren van een rapport, zie het artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref"> een douanerapport </a> creëren.</p> </td> 
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
         <p>Voor meer informatie over het creëren van een rapport, zie het artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref"> een douanerapport </a> creëren.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>Elke andere vermelding van [!UICONTROL Budgeted Hours] in [!DNL Adobe Workfront] verwijst naar uren die in de begroting zijn opgenomen met vervangen functies die uit Workfront zijn verwijderd. Dit zijn alleen-weergeven velden en werken niet bij met de huidige informatie wanneer u de huidige bronnen in de begroting opneemt. </p>
    <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the  Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy  Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy  Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial  Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task  report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul> --> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgeted Labor Cost]</td> 
   <td> <p>Dit is de kosten verbonden aan de uren die u, als Manager van het Middel, begroting voor uw baanrollen voor het werk dat zij aan projecten moeten voltooien. </p> <p>[!UICONTROL Budgeted Labor Cost] in een projectrapport wordt berekend gebruikend de volgende formule:</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>Dit veld kan naar het volgende verwijzen:</p> 
    <ul> 
     <li> <p>De arbeidskosten die in [!UICONTROL Resource Budgeting] gebied van [!UICONTROL Business Case] of in [!UICONTROL Resource Planner] worden getoond die met de kosten van baanrollen op een project worden geassocieerd. Zie het artikel [!UICONTROL Budgeted Labor Cost] en <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL Understand Budgeted Labor Cost] voor projecten [!UICONTROL Budgeted Hours] voor informatie over het berekenen van de </a> .</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>De arbeidskosten die worden weergegeven in het [!UICONTROL Resource Budgeting] -gebied van [!UICONTROL Business Case] en die de [!UICONTROL People Costs] weerspiegelen die worden geschat in een initiatief dat is gekoppeld aan het project van [!DNL Scenario Planner] wanneer u de Scenario-planner gebruikt om uw projectmiddelen te begroten. Voor informatie over initiatieven, zie <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref"> Overzicht van Initiatieven in de Planner van het Scenario </a>. </p> <p>Voor [!DNL Scenario Planner] is een aanvullende licentie vereist. Voor informatie over [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref"> het [!DNL Scenario Planner] overzicht </a>. </p> </li> 
     <p>Deze wordt in de volgende gebieden onder de volgende namen weergegeven:</p>
   <ul>
   <li><strong>[!UICONTROL Budgeted Labor Cost]</strong>: in het [!UICONTROL Resource Budgeting] -gebied van [!UICONTROL Business Case] .
   <li><strong>[!UICONTROL Budgeted Cost]</strong>: in de weergave [!UICONTROL Utilization] report [!UICONTROL Cost]
   <p>Voor meer informatie, zie <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref"> de informatie van het middelgebruik van de Mening </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>: in de weergaven [!DNL Resource Planner] Project of [!DNL Role] , bij weergave op kosten
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>: in de volgende verslagen: 
   <ul>
    <li>[!UICONTROL Project] verslag</li>
    <li>[!UICONTROL Project (Financial Data)] verslag</li>
    <li>[!UICONTROL Task] verslag</li>
    <li>[!UICONTROL Issue] verslag</li>
    <li>[!UICONTROL Budgeted Hour] verslag</li> 
    </ul>
    <p>Voor meer informatie over het creëren van een rapport, zie het artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref"> een douanerapport </a> creëren.</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in  Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task  report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task  report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>  .  </p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Budgeted Start Date]</td> 
  <td> <p>Dit is een verouderd veld. Alle informatie die in dit veld wordt weergegeven, is gerelateerd aan een functie die door [!DNL Workfront] is verwijderd. Dit veld kan niet worden bijgewerkt.</p>
  <p>Deze gebieden zijn verwijderd uit [!DNL Workfront] . </p> 
  <p>Het veld is nog steeds zichtbaar in [!UICONTROL project] -rapporten en -lijsten.</p>
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
   <td> <p>Een hulpmiddel dat wordt gebruikt om te beoordelen of een project van de [!UICONTROL Idea] status aan de [!UICONTROL Planning] status vooruit zou moeten worden verplaatst. Met andere woorden, een [!UICONTROL business case] helpt de organisatie om te beslissen of het de moeite waard is om het project te lanceren en te voltooien of niet, vooral wanneer het vergelijken van projecten met anderen in een portefeuille.</p> <p>Zie <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref"> Een [!UICONTROL Business Case] project </a> maken voor meer informatie.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case Budgeted Hours]</td> 
   <td> <p>Dit is een verouderd veld. Alle informatie die in dit veld wordt weergegeven, is gerelateerd aan een functie die door [!DNL Workfront] is verwijderd. Dit veld kan niet worden bijgewerkt.</p> <p>Dit veld is nog steeds zichtbaar in project en [!UICONTROL task] lijsten en rapporten. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Assignment]</td> 
   <td> <p>Een van de taken [!UICONTROL Duration Types] . Hiermee wordt het percentage berekend van een 8-uurs werkdag dat de gebruiker die aan de taak is toegewezen, aan de taak zal worden toegewezen op basis van [!UICONTROL Duration] van de taak en [!UICONTROL Work Required] .</p> <p>Zie <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref"> Overzicht van Taak [!UICONTROL Duration] en [!UICONTROL Duration Type]</a> voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Work]</td> 
   <td> <p>Een van de taken [!UICONTROL Duration Types] . Dit zal [!UICONTROL Work Required] op een taak berekenen, gezien de [!UICONTROL Duration] en gebruiker [!UICONTROL Assignment] percentages (die op een 8-uurs het werkdag gebaseerd zijn).</p> <p>Zie <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref"> Overzicht van Taak [!UICONTROL Duration] en [!UICONTROL Duration Type]</a> voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar]</td> 
   <td> <p>In Workfront is een kalenderrapport een dynamisch rapport waarin gebruikers de datum en andere belangrijke details van een gebeurtenis kunnen bekijken, waaronder de vervaldatum, de status van het werk en de gebruiker aan wie de gebeurtenis is toegewezen.</p> <p> Voor meer informatie over kalenderrapporten, zie <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref"> overzicht van de rapporten van de Kalender </a>.</p>
   <p> In de Planning van Workfront, is een mening van de Kalender een type van mening voor een verslagtype dat verslagen op een kalender toont. U moet een extra licentie hebben om toegang te krijgen tot Workfront Planning. </p>
    </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Can Start]</td> 
   <td> <p>In dit veld wordt aangegeven of een taak gereed is om te worden bewerkt. Als het begin gereed is om te worden bewerkt in het veld [!UICONTROL Can Start] voor de taak, is dit ingesteld op [!UICONTROL True] . </p> <p>Voor meer informatie, zie <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">"[!UICONTROL Can Start] "overzicht voor taken </a>.</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    --> <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.  </li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.  </li> 
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
   <td>Een van de projecten [!UICONTROL Update Types] . Het werkt [!UICONTROL Project Projected] en [!UICONTROL Planned] slechts chronologie bij wanneer de Updates aan taken worden gemaakt of uitgeeft op het project of de taken worden uitgevoerd.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Order]</td> 
   <td> <p>Een van de [!UICONTROL Issue] -typen geeft meestal aan dat een ongeplande hoeveelheid werk moet worden uitgevoerd voordat het project kan worden voltooid.</p> <p>Voor meer informatie over [!UICONTROL Issue] types, zie de sectie "Standaard uitgeverstypes"in het artikel <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref"> aanpassen standaard uitgeverstypes </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Child Task]</td> 
   <td>Een taak die een [!UICONTROL Subtask] van a [!UICONTROL Parent Task] ([!UICONTROL Summary Task]) is.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Children]</td> 
   <td>De verzameling van [!UICONTROL Subtasks] naar een [!UICONTROL Parent Task] ([!UICONTROL Summary Task]).</td> 
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
   <td> <p>Een [!UICONTROL Company] is een organisatie-eenheid in [!DNL Workfront] . </p> 
   <p> U kunt een gebruiker of een project met één bedrijf associëren. Voor meer informatie, zie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md"> bedrijven </a> creëren en uitgeven.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion date]</td> 
   <td> <p>De datum waarop een project, een taak of een uitgave moet worden voltooid. Er zijn verschillende typen [!UICONTROL Completion dates] in [!DNL Workfront] :</p> 
    <ul> 
     <li>[!UICONTROL Actual Completion Date]. Zie <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref"> Overzicht van het project [!UICONTROL Actual Completion Date] </a> voor meer informatie.</li> 
     <li>[!UICONTROL Planned Completion Date]. Voor meer informatie, zie <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref"> Plaats het project [!UICONTROL Planned Completion Date]</a> en <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref"> Overzicht van de taak [!UICONTROL Planned Completion Date]</a>.</li> 
     <li>[!UICONTROL Projected Completion Date]. Voor meer informatie, zie <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref"> Overzicht van [!UICONTROL Projected Completion Date] voor projecten, taken, en kwesties </a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Day]</td> 
   <td>De dag, relatief ten opzichte van het begin van de [!UICONTROL Template] , dat een [!UICONTROL Template Task] of a [!UICONTROL Template] voltooid moet zijn.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Mode]</td> 
   <td> <p>Dit geeft aan hoe een project wordt gemarkeerd als [!UICONTROL Complete] . Deze kan twee waarden hebben:</p> 
    <ul> 
     <li>[!UICONTROL Manual]: Een gebruiker moet de projectstatus wijzigen in [!UICONTROL Complete] .</li> 
     <li>[!UICONTROL Automatic]: De status van het project wordt automatisch gewijzigd in [!UICONTROL Complete] wanneer alle taken in het project voor 100% zijn voltooid en alle problemen zijn gesloten.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition]</td> 
   <td> <p>Dit is een visuele weergave van de voortgang van een taak, kwestie of project.</p> <p>Voor projecten kan de voorwaarde handmatig worden ingesteld door de eigenaar van het project of automatisch worden ingesteld door [!DNL Workfront] , afhankelijk van de vorderingsstatus van het project. </p> <p>De mogelijke waarden voor de projectvoorwaarde zijn:</p> 
    <ul> 
     <li>[!UICONTROL On Target]</li> 
     <li>[!UICONTROL At Risk]</li> 
     <li>[!UICONTROL In Trouble]</li> 
    </ul> <p>Voor meer informatie over projectvoorwaarden, zie het artikel <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref"> Overzicht van [!UICONTROL Project Condition] en [!UICONTROL Condition Type]</a>.</p>
     <p>U kunt taak en uitgiftevoorwaarden met een aantal associëren dat in rapporten kan tonen. In de onderstaande lijsten staan de standaardnamen en -nummers voor taken en uitgaven. Uw systeembeheerder kan de namen van voorwaarden bijwerken en zij kunnen nieuwe voorwaarden met verschillende aantallen toevoegen. Nadat een getal aan een voorwaarde is gekoppeld, kan het niet worden bewerkt.  </p> 
     <p>Voor taken wordt de voorwaarde handmatig ingesteld door de eigenaar van de taak. De mogelijke waarden voor de taakvoorwaarde zijn:</p> 
    <ul> 
     <li>[!UICONTROL Going Smoothly] (0)<br></li> 
     <li> [!UICONTROL Some Concerns] (1)<br></li> 
     <li>[!UICONTROL Major Roadblocks] (2)</li> 
    </ul> <p>Voor meer informatie over taakvoorwaarden, zie de artikel <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref"> Update [!UICONTROL Condition] voor taken en kwesties </a>.</p> <p>Voor uitgaven wordt de voorwaarde handmatig ingesteld door de eigenaar van de uitgave. De mogelijke waarden voor de uitgiftevoorwaarde zijn:<br></p> 
    <ul> 
     <li>[!UICONTROL Going Smoothly] (0)<br></li> 
     <li>[!UICONTROL Some Concerns] (1)<br></li> 
     <li>[!UICONTROL Major Roadblocks] (2)</li> 
    </ul> 
   <p><b>OPMERKING</b></p>
    <p>Wanneer het veld [!UICONTROL Condition] wordt bijgehouden in [!UICONTROL Journal Entry] -rapporten, geven de [!UICONTROL New] en [!UICONTROL Old Number Values] het nummer weer dat aan de voorwaarde is gekoppeld in plaats van de naam ervan. Als een voorwaarde oorspronkelijk niet is gedefinieerd voor een taak of een uitgave en u deze later bijwerkt, wordt de [!UICONTROL Old Number Value] van het [!UICONTROL Condition] -veld weergegeven als -2.147.483.648. Zie ook "[!UICONTROL New Number Value]", "[!UICONTROL Old Number Value]", en "[!UICONTROL Journal Entry]"in dit artikel. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition Update]</td> 
   <td> <p>Dit gebied toont de huidige staat van taken, projecten of kwesties. Deze optie toont de meest recente updates die de eigenaars van taken, projecten of problemen hebben verstrekt op het [!UICONTROL Update Status] gebied, samen met de nieuwe voorwaarde.</p> <p>Opmerkingen die zijn gemaakt tijdens voorwaarde-updates worden niet weergegeven in de kolom [!UICONTROL Condition Update] . Alleen de hoofdupdate wordt weergegeven.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Connected record types]</td> 
   <td> <p>In de Planning van Workfront, kunt u een verbinding tussen één van het volgende tot stand brengen: </p>
   <ul>
   <li>Twee recordtypen</li>
   <li>Een recordtype en een Workfront-objecttype</li>
   <li>Een recordtype en een Adobe Experience Manager-element</li></ul>
   <p>Door recordtypen te verbinden, kunt u informatie van het ene record of objecttype weergeven op een ander recordtype.</p>
   <p>Voor informatie, zie <a href="/help/quicksilver/planning/architecture/connect-record-types-overview.md"> Verbonden verslagtypes overzicht </a>  </p>
  <p>Voor Workfront Planning is een extra licentie vereist. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Connected records]</td> 
   <td> <p>In de Planning van Workfront, nadat u twee verslagtypes verbindt, kunt u twee individuele verslagen van die types met elkaar verbinden.  </p>
   <p>Door records te verbinden, kunt u gegevens van een record of object vanuit een andere toepassing in een andere record weergeven.</p>
   <p>Voor informatie, zie <a href="/help/quicksilver/planning/records/connected-records-overview.md"> Verbonden verslagenoverzicht </a>. </p>

<p>Voor Workfront Planning is een extra licentie vereist. </p>
 </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Connections]</td> 
   <td> <p>In de Planning van Workfront, kunnen de verbindingen naar verbonden verslagtypes of verbonden verslagen verwijzen. Voor Workfront Planning is een extra licentie vereist.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Constraint Date]</td> 
   <td> <p>Als u een [!UICONTROL Task Constraint] gebruikt die is gekoppeld aan een bepaalde datum, zoals [!UICONTROL Must Start On] , wordt die specifieke datum de [!UICONTROL Constraint Date] van de taak.</p> <p>Met de volgende taakbeperkingen wordt het veld [!UICONTROL Constraint Date] bijgewerkt:</p> 
    <ul> 
     <li>[!UICONTROL Must Start On]</li> 
     <li>[!UICONTROL Must Finish On]</li> 
     <li>[!UICONTROL Start No Later Than]</li> 
     <li>[!UICONTROL Start No Earlier Than]</li> 
    </ul> <p><b>TIP</b></p>   
     <ul> 
      <li> <p>Een taak met een [!UICONTROL Constraint] van [!UICONTROL Fixed Dates] heeft geen [!UICONTROL Constraint Date] . </p> </li> 
      <li> <p> [!UICONTROL Constraint Date] kan alleen worden weergegeven in een rapport of aangepaste weergave.</p> </li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Day]</td> 
   <td> <p>Als u een Restrictie van de Taak in een malplaatjetaak gebruikt die aan een specifieke dag, zoals moet op beginnen is, dan wordt die specifieke dag de Dag van de Beperking van de malplaatjetaak.</p> <p>Met de volgende taakbeperkingen wordt het veld [!UICONTROL Constraint Day] bijgewerkt:</p> 
    <ul> 
     <li>[!UICONTROL Must Start On]</li> 
     <li>[!UICONTROL Must Finish On]</li> 
     <li>[!UICONTROL Start No Later Than]</li> 
     <li>[!UICONTROL Start No Earlier Than]</li> 
    </ul> <p><b>TIP</b></p> <p>  [!UICONTROL Constraint Day] kan alleen worden weergegeven in een rapport of aangepaste weergave. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Type]</td> 
   <td> <p>De planningsneiging van een taak. [!UICONTROL As Soon as Possible] plant bijvoorbeeld een taak die zo snel mogelijk moet beginnen en [!UICONTROL Finish No Later Than] plant een taak die door [!UICONTROL Constraint Date] moet worden voltooid, en niet later.</p> <p>Zie <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[!UICONTROL Task Constraint] overview </a> voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contextual Menu]</td> 
   <td>Een menu, dat zich aan de linkerkant van het scherm bevindt, waarop de items worden gewijzigd in de correlatie met de actieve inhoud. Wanneer een gebruiker bijvoorbeeld een project weergeeft, geeft de [!UICONTROL Contextual Menu] koppelingen weer naar projectgerelateerde informatie en gereedschappen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converted Issue Originator]</td> 
   <td>Een gebied in een project of taakrapport dat informatie over de gebruiker toont die [!UICONTROL Primary Contact] van een kwestie is wanneer de kwestie in een project of een taak wordt omgezet. Het veld wordt ook weergegeven in de sectie [!UICONTROL Project Details] waar de naam van de [!UICONTROL Primary Contact] -publicatie van de omgezette uitgave wordt weergegeven. Zie ook "[!UICONTROL Primary Contact]"in dit artikel.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Cost]</td> 
   <td> <p>Het geldbedrag dat u moet uitgeven wanneer het voltooien van een project, een taak, of een kwestie. </p> <p>U kunt diverse soorten kosten voor arbeid, uitgaven, risico's volgen die op het project betrekking hebben.Voor informatie over het volgen van kosten in [!DNL Workfront] zie <a href="../../../manage-work/projects/project-finances/track-costs.md"> de kosten van het Spoor </a>.</p> 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Cost Performance Index (CPI)]</td> 
   <td> <p>In [!UICONTROL Cost Performance Index (CPI)] wordt de relatie op project- of taakniveau beschreven tussen de geplande kosten en de werkelijke kosten. De Managers van het project herzien dit metrisch om taken of projecten te identificeren die momenteel onder of over kosten op een bepaald punt volgen. De kosten kunnen worden gemeten in uren of valuta, afhankelijk van uw [!UICONTROL Performance Index Method (PIM)].</p> 
    <p> Voor informatie, zie <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-cpi.md"> de Index van de Prestaties van de Kosten berekenen (CPI) </a>.</p>

</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Cost Schedule Performance Index (CSI)]</td> 
   <td> <p>[!UICONTROL Cost Schedule Performance Index (CSI)] is een automatische berekening die de [!UICONTROL Cost Performance Index (CPI)] en [!UICONTROL Schedule Performance Index (SPI)] in één algemene maatstaf combineert die kosten en schema in evenwicht brengt. Door deze waarden samen te vermenigvuldigen, kan één enkele metrisch een langdurig programma bij een lager budget of vice versa verklaren. De managers van het project kunnen dit gebruiken om algemene project of taakgezondheid te bepalen wanneer de kosten worden opgeofferd om planning midden-project te drijven.</p> 
    <p> Voor informatie, zie <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-csi.md"> de Index van de Prestaties van het Programma van de Kosten berekenen </a>.</p>
    </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Cost Type]</td> 
   <td>Voor een taak bepaalt [!UICONTROL Cost Type] hoe de taak kosten zal oplopen. Voorbeelden zijn [!UICONTROL Fixed Hourly] , [!UICONTROL User Hourly] en [!UICONTROL User Hourly plus Fixed] . </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cross-Project Dependencies]</td> 
   <td> <p>Een taak van één project is afhankelijk van een taak van een verschillend project.</p> <p>Voor meer informatie, zie <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref"> tot dwars-project predecessors </a> leiden.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custom Data]</td> 
   <td> <p>Gegevens die uniek zijn voor een organisatie. Organisaties kunnen de [!DNL Workfront] -toepassing aanpassen door aangepaste formulieren en aangepaste velden te maken. Deze douaneinformatie kan rapportering voor KPIs, controle, en vraagmengeling drijven. </p> <p>[!UICONTROL Custom Data] kan worden gekoppeld aan:</p> 
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
   <td>De optie om op te geven of een veld [!UICONTROL Custom Data] in de database wordt opgeslagen als Tekst, Datum, Getal of Valuta.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Display Type]</td> 
   <td>Het weergavetype van een aangepast veld. Voorbeelden zijn [!UICONTROL Drop-Down] , [!UICONTROL Text Field] , [!UICONTROL Text Area] , [!UICONTROL Radio Buttons] , enzovoort.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Field]</td> 
   <td>Voor de gegevens van de Douane die de gebruiker toestaan om uit verscheidene opties te selecteren, zijn dit de waarden waarvan een gebruiker kan selecteren. Aangepaste opties zijn alleen geldig voor [!UICONTROL Drop-Down] , [!UICONTROL Multi-Select Drop-Down] , [!UICONTROL Radio Buttons] en [!UICONTROL Checkboxes] .</td> 
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
   <td> <p> U kunt dit gebied in een rapport of een mening van het voorwerp van het Rapport toevoegen, om de dashboards te tonen waarop het rapport in een lijst wordt vermeld. </p> <p> U kunt dit veld gebruiken om te filteren op rapporten die ook op een specifiek dashboard worden weergegeven. </p> <p> Voor meer informatie over het omvatten van dashboardinformatie over rapportobjecten rapporten, zie "Begrijpen welke Rapporten op Dashboards"sectie in de artikel <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref"> Toegang worden vermeld en rapporten </a> organiseren</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data Type]</td> 
   <td>Zie "[!UICONTROL Custom Data Type]".</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Days Late]</td> 
   <td> <p>In dit veld wordt een datumverschil weergegeven tussen [!UICONTROL Planned Start] en [!UICONTROL Today] als [!UICONTROL Actual Completion Date] ontbreekt.</p> <p>Geeft ook een datumverschil weer tussen [!UICONTROL Actual Completion] en [!UICONTROL Planned Completion] , wanneer een [!UICONTROL Actual Completion Date] aanwezig is.</p> </td> 
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
   <td> <p>Het type van het plannen van verhouding tussen een taak en zijn voorganger(s). Een voorbeeld is [!UICONTROL Finish-Start] , waarvoor de eerste taak moet zijn voltooid voordat de tweede taak kan worden gestart.</p> <p>Voor meer informatie, zie <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref"> Overzicht van de types van taakgebiedsdeel </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document]</td> 
   <td>Elk bestand dat binnen [!DNL Workfront] aan een object is gekoppeld.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document Version]</td> 
   <td> <p>Telkens wanneer hetzelfde document naar hetzelfde object wordt geüpload, wordt er een versienummer aan toegewezen. Gebruikers kunnen verschillende opties voor een vorige versie van een document weergeven en wijzigen.</p> <p>Voor meer informatie, zie <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref"> documentversies beheren </a>.</p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Due Date]</td> 
   <td> <p>De datum waarop een taak of een kwestie moet worden voltooid. De vervaldatum van een taak of uitgifte is dezelfde datum als de geplande afsluitende datum.</p>
    <p>De taak en het Eind van de uitgave zijn zichtbaar in taak en geeft lijsten en rapporten uit.</p> 
    <p>Zie ook Geplande Voltooiingsdatum in deze tabel. 
    </td> 
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration]</td> 
   <td> <p>Het tijdsvenster dat is toegewezen voor het voltooien van een taakprobleem of project (zoals wordt bepaald door het aantal dagen tussen de [!UICONTROL Planned Start] en de geplande voltooiing).</p> 
    <ul> 
     <li>Voor taken, is de Duur een editable gebied als het Type van Duur van de taak niet Eenvoudig is. Als het Type van Duur van de taak Eenvoudig is, of als de Beperking van de Taak Vaste Datums is, is de Duur een berekening die door Workfront wordt uitgevoerd.</li> 
     <li>Voor kwesties, is de Duur altijd een editable gebied en het zou een schatting van een aantal dagen moeten vertegenwoordigen die de kwestie zouden vereisen om worden opgelost.</li> 
     <li>Voor projecten is de Duur een berekening die door [!DNL Workfront] wordt uitgevoerd en het vertegenwoordigt het verschil in dagen tussen het geplande Begin van de vroegste taak en [!UICONTROL Planned Completion] van de recentste taak op het project.</li> 
    </ul> <p>Voor meer informatie over het verschil tussen [!UICONTROL Duration] en [!UICONTROL Planned Duration] voor taken, zie het artikel <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md"> Verschil tussen [!UICONTROL Planned Duration] en [!UICONTROL Duration] voor taken </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration in Minutes]</td> 
   <td>In dit veld wordt dezelfde informatie weergegeven als in het veld [!UICONTROL Duration] in minuten in plaats van in dagen. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Duration per Occurrence]</td> 
   <td> <p>Dit wordt weergegeven in de vakken [!UICONTROL Task Details] en [!UICONTROL Edit Task] van een bovenliggende map van terugkerende taken. Het toont de duur van elke terugkomende taak. Voor informatie over het creëren van terugkomende taken, zie <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref"> terugkomende taken </a> creëren. </p> <p> <span> Duur die in individuele terugkomende taken wordt gewijzigd toont niet de waarde op dit gebied wordt vermeld.</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Duration Type]</td> 
   <td> <p>Een taakgebied dat erop wijst hoe het werk dat wordt vereist om de taak te voltooien aan de wijzers over de taakduur wordt toegewezen. Deze vertegenwoordigt de relatie tussen de [!UICONTROL Duration] van de taak, de [!UICONTROL Work Required] en de hoeveelheid tijd, of [!UICONTROL Allocation], dat de toegewezen bronnen aan de taak moeten besteden om de taak te voltooien. </p> <p>Dit veld wordt weergegeven op het tabblad [!UICONTROL Details] van een taak. </p> <p>De opties voor het Type van Duur van een taak zijn:</p> 
    <ul> 
     <li>[!UICONTROL Calculated assignment]</li> 
     <li>[!UICONTROL Calculated Work]</li> 
     <li>[!UICONTROL Effort Driven]</li> 
     <li>[!UICONTROL Simple]</li> 
    </ul> <p>Zie <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref"> Overzicht van Taak [!UICONTROL Duration] en [!UICONTROL Duration Type]</a> voor meer informatie.</p> 
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
   <td> <p>[!UICONTROL Elapsed time] is een tijdseenheid voor een taak [!UICONTROL Duration]. Dit is de tijd tussen de [!UICONTROL Planned Start Date] en de [!UICONTROL Planned Completion Date] van een taak die feestdagen, weekends en vrije tijd omvat. Met andere woorden, de verstreken tijd is de doorloop van kalenderdagen. </p> <p>[!DNL Workfront] ondersteunt de volgende verstreken tijdeenheden voor de taakduur:</p> 
    <ul> 
     <li> <p>[!UICONTROL Elapsed Minutes]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Hours]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Days]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Weeks]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Months]</p> </li> 
    </ul> <p>Voor meer informatie over taakduur, met inbegrip van verstreken tijd, zie <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref"> Overzicht van Taak [!UICONTROL Duration] en [!UICONTROL Duration Type]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL End Date]</td> 
   <td> <p> In een [!UICONTROL Rate] -rapport is dit de datum waarop een nieuwe factureringsfrequentie voor een taakrol op projectniveau eindigt. De uren verbonden aan het project die vóór deze datum zijn worden vermenigvuldigd met dit het factureringspercentage om de opbrengst op het project te berekenen. </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Engagement]</td> 
   <td>[!UICONTROL Work Performance Indicator] (WPI) die erop wijst wanneer het engagement en het geloof in de taak, het project, het team, of de organisatie verminderen. Dit geeft aan dat je moet optreden om dat geloof en engagement nieuw leven in te blazen. WPI zou worden gemeten door de eenvoudige vragen te stellen: "Heb je begrepen wat van je werd verwacht? Heeft het werk dat u hebt toegewezen een verschil gemaakt met de organisatie? Heb je geweldig werk gedaan?"</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Enterprise Goals]</td> 
   <td>Interfunctionele doelstellingen die tot de metriek van de bedrijfsdoelstellingen bijdragen.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Estimate at Completion]</td> 
   <td><p>Als metrische projectprestaties, vertegenwoordigt de Schatting bij Voltooiing (EAC) de verwachte totale kosten van uw project of taak wanneer het voltooit.</p>
   <p>Als project het plaatsen, staat het u toe om te bepalen hoe de waarde EAC zou moeten worden berekend.</p>
   <p>Voor informatie, zie <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-eac.md"> Schatting bij Voltooiing (EAC) berekenen </a>. </p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Estimated Due Date]</td> 
   <td>In project-, taak- en uitgifterapporten is de geschatte vervaldatum de datum waarop Workfront schat dat het item moet worden voltooid.</td> 
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
   <td> <p>Dit is doorgaans een licentietype of een gebruiker met een dergelijke licentie. Een gebruiker met een dergelijk licentietype kan alleen informatie in het systeem controleren. Zij kunnen niet actief aan het werk deelnemen.</p> <p>Zie <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] Overzicht van licenties </a> voor meer informatie.</p> </td> 
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

<p>Voor meer informatie, zie <a href="../../../wf-api/general/api-explorer.md"> API Ontdekkingsreiziger </a> en <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md"> Overzicht van de Wijze van de Tekst </a>.</p>

<p>Workfront wordt standaard geleverd met een set velden die zowel objecten als hun gegevens definiëren. U kunt ook aangepaste velden maken om objecten te definiëren, maar u kunt geen aangepaste objecten maken.</p>

<p>In Workfront Planning kunt u aangepaste velden maken voor alle recordtypen. Workfront-recordtypen bevatten een zeer beperkt aantal velden. U moet alle velden helemaal opnieuw maken en deze koppelen aan recordtypen. Voor informatie, zie <a href="/help/quicksilver/planning/fields/fields-overview.md"> overzicht van het Gebied </a>. </p> <p>Voor Workfront Planning is een extra licentie vereist. </p>   
  </tr>
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>Één van de belangrijkste bouwstenen van een rapport of een lijstelement dat bepaalt welke informatievertoningen op het scherm. Voor meer informatie over het melden van elementen, zie <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref"> Rapporterende elementen: filters, meningen, en groeperingen </a>.</p> <p>De filter bepaalt de resultaten die in een rapport of op een [!DNL Workfront] paneellijst, zoals projecten, taken, of kwesties tonen.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>Proces voor het beheren van de loonkosten, kosten en inkomstengegevens in [!DNL Workfront] .</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fixed Cost]</td> 
   <td>U kunt een vast bedrag van kosten voor een project bepalen. Dit maakt deel uit van [!UICONTROL Planned Cost] van het project dat het bedrag vertegenwoordigt dat u nodig hebt om het project te voltooien. Voor informatie over kosten, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref"> Kosten van het Spoor </a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fixed Revenue]</td> 
   <td>U kunt een vast bedrag van opbrengst voor een project bepalen. Dit maakt deel uit van [!UICONTROL Planned Revenue] van het project dat de hoeveelheid geld vertegenwoordigt die u zou kunnen verkrijgen als u het project voltooit. Voor informatie over opbrengst, zie <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref"> Overzicht van Facturering en Ontvangsten </a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Flags]</td> 
   <td> <p> Dit is hetzelfde veld als [!UICONTROL Status Icons] , maar het is alleen beschikbaar voor de volgende weergaven: </p> 
    <ul> 
     <li> [!UICONTROL Templates] </li> 
     <li> [!UICONTROL Expenses] </li> 
    </ul> <p> Voor meer informatie, zie de artikel <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref"> Ingebouwde Pictogrammen van de Status in Meningen </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>Mappen worden gebruikt om documenten of rapporten te ordenen die aan een object zijn gekoppeld.</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] (voltijdequivalent)</td> 
   <td>Dit is het Voltijdequivalent dat op de hoeveelheid tijd wijst dat een middel voor het werk beschikbaar is. 
   Het veld [!UICONTROL FTE] wordt weergegeven in de volgende gebieden: 
  <ul>
   <li> Gebruikersprofiel, bij het bewerken of maken van de gebruiker </li>
   <li> [!UICONTROL Resource Planner] </li>
   <li> [!UICONTROL Scenario Planner] (aanvullende licentie vereist voor de Workfront Scenario Planner) </li>
   <li> Gebruikerslijsten en -rapporten </li> </ul>

<p>De [!UICONTROL FTE] moet een decimaal getal tot en met 1 zijn en mag niet 0 zijn. </p>
   <p> Een [!UICONTROL FTE] van 1 (de standaardwaarde voor het [!UICONTROL FTE] -veld van een gebruiker, zoals gedefinieerd in het profiel van de gebruiker) betekent dat een resource (gebruiker of rol) het volledige aantal uren werkt, op basis van het schema dat de beschikbaarheid ervan berekent. </p>
   <p>Uw Workfront-beheerder bepaalt welk schema wordt gebruikt om de beschikbaarheid van de gebruiker te bepalen.  </p>
   <ul>
   <li> Wanneer [!UICONTROL Default Schedule] wordt gebruikt, gebruikt Workfront [!UICONTROL FTE] van de gebruiker in hun profiel om beschikbaarheid te berekenen. </li>
   <li> Wanneer het Programma van de Gebruiker wordt gebruikt, gebruikt Workfront de tijd van de gebruiker weg, [!UICONTROL Work Time] waarde, en [!UICONTROL Default Schedule] uren om de gebruiker te berekenen [!UICONTROL FTE]. </li> </ul>

<p>Voor meer informatie, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md"> de voorkeur van het Beheer van het Middel </a> vormen.  </p>
   <p>Voor meer informatie over het creëren van programma's in [!DNL Workfront], zie <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md"> een programma </a> creëren. </p>

<p><b>OPMERKING</b></p>
   <p>Voor alle berekeningen in [!UICONTROL Scenario Planner] gebruikt Workfront de volgende waarde: 1 [!UICONTROL FTE] = 8 uur.</p>
   <p>Voor meer informatie, zie <a href="../../../scenario-planner/get-started-with-scenario-planning.md"> begonnen worden met [!UICONTROL Scenario Planner]</a>. </p>
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
   <td><p>Er zijn twee concepten van doelen in [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b> de doelstellingen van het Project </b>: Een reeks bedrijfsdoelstellingen die door de relevante belanghebbenden van een project worden goedgekeurd. De doelstellingen van het project maken deel uit van het BedrijfsGeval van een project. </p> <p>U kunt projectdoelstellingen niet in lijsten of rapporten tonen maar u kunt tot hen door API toegang hebben. </p> <p>Voor informatie over de doelstellingen van het BedrijfsGeval project, zie <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md"> BedrijfsGevallendoelstellingen creëren </a>. </p> </li> 
     <li> <p><b> Strategische doelstellingen </b>: Een strategisch doel is een doel dat u creeert om uw het werkstrategie voor een specifieke periode te plannen. U kunt deze typen doelen maken met [!DNL Workfront Goals] . Uw organisatie moet een extra licentie aanschaffen en u moet toegang hebben tot deze functie om strategische doelen te kunnen maken. [!DNL Workfront Goals] zijn alleen beschikbaar met een extra licentie.</p> 
     <p>Zie <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] Overzicht </a> voor meer informatie. </p> 
     <p>U kunt strategische doelstellingen in een doel of een projectrapport tonen en tot hen toegang hebben door API. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal Hierarchy]</td> 
   <td> <p>In [!UICONTROL Goal] - en [!UICONTROL Project] -rapporten is dit een verzamelingsveld waarin de doelen in de hiërarchie worden weergegeven waartoe een strategisch doel behoort wanneer het wordt uitgelijnd op andere doelen. De doelen worden gescheiden door een ▸ scheidingsteken. </p> <p>Alleen de ouders van het doel en het doel tonen op dit gebied. Onderliggende doelen worden niet weergegeven. </p> <p>Voor informatie over het richten van doelstellingen in [!DNL Workfront Goals], zie <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md"> Goal groeperingsoverzicht in [!DNL Workfront Goals]</a>. </p> 
   <p>Dit veld is alleen zichtbaar als uw organisatie [!DNL Workfront Goals] heeft aangeschaft. Zie [!DNL Workfront Goals] overview <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] voor informatie over het beheer van strategische doelen met </a> . </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal Success Score]</td> 
   <td> In een [!UICONTROL Project report] -veld verwijst dit veld naar de doelen op projectniveau die aan de case [!UICONTROL Business] zijn gekoppeld. Dit is momenteel een verouderd veld en is niet gekoppeld aan functionaliteit.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Goals] </td> 
   <td> <p>In een [!UICONTROL Project] rapport, is dit een inzamelingsgebied dat alle strategische doelstellingen toont die met een project worden geassocieerd. De doelen worden gescheiden door komma's.</p> <p>Dit veld is alleen zichtbaar als uw organisatie [!DNL Workfront Goals] heeft aangeschaft. Voor informatie over het beheren van strategische doelstellingen die [!DNL Workfront Goals] gebruiken, zie <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] overzicht </a>. Voor meer informatie over strategische doelstellingen en projectdoelstellingen in [!DNL Workfront], zie "[!UICONTROL Goal]"in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global Interface Preferences]</td> 
   <td>Interfacemontages die alle gebruikers beïnvloeden. [!UICONTROL Global Interface Preferences] kan worden overschreven door [!UICONTROL User Interface Preferences] .</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Group]</td> 
   <td> <p>Een verzameling gebruikers (mogelijk van dezelfde afdeling of bedrijfseenheid) die toegang hebben tot dezelfde objecten. Naast gebruikers, kunnen de groepen met portefeuilles, programma's, projecten, <span> projectmalplaatjes, </span> bedrijven, teams, programma's, lay-outmalplaatjes, en timesheet profielen worden geassocieerd.</p> <p>U kunt objecten ook machtigingen per groep geven. Voor meer informatie, zie <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref"> Overzicht van Groepen </a>.</p> <p>In een lijst of een rapport van voorwerpen van één van de volgende types, kunt u het [!UICONTROL Group] gebied gebruiken om van te maken welke voorwerpen van dat type met een bepaalde groep worden geassocieerd: gebruiker, portefeuille, programma, project, <span> projectmalplaatje </span>, bedrijf, team, programma, lay-outmalplaatje of timesheet profiel.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Group Administrator]</td> 
   <td> <p>Gebruikers die de objecten, toegang en gebruikers van bepaalde gebruikersgroepen beheren.</p> <p> In een [!UICONTROL Group] -rapport worden in dit veld de namen weergegeven van de gebruikers die zijn aangewezen als [!UICONTROL Group Administrators] in de groep. Voor meer informatie over de Beheerders van de Groep, zie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref"> de beheerders van de Groep </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group with Administration Access]</td> 
   <td> <p> In een [!UICONTROL Layout Template], [!UICONTROL Timesheet Profile], of [!UICONTROL Schedule report], toont dit gebied de Groepen waarvan de Beheerders van de Groep toegang hebben om het malplaatje te wijzigen. U kunt dit rapport ook filteren op dit veld. </p> <p> Voor meer informatie, zie <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref"> lay-outmalplaatjes </a> creëren en beheren.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Grouping]</td> 
   <td> <p>A reporting element used to categorize information in a list by a common criterium.</p> <p>Voor meer informatie, zie de "[!UICONTROL Groupings]"sectie in het artikel <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref"> Meldend elementen: filters, meningen, en groeperingen </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Handoff Date]</td> 
   <td> <p>De datum waarop een taak beschikbaar wordt voor het werk. [!UICONTROL Handoff Date] is een berekening en kan niet handmatig worden ingesteld. <br> voor meer informatie over [!UICONTROL Handoff Date], zie het artikel <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[!UICONTROL Task Handoff Date] overzicht </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help Desk]</td> 
   <td>Een alternatieve naam om het [!UICONTROL Requests] -gebied van [!DNL Workfront] te beschrijven. U kunt het [!UICONTROL Requests] gebied gebruiken om klantensteunkaartjes, projectverzoeken, helpdeskkaartjes, enz. te verwerken.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Owner]</td> 
   <td>In een [!UICONTROL Hour] -rapport is [!UICONTROL Owner] de gebruiker aan wie de uren worden toegewezen. Dit is anders dan de gebruiker die de tijd registreert. Deze twee entiteiten kunnen soms twee verschillende gebruikers zijn. <br> voor meer informatie over logboektijd voor een andere gebruiker, zie de tijd van het artikel <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref"> Logboek </a>.</td> 
  </tr>

<tr> 
   <td>Uur</td> 
   <td> <p>An attribute set by Workfront for the Actual Hours that users log for tasks, issues, or projects. </p>

Uur-items kunnen een van de volgende statussen in Workfront hebben:
<ul>
   <li><b> voorgelegde </b>: de uren zijn het programma geopend op een project, een taak, of een kwestie. Ze maken deel uit van een factureringsrecord of worden nog niet toegevoegd aan een factureringsrecord.</li>
   <li><b> Goedgekeurd </b>: de uren zijn geregistreerd en zij zijn goedgekeurd door de Eigenaar van het Project. Ze maken deel uit van een factureringsrecord of worden nog niet toegevoegd aan een factureringsrecord.</li> 
   <li><b> niet Goedgekeurd </b>: de uren zijn geregistreerd en verworpen door de Eigenaar van het Project. Ze maken deel uit van een factureringsrecord of worden nog niet toegevoegd aan een factureringsrecord.</li>
   <li><b> Gevulde </b>: de uren zijn geregistreerd, toegevoegd aan een het facturerings verslag, en de het facturerings verslagstatus is duidelijk als Gevuld. Zij hoefden niet te worden goedgekeurd door de eigenaar van het project.</li>
   <li><b> in rekening gebracht en Goedgekeurd </b>: de uren zijn geregistreerd, door de Eigenaar van het Project goedgekeurd, en de het registrerende verslagstatus is duidelijk zoals Gevuld.</li>
   </ul>

<p>Wanneer de uren deel van een facturerings verslag uitmaken, wijst de Status van het Uur erop of de uren zijn goedgekeurd of als het het FactureringsVerslag van hen tot behoren in rekening is gebracht. De Status van het uur van een ureningang is slechts zichtbaar in een uurlijst of een rapport. </p>

<p>Voor meer informatie over het toevoegen van uren aan het factureren verslagen, zie de sectie "Uren aan het factureren verslagen"in artikel <a href="../../../manage-work/projects/project-finances/create-billing-records.md" > creëren het facturerings verslagen </a>.</p>

<p>Voor meer informatie over het goedkeuren van tijd op projecten, zie <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" > tijd vereisen om voor een project </a> worden goedgekeurd.</p>

<p><b>TIP</b></p>

<p>De algemene uren die niet direct op het werkpunten worden geregistreerd tonen geen Status van het Uur. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Hour Type]</td> 
   <td> <p>An attribute that can be set for Actual Hours that users log for tasks, issues, or projects. Dit is ook een kenmerk voor de geregistreerde uren die niet rechtstreeks aan het werk zijn gekoppeld, zoals [!UICONTROL Vacation] en [!UICONTROL Time Off] .</p> <p>Voor meer informatie, zie <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref"> de types van uren </a> leiden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>De id is een alfanumerieke indicator die aan elk object in [!DNL Workfront] is gekoppeld. Elk object in de [!DNL Workfront] -database wordt op unieke wijze geïdentificeerd. U kunt de id van elk object weergeven in een rapport of een lijst voor elk object. </p> <p><b>TIP</b></p>   <p>U kunt de id ook weergeven in de URL van de objectpagina. De id van een project kan er bijvoorbeeld ongeveer zo uitzien als het getal dat in de volgende URL wordt weergegeven wanneer u de pagina [!UICONTROL Project Details] opent:</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL IMS]</td> 
   <td>Identity Management System. Voor Adobe IMS moet u zich via Adobe aanmelden bij Workfront in plaats van uw Workfront-gebruikersnaam en -wachtwoord te gebruiken.</td> 
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
   <td> <p>In [!DNL Workfront Scenario Planner], kunt u een plan in verscheidene initiatieven verdelen om het gemakkelijker te maken om het plan te beheren. <span> u kunt een [!UICONTROL Initiative] rapport bouwen en u kunt tot [!UICONTROL Initiative] informatie in een [!UICONTROL Project] rapport toegang hebben.</span></p> <p>Voor [!DNL Scenario Planner] is een aanvullende licentie vereist. Voor informatie over [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref"> het [!DNL Scenario Planner] overzicht </a>. </p> <p>Het [!DNL Initiative] -rapport is alleen zichtbaar in een [!DNL Workfront] -instantie als uw bedrijf een [!DNL Workfront Scenario Planner] -licentie heeft aangeschaft. U hebt geen toegang tot [!UICONTROL Initiatives] via de API.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role]</span> </td> 
   <td> <p><span> het [!UICONTROL Initiative Job Role] rapporttype toont informatie over de baanrollen verbonden aan een planinitiatief in [!DNL Workfront Scenario Planner].</span> </p> <p>Voor [!DNL Scenario Planner] is een aanvullende licentie vereist. Voor informatie over [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md"> het [!DNL Scenario Planner] overzicht </a>. </p> <p><span>Dit rapporttype is alleen zichtbaar in uw [!DNL Workfront] -instantie als uw bedrijf een [!DNL Workfront Scenario Planner] -licentie heeft aangeschaft.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role Hours]</span> </td> 
   <td> <p><span> In een [!UICONTROL Initiative Job Role] -rapport geeft dit het aantal uren weer dat is gekoppeld aan een taakrol in een initiatief. </span> </p> <p>Voor [!DNL Scenario Planner] is een aanvullende licentie vereist. Voor informatie over [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md"> het [!DNL Scenario Planner] overzicht </a>. </p> <p>Dit veld en het rapporttype [!UICONTROL Initiative Job Role] zijn alleen zichtbaar in een [!DNL Workfront] -instantie als uw bedrijf een [!DNL Workfront Scenario Planner] -licentie heeft aangeschaft.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role Count]</td> 
   <td> <p>In een [!UICONTROL Initiative Job Role] -rapport geeft dit het aantal specifieke functies weer die aan een initiatief zijn gekoppeld.</p> <p>Voor [!DNL Scenario Planner] is een aanvullende licentie vereist. Voor informatie over [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md"> het [!DNL Scenario Planner] overzicht </a>. </p> <p>Dit veld en het rapporttype [!UICONTROL Initiative Job Role] zijn alleen zichtbaar in een [!DNL Workfront] -instantie als uw bedrijf een [!DNL Workfront Scenario Planner] -licentie heeft aangeschaft.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Last Published Date]</td> 
   <td> <p>Een veld in een [!UICONTROL Initiative] -, [!UICONTROL Initiative Job Role] - en [!UICONTROL Project] -rapport waarin de datum wordt weergegeven waarop een planinitiatief voor het laatst naar een project is gepubliceerd. U kunt initiatieven publiceren om projecten tot stand te brengen of projecten bij te werken met betrekking tot de initiatieven.</p> <p>Voor [!DNL Scenario Planner] is een aanvullende licentie vereist. Voor informatie over [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md"> het [!DNL Scenario Planner] overzicht </a>. </p> <p><span> voor informatie over het publiceren initiatieven, zie </span> <a href="../../../scenario-planner/publish-scenarios-update-projects.md"> scenario's publiceren om projecten in [!DNL Workfront Scenario Planner]</a> tot stand te brengen en bij te werken. Dit veld is alleen zichtbaar in een [!DNL Workfront] -instantie als uw bedrijf een [!DNL Workfront Scenario Planner] -licentie heeft aangeschaft.</p> </td> 
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
   <td> <p>In [!DNL goal reports], toont dit een "[!UICONTROL True]/ [!UICONTROL False]"waarde voor elk strategisch doel om erop te wijzen of uw organisatie aan het doel als zijn eigenaar wordt toegewezen. </p> 
   <p>Dit veld is alleen zichtbaar als uw organisatie [!DNL Workfront Goals] heeft aangeschaft. Zie [!DNL Workfront Goals] overview <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] voor informatie over het beheer van strategische doelen met </a> .</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue]</td> 
   <td> <p>Een niet-gepland het werkpunt dat gewoonlijk wijst op een probleem verhinderend de voltooiing van een taak of een project. Het wordt getrigeerd en geëvalueerd voor verdere werkzaamheden</p> <p>Een [!UICONTROL Issue] kan ook een [!UICONTROL Help Desk] -aanvraag zijn. [!UICONTROL Change Orders] , [!UICONTROL Requests] en [!UICONTROL Bugs] zijn ook [!UICONTROL Issues] .</p> </td> 
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
   <td> <p>Wordt gebruikt om de dagelijkse functies en verantwoordelijkheden van een gebruiker te identificeren. De rollen van de baan kunnen aan de werkpunten worden toegewezen om de vereiste vaardigheid te identificeren nodig om een het werkproces te voltooien zonder het aan een specifieke gebruiker toe te wijzen. </p> <p>Een gebruiker kan meerdere rollen hebben. Voorbeelden zijn Graphic Designer of Consultant.</p> <p>Voor meer informatie, zie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref"> baanrollen </a> creëren en beheren.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Journal Entry]</p> </td> 
   <td> <p>Een te rapporteren object dat u informatie geeft over systeemupdates voor bijgehouden velden die worden weergegeven in het gebied [!UICONTROL Updates] met projecten, taken, problemen en andere objecten.</p> <p>Meer leren, zie <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref"> Rapport over het gebied van Updates met een rapport van de Ingang van het Dagboek </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kanban Flag]</td> 
   <td> <p>In een [!UICONTROL Task] Rapport of [!UICONTROL Issue] Rapport [!UICONTROL Kanban Flag] geeft het veld de vlagstatus weer die is ingesteld in het artikel op [!UICONTROL Kanban board] . Mogelijke waarden zijn [!UICONTROL On Track] , [!UICONTROL Ready to Pull] en [!UICONTROL Is Blocked] .</p> <p>Voor meer informatie over het instellen van vlagstatus in artikelen op de [!UICONTROL Kanban story board] raadpleegt u  het artikel <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref"> vlaggen van het Gebruik op verhalen op [!UICONTROL Kanban board]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI's</td> 
   <td>Een meetbare waarde die aantoont hoe effectief een bedrijf belangrijke bedrijfsdoelstellingen bereikt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>De hoeveelheid tijd die moet verstrijken nadat de [!UICONTROL Planned Completion Date] -taak van de voorganger is voltooid tot de afhankelijke taak kan beginnen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag Types]</td> 
   <td> <p>De methode voor het berekenen van de [!UICONTROL Lag] . Het kan zijn:</p> 
    <ul> 
     <li>[!UICONTROL Days] (werkdagen)</li> 
     <li>[!UICONTROL Calendar Days] (feestdagen negeren)</li> 
     <li>[!UICONTROL Percent]</li> 
     <li>[!UICONTROL Day of Week]</li> 
    </ul> <p>Voor meer informatie, zie <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref"> overzicht van de Types van Lag </a>.</p> </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Large Thumbnail]</td> 
   <td> <p> In een [!UICONTROL Document] -lijst of -rapport wordt een voorbeeld van het document in een miniatuur weergegeven. </p> <p>Selecteer <strong>[!UICONTROL Large Thumbnail]</strong> om een miniatuur van 400 pixels breed in het rapport weer te geven.</p> <p>De grootte van de miniatuur wordt aangepast wanneer u de breedte van de kolom in een lijst of rapport wijzigt.</p> <p>Zie ook "[!UICONTROL Thumbnail]"in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last 10 Viewers]</td> 
   <td> <p>In een rapportlijst, toont dit gebied de namen van maximaal 10 gebruikers die het rapport onlangs hebben bekeken.<br> voor meer informatie over gebruiksinformatie in rapportlijsten, zie het het rapportgebruik van het artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref"> Mening </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Condition Note]</td> 
   <td> <p>In dit veld wordt de laatste update weergegeven die de eigenaar van het object voor een object heeft ingevoerd. Dit is de meest recente activiteit of interactie van de eigenaar van een object.</p> <p>De kolom [!DNL Last Condition Note] is leeg als de notitietekst van de laatste notitie van een object is verwijderd. Wanneer een nieuwe notitie op het object wordt ingevoerd, wordt deze de laatste notitie en wordt deze opnieuw weergegeven in de kolom. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Finance Update Date]</td> 
   <td>In een [!UICONTROL project] -rapport geeft dit veld de datum en het tijdstip weer waarop de projectfinanciering voor het laatst is berekend en bijgewerkt. Voor informatie over projectfinanciën, zie <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref"> overzicht van de financiën van het Project </a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Note]</td> 
   <td> <p>In dit veld wordt de laatste update weergegeven die een gebruiker voor een object heeft ingevoerd. Dit is de meest recente activiteit of interactie op een voorwerp.</p> <p>De kolom [!UICONTROL Last Note] is leeg als de tekst van de laatste notitie van een object is verwijderd. Wanneer een nieuwe notitie op het object wordt ingevoerd, wordt deze de laatste notitie en wordt deze opnieuw weergegeven in de kolom.</p>
   <p>Wanneer dit veld wordt toegevoegd aan een [!UICONTROL Task] -rapport, worden de resterende updates van onderliggende objecten (zoals problemen, subtaken of documenten) van de taak niet weergegeven in deze kolom.</p> 
   <p><b>OPMERKING</p>
   <p>De laatste notitie die met de API aan een object is toegevoegd, wordt niet weergegeven in een rapport in Workfront. Het veld [!DNL Last Note] is leeg als de laatste update voor een object is toegevoegd met de API. </p>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Viewed By]</td> 
   <td> <p>In een rapportlijst, toont dit gebied informatie over de gebruiker die het rapport het laatst bekeken.<br> voor meer informatie over gebruiksinformatie in rapportlijsten, zie het het rapportgebruik van het artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref"> Mening </a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Viewed Date]</td> 
   <td> <p>In een rapportlijst, toont dit gebied de datum waarop het rapport het laatst werd getoond.<br> voor meer informatie over gebruiksinformatie in rapportlijsten, zie het het rapportgebruik van het artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref"> Mening </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Layout Template]</td> 
   <td>Gedefinieerd door de systeembeheerder of groepsbeheerder om de tabbladen en rapporten te identificeren die worden weergegeven in de werkruimte van een bepaalde gebruiker.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Layout Type]</td> 
   <td>In combinatie met [!UICONTROL Custom Views] geeft [!UICONTROL Layout Type] het type [!UICONTROL Custom View] op. Momenteel is alleen de lijst beschikbaar. In de toekomst is [!UICONTROL Detail] (de [!UICONTROL Detail] -weergave van een object) mogelijk beschikbaar.</td> 
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
       <br>If there  are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.   
     </p> </td> </tr> -->
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.  </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>    </p>
    --> </td> 
  </tr> 
  <tr> 
   <!-- <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection  of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Legacy Actual Hours]</td> 
   <td> <p>In een project, een taak, of een uitgifterapport, [!UICONTROL Legacy Actual Hours] is de som alle uren het programma geopend op het project, de taak, of geeft om het even welke tijd, met inbegrip van vóór mei 2021 uit.</p>  
   <p>De oudere Werkelijke Uren tonen als Werkelijke Uren in een project, een taak, of gebied van de Details van de kwestie. </p>
   <p>Zie ook <strong> Ware Uren </strong>.
    <p>Voor meer informatie, zie <a href="/help/quicksilver/manage-work/tasks/task-information/actual-hours.md"> Ware Uren van de Mening </a>.</p>
    </td> 
  </tr>  <tr> 
   <td>[!UICONTROL License Type]</td> 
   <td>Het type licentie dat is toegewezen aan een [!UICONTROL Access Level] . Het is [!UICONTROL Full User] , [!UICONTROL Limited User] of [!UICONTROL Requester] .</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Plan]</td> 
   <td> <p>In een [!UICONTROL Group] -weergave of -rapport wordt in dit veld het maximumaantal [!UICONTROL Plan] -licenties weergegeven dat kan worden toegewezen aan gebruikers met de desbetreffende groep als hun [!UICONTROL Home Group] .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Work]</td> 
   <td> <p>In een [!UICONTROL Group] -weergave of -rapport wordt in dit veld het maximumaantal [!UICONTROL Work] -licenties weergegeven dat kan worden toegewezen aan gebruikers met de desbetreffende groep als hun [!UICONTROL Home Group] .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limited User]</td> 
   <td>A License Type that allows creation of an [!DNL Access Level] that contains view-only privileges, with the ability to submit issues, enter notes, and upload documents.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL List Controls]</td> 
   <td> <p>Een onderdeel van [!UICONTROL Interface Setup] dat het mogelijk maakt aangepaste filters, weergaven en groepen te koppelen aan individuele gebruikers of globaal aan alle gebruikers.</p> </td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Lookup fields]</td> 
   <td> <p>In de Planning van Workfront, nadat u de verbinding tussen twee verslagtypes vestigt en u individuele verslagen verbindt samen, kunt u de verbonden verslagen' gebieden op het verslag van verwijzingen voorzien u van verbindt.</p>
   <p>Bijvoorbeeld, als u een type van het verslag van de Campagne met een de objecten van het Project van Workfront type verbindt, kunt u het gebied van de Begroting van verbonden projecten op de campagneverslagen tonen. Het projectgebied van de Begroting is een raadplegingsgebied van projecten op een campagne.</p> <p>De waarden van opzoekvelden worden automatisch ingevuld in de records waarmee ze zijn verbonden.</p>
   <p>Voor informatie, zie <a href="/help/quicksilver/planning/records/connected-records-overview.md"> Verbonden verslagenoverzicht </a>.</p>
   <p>Voor Workfront Planning is een extra licentie vereist.</p>
    </td> 
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
   <td> <p>Een van de [!UICONTROL Project] s [!UICONTROL Update Types] . Met deze instelling kunnen [!UICONTROL Project Projected] - en [!UICONTROL Planned] -tijdlijnen alleen worden bijgewerkt wanneer op "[!UICONTROL Recalculated Timelines]" wordt geklikt. Projecten die op deze manier worden ingesteld, worden tijdens het nachtelijke herberekeningsproces genegeerd en wanneer het project of de taken in het project worden bijgewerkt.</p> <p>Zie <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref"> Het project selecteren [!UICONTROL Update Type] </a> voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>Dit verwijst naar de momenteel aangemelde gebruiker. </p> <p>Wij adviseren gebruikend dit gebied in een filter om rapporten generischer te maken wanneer het delen van hen met andere gebruikers. Deze manier, kunt u slechts één rapport bouwen dat verschillende informatie afhankelijk van zal tonen wie het programma opent om het te bekijken, aangezien de informatie altijd voor de het programma geopende gebruiker wordt aangepast. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Max Users]</td> 
   <td> <p>Dit is een verouderd veld. Alle informatie die in dit veld wordt weergegeven, is gerelateerd aan een functie die door [!DNL Workfront] is verwijderd en het veld kan niet worden bijgewerkt. </p> <p>In eerdere versies van [!DNL Workfront] kon u dit veld bijwerken tijdens het maken of bewerken van een taakrol. Het toonde het totale aantal gebruikers die met een rol op elk project kunnen worden geassocieerd. De waarde nul is toegestaan voor een onbeperkt aantal gebruikers dat aan een project kan worden toegewezen. </p>Het veld is in sommige rapporten en lijsten nog steeds zichtbaar, maar de weergegeven informatie kan niet worden bijgewerkt. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone]</td> 
   <td> <p>Een teller die u met een taak kunt associëren om erop te wijzen dat een zeer belangrijk punt in het project is bereikt wanneer de taak wordt voltooid. In het algemeen kunt u mijlpalen gebruiken om een belangrijke gebeurtenis weer te geven, zoals de voltooiing van een fase van het project of een reeks kritieke activiteiten. [!UICONTROL Milestones] worden doorgaans gekoppeld aan bovenliggende taken. U moet de mijlpalen creëren alvorens u hen aan taken kunt vastmaken. Voor informatie over mijlpalen, zie <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md"> een milestone weg </a> creëren en <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md"> mijlpalen met taken </a> associëren. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Milestone Path]</td> 
   <td>Een verzameling van [!UICONTROL milestones]. [!UICONTROL Milestone Paths] wordt gebruikt voor projecten om projecten met bepaalde typen [!UICONTROL Milestones] te onderscheiden van projecten met een andere set [!UICONTROL Milestones] .</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone Task]</td> 
   <td>Een taak die is gemarkeerd om een te meten te melden gebeurtenis aan te geven.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Module]</td> 
   <td>Eén stap in een scenario in [!DNL Workfront Fusion] dat een functie uitvoert op basis van de bijbehorende app.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Primary Role]</td> 
   <td> <p>Wanneer naar dit in filters wordt verwezen, toont dit of gebruikers die het zelfde [!UICONTROL Primary Role] hebben zoals het programma geopende gebruiker, of het werkpunten die aan [!UICONTROL Primary Role] van de het programma geopende gebruiker worden toegewezen.</p> <p>Wij adviseren gebruikend dit gebied in een filter om rapporten generischer te maken wanneer het delen van hen met andere gebruikers. Deze manier, kunt u slechts één rapport bouwen dat verschillende informatie afhankelijk van zal tonen wie het programma opent om het te bekijken, aangezien de informatie altijd voor de het programma geopende gebruiker wordt aangepast. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Home Team]</td> 
   <td> <p>Wanneer naar dit in filters wordt verwezen, toont dit gebied of gebruikers die tot [!UICONTROL Home Team] van de het programma geopende gebruiker behoren, of het werkpunten die aan [!UICONTROL Home Team] van de het programma geopende gebruiker worden toegewezen. </p> <p>Wij adviseren gebruikend dit gebied in een filter om rapporten generischer te maken wanneer het delen van hen met andere gebruikers. Deze manier, kunt u slechts één rapport bouwen dat verschillende informatie afhankelijk van zal tonen wie het programma opent om het te bekijken, aangezien de informatie altijd voor de het programma geopende gebruiker wordt aangepast. </p> </td> 
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
   <td>Het middelste bovenste deelvenster van de toepassing dat koppelingen bevat naar de hoofdgebieden van [!UICONTROL Workfront] .</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL New Number Value]</td> 
   <td>In een [!UICONTROL Journal Entry] -rapport wordt hiermee de bijgewerkte waarde weergegeven van een veld dat [!UICONTROL Old Number Value] vervangt.
   Voor meer informatie, zie "[!UICONTROL Old Number Value]"in dit artikel.</td> 
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
   <p>Voor meer informatie over het merken van een uitgave als factureerbaar, zie <a href="/help/quicksilver/manage-work/projects/project-finances/manage-project-expenses.md"> projectuitgaven beheren </a>.</p>
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Non Work Day]</td> 
   <td>Een dag die niet wordt toegewezen aan het uitvoeren van een opdracht. Dit is meestal een feestdag, vakantie of weekend. De term wordt weergegeven in de API-verkenner. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note]</td> 
   <td>Een opmerking of update voor een [!DNL Workfront] -object.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note Text]</td> 
   <td> <p>Hiermee wordt de tekst weergegeven van een update die een gebruiker heeft ingevoerd voor een willekeurig object. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Number of Linked Goals]</td> 
   <td> <p>In een [!UICONTROL Project] -rapport is dit het aantal strategische doelen dat aan het project is gekoppeld. Voor informatie over het associëren van projecten met strategische doelstellingen, zie <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> projecten aan doelstellingen in [!DNL Adobe Workfront Goals]</a> toevoegen.</p> 
   <p>Voor informatie over strategische doelstellingen, zie ook "[!UICONTROL Goal]"in dit artikel.</p> 
   <p>Dit veld is alleen zichtbaar als uw organisatie [!DNL Workfront Goals] heeft aangeschaft. Voor informatie over het beheren van strategische doelstellingen die [!DNL Workfront Goals] gebruiken, zie <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> projecten aan doelstellingen in [!UICONTROL Adobe Workfront Goals]</a> toevoegen. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object]</td> 
   <td> <p>De informatie die u in [!DNL Adobe Workfront] weergeeft, wordt vertegenwoordigd door objecten die in de [!DNL Workfront] -database zijn opgeslagen. De objecten zijn de drijvende kracht achter de informatie in Workfront. Voorbeelden van objecten zijn:</p> 
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

</ul> <p>Voor meer informatie, zie <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref"> voorwerpen in [!UICONTROL Adobe Workfront]</a> begrijpen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object Types]</td> 
   <td>Als u een rapport of lijst maakt met al uw aangepaste formulieren, kunt u dit veld gebruiken als weergave of filter om te zien welke objecttypen aan elk formulier zijn gekoppeld. </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Old Number Value]</td> 
   <td>In een [!UICONTROL Journal Entry] -rapport wordt hiermee de oorspronkelijke waarde van een veld weergegeven voordat het werd bijgewerkt. Zodra de waarde van een veld is bijgewerkt, wordt deze weergegeven als de [!UICONTROL New Number Value] in een [!UICONTROL Journal Entry] -rapport. Voor meer informatie, zie ook "[!UICONTROL New Number Value]".</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL On Change Only]</td> 
   <td> <p>Een van de [!UICONTROL Project Update] -typen. Wanneer deze optie is geselecteerd, worden de tijdlijnen [!UICONTROL Project Projected] en [!UICONTROL Planned] alleen bijgewerkt wanneer het project of een taak in het project wordt bijgewerkt of gewijzigd. Het werkt het project niet elke nacht bij.</p> <p>Voor meer informatie, zie <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref"> het Type van projectupdate selecteren </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Op Task]</td> 
   <td> <p>De naam voor [!UICONTROL Issue] in de [!DNL Workfront] -database, die wordt gebruikt in de tekstmodus, rapporteert of berekende aangepaste gegevens.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Open]</td> 
   <td>Een kwestie of een taak die niet volledig is, maar aan wordt gewerkt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Org Chart]</td> 
   <td>Kort voor organisatieschema. Dit is een grafiek die de hiërarchie van een organisatie toont. Deze bevindt zich ook op de tab op het detailscherm van [!UICONTROL User] die de relaties [!UICONTROL User] ''s [!UICONTROL Company] en [!UICONTROL Reporting] ' weergeeft en toestaat.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organizational Setup]</td> 
   <td>Hiermee worden [!UICONTROL Companies] , [!UICONTROL Groups] en [!UICONTROL Security Profiles] voor uw organisatie gedefinieerd.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Other Groups]</td> 
   <td> <p>In een rapport of een mening die van gebruikers een lijst maakt, toont dit gebied alle groepen waar elke gebruiker een lid is. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency]</span> </td> 
   <td> 
    <div> 
     <p>In een [!UICONTROL Job Role] -rapport is dit de valuta die is gekoppeld aan een taakrol. Het is een overschrijving van de [!UICONTROL Base Currency] die in het [!UICONTROL Setup] -gebied door de [!DNL Workfront] -beheerder is ingesteld. </p> 
     <p>Voor meer informatie, zie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref"> baanrollen </a> creëren en beheren.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Billing/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>In een [!UICONTROL Job Role] -rapport is dit de facturering per uur van de taakrol met de geselecteerde [!UICONTROL Override Currency] van de taakrol.</p> 
     <p> Voor meer informatie, zie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref"> baanrollen </a> creëren en beheren.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Cost/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>In een [!UICONTROL Job Role] -rapport is dit de kosten per uur van de taakrol met de geselecteerde [!UICONTROL Override Currency] van de taakrol. </p> 
     <p>Voor meer informatie, zie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref"> baanrollen </a> creëren en beheren.</p> 
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
     <p>In een [!UICONTROL Goal] -rapport geeft dit het type eigenaar weer dat is toegewezen aan een strategisch doel. Het volgende is de types van doeleigenaar:</p> 
     <ul> 
      <li> <p>[!UICONTROL User]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL Group]</p> </li> 
     </ul> 
     <p>Er wordt geen waarde in dit veld weergegeven wanneer de eigenaar van het doel uw organisatie is. </p> 
     <p>Hiervoor is een aanvullende licentie vereist. Voor informatie over [!DNL Workfront Goals], zie <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] overzicht </a>. </p> 
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
   <td> <p>Een [!UICONTROL parameter] is een aangepast veld. U kunt een rapport maken voor alle parameters of aangepaste velden in uw systeem. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent]</td> 
   <td>In een rapport bevat dit veld informatie over het bovenliggende element van het object. Bijvoorbeeld, in een [!UICONTROL issue] rapport, zou het informatie over de taak of het project kunnen tonen dat de kwestie onder wordt geregistreerd; in een taakrapport, zou het informatie over de directe oudertaak of over het project kunnen tonen. Voor meer informatie over welke voorwerpen ouders in [!DNL Workfront] zouden kunnen hebben, zie de "Interdependentie en hiërarchie van voorwerpen"sectie in het artikel <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref"> begrijpt voorwerpen in [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent Lag]</td> 
   <td>De hoeveelheid tijd die moet verstrijken tussen het [!UICONTROL Parent Task] begin en het [!UICONTROL Subtask] begin.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent Task]</td> 
   <td>Wordt ook wel een [!UICONTROL Summary Task] genoemd. Dit is een taak met subtaken (ook wel [!UICONTROL Children Tasks] genoemd). De waarden [!UICONTROL Duration] , [!UICONTROL Work Required] en [!UICONTROL Percent Complete] van de bovenliggende taak worden berekend op basis van de subtaken.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Part-Time Resources]</td> 
   <td>Een gebruiker met licentie die minder capaciteit heeft dan het standaardschema dat in het systeem is gedefinieerd.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percent Complete]</td> 
   <td> <p>Een project, een taak, of een probleemgebied dat toont welk percentage van het werk verbonden aan de taak, het project, of de kwestie wordt voltooid.</p> <p>U kunt dit veld handmatig bijwerken voor problemen en werktaken. </p> <p>Voor projecten en oudertaken, is dit gebied een roll-up van alle het werk taken en u kunt niet het manueel bijwerken. </p> <p>Voor meer informatie, zie <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref"> overzicht [!UICONTROL Percent Complete] van het Project </a>.</p> </td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Performance Index Method (PIM)]</td> 
   <td> <p>[!UICONTROL Performance Index Method (PIM)] voor het project controleert de methode Adobe Workfront gebruikt om de metriek van projectprestaties zoals de Index van de Prestaties van de Kosten (CPI), de Index van de Prestaties van het Programma van de Kosten (CSI), de Index van de Prestaties van het Programma (SPI), en Schatting bij Voltooiing (EAC) te berekenen.</p> 
   <p>Workfront berekent deze waarden aan de hand van uren of kosten.</p>
   <p>Voor informatie, zie <a href="/help/quicksilver/manage-work/projects/project-finances/set-pim.md"> plaats de Methode van de Index van Prestaties (PIM) </a>.</p>
   </td> 
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
    </ul> <p>Voor meer informatie, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref"> Overzicht van het delen van toestemmingen op voorwerpen </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]</td> 
   <td> <p>Dit is een volledig licentietype in het [!DNL Workfront] -systeem. Gebruikers moeten dit doen om toegang te krijgen tot alle functies in [!DNL Workfront] .</p> <p>Zie <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] Overzicht van licenties </a> voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan] (in de [!DNL Scenario Planner] )</td> 
   <td> <p>Een plan is het belangrijkste voorwerp wanneer het werken met de [!DNL Workfront] Planner van het Scenario. U kunt de strategie voor de nabije en lange termijn toekomst van uw bedrijf schetsen en elk resultaat op hoog niveau identificeren en het toevoegen als plan aan de [!DNL Workfront] Planner van het Scenario. </p> <p>U kunt [!DNL Scenario Planner] -plannen niet weergeven in een rapport en u kunt ze niet openen via de [!DNL Workfront] -API. </p> <p>Voor [!DNL Scenario Planner] is een aanvullende licentie vereist. Voor informatie over [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md"> het [!DNL Scenario Planner] overzicht </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned]</td> 
   <td> <p>Het tijdkader waarbinnen iets gepland is voor te komen. Wanneer u projecten, taken, of kwesties in [!DNL Workfront] creeert, vestigt u de geplande begin en einddata, evenals het geplande tijdskader waarin zij voorkomen. Deze waarden geven uw oorspronkelijke intentie weer of schatten hoe lang het duurt voordat een object is voltooid. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Benefit]</td> 
   <td>Dit is een handmatige vermelding voor de projectmanager om te schatten of de voltooiing van een project de organisatie enig geldelijk voordeel zou opleveren. Het opgeven van deze waarde kan onderdeel zijn van het samenstellen van een [!UICONTROL Business Case] voor het project. U moet [!UICONTROL Manage] machtigingen voor het project hebben om deze waarde bij te werken.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Planned Budgeted Hours]</td> 
   <td> <p>In een [!UICONTROL Budgeted Hour] -rapport geeft dit het aantal uren weer dat is begroot voor projecten of [!UICONTROL Job Roles] in de [!UICONTROL Resource Planner] . </p> <p>Voor informatie over het in de begroting opnemen van projecten of rollen in [!UICONTROL Resource Planner], zie de artikel <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref"> middelen van de Begroting in [!UICONTROL Resource Planner] gebruikend [!UICONTROL Project] en [!UICONTROL Role] meningen </a>. Voor informatie over het [!UICONTROL Budgeted Hours] rapport, zie het artikel <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref"> Rapport: Beoogde Uur </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Completion Date]</td> 
   <td> <p>U kunt de [!UICONTROL Planned Completion Date] van een taak, project of uitgave handmatig instellen op een datum die u kiest. Als u de eigenschap [!UICONTROL Planned Completion Date] niet instelt, wordt deze automatisch door [!DNL Workfront] ingesteld. Wanneer de waarde automatisch wordt ingesteld, is [!UICONTROL Planned Completion Date] : [!UICONTROL Planned Start Date] + [!UICONTROL Duration]</p> <p>Raadpleeg de volgende artikelen voor meer informatie:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref"> Overzicht van de taak [!UICONTROL Planned Completion Date]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref"> Plaats het project [!UICONTROL Planned Completion Date]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Cost]</td> 
   <td> <p>Een totaal van [!UICONTROL Planned Labor Cost] en [!UICONTROL Planned Expense Cost] van het project. Hierbij wordt de eigenschap [!UICONTROL Planned Risk Cost] niet in het project opgenomen.  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Date Alignment]</td> 
   <td> <p>Dit is een automatische indicator dat Workfront projecten, taken, en kwesties toewijst om te tonen wanneer een punt met betrekking tot zijn Geplande Datum van de Voltooiing zal worden voltooid. </p>
   <p>Hieronder vindt u mogelijke waarden voor de indicator voor het uitlijnen van de geplande datum: </p>
<ul>
<li>Wordt uitgevoerd op de geplande einddatum</li>
<li>Wordt uitgevoerd vóór de geplande einddatum</li>
<li>Wordt uitgevoerd na de geplande einddatum</li></ul>
<p>De geplande datumuitlijning is zichtbaar in project-, taak- en uitgiftenlijsten en -rapporten. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration]</td> 
   <td> <p>De waarde [!UICONTROL Planned Duration] van een taak is meestal gelijk aan die van de taak [!UICONTROL Duration] . Het geeft het verschil in dagen weer tussen de [!UICONTROL Planned Start] en de [!UICONTROL Planned Completion Dates] van de taak. </p> <p>Als de taak een [!UICONTROL Duration] type [!UICONTROL Effort Driven] heeft, kan [!UICONTROL Planned Duration] afwijken van [!UICONTROL Duration] van de taak, afhankelijk van het aantal bronnen dat u aan de taak toewijst. </p> <p>Als een taak met een [!UICONTROL Duration] type [!UICONTROL Effort Driven] bijvoorbeeld een [!UICONTROL Duration] tijd heeft van 3 dagen en u één bron met een volledig tijdschema toewijst aan de taak, is de [!UICONTROL Planned Duration] ook drie dagen. Als u drie bronnen met een volledig tijdschema aan dezelfde taak toewijst, blijft [!UICONTROL Duration] 3 dagen, maar wordt [!UICONTROL Planned Duration] 1 dag. In [!UICONTROL Planned Duration] worden ook de [!UICONTROL Planned Start] - en [!UICONTROL Planned Completion] -datums van de taak gewijzigd, zodat deze de nieuwe [!UICONTROL Planned Duration] weerspiegelen. Hierdoor wordt ook de tijdlijn van het project beïnvloed. </p> <p>Voor meer informatie over het verschil tussen [!UICONTROL Duration] en [!UICONTROL Planned Duration] voor taken, zie het artikel <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref"> Verschil tussen [!UICONTROL Planned Duration] en [!UICONTROL Duration] voor taken </a>.</p> <p>Projecten en problemen hebben geen [!UICONTROL Planned Duration] . </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration Minutes]</td> 
   <td> <p>De [!UICONTROL Planned Duration Minutes] van een project of een uitgave is de [!UICONTROL Duration] van het project of de uitgave in minuten. </p> <p>Taken hebben geen veld [!UICONTROL Planned Duration Minutes] . </p> <p>[!UICONTROL Template Tasks] beschikken over een veld [!UICONTROL Planned Duration Minutes] waarin de [!UICONTROL Planned Duration] van de taak in minuten wordt weergegeven. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Expense Cost]</td> 
   <td> <p>De som van [!UICONTROL Planned Amounts] voor alle uitgaven die voor een project of een taak worden geregistreerd.</p> <p><b>VOORBEELD</b></p>
   <p>Als u een uitgave voor Taak 1 creeert en $600.00 op het [!UICONTROL Planned Amount] gebied ingaat, is [!UICONTROL Planned Expense Cost] voor deze taak $600.00. </p> 
   <p>Voor een project gebruikt [!DNL Workfront] de volgende formule om te berekenen [!UICONTROL Planned Expense Cost] :</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Hours]</td> 
   <td> <p>Dit veld wordt weergegeven in het venster [!UICONTROL projects] , [!UICONTROL tasks] en geeft gebieden, rapporten voor projecten, taken of problemen en hulpmiddelen voor resourcebeheer, zoals het rapport [!UICONTROL Resource Planner] , [!UICONTROL Workload Balancer] en [!UICONTROL Utilization] . </p> <p>Het toont het aantal uren dat de Eigenaar van het Project schat dat elke taak of kwestie zou moeten voltooien. Voor projecten is het doorgaans een roll-up van de [!UICONTROL Planned Hours] -code van de taken in het project. </p> <p>In het veld [!UICONTROL Planned Hours] kan andere informatie worden weergegeven, afhankelijk van de locatie waar u de informatie weergeeft. Voor informatie over Geplande Uren, zie <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref"> Gepland overzicht van Uren </a>.</p> <p>Geplande uren worden in minuten opgeslagen in de database van [!DNL Workfront] . Zorg er bij het schrijven van berekeningen met dit veld voor dat de uren als minuten worden weergegeven.<br></p> <p>Door gebrek, worden de Geplande Uren gelijkelijk verdeeld over alle dagen binnen de duur van een het werkpunt en ook voor alle middelen die aan de taak worden toegewezen. Gebruikers kunnen het dagelijkse aantal geplande uren voor een werkartikel of de individuele geplande uren voor elke toegewezen persoon bijwerken.</p> <p>Het bijwerken van dit gebied verschilt voor projecten, taken, en kwesties: </p> 
    <ul> 
     <li> <p>Voor uitgaven kunt u dit veld handmatig bijwerken. De geplande uren van de uitgave worden niet toegevoegd aan het Geplande Uren van het Project. </p> <p><b>TIP</b></p> <p>In een uitgifterapport wordt een van de velden [!UICONTROL Planned Hours] vervangen door het veld [!UICONTROL Work] . In het veld wordt het aantal geplande uren weergegeven. Zie de velden "work" of "[!UICONTROL Work]" in deze tabel voor meer informatie. </p> </li> 
    </ul> 
    <ul> 
     <li> <p>Voor taken kunt u dit veld handmatig bijwerken wanneer [!UICONTROL Duration Type] van de taak [!UICONTROL Calculated Assignment] of [!UICONTROL Simple] is. Dit veld wordt berekend door [!DNL Workfront] wanneer [!UICONTROL Duration Type] van de taak [!UICONTROL Calculated Work] of [!UICONTROL Effort Driven] is.<br> voor informatie over [!UICONTROL Task Duration], zie het artikel <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref"> Overzicht van Taak [!UICONTROL Duration] en [!UICONTROL Duration Type]</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Voor projecten berekent [!DNL Workfront] de Geplande Uren door alle Geplande Uren van alle taken op het project toe te voegen. </p> </li> 
    </ul> <p><b>TIP</b></p> <p>U kunt [!UICONTROL Planned Hours] ook weergeven in [!UICONTROL project] -, [!UICONTROL task] - of [!UICONTROL issues] -rapporten door de tekstmodus te gebruiken en te verwijzen naar aanvullende velden. Voor meer informatie, zie "<code>work</code>", "[!UICONTROL Work]", en "<code>workRequiredExpression</code>"gebieden in deze lijst. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Labor Cost]</td> 
   <td> 
    <p>Voor een taak, het uurtarief van de gebruiker of de rol vermenigvuldigd met het aantal uren die aan de gebruiker of de rol worden toegewezen.</p> <p>Voor een project is het een totaal van alle [!UICONTROL Planned Labor Costs] taken.</p> <p>Of het tarief van de gebruiker of de rol wordt gebruikt hangt van het Type van Kosten af dat voor de bepaalde taak wordt geselecteerd. </p> <p>Voor meer informatie, zie <a href="../../../manage-work/projects/project-finances/track-costs.md"> kosten van het Spoor </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Revenue]</td> 
   <td> <p>Taken en projecten kunnen een waarde voor [!UICONTROL Planned Revenue] in [!DNL Workfront] weergeven. [!UICONTROL Planned Revenue] geeft het bedrag aan dat is gekoppeld aan de [!UICONTROL Planned Hours] -taken van het project. Voor projecten kan het ook de [!UICONTROL Fixed Revenue] van het project bevatten. </p> <p>Voor taken is dit de opbrengst verbonden aan [!UICONTROL Planned Hours] van taken. De geplande uren van alle taken lopen tot de geplande uren van het project om bij te dragen aan de berekening van het project [!UICONTROL Planned Hours] . </p> 
   <p>[!DNL Workfront] berekent [!UICONTROL Planned Revenue] voor taken en projecten met de volgende formules:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>Het project [!UICONTROL Planned Revenue] dat wordt weergegeven in het [!UICONTROL Project Details] -gebied en in projectrapporten, verschilt van de geplande omzet die wordt weergegeven in het [!UICONTROL Utilization] -rapport. </p> <p>[!UICONTROL Planned Revenue] in het [!UICONTROL Project Details] gebied weerspiegelt de taakopbrengsten evenals de Vaste Ontvangsten van het project. De [!UICONTROL Planned Revenue] in de [!UICONTROL Utilization Report] displays [!UICONTROL Planned Revenue] zijn alleen gekoppeld aan de taken in het project. </p> 
     <p><b>VOORBEELD</b></p>  
      <p>Als het project 1 taak met 10 uren heeft, toegewezen aan een consultant met een frequentie van $20 uur en het project $100 [!UICONTROL Fixed Revenue] heeft, geeft het [!UICONTROL Utilization] -rapport $200 voor [!UICONTROL Planned Revenue] weer (de [!UICONTROL Planned Revenue] die gekoppeld is aan de uren op de taak). In de sectie [!UICONTROL Project Details] wordt $300 weergegeven (de [!UICONTROL Planned Revenue] van de taak en de Vaste inkomsten voor het project.) </p> 
    <p>Voor informatie over het volgen van opbrengst in [!DNL Workfront] zie <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md"> Overzicht van Facturering en Ontvangsten </a>. </p> 
    <p>Voor informatie over [!UICONTROL Planned Revenue] berekeningen in [!UICONTROL Utilization report], zie <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md"> de informatie van het middelgebruik van de Mening </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Risk Cost]</td> 
   <td> <p>The total of the [!UICONTROL Potential Cost] of all the risk on the project factoring in their Probability of occur. Dit bedrag is niet inbegrepen in [!UICONTROL Planned Cost] van het project.</p> <p>De [!UICONTROL Planned Risk Cost] van een project wordt berekend met de volgende formule:</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Profile]</td> 
   <td>Een door de beheerder gedefinieerde verzameling met tabs en secties die wordt weergegeven in [!DNL Workfront] .</td> 
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
   <td> <p>Een verzameling projecten met verenigende kenmerken. Deze projecten concurreren doorgaans met dezelfde middelen, hetzelfde budget of dezelfde tijd. U kunt portfolio's opsplitsen in programma's en de projecten koppelen aan de programma's voordat ze aan een Portfolio worden toegevoegd.</p> <p>Voor meer informatie over portefeuilles, zie <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md"> portefeuillemethodologie </a> begrijpen.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Management]</td> 
   <td>Een praktijkgebied dat gericht is op het beheer van een collectie of verwante programma's en projectinspanningen.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Optimizer]</td> 
   <td>Een [!DNL Workfront] -hulpmiddel voor het beoordelen en prioriteren van projecten in een portfolio.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Owner]</td> 
   <td>De belanghebbende die verantwoordelijk is voor de prioritering en de begroting van een portefeuille.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Potential Risk Cost]</td> 
   <td>Dit is een projectgebied dat u in lijsten en rapporten kunt de plaats bepalen. Het toont de potentiële kosten voor de risico's verbonden aan het project, als zij voorkomen. Voor meer informatie zie <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref"> de Mogelijke Kosten van het Risico berekenen </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Predecessor]</td> 
   <td> <p>Een taak die vóór de voltooiing van een afhankelijke taak moet worden voltooid. Een taak die is gemarkeerd als een [!UICONTROL Dependency] voor een andere taak. De voorgangers staan de planner toe om opeenvolging-gebiedingslogica te plaatsen, zoals om een taak te beginnen nadat een andere taak eindigt.</p> <p>Voor meer informatie, zie <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref"> Overzicht van taakvoordecessors </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Company]</td> 
   <td>Het bedrijf tot wie de gebruiker behoort zoals aangewezen in hun gebruikersmontages. Bedrijven kunnen ook met projecten worden geassocieerd.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Contact]</td> 
   <td><p>[!UICONTROL Primary Contact] is de maker van een uitgave en wordt automatisch door [!DNL Workfront] aangewezen wanneer de persoon de uitgave maakt. U kunt dit veld handmatig bijwerken als u [!DNL Manage] -machtigingen hebt voor de uitgave. Een kwestie kan slechts één Primaire Contact hebben.</p> 
   <p>Als u de primaire contactpersoon wijzigt, heeft de gebruiker die oorspronkelijk als de primaire contactpersoon was aangewezen, nog steeds [!UICONTROL Manage] toegang tot de uitgave.</p>
   <p>Wanneer u een uitgave omzet in een taak of een project, wordt de gebruiker die als [!UICONTROL Primary Contact] van de uitgave is aangewezen, de [!UICONTROL Converted Issue Originator] van het project of de taak. Als [!UICONTROL Primary Contact] van het probleem wordt bijgewerkt nadat het probleem is omgezet, blijft [!UICONTROL Converted Issue Originator] behouden als de [!UICONTROL Primary Contact] van het probleem op het moment dat de conversie heeft plaatsgevonden. Zie ook "[!UICONTROL Converted Issue Originator]"in dit artikel.</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Priority]</td> 
   <td>Een waarde die aan een taak, kwestie of een project kan worden toegewezen om aan te wijzen hoe belangrijk het is. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Private]</td> 
   <td>Op een [!UICONTROL Note] of [!UICONTROL Document] wordt dat object met deze optie verborgen voor de meeste viewers. Voor een Privé Rij van het Verzoek van de Hulp, slechts kunnen de gebruikers op het Team van het Project kwesties aan die rij (of project) door het [!UICONTROL Requests] gebied voorleggen.</td> 
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
   <td> <p>In een [!UICONTROL Goal] -rapport geeft dit het percentage weer van hoe dicht een strategisch doel bij het voltooien ligt. Het percentage van de voortgang wordt weergegeven als een getal. Voor informatie over strategische doelstellingen, zie ook "[!UICONTROL Goal]"in deze lijst.</p> <p>Dit veld is alleen zichtbaar als uw organisatie [!DNL Workfront] Doelen heeft aangeschaft. Zie [!DNL Workfront Goals] Projecten toevoegen aan doelen in <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> [!DNL Adobe Workfront Goals] voor informatie over het beheren van strategische doelen met </a> . </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Progress Status]</td> 
   <td> <p>In een project, een Taak, en een rapport van het Doel, toont dit gebied de Status van de Voortgang van projecten, taken, of strategische doelstellingen. Raadpleeg de volgende artikelen voor meer informatie:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref"> Overzicht van de Status van de Voortgang van het Project </a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref"> Overzicht van de Status van de Voortgang van de Taak </a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md"> Overzicht van de vooruitgang en de toestand van het doel in [!DNL Adobe Workfront Goals]</a> </p>
     <p>Het [!UICONTROL Goal] -rapport en het [!UICONTROL Progress Status] for [!DNL goals] -veld zijn alleen zichtbaar als uw organisatie [!DNL Workfront Goals] heeft aangeschaft. Voor informatie over strategische doelstellingen in [!DNL Workfront Goals], zie <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] overzicht </a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Project]</td> 
   <td> <p>Een groot deel van de werkzaamheden moet binnen een bepaald tijdsbestek worden voltooid en moet een specifiek budget en een bepaald aantal middelen gebruiken. Om het beheersbaar te maken, verdeelt u het project in een reeks taken. Als u alle taken uitvoert, wordt het project voltooid. Voor informatie over de planning van een project, zie <a href="../../../manage-work/projects/planning-a-project/plan-project.md"> Plan een projectoverzicht </a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Assignment Planned Hours]</td> 
   <td> <p>In een [!UICONTROL Initiative Job Role] -rapport wordt hiermee het aantal [!UICONTROL Planned Hours] weergegeven dat is gekoppeld aan een taakrol die is toegewezen aan taken of problemen in het project. Dit veld en het rapporttype [!UICONTROL Initiative Job Role] worden alleen weergegeven in een [!DNL Workfront] -instantie als uw bedrijf een [!DNL Workfront Scenario Planner] -licentie heeft aangeschaft. Voor informatie over [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md"> het [!DNL Workfront Scenario Planner] overzicht </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Details]</td> 
   <td>De details van de huidige status van een project.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Budgeted Cost]</td> 
   <td> <p> Dit is de [!UICONTROL Budgeted Cost] van een project zoals het in lijsten en rapporten toont.</p><p>Zie ook "[!UICONTROL Budgeted Cost]"in dit artikel.</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Project Management]</td> 
   <td>Een reeks beleid dat de drempels voor projectverwezenlijking, categorisering, en het noemen van de projecten beheerst.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Project Overhead]</td> 
   <td>In een [!UICONTROL Hour] -rapport is dit veld gereserveerd voor financiële informatie die is gekoppeld aan de uren die zijn geregistreerd met het uurtype [!UICONTROL Project Time] . De projecten kunnen hun eigen het Factureren Tarieven hebben en als een uur rechtstreeks op een project wordt geregistreerd, dan zullen die tarieven in berekeningen worden gebruikt. Op basis van de projectinstellingen kunnen projecten ook verschillende valuta's hebben en kan er voor die uren een valutaomrekening plaatsvinden. Met het [!UICONTROL Project Overhead] -object kan [!DNL Workfront] die informatie ophalen.</td> 
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
   <td>Een profiel van een aangewezen belanghebbende waaraan elk van uw gebruikers zou moeten betrekking hebben. In [!DNL Workfront] worden deze aangeduid als [!UICONTROL Access Levels]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Teams]</td> 
   <td> <p>De inzameling van gebruikers of rollen die aan een project worden toegewezen</p> <p>Voor meer informatie, zie <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md"> Overzicht van het Team van het Project </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project tracking]</td> 
   <td>De gegevens die worden gebruikt om de gezondheid en de reikwijdte van een project te meten</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projected]</td> 
   <td> <p>Een schatting van de tijdstempel van wanneer het werk zal worden voltooid op basis van de geplande uren en het percentage dat een taak, uitgave of project voltooid zal zijn.</p> <p>Dit verwijst naar datums of de [!UICONTROL Duration] taken, problemen of projecten. Doorgaans worden datums en tijdsduur aangegeven die meer gelden voor het leven van de onderdelen van het werk, nadat een deel van het werk al is voltooid of enige tijd is verstreken. </p> <p>De datum [!UICONTROL Projected Completion Date] van een taak is bijvoorbeeld de datum waarop [!DNL Workfront] schat dat de taak zal worden voltooid, op basis van hoeveel werk er tot nu toe is verricht, hoeveel personen eraan zijn toegewezen en hoeveel tijd er is verstreken sinds de begindatum.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Deadline]</td> 
   <td> <p>In rapporten die het [!UICONTROL Document Version] -object bevatten (zoals een [!UICONTROL Document Version] report en [!UICONTROL Proof Approval] -rapport), wordt in dit veld de dag van de week, de datum, het tijdstip en het jaar van de proefdrukdeadline weergegeven.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Decision]</td> 
   <td> <p>In rapporten die het [!UICONTROL Document Version] -object bevatten (zoals een [!UICONTROL Document Version] -rapport  en [!UICONTROL Proof Approval] -rapport) geeft dit veld de beslissingsstatus van de proefdruk weer (in behandeling, vereiste of goedgekeurde wijzigingen)</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Name]</td> 
   <td> <p>In rapporten die het [!UICONTROL Document Version] -object bevatten (zoals een [!UICONTROL Document Version] report en [!UICONTROL Proof Approval] -rapport), wordt in dit veld de proefdruknaam weergegeven.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Pages]</td> 
   <td> <p>In rapporten die het [!UICONTROL Document Version] -object bevatten (zoals een [!UICONTROL Document Version] report en [!UICONTROL Proof Approval] -rapport), geeft dit veld het aantal pagina's weer dat in de proefdruk is opgenomen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Progress]</td> 
   <td> <p>In rapporten die het [!UICONTROL Document Version] -object bevatten (zoals een [!UICONTROL Document Version] report en [!UICONTROL Proof Approval] -rapport), wordt de voortgangsstatus van de proefdruk weergegeven ( [!UICONTROL Sent], [!UICONTROL Opened], [!UICONTROL Commented], [!UICONTROL Decision Made]).</p> <p>Voor meer informatie, zie <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref"> overzicht van de vooruitgang van het Bewijs </a> in <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref"> vooruitgang van het Bewijs en statusoverzicht </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proofing]</td> 
   <td>Een revisieproces waarbij een of meer gebruikers de inhoud markeren en opmerkingen plaatsen die moet worden gewijzigd in een afbeelding, een tekstdocument, een video of interactieve webinhoud.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>Op een [!UICONTROL Note] of [!UICONTROL Document] maakt deze optie dat object toegankelijk voor andere gebruikers of zelfs voor personen van buiten [!DNL Workfront] . Voor een [!UICONTROL Help Request Queue] betekent [!UICONTROL Public] dat alle gebruikers die problemen kunnen verzenden naar een project, problemen kunnen verzenden via het [!UICONTROL Requests] -gebied.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Quality]</td> 
   <td>De perceptie van de arbeidskwaliteit binnen de organisatie.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue]</td> 
   <td>Wordt ook wel Help Desk Queue of [!UICONTROL Help Request Queue] genoemd. Dit is een project dat naar het [!UICONTROL Requests] -gebied is gepubliceerd, zodat gebruikers er problemen mee kunnen verzenden. Gewoonlijk worden wachtrijen gemaakt voor bepaalde onderwerpen, zoals [!UICONTROL Bugs] , [!UICONTROL Project Requests] , enz.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Properties]</td> 
   <td>Met deze instellingen worden regels voor het verzenden van uitgaven gedefinieerd voor een project dat wordt gepubliceerd naar het [!UICONTROL Requests] -gebied.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Topic]</td> 
   <td> <p>Een eigenschap op een [!UICONTROL Help Request Queue] waarmee gebruikers die een uitgave verzenden een onderwerp kunnen selecteren. Onderwerpen kunnen:</p> 
    <ul> 
     <li>Aan een aangepast gegevensformulier worden gekoppeld.</li> 
     <li>Wijs de kwestie automatisch aan een gebruiker toe, rol, of team door de Verpletterende Regel die op het geselecteerde Onderwerp wordt geplaatst.</li> 
     <li>Verplaats de kwestie naar een verschillend project of rij door de verpletterende regel die op het geselecteerde onderwerp wordt geplaatst.</li> 
    </ul> <p>Voor meer informatie, zie <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref"> de Onderwerpen van de Rij </a> creëren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rank]</td> 
   <td> <p>In een [!UICONTROL Access Level] -rapport kunt u handmatig een [!UICONTROL Rank] van de [!UICONTROL Access Level] -instructie opgeven. Dit helpt u, als [!DNL Workfront] beheerder, om het niveau van ingewikkeldheid visueel te identificeren verbonden aan elk Niveau van de Toegang. Bijvoorbeeld, kunt u lagere aantallen voor complexere ([!UICONTROL Plan] - niveau) Niveaus van de Toegang, en hogere aantallen voor minder complexe ([!UICONTROL Requester] - niveau) Niveaus van de Toegang geven. U kunt de standaardtoegangsniveaus niet rangschikken. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ready]</td> 
   <td> <p>In dit veld op een taakrapport wordt aangegeven of een [!UICONTROL Agile] -taak op de achtergrond is gemarkeerd als [!UICONTROL Ready] . Deze markering is alleen van toepassing op [!UICONTROL Agile] -taken. Dit zijn taken die zijn toegewezen aan een [!UICONTROL Agile] -team. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Record]</td> 
   <td> <p>In de Planning van Workfront, is een verslag een uniek geval van een verslagtype.</p>
<p>Nadat u een recordtype aan een werkruimte hebt toegevoegd, kunt u records van dat type op de pagina van het recordtype toevoegen.</p>
<p>'Campagne' kan bijvoorbeeld een recordtype zijn en 'Summer Campaign for EMEA' is een record van het type Campagne-record.</p>
<p>Voor informatie over het creëren van verslagen, zie <a href="/help/quicksilver/planning/records/create-records.md"> verslagen </a> creëren. </p> <p>Voor Workfront Planning is een extra licentie vereist. </p></td> 
  </tr>


<tr> 
   <td>[!UICONTROL Record type]</td> 
   <td> <p>Het objecttype van Workfront Planning.</p>
<p>In tegenstelling tot Workfront, waar de objecten types vooraf bepaald zijn, in de Planning van Workfront, kunt u uw eigen objecten types tot stand brengen.Workfront de objecten van de Planning worden genoemd verslagtypes.</p>
<p>In Workfront zijn bijvoorbeeld al de objecttypen Program, Portfolio, Project, Task of Issue gemaakt.</p>
<p>In de Planning van Workfront, kunt u om het even welke verslagtypes tot stand brengen die aan de werkschema's van uw organisatie voldoen. Later kunt u bepalen hoe de recordtypen op elkaar betrekking hebben of hoe afhankelijk van het formulier is.</p> Voor informatie over het creëren van verslagtypes, zie <a href="/help/quicksilver/planning/architecture/create-record-types.md"> recordtypes </a> creëren. </p> <p>Voor Workfront Planning is een extra licentie vereist. </p></td> 
  </tr>

<tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Recurrence Frequency]</td> 
   <td> <p>Een veld dat wordt weergegeven in het vak [!UICONTROL Task Details] of [!UICONTROL Edit Task] van een bovenliggend item van terugkerende taken. Het is de frequentie waarmee de taken in de herhaling voorkomen. Voor informatie over het creëren van terugkomende taken, zie <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref"> terugkomende taken </a> creëren. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reference Number]</td> 
   <td> <p>Projecten, taken en problemen worden automatisch gekoppeld aan een uniek referentienummer wanneer ze worden gemaakt. U kunt [!UICONTROL Reference Number] in de [!UICONTROL Details] pagina van projecten, taken, of kwesties, of in een lijst of een rapport bekijken. </p> <p><b>TIP</b><p><br>U kunt verwijzen naar referentienummers wanneer twee items dezelfde naam hebben, omdat referentienummers altijd uniek zijn. </p> <p>[!DNL Workfront] genereert automatisch opeenvolgende referentienummers op systeemniveau. Elk project, elke taak, of elke kwestie krijgt het volgende beschikbare aantal in de opeenvolging. <br></p> <p>Als gebruiker A bijvoorbeeld een taak maakt, wijst [!DNL Workfront] de taak mogelijk automatisch het referentienummer 100 toe. Als Gebruiker B een kwestie onmiddellijk na dit creeert, wijst [!DNL Workfront] de kwestie het Aantal van de Verwijzing 101 toe. U kunt referentienummers niet handmatig bewerken. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rejection Issue]</td> 
   <td>In een project of een taakrapport, is dit de kwestie die wordt gecreeerd wanneer de goedkeuring voor het project of de taak wordt verworpen. Voor informatie over verwerpingskwesties, zie het artikel <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref"> een goedkeuringsproces voor het werkpunten </a> creëren. </td> 
  </tr>

<tr>
  <td>Relatietypen</td>
  <td><p>Workfront-objecten worden altijd met elkaar verbonden via een van de volgende relatietypen:</p>

<ul><li> <b> Één aan vele </b>: In deze verhouding, kan één voorwerp met veelvoudige andere voorwerpen van verschillende types worden verbonden. Een project kan bijvoorbeeld meerdere taken hebben. De project-Taken verhouding is één aan vele verhouding. U kunt deze verhouding niet tonen in een rapport gebruikend de Standaardinterface. U moet tekstmodusrapportage gebruiken om een tot veel relaties weer te geven.</li>
  <li><b> Één aan één </b>: In deze verhouding, kan één voorwerp slechts met één ander voorwerp van een verschillend type worden verbonden. Een project kan bijvoorbeeld maar één groep hebben. De project-groep verhouding is één aan één verhouding. U kunt een-op-een-relatie tussen objecten weergeven in een standaardrapport.</li>
  <li><b> Velen aan één </b>: In deze verhouding, kunnen de veelvoudige voorwerpen met slechts één andere voorwerpen van een verschillend type worden verbonden. Bijvoorbeeld, kunnen de veelvoudige taken met het zelfde project worden verbonden. De taak-project verhouding is vele aan één verhouding. U kunt vele aan één verhouding tussen voorwerpen in een Standaard rapport tonen. </li>
  <li><b> Velen aan vele </b>: In deze verhouding, kunnen de veelvoudige voorwerpen van het zelfde type met veelvoudige voorwerpen van een verschillend type worden verbonden. Verschillende gebruikers kunnen bijvoorbeeld tot meerdere andere teams behoren en de teams kunnen tot verschillende gebruikers behoren. U kunt deze verhouding niet tonen in een rapport gebruikend de Standaardinterface. U moet tekstmodusrapporten gebruiken om veel relaties weer te geven. </li> </ul>
  </td></tr>
<tr> 
   <td>[!UICONTROL Remaining Risk Cost]</td> 
   <td> <p>Een projectveld dat het verschil weergeeft tussen de [!UICONTROL Planned Risk Cost] van een project en het totaal van alle [!UICONTROL Actual Costs] -risico's voor het project. </p> <p>[!UICONTROL Remaining Risk Cost] voor een project wordt berekend gebruikend de volgende formule:</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Replanning]</td> 
   <td>De datums van een project wijzigen om problemen te verhelpen of te verhelpen. Een project dat bijvoorbeeld al enkele maanden in de wachtstand staat, moet opnieuw worden gepland om nauwkeurige data te weerspiegelen. Dit is een handmatige bewerking waarbij de data van het project of die van de taken worden aangepast. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Report]</td> 
   <td>Een grafiek of tabel met informatie over een bepaald [!DNL Workfront] -object en de bijbehorende kenmerken.</td> 
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
   <td> <p>Gebruik dit veld in weergaven of filters in een uitgifterapport om te verwijzen naar het probleem dat het probleem verhelpt. </p> <p>Voor informatie over het tonen van het oplossen van voorwerpen in rapporten, zie <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref"> Weergave Verlosbaar en het Oplossen van de informatie van Objecten in een rapport </a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref"> Overzicht van het Oplossen van en Oplosbare Voorwerpen </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Project]</td> 
   <td> <p>In een probleemrapport gebruikt u dit veld in weergaven of filters om te verwijzen naar het project dat het probleem verhelpt. </p> <p>Voor informatie over het tonen van het oplossen van voorwerpen in rapporten, zie <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref"> Weergave Verlosbaar en het Oplossen van de informatie van Objecten in een rapport </a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref"> Overzicht van het Oplossen van en Oplosbare Voorwerpen </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Task]</td> 
   <td> <p>Gebruik dit veld in weergaven of filters in een probleemrapport om te verwijzen naar de taak die het probleem verhelpt. </p> <p>Voor informatie over het tonen van het oplossen van voorwerpen in rapporten, zie <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref"> Weergave Verlosbaar en het Oplossen van de informatie van Objecten in een rapport </a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref"> Overzicht van het Oplossen van en Oplosbare Voorwerpen </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource]</td> 
   <td>Gebruikers of rollen die in [!DNL Workfront] bestaan en aan projectteams, taken en kwesties worden toegewezen. Zij zijn verantwoordelijk voor de voltooiing van het werk verbonden aan projecten, taken, of kwesties. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in  Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Resource Management]</td> 
   <td> <p>[!UICONTROL Resource Management] is een reeks bedrijfsinstrumenten waarmee u het gebruik van uw middelen nauwkeurig kunt voorspellen op basis van hun beschikbaarheid, zodat het werk dat moet worden gedaan op tijd en op budget wordt voltooid. </p> <p>Met de hulpmiddelen van het Beheer van het Middel kunt u capaciteit op lange termijn en kortetermijnplanningsbehoeften voor uw middelen plannen. </p> <p>Voor informatie over het Beheer van het Middel in [!DNL Workfront], zie <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md"> begonnen met het Beheer van het Middel </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager IDs]</td> 
   <td><p>In een projectrapport, kunt u deze optie gebruiken wanneer het creëren van een filter om een specifieke middelmanager te vinden. </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Managers]</td> 
   <td> <p>In een projectrapport of lijstmening, is dit een informatiegebied dat gebruikers toont die worden aangewezen om middelbeheersactiviteiten op het project uit te voeren.  Wanneer u "[!UICONTROL Resource Managers]"in een rapport gebruikt, wordt een lijst van middelmanagers getoond, met elke middelmanager op het project dat door een komma wordt gescheiden. U kunt maximaal 30 middelmanagers op een bepaald project aanwijzen.</p> <p>Voor meer informatie, zie het artikel <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md"> de Managers van het Middel voor een project of een malplaatje </a> toewijzen.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Resource Planner Budgeted Hours] </td> 
   <td>De begrote uren uren voor het project en de middelen verbonden aan het in [!UICONTROL Resource Planner]. Zie ook "[!UICONTROL Budgeted Hours]"in dit artikel. </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Resource Planner] </td> 
   <td>Een geavanceerd [!DNL Workfront] hulpmiddel dat u middelen over projecten, baanrollen, of gebruikers laat bekijken en beheren. Voor informatie, zie <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref"> overzicht van de Planner van het Middel </a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Planner Budgeted Labor Cost]</td> 
   <td> <p>Dit zijn de kosten verbonden aan de uren die voor de rollen van de projectbaan gebruikend de Planner van het Middel in de begroting worden opgenomen. </p> <p>Zie ook "Budgeted Labour Cost" in dit artikel. </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Resource Pools]</td> 
   <td> <p>Brongroepen zijn verzamelingen van gebruikers die aan een project kunnen worden gekoppeld. De gebruikers in dezelfde bronnenpool behoren gewoonlijk tot dezelfde afdeling, hebben vergelijkbare of aanvullende vaardigheden of worden gefinancierd uit hetzelfde budget. U kunt veelvoudige Pools van het Middel aan een project of aan een gebruiker associëren. Een bronnenpool kan uitsluitend aan een project worden toegewezen of door meerdere projecten worden gedeeld.</p> 
   <p>Zie <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Overzicht van bronnenpools </a> voor meer informatie over bronnenpools.</p> 
   <p>In projectrapporten, tonen de Pools van het Middel alle pools verbonden aan een project. Dit object kan niet in een groep worden gebruikt.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Utilization]</td> 
   <td>Een rapport met het aantal uren dat beschikbaar is tijdens een bepaalde periode en het aantal uren dat is gepland voor elke gebruiker in het rapport. Dit wordt ook berekend in [!UICONTROL Average Hours Per Day] en een toewijzingspercentage.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Result]</td> 
   <td>In [!DNL Workfront Goals] is een resultaat een voortgangsindicator voor een doel. Dit kan een getal, een percentage of een valutabedrag zijn dat u handmatig bijwerkt. U kunt geen resultaten weergeven in een rapport en u kunt ze niet openen via de API van [!DNL Workfront] . Voor informatie over activiteiten, zie <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref"> begonnen worden met resultaten en activiteiten in de Doelen van Adobe Workfront </a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Revenue]</td> 
   <td>Een factureerbare hoeveelheid voor de taak of het project. Het bedrag kan per uur, vast of een combinatie van beide zijn.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Revenue Type]</td> 
   <td>Het type inkomsten bepaalt hoe de taak inkomsten zal genereren. Voorbeelden zijn [!UICONTROL Fixed Hourly] , [!UICONTROL Role Hourly] en [!UICONTROL Role Hourly w/Cap] . Voor informatie over het volgen van opbrengst in [!DNL Workfront] zie <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref"> Overzicht van Facturering en Ontvangsten </a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>Doorgaans een licentietype. Een gebruiker met een [!UICONTROL Reviewer] -licentie kan werkitems in het systeem controleren en goedkeuren.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk]</td> 
   <td> <p>Dit kan naar de volgende concepten in [!DNL Workfront] verwijzen:</p> 
    <ul> 
     <li> <p>Een gebied op een project dat erop wijst hoe riskant een project kan zijn. U kunt de uitvoering van uw projecten prioriteren op basis van het risiconiveau. Projecten kunnen de volgende risiconiveaus hebben:</p> <p>- [!UICONTROL Very Low]</p> <p>- [!UICONTROL Low]</p> <p>- [!UICONTROL Medium]</p> <p>- [!UICONTROL High]</p> <p>- [!UICONTROL Very High]</p> <p>De risiconiveaus die u aangeeft voor een project kunnen niet worden aangepast. </p> <p> Voor informatie over het bijwerken van het risico van een project, zie de " sectie van de Montages van het Project"van het artikel <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref"> projecten </a> uitgeven. U kunt het risicogebied van een project in rapporten tonen. </p> </li> 
     <li> <p>Een gebeurtenis die tijdens de duur van een project kan voorkomen die een potentiële invloed op de kosten, het werkingsgebied, of het programma van het project identificeert. U bepaalt potentiële risico's aan een project en associeert een waarschijnlijkheid dat zij of kosten voorkomen aangezien u het BedrijfsGeval van het project bouwt. Voor informatie over het toevoegen van risico's aan het BedrijfsGeval van het project, zie "tot stand brengen en risico's op projecten uitgeven". </p> <p>U kunt risico's die in [!UICONTROL Business Case] in rapporten worden bepaald niet tonen. U kunt slechts verscheidene soorten Kosten van het Risico in rapporten en lijsten tonen. </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Cost]</td> 
   <td> <p>De kosten in verband met de risico's voor een project. Hier volgt een overzicht van de risicokosten voor projecten die u in rapporten kunt weergeven:</p> 
    <ul> 
     <li> <p>[!UICONTROL Actual Cost]: een veld met een risico dat de werkelijke kosten van het risico toont. Naast rapporten en lijsten kunt u deze zoeken in het vak [!UICONTROL Edit Risk] wanneer u een risico bewerkt of maakt. </p> <p>Voor project, taak, of uitgiftekosten, zie "[!UICONTROL Actual Cost]"in dit artikel. </p> </li> 
     <li> <p>[!UICONTROL Planned Risk Cost]: een veld in het project waarin in totaal alle [!UICONTROL Potential Risk Costs] voor het project worden weergegeven. Zie ook "[!UICONTROL Planned Risk Cost]"in dit artikel. </p> <p>Voor informatie over de Mogelijke Kosten van het Risico, zie <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref"> de Mogelijke Kosten van het Risico berekenen </a>. </p> </li> 
     <li> <p>[!UICONTROL Remaining Risk Cost]: een veld op het project waarin het verschil wordt weergegeven tussen het totaal van de [!UICONTROL Actual Costs] van alle risico's en de [!UICONTROL Planned Risk Cost] . Zie ook "Resterende risicokosten" in dit artikel. </p> </li>
    </ul> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Management]</td> 
   <td>Processen om risico te identificeren, te verlichten en te controleren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td>Zie [!UICONTROL Job Role] in dit artikel.</td> 
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
   <td>[!UICONTROL Scenario] (in [!DNL Workfront Fusion]) </td> 
   <td> <p>Een scenario bestaat uit een reeks stappen (modules) die aangeven hoe gegevens moeten worden overgebracht en getransformeerd tussen apps/services.</p> <p>Voor informatie over scenario's in [!DNL Workfront Fusion], zie <a href="https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/scenario-overview">[!DNL Adobe Workfront Fusion] scenario overzicht </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scenario] (in de [!DNL Workfront Scenario Planner] ) </td> 
   <td> <p>In [!DNL Scenario Planner], is een scenario een exemplaar van een plan. </p> <p>Voor [!DNL Scenario Planner] is een aanvullende licentie vereist. Voor informatie over [!DNL Workfront Scenario Planner], zie <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref"> het [!DNL Scenario Planner] overzicht </a>. </p> <p>Voor informatie over het creëren van scenario's, zie <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md"> planscenario's in creëren en vergelijken [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule]</td> 
   <td>Het wekelijkse werkschema, met inbegrip van werktijden, gecombineerd met Dagen uit (zoals Vakantiedagen) en uitzonderingsdagen (zoals een zaterdag werkdag). U kunt programma's met projecten en gebruikers associëren.</td> 
  </tr> 
<tr> 
   <td>[!UICONTROL Schedule Performance Index (SPI)]</td> 
   <td><p>In [!UICONTROL Schedule Performance Index (SPI)] wordt de relatie beschreven tussen het geplande schema en het feitelijke schema. Adobe Workfront berekent de SPI op het project en de taakniveaus. De managers van het project herzien dit metrisch om te identificeren of de taken of de projecten momenteel voor of achter programma volgen.</p>
  <p>Voor informatie, zie <a href="/help/quicksilver/manage-work/projects/project-finances/calculate-spi.md"> de Index van de Prestaties van het Programma berekenen (SPI) </a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule Exemption]</td> 
   <td>Wordt ook wel een [!UICONTROL Modified Shift] genoemd. Dagen die gepland zijn in tegenstelling tot de normale wekelijkse arbeidstijden zoals bepaald in het schema. Een zaterdag die gepland is om te werken, zou bijvoorbeeld een [!UICONTROL Schedule Exemption] zijn wanneer de Planning is ingesteld op Alleen maandag tot en met vrijdag werken.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scheduled Report]</td> 
   <td> <p>Wanneer u een rapport van rapporten bouwt, kunt u informatie over de programma's van het rapport tonen, als het rapport voor levering gebruikend het [!UICONTROL Scheduled Report] gebied gepland is. Dit gebied toont veelvoudige waarden, voor elk programma van elk rapport, in een bulleted lijst. Voor meer informatie over het plannen van rapporten, zie het artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref"> de leveringsoverzicht van het Rapport </a>.</p> <p>Omdat in dit veld meerdere waarden worden weergegeven, kan het niet worden gebruikt in een groep. U hebt alleen toegang tot dit bestand in een filter of weergave. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scope Change]</td> 
   <td>An [!UICONTROL Audit Trail] that, if active, generate a note when a change to the Scope of a project or task, such as if a [!UICONTROL Task Duration] or the [!UICONTROL Predecessors] are changed.</td> 
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
   <td>De instellingen waarmee een gebruiker kan communiceren met bepaalde objecten in het systeem en niet met andere. Zie ook "[!UICONTROL Access Levels]"in dit artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Setup]</td> 
   <td>Het gebied waar beheerders systeemconfiguraties en voorkeuren kunnen instellen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severity]</td> 
   <td> <p>[!UICONTROL Severity] geeft aan hoe waarschijnlijk een punt de voltooiing van de werkzaamheden zal beïnvloeden. Een probleem met de waarde high [!UICONTROL Severity] kan bijvoorbeeld de voltooiing van een taak volledig blokkeren, maar een probleem met de waarde low [!UICONTROL Severity] kan slechts cosmetisch zijn.</p> <p>Zie <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> Ernst van uitgave bijwerken </a> voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severities]</td> 
   <td>Zie [!UICONTROL Severity] in dit artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sharing]</td> 
   <td>Het toestaan van andere Gebruikers om een specifiek item in [!DNL Workfront] weer te geven of te bewerken.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Slack Date]</td> 
   <td>In een taakweergave of rapport geeft [!UICONTROL Slack Date] de exacte datum weer waarop een taak beslist invloed kan hebben op [!UICONTROL Completion Date] van het project. Voor informatie over [!UICONTROL Slack Date] van een taak, zie <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref"> het overzicht van de Datum van de Datum van de Taak Slack </a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Smart Assignments]</td> 
   <td> <p>Wanneer het toewijzen van taken of kwesties aan gebruikers, [!DNL Workfront] doet aanbevelingen ([!UICONTROL Smart Assignments]) over wie de beste gebruikers het werk moeten voltooien, die op de tijd wordt gebaseerd zij beschikbaar hebben om het te voltooien en hun verhouding met het project.</p> <p>Voor meer informatie, zie <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref"> Slim toewijzingsoverzicht </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>Geeft het bovenliggende object van een ander object aan. Een document dat aan een taak is gekoppeld, heeft bijvoorbeeld de naam van de taak in het [!UICONTROL Source] -veld van een [!UICONTROL Document] -rapport of -weergave. Een probleem dat in het kader van een project is aangemeld, heeft de naam van het project in het [!UICONTROL Source] -veld van een Issue-rapport of -weergave. </p> 
   <p>De volgende rapporten tonen een kolom van Source waar u informatie over het oudervoorwerp kunt bekijken:</p>
  <ul><li>Problemen melden</li>
    <li>Uur-rapporten</li>
    <li>Documentrapporten </li>
    </ul>
   <p>Als de gebruikers geen toestemmingen aan het oudervoorwerp van een kwestie, een uur, of een document hebben, toont de kolom van Source van het rapport leeg, zelfs wanneer het rapport aan vertoning wordt gevormd, of met de toegangsrechten van een andere gebruiker moet worden geleverd. </p>
   <p> Om informatie over het oudervoorwerp in het rapport te tonen, adviseren wij toevoegend een kolom voor het oudervoorwerp waar u de naam van de ouder kunt tonen. </p>
    <p>U kunt bijvoorbeeld het volgende toevoegen aan een rapport met een Source-kolom: </p>
    <ul><li>De kolommen van de Naam van het Project, van de Naam van de Taak, of van de Naam van de Uitgave aan een document of uurrapport.</li>
    <li>De kolommen van de Naam van het Project of van de Naam van de Taak aan een probleemrapport. </li> </ul>
    Voor meer informatie, zie <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md"> Looppas en lever een rapport met de toegangsrechten van een andere gebruiker </a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Start Date]</td> 
   <td> <p>De datum waarop het werk aan een item moet worden gestart. Er zijn verschillende begindatums in [!DNL Workfront] : </p> 
    <ul> 
     <li>[!UICONTROL Planned]</li> 
     <li>[!UICONTROL Actual]</li> 
     <li>[!UICONTROL Projected] </li> 
    </ul> <p>In een [!UICONTROL Rate report] is dit de datum waarop een nieuwe factureringssnelheid voor een taakrol op projectniveau begint. De uren verbonden aan het project die na deze datum zijn worden vermenigvuldigd met dit het factureringspercentage om de opbrengst op het project te berekenen. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td> <p>Een indicator die wordt gebruikt om een werkschemapositie van een het werkpunt of van een strategisch doel te signaleren.</p> <p>Voor projecten is [!UICONTROL Status] een instelling op het project die aangeeft of het project:</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL On Hold] </li> 
     <li>[!UICONTROL Complete] </li> 
     <li>[!UICONTROL Dead]</li> 
    </ul> <p>Voor meer informatie over de Status van een project, zie <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md"> Toegang tot de lijst van de statussen van het systeemproject </a>.</p>
    <p>Voor taken is [!UICONTROL Status] een instelling op de taak die aangeeft of de taak:</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Complete]</li> 
    </ul> <p>Voor meer informatie over taakstatus, zie <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md"> Toegang tot de lijst van de statussen van de systeemtaak </a></p> <p>Voor problemen is de instelling [!UICONTROL Status] een instelling voor het probleem die aangeeft of dit probleem:</p> 
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
    </ul> <p>Voor meer informatie over uitgiftestatussen, zie <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref"> Toegang tot de lijst van de statussen van de systeemkwestie </a>.</p> 
    <p>Voor strategische doelstellingen is [!UICONTROL Status] een instelling op het doel die aangeeft of het doel:</p> 
     <ul> 
      <li>[!UICONTROL Active]</li> 
      <li>[!UICONTROL Draft]</li> 
      <li>[!UICONTROL Inactive]</li> 
      <li>[!UICONTROL Closed]</li> 
     </ul> 
     <p>Voor meer informatie over strategische doelstellingen, zie ook "[!UICONTROL Goal]"of "[!UICONTROL Goals]"in dit artikel. </p> 
     <p>Voor strategische doelen is dit veld alleen zichtbaar als uw organisatie [!DNL Workfront Goals] heeft aangeschaft. Voor informatie over het beheren van strategische doelstellingen die [!DNL Workfront Goals] gebruiken, zie <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] overzicht </a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Change]</td> 
   <td>An [!UICONTROL Audit Trail]. Een nota wordt geproduceerd wanneer een gebruiker de Status van het project, de taak, of de kwestie verandert.</td> 
  </tr> 
  <tr> 
   <td>Statuspictogrammen</td> 
   <td> <p>U kunt het ingebouwde veld [!UICONTROL Status Icons] als kolom toevoegen in uw weergaven om de zichtbaarheid te verbeteren in belangrijke punten van uw objecten, zoals:</p> 
    <ul> 
     <li>Een object bevat documenten</li> 
     <li>Een object is gekoppeld aan een goedkeuringsproces</li> 
     <li>Aan een object zijn aanvullende notities gekoppeld</li> 
     <li>Een last is factureerbaar of terugbetaalbaar </li> 
     <li>Een taak bevindt zich op een kritiek pad</li> 
     <li>Een gebruiker behoort tot een bedrijf, een team, of is gevestigd in een verschillende tijdzone </li> 
    </ul> <p>U kunt het veld [!UICONTROL Status Icons] toevoegen in de weergaven van de volgende objecten: </p> 
    <ul> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Template Tasks]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Users]</li> 
    </ul> <p>Voor meer informatie, zie <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref"> Ingebouwde pictogrammen van de Status in Meningen </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Update]</td> 
   <td> <p>In een project, een taak, of een uitgifterapport, toont dit gebied de meest recente statusupdate die de objecten eigenaars in het "[!UICONTROL Updates]"gebied hebben verstrekt. Voor projecten betekent dit dat opmerkingen van de eigenaar van het project, en voor taken en kwesties, dat de opmerkingen van de ondertekenaars zijn.</p> 
   <p> Opmerkingen die zijn gemaakt bij het bijwerken van de status van een object, worden niet weergegeven in de kolom [!UICONTROL Status Update] .</p> <p>Om '[!UICONTROL New],' '[!UICONTROL In Process],' en '[!UICONTROL Complete]' statussen te tonen, gebruik de [!UICONTROL Status] kolom.</p> <p>Voor meer informatie over statussen, zie de de taakstatus van de artikel <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref"> Update </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Statuses]</td> 
   <td>Zie [!UICONTROL Status] in dit artikel.</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>Een grafiek die de status van artikelen (taken in de Agile-methodologie) en hoe ze vorderen in de richting van voltooiing.</td> 
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
   <p><code>[!UICONTROL stretch]</code> wordt gebruikt om te identificeren welke kolommen extra ruimte innemen die niet nodig is voor de weergave. De breedte van de gebruikersinterface van de werkruimte voor een standaardgebruiker is ongeveer 850 pixels. Dit betekent dat als u een mening met vier hebt
   de kolommen (150 pixel elk) die uw mening 600 van 850 pixel bezet. Er zijn 250 extra pixel in UI die aan de kolommen zullen worden toegevoegd die een rekbaarheidspercentage hebben verstrekt. </p>
   <p>Het uitrekken van een kolom wordt afgedwongen wanneer u de extra coderegel: <code>[!UICONTROL usewidths=true]</code> gebruikt voor ten minste een van de kolommen in de weergave. 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Subscribers]</td> 
   <td> <p>Gebruikers die zich abonneren op projecten, taken of problemen.</p> <p>Wanneer u dit gebied in een rapport gebruikt, toont een lijst van abonnees, met elke abonnee die door een komma wordt gescheiden.</p> <p>Voor meer informatie, zie het artikel <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref"> Abonneren aan punten in [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Summary Task]</td> 
   <td>Zie [!UICONTROL Parent Task] in dit artikel.</td> 
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
   <td> <p>Een activiteit die als stap naar het bereiken van een definitief doel (het voltooien van het Project) moet worden uitgevoerd.</p>

<p>Taken zijn kleinere werkeenheden die uiteindelijk een project voltooien, dat een grotere werkeenheid vertegenwoordigt.</p>
   <p>Taken kunnen nooit zelfstandig bestaan. Ze maken altijd deel uit van een project. </p>
   <p>Voor meer informatie over taken, zie <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref"> het overzicht van Taken </a>.</p> 
   <p>Voor informatie over het creëren van taken, zie <a href="/help/quicksilver/manage-work/tasks/create-tasks/create-tasks-in-project.md"> taken in een project </a> creëren
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Attribute]</td> 
   <td>Andere velden of objecten die zijn gekoppeld aan een taak en die bepaalde details over de taak aangeven. Sommige voorbeelden zijn [!UICONTROL Planned Completion Date] en [!UICONTROL Status] .</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Constraint]</td> 
   <td>Zie "[!UICONTROL Constraint Type]"en "[!UICONTROL Constraint Date]".</td> 
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
   <td> <p>Een inzameling van gebruikers die aan gelijkaardige doelstellingen of bedrijfsdoelstellingen werken. Deze gebruikers kunnen collectief aan een het werkpunt worden toegewezen door het team aan het het werkpunt toe te wijzen.</p> <p>Voor meer informatie over Teams, zie <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref"> overzicht van Teams </a>.</p> <p>Projecten kunnen een lus [!UICONTROL Project Team] hebben, die alle gebruikers of rollen bevat die zijn gekoppeld aan het werk aan het project.</p> <p>Voor meer informatie over de Teams van het Project, zie <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref"> Overzicht van het Team van het Project </a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Template]</td> 
   <td> <p>De malplaatjes van het project zijn generische overzichten van uw meest herhaalbare projecten. U kunt taken, rijonderwerpen, douaneformulieren bepalen, documenten of goedkeuringen vastmaken wanneer u een projectmalplaatje creeert om u tijd te besparen wanneer u een nieuw project moet creëren. </p> <p>U kunt malplaatjes aan bestaande projecten vastmaken, of u kunt hen gebruiken om nieuwe projecten te bouwen. Alle informatie die op het malplaatje wordt gespecificeerd brengt naar de projecten over die gebruikend het worden gecreeerd. </p> <p>Voor meer informatie over malplaatjes, zie <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md"> overzicht van het malplaatje van het Project </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Template Task]</td> 
   <td>Een taak die deel uitmaakt van een sjabloon. De Taken van het malplaatje worden Taken in het project dat door het malplaatje wordt gecreeerd te gebruiken.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>A [!UICONTROL Note] en de verzameling reacties die betrekking hebben op een bepaald onderwerp.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thumbnail]</td> 
   <td> <p> In een [!UICONTROL Document] -lijst of -rapport wordt een voorbeeld van het document in een miniatuur weergegeven. </p> <p> Selecteren <strong>[!UICONTROL Thumbnail]</strong>  om een miniatuur van 33 tot 66 pixels breed in het rapport weer te geven. </p> <p>De grootte van de miniatuur wordt aangepast wanneer u de breedte van de kolom in een lijst of rapport wijzigt.</p> <p>Zie ook "[!UICONTROL Large Thumbnail]"in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time Off]</td> 
   <td>U kunt een [!UICONTROL Time Off] -rapport maken om te bekijken wanneer gebruikers in hun profiel tijd uit hebben aangegeven. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet]</td> 
   <td> <p>Een tijdschema dat gebruikers toestaat om daadwerkelijke uren in te gaan dat zij het werken aan projecten, taken, of kwesties, of uren besteedden zij aan andere activiteiten niet verwant met het werk, zoals vergaderingen of opleiding. Naast het ingaan van de hoeveelheid tijd u het werken besteedde, kunt u ook erop wijzen of de tijd werk-verwant is of het aan overheadtijd door de Types van Uur te gebruiken om uw tijdingangen te bepalen is. Voor informatie over timesheets, zie <a href="../../../timesheets/timesheets/timesheets-overview.md"> Overzicht Timesheets </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet Profile]</td> 
   <td> <p>Een [!UICONTROL Timesheet Profile] is een sjabloon die [!DNL Workfront] gebruikt om automatisch tijdbladen te maken voor de gebruikers die eraan zijn gekoppeld. </p> <p>U kunt een aantal montages vormen die op elk timesheet zullen van toepassing zijn aangezien het wordt gecreeerd. Enkele van deze instellingen zijn: hoe vaak de tijdpagina moet worden gemaakt (wekelijks, om de week, twee keer per maand of maandelijks), de startdag van het tijdlijnoverzicht, de fiatteurs van het tijdlijnoverzicht en de beschikbare [!UICONTROL Hour Types] die gebruikers kunnen koppelen aan opgenomen uren.</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL Top Parent ID] </td> 
   <td> <p>Met dit veld kunt u gegevens over een groep op hoofdniveau en de bijbehorende subgroepen in een lijst of rapport identificeren en filteren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Top Parent Name] </td> 
   <td> <p>Met dit veld kunt u gegevens over een groep op hoofdniveau en de subgroepen ervan identificeren in een [!UICONTROL View] voor een lijst of rapport.</p> <p>U kunt dit ook doen met het veld [!UICONTROL Top Parent ID] .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total Hours]</td> 
   <td> <p>In een [!UICONTROL project report] wordt in dit veld de afgeronde som van alle uren van het project weergegeven, de laatste keer dat de projectfinanciering werd berekend. [!UICONTROL Actual Hours] geeft de exacte uren weer die zijn aangemeld voor het project. De [!UICONTROL Actual Hours] moet normaal gesproken overeenkomen met de [!UICONTROL Total Hours] . Als [!UICONTROL Total Hours] aanzienlijk anders wordt weergegeven dan in het veld [!UICONTROL Actual Hours] , moet u de financiën voor het project opnieuw berekenen.</p> <p>Voor meer informatie over het opnieuw berekenen van projectfinanciën, zie het artikel <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref"> projectfinanciën </a> opnieuw berekenen.</p> <p>In een timesheet [!UICONTROL Standard] mening, verwijst dit gebied naar de totale uren die voor punten voor de data worden geregistreerd die op timesheet worden getoond. Het [!UICONTROL Total Hours] gebied voor timesheets in deze ingebouwde meningsverwijzingen "[!UICONTROL hoursDuration]"gebied dat dynamisch het verschil in uren tussen de timesheet- Begin en einddata berekent. Dit wordt gebruikt om de kolom [!UICONTROL Total Hours] in rood weer te geven als de gebruiker zich meer tijd dan de beschikbare uren in het tijdspad van de tijdpagina aanmeldt. Voor meer informatie, zie <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref"> Totale uren van de Mening op timesheet </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tracking Mode]</td> 
   <td> <p>An attribute of a task. Hiermee bepaalt u hoe en wanneer de geprojecteerde tijdlijnen worden bijgewerkt voor een taak. Bijvoorbeeld:</p> 
    <ul> 
     <li>[!UICONTROL User Must Update] vereist dat een taak handmatig wordt bijgewerkt. Anders wordt het [!UICONTROL Behind Schedule] en vervolgens [!UICONTROL Late] .</li> 
     <li>[!UICONTROL Auto Complete] automatisch een taak voltooien wanneer de Vervaldatum (of [!UICONTROL Planned Completion Date] ) is verstreken.</li> 
    </ul> <p>Voor meer informatie, zie <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref"> het Volgen van de Taak overzicht van de Wijze </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Trigger]</td> 
   <td>Een gebeurtenis die een scenario start.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trouble Task]</td> 
   <td>Een onvolledige taak met de voorwaarde [!UICONTROL Late], [!UICONTROL Behind Schedule] of [!UICONTROL At Risk] .</td> 
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
    </ul> <p>Voor meer informatie, zie <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref"> het Type van projectupdate selecteren </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User]</td> 
   <td>Een account die is gemaakt in [!DNL Workfront] om een persoon in staat te stellen zich aan te melden en met het systeem te communiceren.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL User Delegation]</p> </td> 
   <td> <p>Een te rapporteren object dat u het volgende vertelt:</p> 
    <ul> 
     <li>Welke gebruikers taak, kwestie, en projectgoedkeuringen hebben gedelegeerd</li> 
     <li>Welke gebruikers taak, kwestie en projectgoedkeuringen hebben gehad die aan hen worden gedelegeerd</li> 
     <li>Wanneer deze delegaties beginnen en eindigen</li> 
    </ul> <p>Meer leren, zie <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref"> een rapport van de Delegatie van de Gebruiker </a> creëren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface]</td> 
   <td>Alle visuele en interactieve aspecten van de [!DNL Workfront] -toepassing.</td> 
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
   <td> <p>Een onderzoek dat met een rapport wordt gecombineerd dat toont hoe de Gebruikers (Middelen) worden toegewezen of over-toegewezen. Zie [!UICONTROL Resource Utilization] in dit artikel.</p> </td> 
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
   <p> De mening verwijst ook naar het recht van een gebruiker om informatie over een voorwerp slechts te bekijken, volgens hun toegangsniveau of op een toestemmingendelend niveau op dat voorwerp.</p> 
   <p>In de Planning van Workfront, verslagenvertoning op de verslagtype pagina in één van de volgende meningstypes:</p>
   <ul><li>Tabel</li>
   <li>Tijdlijn</li>
   <li>Kalender</li></ul>
   <p>In de Planning van Workfront, omvatten de meningen de filters, de groeperingen, het sorteren, en andere montages die op de verslagen op het scherm worden toegepast.</p> <p>Voor informatie, zie <a href="/help/quicksilver/planning/views/manage-record-views.md"> verslagmeningen </a> leiden.</p>   
   <p>Voor Workfront Planning is een extra licentie vereist.</p>
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL View Icons]</td> 
   <td> <p> Dit is hetzelfde veld als statuspictogrammen, maar het is alleen beschikbaar voor de volgende weergaven: </p> 
    <ul> 
     <li> [!UICONTROL Documents] </li> 
    </ul> <p> Voor meer informatie, zie de artikel <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref"> Ingebouwde Pictogrammen van de Status in Meningen </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Month]</td> 
   <td> <p>In een rapportlijst, toont het het aantal tijden het rapport tijdens de laatste maand is bekeken.<br> voor meer informatie over gebruiksinformatie in rapportlijsten, zie het het rapportgebruik van het artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref"> Mening </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Quarter]</td> 
   <td>In een rapportlijst, toont het het aantal tijden het rapport tijdens het laatste kwartaal is bekeken.<br> voor meer informatie over gebruiksinformatie in rapportlijsten, zie het het rapportgebruik van het artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" > Mening </a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Year]</td> 
   <td>In een rapportlijst, toont het het aantal tijden het rapport tijdens het laatste jaar is bekeken.<br> voor meer informatie over gebruiksinformatie in rapportlijsten, zie het het rapportgebruik van het artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref"> Mening </a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Month]</td> 
   <td> <p>In een rapportlijst, toont het het aantal tijden het rapport tijdens deze maand is bekeken.<br> voor meer informatie over gebruiksinformatie in rapportlijsten, zie het het rapportgebruik van het artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref"> Mening </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Quarter]</td> 
   <td>In een rapportlijst, toont het het aantal tijden het rapport tijdens dit kwartaal is bekeken.<br> voor meer informatie over gebruiksinformatie in rapportlijsten, zie het het rapportgebruik van het artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref"> Mening </a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Year]</td> 
   <td>In een rapportlijst, toont het het aantal tijden het rapport tijdens dit jaar is bekeken.<br> voor meer informatie over gebruiksinformatie in rapportlijsten, zie het het rapportgebruik van het artikel <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md"> Mening </a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> In een rapport, wanneer het gebruiken van de [!UICONTROL Text Mode] interface, de lijn van code waar u de breedte van elke kolom in pixel kunt specificeren. Workfront geeft een aanbevolen breedte voor elk veld.
Afhankelijk van het type veld en de notatie kunt u wel aanpassingen aanbrengen.
U moet de extra <code>[!UICONTROL usewidths=true]</code> coderegel gebruiken om de voor de kolom opgegeven breedte in te stellen. 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>In een project, een taak, of een uitgifterapport, die de volgende verklaring op tekstwijze gebruiken toont de Geplande Uren van het project, de taak, of de kwestie:</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>Voor informatie over het gebruiken van tekstwijze, zie <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref"> overzicht van de wijzesyntaxis van de Tekst </a>. </p> 
   <p><b> TIP </b> 
   <p>In een puntenrapport, voegt het toevoegen van één van de [!UICONTROL Planned Hours] gebieden het <code>work </code> gebied aan het rapport toe. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work]</td> 
   <td> <p>Een van de twee primaire licentietypen. Dit heeft minder toegang dan [!UICONTROL Plan], maar kan updates in het systeem tot stand brengen en maken. Een gebruiker met een werkvergunning heeft meer mogelijkheden dan een [!UICONTROL External], [!UICONTROL Reviewer], of [!UICONTROL Requester] vergunninghouder.</p> <p>Zie <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] Overzicht van licenties </a> voor meer informatie.</p> <p>Het werk kan verwijzen naar het aantal [!UICONTROL Planned Hours] voor een project, taak of kwestie. Voor meer informatie, zie het "[!UICONTROL work]"gebied in deze lijst. </p> <p><b>TIP</b></p> <p> In een puntenrapport, voegt het toevoegen van één van de [!UICONTROL Planned Hours] gebieden het <code>work </code> gebied aan het rapport toe. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Breakdown Structure]</td> 
   <td>Een hiërarchische structuur van de taken die door het projectteam moeten worden uitgevoerd die op de ouder/kindverhouding wordt gebaseerd.</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Work Effort] </td> 
   <td> 
    <p>Een projectmanager zou kunnen besluiten om dit gebied in plaats van [!UICONTROL Planned Hours] te gebruiken om de inspanning te schatten nodig om een taak te voltooien. Dit veld is alleen zichtbaar als aan de volgende voorwaarden is voldaan:</p> 
     <ul> 
      <li> <p>De taak heeft een [!UICONTROL Simple Duration Type] . </p> <p><b>TIP</b></p> <p> Als u de taak [!UICONTROL Duration Type] bijwerkt naar een ander type, wordt dit veld verborgen. </p> </li> 
      <li>De projectmanager heeft [!UICONTROL Use Work Effort] in staat gesteld om het taak [!UICONTROL Planned Hours] gebied op het project automatisch te berekenen. </li> 
     </ul> 
     <p>Voor informatie over het gebruiken van [!UICONTROL Work Effort] in plaats van [!UICONTROL Planned Hours] om taakinspanning te schatten, zie <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref"> Overzicht van de Werkinspanning van het Werk </a>. </p> 
     <p>U kunt dit veld weergeven in taakrapporten en lijsten.</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Work Item]</td> 
   <td> <p>Dit veld verwijst naar taken of problemen in [!DNL Workfront] . </p> <p>Het [!UICONTROL Work Item] -rapport bevat informatie voor zowel taken als problemen. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management mix]</td> 
   <td>Een [!UICONTROL Work Performance Indicator] (WPI) van het deel van het werk dat wordt toegewezen om uw zaken in werking te stellen tegenover verandering uw zaken. Met Mix WPI kunt u op organisatorisch niveau begrijpen of er op uw strategie een werkelijke werktoewijzing is toegepast.</td> 
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
   <td>In het [!UICONTROL Proof Approval] -rapport worden in dit veld workflowsjablonen weergegeven die aan een proefdruk zijn gekoppeld. Als er geen sjablonen zijn gekoppeld, is de kolom leeg.</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Work Time]</td> 
   <td>

<p>Vertegenwoordigt het percentage van de Equivalente van de Volledige Tijd ([!UICONTROL FTE]) tijd dat de gebruiker voor werkelijk werk, exclusief overheadkosten beschikbaar is. [!UICONTROL Work Time] moet een decimaal getal tot en met 1 zijn en mag niet 0 zijn. Een beschikbaarheid van 20% voor werkelijk werk zou bijvoorbeeld 0,2 zijn.</p>
   </p>De standaardwaarde van het veld is 1. Dit geeft aan dat een gebruiker de volledige [!UICONTROL FTE] besteedt aan daadwerkelijk, projectgerelateerd werk.  </p>
   <p>Het systeem gebruikt dit aantal om de beschikbaarheid van de gebruiker voor daadwerkelijke, op project betrekking hebbende werk te berekenen. </p>
   <p> De uitzonderingen van het programma en de onderbreking van het programma zouden ook de gebruikerscapaciteit kunnen beïnvloeden. </p>
   <p>Voor meer informatie over het creëren van programma's in Workfront, zie <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md"> een programma </a> creëren. </p>
    <p>Workfront berekent de beschikbaarheid van een gebruiker op basis van de voorkeuren voor Resource Management in het [!UICONTROL Setup] -gebied. Voor meer informatie, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/"> de voorkeur van het Beheer van het Middel </a> vormen. </p> 
   <p>U kunt de [!UICONTROL Work Time] van een gebruiker bijwerken wanneer u de gebruiker bewerkt of maakt. Voor informatie, zie <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md"> het profiel van een gebruiker </a> uitgeven</p> 
   <b> TIP </b> 
   <p>Stel de [!UICONTROL Work Time] -waarde in op 1 om aan te geven dat de gebruiker beschikbaar is voor projectgerelateerd werk en dat het volledige equivalent in voltijd overeenkomt.</p> 
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
    <p>Voor informatie over het gebruiken van tekstwijze, zie <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref"> overzicht van de wijzesyntaxis van de Tekst </a>. </p> </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Workspace] </td> 
   <td> <p>In de Planning van Workfront, is een werkruimte een inzameling van verslagtypes die de operationele levenscyclus van een bepaalde organisatie bepalen. Een werkruimte is het werkkader van een organisatorische eenheid.</p>
   <p>Voor Workfront Planning is een extra licentie vereist. </p>
   <p>Voor informatie, zie <a href="/help/quicksilver/planning/architecture/create-workspaces.md"> werkruimten </a> creëren. </p> </td> 
  </tr> 
 </tbody> 
</table>


