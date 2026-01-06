---
content-type: overview
product-area: projects
keywords: terugkerend, opnieuw voorkomen, terugkerend
navigation-topic: manage-tasks
title: Het terugkeren van het Overzicht van Taken
description: Overzicht van terugkerende taken
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 9ddb75bf-1c7b-4f4b-b80b-a9512192920d
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Overzicht van terugkerende taken

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: DO NOT DO NOT EDIT OR CHANGE!!! linked to the NWE UI, this is not linked to classic - direct links:</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=workfront-classic</p>
<p>https://one.workfront.com/s/csh?context=2288&pubname=the-new-workfront-experience >> this)</p>
</div>
-->

U kunt terugkomende taken voor activiteiten tot stand brengen die u als deel van één enkel project moet herhalen.

In dit artikel worden informatie en overwegingen beschreven over het maken en bewerken van terugkerende taken.

Voor informatie over hoe te om terugkomende taken in Adobe Workfront tot stand te brengen, zie [&#x200B; terugkomende taken &#x200B;](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md) creëren.

## Het terugkomen Overzicht van Taken en overwegingen

U kunt terugkomende taken tot stand brengen om op herhaalbaar werk tijdens het leven van een project te wijzen.

Tijdens bijvoorbeeld een IT-project moet waarschijnlijk regelmatig een back-up van de software worden gemaakt. Het maken van een terugkerende taak voor deze activiteit verkort de tijd die nodig is om meerdere individuele taken in te stellen.

Houd rekening met het volgende wanneer u terugkerende taken maakt in Workfront:

* U kunt geen terugkerende taken aan een sjabloon toevoegen.
* U kunt geen herhalingsfrequentie aan een bestaande taak toevoegen.
* Herhalende taken worden weergegeven als subtaken of onderliggende taken voor de hoofdinstantie die als bovenliggende taak wordt weergegeven.
* U kunt geen goedkeuring aan een ouder terugkomende taak vastmaken.
* Workfront brengt de meeste velden die u voor de bovenliggende herhaling bijwerkt, over naar de onderliggende taken. De volgende velden worden niet overgedragen naar de onderliggende taken wanneer deze worden gemaakt:

   * De beperking van de Taak van de kindtaken verandert automatisch in:

      * Moet bij projecten die vanaf de begindatum zijn gepland, van start gaan.
      * Moet worden voltooid op voor projecten die vanaf de voltooiingsdatum zijn gepland.

   * Documenten die aan het bovenliggende element zijn gekoppeld, worden niet naar de onderliggende elementen overgedragen.

* De volgende veranderingen komen op de oudertaak voor nadat u erop wijst dat de taak terugkomt:

   * Het veld Duur krijgt een andere naam in Duur per instantie voor de bovenliggende taak. Het blijft Duur voor de kindtaken.
   * De status is uitgeschakeld op de bovenliggende taak en wordt automatisch ingesteld op Nieuw op de onderliggende items. De bovenliggende taak wordt automatisch voltooid en de status wordt bijgewerkt naar Voltooid wanneer alle onderliggende items zijn voltooid.
   * De enige beschikbare Types van Duur voor terugkomende taken zijn:

      * eenvoudig
      * Inzet gedreven
* De duur en de geplande uren die voor een nieuwe terugkerende taak worden vermeld zijn de Duur en de Geplande Uren van elk voorkomen. De Duur van de oudertaak is de tijd tussen de Geplande Datum van het Begin van de vroegste taak en de Geplande Datum van de Voltooiing van de recentste taak. De geplande uren van de bovenliggende taak is het totaal van alle geplande uren van alle voorvallen.

## Overwegingen bij het bewerken van terugkerende taken

Sommige wijzigingen die u aanbrengt in een bovenliggende taak die terugkeert, worden mogelijk niet op alle bestaande exemplaren bijgewerkt. Onderliggende taken die de voortgang tonen of afzonderlijk zijn bijgewerkt, worden niet bijgewerkt wanneer u het bovenliggende onderdeel bijwerkt. Workfront is van mening dat een taak vooruitgang laat zien in de volgende situaties:

* De status wordt bijgewerkt en de taak is niet langer Nieuw
* Het percentage voltooide taak is hoger dan nul
* De taak heeft voorgaande relaties

In de volgende tabel wordt aangegeven of wijzigingen die zijn aangebracht in de bovenliggende trigger, worden bijgewerkt met onderliggende elementen die niet afzonderlijk zijn bewerkt of die voortgang tonen:

| Velden bijgewerkt op de bovenliggende taak | Overdracht van updates naar onbewerkte kinderen of kinderen zonder geregistreerde voortgang |
|---|---|
| Herhalingsfrequentie * | ✔ |
| Toewijzingen | ✔ |
| Naam | ✔ |
| Beschrijving | ✔ |
| Prioriteit | ✔ |
| Duur | ✔ |
| Geplande uren | ✔ |
| Kostensoort | ✔ |
| Type inkomsten | ✔ |
| Bronniveaus | ✔ |
| Vertraging Niveaus | ✔ |
| Taakbeperking | De onderliggende items worden niet bijgewerkt |
| Aangepaste Forms koppelen of verwijderen | De onderliggende items worden niet bijgewerkt |
| Duur | De onderliggende items worden niet bijgewerkt |
| Aangepaste formuliergegevens | De onderliggende items worden niet bijgewerkt |

{style="table-layout:auto"}

&#42; De volgende scenario&#39;s bestaan wanneer u de Frequentie van de Herhaling van een oudertaak bijwerkt:

* Als u de Frequentie van de Herhaling op een bestaande oudertaak verandert, worden de bestaande subtaken geschrapt en met nieuwe subtaken vervangen die de nieuwe herhalingsfrequentie volgen als zij geen vooruitgang tonen en als u niet manueel hen hebt bijgewerkt.
* Als u de Frequentie van de Herhaling op een bestaande oudertaak verandert, worden de subtaken die vooruitgang tonen niet geschrapt. Deze taken worden los van de herhaling op dit punt beschouwd.

&#42;&#42; Toewijzingen die op de bovenliggende taak zijn uitgevoerd, worden toegepast op alle subtaken in de herhaling. Eventuele wijzigingen die in de toewijzing in de bovenliggende taak zijn aangebracht, overschrijven elke afzonderlijke toewijzing in de subtaak. Als de taak de voortgang weergeeft, verandert de toewijzing niet.


