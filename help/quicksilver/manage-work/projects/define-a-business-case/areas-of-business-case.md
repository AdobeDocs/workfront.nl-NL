---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Overzicht van de gebieden van de bedrijfscase
description: Dit artikel beschrijft de gebieden van het BedrijfsGeval van een project.
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 0%

---

# Overzicht van de gebieden van de bedrijfscase

Dit artikel beschrijft de gebieden van het BedrijfsGeval van een project.

Voor informatie over het creëren van een BedrijfsGeval voor een project, zie [Een bedrijfscase maken voor een project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Uw beheerder van Adobe Workfront of groepsbeheerder moet alle secties in het BedrijfsGeval toelaten alvorens zij op het project, behalve de sectie van Info van het Project zichtbaar zijn. Het gedeelte Projectinfo is standaard ingeschakeld.

Raadpleeg voor meer informatie over het inschakelen van de gebieden in de Business Case de sectie &quot;Business Case&quot; in  [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Hier volgt een overzicht van de gebieden in het Business Case van een project:

* Projectinfo
* Doelen
* Uitgaven
* Bronnen begroten
* Risico&#39;s
* Scorecard
* Aangepaste Forms
* Overzicht van bedrijfscase

## Projectinfo

De **Projectinfo** van de BedrijfsGeval is niet configureerbaar door de beheerder van Workfront. Alle projecten hebben een gebied van Info van het Project in het BedrijfsGeval. 

Het gedeelte Projectinfo van de bedrijfscase bevat de basisinformatie van een project, voordat het project daadwerkelijk is gestart.

U kunt de volgende velden bewerken:

* **Beschrijving**: Geef een beschrijving op voor uw project.
* **Projecteigenaar**

   Door gebrek, is de gebruiker die het project creeert ook de Eigenaar van het Project. U kunt dit gebied uitgeven en op een andere actieve gebruiker als eigenaar van het project wijzen.

* **Projectsponsor**

   U kunt ook iemand anders dan de projecteigenaar toevoegen als sponsor van het project. De sponsor ontvangt de goedkeuring van de Business Case. 

* **Portfolio**: Geef een Portfolio op voor het project. U moet de Portfolio maken en deze in de status van **Actief** voordat deze beschikbaar is om te selecteren in dit vervolgkeuzemenu.

   Zie voor meer informatie over portfolio&#39;s [Portfolio-overzicht in Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

   Voor meer informatie over het maken van Portfolio raadpleegt u [Een portfolio maken](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

* **Gepland voordeel**: Schatting wat het geldelijke voordeel voor uw organisatie gepland is wanneer dit project wordt voltooid. Het kan om het even welk bedrag van munt zijn en het moet een positieve waarde zijn. Bijvoorbeeld $10.000.
* **Status**: Door gebrek, wordt de Status voor een projectverzoek geplaatst aan **Idea**.

   Als u de Status in om het even wat buiten Idee of Planning verandert, **Verzenden** verdwijnt uit het gebied Business Case Summary en u kunt de Business Case niet langer ter goedkeuring verzenden. 

* **Vaste begindatum**: Geef een datum op waarop het project moet worden gestart.
* **Vaste einddatum**: Geef een datum op waarop het project moet worden beëindigd.

   >[!NOTE]
   >
   >De vaste begin- en einddatum in het bedrijfscase hebben geen invloed op de geplande begin- en einddatum van het project. Deze staan voor de data waarop de projectmaker het project ideaal zou ontwikkelen. In plaats daarvan geven de geplande aanvangs- en einddatum van het project de geplande tijdlijn voor het project aan, die is gebaseerd op de taken van het project.

## Doelen

Doelstellingen bepalen de doelstellingen van het project. Dit gebied is standaard ingeschakeld in het geval Business, maar de Workfront-beheerder kan ervoor kiezen dit gebied niet weer te geven. In dit veld worden de doelstellingen in volgorde van prioriteit weergegeven.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
U kunt strategische doelstellingen voor uw organisatie tot stand brengen die niet met de individuele BedrijfsGeval van een project worden verbonden. U moet toegang hebben tot Adobe Workfront-doelen om strategische doelen te kunnen maken. U kunt hen dan met projecten buiten hun Zaken verbinden. Voor informatie over het maken van doelen met behulp van Workfront Goals raadpleegt u [Overzicht van Adobe Workfront-doelen](../../../workfront-goals/goal-management/wf-goals-overview.md).

Het bepalen van de doelstellingen is facultatief voor het project om een Score in Portfolio te ontvangen Optimizer. Deze sectie is de enige optionele sectie in de Business Case. Alle andere secties van het BedrijfsGeval moeten worden voltooid alvorens het project in Portfolio Optimizer wordt gescoord. U kunt een prioriteitsniveau voor een doel aangeven terwijl u het doel maakt.

Voor meer informatie over doelstellingen, zie  [Zakelijke hoofddoelen maken](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## Uitgaven

De kosten vertegenwoordigen de niet-loonkosten die tijdens de looptijd van een project kunnen worden gemaakt. Dit gebied is standaard ingeschakeld in het geval Business, maar de Workfront-beheerder kan ervoor kiezen dit gebied niet weer te geven. 

Eventuele kosten die u in de Business Case opgeeft, worden ook op het tabblad Uitgaven van het project vermeld als geplande uitgaven.

De uitgaven beïnvloeden de volgende gebieden op het project:

* Geraamde kosten
* Nettowaarde

Voor meer informatie over de begrote Kosten en Netto Waarden, zie [Overzicht van de financiële vakgebieden Bedrijfscase](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Voor meer informatie over uitgaven, zie  [Projectkosten beheren](../../../manage-work/projects/project-finances/manage-project-expenses.md) .

Uw Workfront-beheerder kan aangepaste kostentypen instellen.

Voor meer informatie over het creëren van de Types van Uitgaven van douane, zie [Aangepaste uitgaventypen maken](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md). 

## Bronnen begroten

U kunt de volgende acties op het gebied van de Begroting van het Middel van de BedrijfsKwestie uitvoeren:

* Brongroepen koppelen aan het project.
* Maak een budget voor uw middelen op projectniveau.

De uren die voor de middelen op het project in de begroting worden opgenomen tonen op het gebied van de Begroting van het Middel van het BedrijfsGeval, die de Begrotende Arbeidskosten van het project produceren. Dit gedeelte van de Business Case is standaard ingeschakeld.

Voor meer informatie over het begroten van middelen voor het project in het BedrijfsGeval, zie [Begrotingsmiddelen in het bedrijfscase](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

![](assets/business-case-sp-selected-with-choose-button-350x121.png)

Overweeg het volgende wanneer het bekijken van de sectie van de Begroting van het Middel van het BedrijfsGeval:

* U kunt hier broninformatie begroten met behulp van de volgende hulpmiddelen:

   * De bronnenplanner

      Zie voor meer informatie [De middelen van de begroting in BedrijfsGeval die de Planner van het Middel gebruiken](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md).

   * Scenario Planner , als uw bedrijf een extra licentie voor Adobe Scenario Planner heeft gekocht

      Zie voor meer informatie [De middelen van de begroting in BedrijfsGeval die Scenario Planner gebruiken](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

      De Scenario Planner is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring en vereist een aanvullende licentie. Voor informatie over de Workfront Scenario Planner raadpleegt u [Overzicht van de functie Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

* De informatie die hier wordt getoond toont ook in de Planner van het Middel op systeemniveau of de Planner van het Scenario. 

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* Na het begroten van uw middelen, tonen de Begroeide Arbeidskosten van het project in het gebied van de Begroting van het Middel als de rollen met Kosten per uren worden geassocieerd. De begrote arbeidskosten worden weergegeven in de valuta van het project.

   >[!IMPORTANT]
   De begrote arbeidskosten zijn de kosten verbonden aan de rollen op het project, en niet aan de gebruikers. De som van alle begrote arbeidskosten voor de gebruikers kan al dan niet gelijk zijn aan de begrote arbeidskosten van de aan de gebruikers gekoppelde functie. 

   Voor meer informatie over de begrote arbeidskosten, zie [Overzicht van de financiële vakgebieden Bedrijfscase](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

   Voor meer informatie over het creëren van baanrollen en het associëren van Kosten per uren tarieven met hen, zie [Taakrollen maken en beheren](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## Risico&#39;s

Risico&#39;s zijn factoren die kunnen verhinderen dat een project op tijd of op de begroting wordt afgerond. Het definiëren van deze factoren is belangrijk voor de Portfolio-beheerder of de projectsponsor om een gefundeerd besluit te nemen over de goedkeuring van het project. Dit gebied is standaard ingeschakeld in het geval Business, maar de Workfront-beheerder kan ervoor kiezen dit gebied niet weer te geven.

U kunt potentiële kosten met de risico&#39;s associëren u bepaalt voor het geval zij zouden moeten voorkomen. De kosten van de risico&#39;s voor een project zijn van invloed op de nettowaarde van het project. 

Voor meer informatie over de Netto Waarde van het project, zie [Overzicht van de financiële vakgebieden Bedrijfscase](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Zie voor meer informatie over het maken van risico&#39;s  [Risico&#39;s maken en bewerken voor projecten](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

Uw Workfront-beheerder kan aangepaste typen risico instellen.

Voor meer informatie over het creëren van en het uitgeven van de Types van Risico van douane, zie [Risicotypen bewerken en maken](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

## Scorecard

Scorecards meten de Uitlijning van het project. Dit gebied is standaard ingeschakeld in het geval Business, maar de Workfront-beheerder kan ervoor kiezen dit gebied niet weer te geven.

Voor meer informatie over het toepassen van een scorecard op een project en het produceren van een groeperingsscore, zie [Pas een scorecard op een project toe en produceer een Score van de Uitlijning](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Als u een scorecard wilt toepassen, moet uw Workfront-beheerder er een maken. De **Scorecard** in de Business Case-weergave wordt alleen weergegeven als er een scorecard is gemaakt.

Voor meer informatie over het creëren van een scorecard, zie  [Een scorecard maken](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Aangepaste Forms

Bij het definiëren van een bedrijfscase kunt u Aangepaste Forms aan een project koppelen. Dit gebied is niet standaard ingeschakeld in het geval Business. De beheerder van Workfront moet het toelaten om het in het BedrijfsGeval te tonen.

Voor meer informatie over het toelaten van de gebieden van het BedrijfsGeval, zie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Als u een aangepast formulier wilt toepassen, moet uw Workfront-beheerder eerst een aangepast formulier maken.

Voor meer informatie over het maken van een aangepast formulier raadpleegt u [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

U kunt aangepaste formulieren gebruiken voor het verzamelen van aanvullende informatie die niet wordt weergegeven in de andere velden van de kwestie Business.

Zie voor meer informatie over het toepassen van een aangepast formulier [Een aangepast formulier toevoegen aan een bedrijfscase](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md).

## Overzicht van bedrijfscase

* [Overzicht van de samenvatting van bedrijfscase](#overview-of-the-business-case-summary)
* [De Business Case exporteren](#export-the-business-case)

### Overzicht van de samenvatting van bedrijfscase {#overview-of-the-business-case-summary}

U kunt een samenvatting van de belangrijkste projectfinanciën zien en of een project of niet met een Scorecard in het BedrijfsGevallenoverzicht, in de hogere juiste hoek van de BedrijfsGeval wordt gericht.

U kunt de samenvatting van bedrijfscase niet bewerken. Dit is slechts een kort overzicht van de stand van zaken van het project, aangezien het betrekking heeft op financiële gebieden en het scorebord. \
 

De volgende velden worden weergegeven in het Business Case Summary:

* De nettowaarde van het project
* De begrote kosten van het project
* De potentiële risicokosten
* Het geplande voordeel
* De uitlijningsscore

Zie voor meer informatie over deze velden [Overzicht van de financiële vakgebieden Bedrijfscase](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

### De Business Case exporteren {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

U kunt de Business Case naar een PDF-bestand exporteren, voor het geval u deze wilt afdrukken of in een gecondenseerde indeling aan een e-mailbericht wilt koppelen. 

Zie voor meer informatie [De bedrijfscase van een project exporteren](../../../manage-work/projects/define-a-business-case/export-business-case.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To export a Business Case:</p>
<ol>
<li value="1">Go to the <strong>Business Case</strong> area of a project. </li>
<li value="2"> <p>In the<strong>Business Case Summary</strong> area, click <strong>Export</strong>.<br>A PDF file is downloaded to your computer. The file contains all areas of the Business Case in an easy to read format.</p> <p> <img src="assets/bc-summary-exported-350x160.png" alt="BC_Summary_exported.png" style="width: 350;height: 160;"> </p> </li>
<li value="3">(Optional) You can attach the PDF file to an email, or print it.&nbsp;</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>You can export the Business Case to a PDF file, in case you need to print it or attach it to an email in a more condensed format.&nbsp; The file contains all areas of the Business Case in an easy to read format.</p>
<p>For information about how to export the Business Case, see <a href="../../../manage-work/projects/define-a-business-case/export-business-case.md" class="MCXref xref">Export the Business Case of a project </a></p> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and will replace the info above, when the standalone arrticle is live >> Becky!)</p>
-->
</div>
--&gt;
