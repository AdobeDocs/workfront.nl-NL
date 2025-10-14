---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Handelingen die moeten worden uitgevoerd na de installatie van een blauwdruk
description: Dit artikel schetst wat u zou moeten doen nadat u een blauwdruk in  [!DNL Adobe Workfront]  installeert om de blauwdruk aan uw systeemgebruikers volledig op te stellen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1132'
ht-degree: 0%

---

# Handelingen die moeten worden uitgevoerd na de installatie van een blauwdruk

Dit artikel beschrijft wat u zou moeten doen nadat u een blauwdruk in [!DNL Adobe Workfront] installeert om de blauwdruk aan uw systeemgebruikers volledig op te stellen.

* [Aanbevelingen voor projectsjablonen](#project-template-recommendations)
* [Aanbevelingen inzake de organisatiestructuur](#organizational-structure-recommendations)
* [Aanbevelingen voor het dashboard](#dashboard-recommendations)

## Aanbevelingen voor projectsjablonen {#project-template-recommendations}

Deze sectie bevat aanbevelingen voor de projectmalplaatjes die met uw blauwdrukken worden geïnstalleerd.

### Gebruikers toewijzen aan nieuwe rollen en teams {#assign-users-to-newly-created-roles-and-teams}

De rollen en/of de teams die tijdens het proces van de blauwdrukinstallatie worden gecreeerd hebben geen gebruikers automatisch verbonden aan hen. Zonder gebruikers toe te wijzen aan de onlangs toegevoegde rollen of teams, zult u werk voor een functie tot stand brengen die niemand zal opnemen. In sommige gevallen, zou u nieuwe gebruikers kunnen moeten creëren om deze rollen en teams te vullen. Voor informatie bij het creëren van nieuwe gebruikers, zie [&#x200B; gebruikers &#x200B;](../../administration-and-setup/add-users/create-and-manage-users/add-users.md) toevoegen.

### Een aangepast formulier toepassen op de sjabloon en de sjabloontaken {#apply-a-custom-form-to-the-template-and-the-template-tasks}

Het installatieproces koppelt de projectsjabloon niet aan aangepaste formulieren. Als voor uw projecten of taken specifieke formulieren of velden moeten worden ingevuld om consistentie in de rapportage te creëren, of als uw digitale aanvraagformulier velden bevat die op projectniveau moeten worden behouden, raden we u aan de sjabloon of de sjabloontaken aan die formulieren te koppelen. Voor informatie, zie [&#x200B; een douanevorm aan een voorwerp &#x200B;](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toevoegen.

### Tijdsduur en inspanningsramingen van sjabloontaken bijwerken {#update-template-task-duration-and-effort-estimates}

Elke taak in het malplaatje bevat een geplande duur en een geplande inspanningsraming. Deze ramingen dienen als uitgangspunt voor de duur en de tijd die voor deze activiteiten worden besteed. De mogelijkheden, vaardigheden en snelheid van uw organisatie zijn echter uniek. U zou de geschatte duur en de inspanning van elke taak moeten herzien om het aan te passen aan de behoeften van uw organisatie. Voor informatie, zie [&#x200B; taakinformatie in het [!UICONTROL Task Details Overview] gebied &#x200B;](../../manage-work/tasks/manage-tasks/task-information-in-overview.md) beheren.

### Een milestone-pad en mijlpalen koppelen {#associate-a-milestone-path-and-milestones}

Het installatieproces koppelt het projectmalplaatje niet met een milestone weg. Pas een milestone-pad toe op de sjabloon en pas mijlpalen toe op belangrijke taken in de sjabloon ter ondersteuning van uw rapportagevereisten voor mijlpalen. Voor informatie, zie [&#x200B; mijlpalen met taken &#x200B;](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md) associëren.

### Het malplaatje aan uw team uitrollen {#roll-out-the-template-to-your-team}

Bereid opleidingsmateriaal voor zowel de werkmanagers die dit malplaatje zullen gebruiken als de individuele medewerkers voor die het werk binnen het projectmalplaatje zullen uitvoeren.

### Rapporten en dashboards maken of bijwerken {#create-or-update-reports-and-dashboards}

Als de oplossing een nieuw type werk vertegenwoordigt dat uw organisatie niet eerder in [!DNL Workfront] heeft uitgevoerd, kunt u nieuwe rapporten en dashboards moeten tot stand brengen om het werk te steunen. Voor informatie, zie [&#x200B; een douanerapport &#x200B;](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren en [&#x200B; een dashboard &#x200B;](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md) creëren.

Als de oplossing vergelijkbaar is met het werk dat u al hebt uitgevoerd in [!DNL Workfront] , moet u controleren of het werk doorwerkt in bestaande rapporten en dashboards zoals u had verwacht. Als dit item niet wordt meegenomen in uw bestaande rapportage, voert u actie om filters bij te werken of nieuwe rapporten te maken.

## Aanbevelingen inzake de organisatiestructuur {#organizational-structure-recommendations}

Deze sectie bevat aanbevelingen voor de organisatorische structuurelementen die met uw blauwdrukken worden geïnstalleerd.

### Bedrijven

Na het installeren van een blauwdruk die een bedrijf omvat:

* Voeg een aangepast formulier toe om het bedrijfsrecord te verfraaien met nuttige details (het formulier en de details zijn uniek voor u). Voor informatie, zie [&#x200B; een douanevorm aan een voorwerp &#x200B;](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toevoegen.
* Als het bedrijf een cliënt vertegenwoordigt, herzie de met het bedrijf verbonden met voeten treden tarieven. Voor informatie, zie [&#x200B; het factureren van de baanrol van de Opheffing tarieven op het bedrijfsniveau &#x200B;](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* Als het bedrijf een cliënt vertegenwoordigt, en als er andere uniek-aan-dat-organisatie projectmalplaatjes zijn, preassocieer eerst de projectmalplaatjes met het onlangs toegevoegde bedrijf. Voor informatie, zie [&#x200B; projectmalplaatjes &#x200B;](../../manage-work/projects/create-and-manage-templates/edit-templates.md) uitgeven.
* Als het bedrijf een cliënt of een verkoper vertegenwoordigt, associeer bestaande gebruikers van de externe organisatie die reeds in uw milieu kan zijn. Voor informatie, zie [&#x200B; bedrijven &#x200B;](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md) creëren en uitgeven.
* Als het bedrijf een cliënt of een verkoper vertegenwoordigt, creeer extra samenwerkende gebruikers voor de externe organisatie die u in uw milieu kunt nodig hebben om mededeling, werkuitvoering, en goedkeuringen te stroomlijnen. Voor informatie bij het creëren van nieuwe gebruikers, zie [&#x200B; gebruikers &#x200B;](../../administration-and-setup/add-users/create-and-manage-users/add-users.md) toevoegen.
* Werk organisatorische grafiekverhoudingen voor om het even welke gebruikers bij nu verbonden aan het onlangs toegevoegde bedrijf. Voor informatie, zie [&#x200B; directe rapporten &#x200B;](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) creëren en [&#x200B; Mening de organisatorische grafiek &#x200B;](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

Voor extra informatie over bedrijven, zie [&#x200B; bedrijven &#x200B;](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md) creëren en uitgeven.

## Aanbevelingen voor het dashboard {#dashboard-recommendations}

Deze sectie bevat aanbevelingen voor de dashboards en de rapporten die met een blauwdruk worden geïnstalleerd.

### Pas gemaakte dashboards bijwerken om rapporten toe te voegen/te verwijderen

De dashboards die van een blauwdruk worden toegevoegd hebben één of meerdere rapporten, externe pagina&#39;s, of kalenders. Het is waarschijnlijk dat u niet alle rapporten en andere dashboardelementen nodig hebt of dat u het dashboard moet uitbreiden met bestaande rapporten, externe pagina&#39;s en kalenders voordat het met anderen kan worden gedeeld. Voor informatie, zie [&#x200B; een rapport aan een dashboard &#x200B;](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md) toevoegen.

### Pas gemaakte rapporten bijwerken om kolommen of filtercriteria toe te voegen/te verwijderen

De rapporten die door een dashboardblauwdruk worden verdeeld hebben niet alle kolommen of filtercriteria om uw configuratie van [!DNL Workfront] te steunen. Naar verwachting zult u de rapporten op enkele punten aanpassen zodat deze aan uw normen voldoen. Om consistentie met andere rapporten in uw milieu te bouwen, kunt u een kolom willen toevoegen u op alle rapporten voor het voorwerp dat opneemt, of om sommige filtercriteria toe te voegen die resultaten aan een bepaald projecttype of een gebruikersgroep beperken. Voor informatie, zie [&#x200B; meningen &#x200B;](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) creëren of uitgeven en [&#x200B; creeer of geef filters &#x200B;](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md) uit.

### De dashboards of rapporten delen met gebruikers

Als u het dashboard niet op een lay-outmalplaatje wilt plaatsen, zou u het dashboard met de mensen moeten delen die het nuttig zullen vinden. Voor informatie, zie [&#x200B; een dashboard &#x200B;](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) delen en [&#x200B; een rapport &#x200B;](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md) delen.

### De dashboards toevoegen aan lay-outsjablonen

De beste manier om informatie beschikbaar te maken voor andere mensen is het toevoegen van dashboards aan lay-outmalplaatjes. Identificeer de lay-outmalplaatjes van de mensen die het meest van het herzien van het dashboard op een regelmatige basis zouden profiteren en voeg het nieuwe dashboard aan die lay-outmalplaatjes toe. Voor informatie, zie [&#x200B; lay-outmalplaatjes &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.

### Andere dashboards en rapporten bijwerken

Door de invoering van een nieuw dashboard en de bijbehorende verslagen kan het mogelijk zijn andere bestaande dashboards en rapporten af te schaffen en aan te passen. Neem de tijd om uw bestaande rapporten te herzien om het even welke overtollige en tegenstrijdige rapporten te identificeren.

### Aangepaste gegevens distribueren naar relevante formulieren

Sommige rapporten inbegrepen in een dashboardblauwdruk hebben de gebieden van douanegegevens in of de mening, de filter, of de groepering van het rapport. In sommige gevallen heeft de blauwdruk ook een formulier waaraan deze velden zijn gekoppeld. De aangepaste velden worden echter vaker dan niet toegepast op een aangepast formulier. De kolommen, filters of groepen werken alleen correct als deze velden zijn gekoppeld aan formulieren die zijn verbonden met een gebruiker, project, taak of andere objectreeks. Voor informatie, zie [&#x200B; een douaneformulier &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.
