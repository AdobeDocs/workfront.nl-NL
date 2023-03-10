---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Handelingen die moeten worden uitgevoerd na de installatie van een blauwdruk
description: In dit artikel wordt beschreven wat u moet doen nadat u een blauwdruk hebt geïnstalleerd in [!DNL Adobe Workfront] om de blauwdruk volledig op te stellen voor uw systeemgebruikers.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '1136'
ht-degree: 0%

---

# Handelingen die moeten worden uitgevoerd na de installatie van een blauwdruk

In dit artikel wordt beschreven wat u moet doen nadat u een blauwdruk hebt geïnstalleerd in [!DNL Adobe Workfront] om de blauwdruk volledig op te stellen voor uw systeemgebruikers.

* [Aanbevelingen voor projectsjablonen](#project-template-recommendations)
* [Aanbevelingen inzake de organisatiestructuur](#organizational-structure-recommendations)
* [Aanbevelingen voor het dashboard](#dashboard-recommendations)

## Aanbevelingen voor projectsjablonen {#project-template-recommendations}

Deze sectie bevat aanbevelingen voor de projectmalplaatjes die met uw blauwdrukken worden geïnstalleerd.

### Gebruikers toewijzen aan nieuwe rollen en teams {#assign-users-to-newly-created-roles-and-teams}

De rollen en/of de teams die tijdens het proces van de blauwdrukinstallatie worden gecreeerd hebben geen gebruikers automatisch verbonden aan hen. Zonder gebruikers toe te wijzen aan de onlangs toegevoegde rollen of teams, zult u werk voor een functie tot stand brengen die niemand zal opnemen. In sommige gevallen, zou u nieuwe gebruikers kunnen moeten creëren om deze rollen en teams te vullen. Voor informatie over het maken van nieuwe gebruikers raadpleegt u [Gebruikers toevoegen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### Een aangepast formulier toepassen op de sjabloon en de sjabloontaken {#apply-a-custom-form-to-the-template-and-the-template-tasks}

Het installatieproces koppelt de projectsjabloon niet aan aangepaste formulieren. Als voor uw projecten of taken specifieke formulieren of velden moeten worden ingevuld om consistentie in de rapportage te creëren, of als uw digitale aanvraagformulier velden bevat die op projectniveau moeten worden behouden, raden we u aan de sjabloon of de sjabloontaken aan die formulieren te koppelen. Zie voor meer informatie [Een aangepast formulier toevoegen aan een object](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### Tijdsduur en inspanningsramingen van sjabloontaken bijwerken {#update-template-task-duration-and-effort-estimates}

Elke taak in het malplaatje bevat een geplande duur en een geplande inspanningsraming. Deze ramingen dienen als uitgangspunt voor de duur en de tijd die voor deze activiteiten worden besteed. De mogelijkheden, vaardigheden en snelheid van uw organisatie zijn echter uniek. U zou de geschatte duur en de inspanning van elke taak moeten herzien om het aan te passen aan de behoeften van uw organisatie. Zie voor meer informatie [Taakgegevens beheren in het dialoogvenster [!UICONTROL Task Details Overview] gebied](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### Een milestone-pad en mijlpalen koppelen {#associate-a-milestone-path-and-milestones}

Het installatieproces koppelt het projectmalplaatje niet met een milestone weg. Pas een milestone-pad toe op de sjabloon en pas mijlpalen toe op belangrijke taken in de sjabloon ter ondersteuning van uw rapportagevereisten voor mijlpalen. Zie voor meer informatie [Mijlpalen koppelen aan taken](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### Het malplaatje aan uw team uitrollen {#roll-out-the-template-to-your-team}

Bereid opleidingsmateriaal voor zowel de werkmanagers die dit malplaatje zullen gebruiken als de individuele medewerkers voor die het werk binnen het projectmalplaatje zullen uitvoeren.

### Rapporten en dashboards maken of bijwerken {#create-or-update-reports-and-dashboards}

Als de oplossing een nieuw type werk vertegenwoordigt dat uw organisatie niet eerder in heeft uitgevoerd [!DNL Workfront]kunt u nieuwe rapporten en dashboards moeten creëren om het werk te steunen. Zie voor meer informatie [Een aangepast rapport maken](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) en [Een dashboard maken](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

Als de oplossing vergelijkbaar is met het werk dat u al hebt uitgevoerd in [!DNL Workfront], dan zou u moeten verifiëren dat het werk in bestaande rapporten en dashboards zoals verwacht voedt. Als dit item niet wordt meegenomen in uw bestaande rapportage, voert u actie om filters bij te werken of nieuwe rapporten te maken.

## Aanbevelingen inzake de organisatiestructuur {#organizational-structure-recommendations}

Deze sectie bevat aanbevelingen voor de organisatorische structuurelementen die met uw blauwdrukken worden geïnstalleerd.

### Bedrijven

Na het installeren van een blauwdruk die een bedrijf omvat:

* Voeg een aangepast formulier toe om het bedrijfsrecord te verfraaien met nuttige details (het formulier en de details zijn uniek voor u). Zie voor meer informatie [Een aangepast formulier toevoegen aan een object](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* Als het bedrijf een cliënt vertegenwoordigt, herzie de met het bedrijf verbonden met voeten treden tarieven. Zie voor meer informatie [Factureringstarieven voor de rol van de werknemer op bedrijfsniveau overschrijven](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* Als het bedrijf een cliënt vertegenwoordigt, en als er andere uniek-aan-dat-organisatie projectmalplaatjes zijn, preassocieer eerst de projectmalplaatjes met het onlangs toegevoegde bedrijf. Zie voor meer informatie [Projectsjablonen bewerken](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Als het bedrijf een cliënt of een verkoper vertegenwoordigt, associeer bestaande gebruikers van de externe organisatie die reeds in uw milieu kan zijn. Zie voor meer informatie [Bedrijven maken en bewerken](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* Als het bedrijf een cliënt of een verkoper vertegenwoordigt, creeer extra samenwerkende gebruikers voor de externe organisatie die u in uw milieu kunt nodig hebben om mededeling, werkuitvoering, en goedkeuringen te stroomlijnen. Voor informatie over het maken van nieuwe gebruikers raadpleegt u [Gebruikers toevoegen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Werk organisatorische grafiekverhoudingen voor om het even welke gebruikers bij nu verbonden aan het onlangs toegevoegde bedrijf. Zie voor meer informatie [Directe rapporten maken](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) en [Het organigram weergeven](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

Zie voor meer informatie over bedrijven [Bedrijven maken en bewerken](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Aanbevelingen voor het dashboard {#dashboard-recommendations}

Deze sectie bevat aanbevelingen voor de dashboards en de rapporten die met een blauwdruk worden geïnstalleerd.

### Pas gemaakte dashboards bijwerken om rapporten toe te voegen/te verwijderen

De dashboards die van een blauwdruk worden toegevoegd hebben één of meerdere rapporten, externe pagina&#39;s, of kalenders. Het is waarschijnlijk dat u niet alle rapporten en andere dashboardelementen nodig hebt, of dat u het dashboard moet uitbreiden met bestaande rapporten, externe pagina&#39;s en kalenders voordat het met anderen kan worden gedeeld. Zie voor meer informatie [Een rapport toevoegen aan een dashboard](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### Pas gemaakte rapporten bijwerken om kolommen of filtercriteria toe te voegen/te verwijderen

De rapporten die door een dashboardblauwdruk worden verdeeld hebben niet alle kolommen of filtercriteria om uw configuratie van te steunen [!DNL Workfront]. Naar verwachting zult u de rapporten op enkele punten aanpassen zodat deze aan uw normen voldoen. Om consistentie met andere rapporten in uw milieu te bouwen, kunt u een kolom willen toevoegen u op alle rapporten voor het voorwerp dat opneemt, of om sommige filtercriteria toe te voegen die resultaten aan een bepaald projecttype of een gebruikersgroep beperken. Zie voor meer informatie [Weergaven maken of bewerken](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) en [Filters maken of bewerken](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### De dashboards of rapporten delen met gebruikers

Als u het dashboard niet op een lay-outmalplaatje wilt plaatsen, zou u het dashboard met de mensen moeten delen die het nuttig zullen vinden. Zie voor meer informatie [Een dashboard delen](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) en [Een rapport delen](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### De dashboards toevoegen aan lay-outsjablonen

De beste manier om informatie beschikbaar te maken voor andere mensen is het toevoegen van dashboards aan lay-outmalplaatjes. Identificeer de lay-outmalplaatjes van de mensen die het meest van het herzien van het dashboard op een regelmatige basis zouden profiteren en voeg het nieuwe dashboard aan die lay-outmalplaatjes toe. Zie voor meer informatie [Lay-outsjablonen maken en beheren](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### Andere dashboards en rapporten bijwerken

Door de invoering van een nieuw dashboard en de bijbehorende verslagen kan het mogelijk zijn andere bestaande dashboards en rapporten af te schaffen en aan te passen. Neem de tijd om uw bestaande rapporten te herzien om het even welke overtollige en tegenstrijdige rapporten te identificeren.

### Aangepaste gegevens distribueren naar relevante formulieren

Sommige rapporten inbegrepen in een dashboardblauwdruk hebben de gebieden van douanegegevens in of de mening, de filter, of de groepering van het rapport. In sommige gevallen heeft de blauwdruk ook een formulier waaraan deze velden zijn gekoppeld. De aangepaste velden worden echter vaker dan niet toegepast op een aangepast formulier. De kolommen, filters of groepen werken alleen correct als deze velden zijn gekoppeld aan formulieren die zijn verbonden met een gebruiker, project, taak of andere objectreeks. Zie voor meer informatie [Een aangepast veld toevoegen aan een aangepast formulier](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
