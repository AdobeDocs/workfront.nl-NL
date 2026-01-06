---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Overzicht van het project Werkelijke uitvoeringsdatum
description: Projecten, taken en problemen hebben een datum waarop ze daadwerkelijk zijn voltooid in Adobe Workfront. Dit is de datum waarop het project, de taak of de kwestie als voltooid werden gemarkeerd.
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Overzicht van het project Werkelijke uitvoeringsdatum

Projecten, taken en problemen hebben een datum waarop ze daadwerkelijk zijn voltooid in Adobe Workfront. Dit is de datum waarop het project, de taak of de kwestie als voltooid werden gemarkeerd.

## Werkelijke einddata

De datum van daadwerkelijke voltooiing vertegenwoordigt de echte datum en de tijd wanneer het werk wordt voltooid. Wanneer een taak of een kwestie als Gedaan of Voltooid wordt gemerkt, plaatst Workfront automatisch de datum van de verandering in status van het punt als Ware VoltooiingsDatum van de taak of de kwestie. Als die datum geen nauwkeurige weerspiegeling van is wanneer de taak of de kwestie werkelijk werd voltooid, dan kunt u de Ware Datum van Voltooiing manueel uitgeven.

U kunt bijvoorbeeld een taak of een probleem markeren Gereed op maandag, maar u weet dat het werk de vorige vrijdag is voltooid. Nadat u de taak of het probleem hebt gemarkeerd als Gereed, kunt u vervolgens handmatig de werkelijke Voltooiingsdatum van de taak of uitgave bijwerken naar de datum van de vorige vrijdag om de werkelijke voltooiing te weerspiegelen.

U kunt niet manueel de Ware Datum van de Voltooiing van een project uitgeven, maar u kunt de status van een project manueel veranderen dat een verandering in zijn Ware Datum van de Voltooiing kan teweegbrengen.

De daadwerkelijke VoltooiingsDatum van een project wordt geplaatst op de volgende manieren:

* Door de status van het project manueel bij te werken: als de Wijze van de Voltooiing van het project aan Handboek wordt geplaatst en u manueel de status van het project in Voltooid verandert, teweegbrengt dit de Ware Datum van de Voltooiing van het project dat tot de datum en de tijd van de laatste voltooide taak wordt bijgewerkt.
* Automatisch, wanneer de laatste taak van het project voltooit: als de Wijze van de Voltooiing van het project aan Automatisch wordt geplaatst en u de laatste taak als Voltooid merkt of de Ware Datum van de Voltooiing van de laatste taak bijwerkt, wordt de Ware Datum van de Voltooiing van het project ook bijgewerkt met die datum.

  Voor informatie over het plaatsen van de Wijze van de Voltooiing van een project, zie het artikel [&#x200B; projecten &#x200B;](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

  >[!NOTE]
  >
  >Workfront gebruikt de datum van daadwerkelijke voltooiing van de taak van het project die het laatst voltooide als de datum van daadwerkelijke voltooiing voor het volledige project.

Een Workfront of groepsbeheerder bepaalt of Workfront de datum van vandaag of de Geplande Datum van Voltooiing van een taak of een kwestie gebruikt wanneer deze aan Voltooid of Gesloten worden geplaatst. Voor informatie over het plaatsen van taak en van de kwestie voorkeur, zie [&#x200B; systeembrede taak vormen en voorkeur uitgeven &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## Werkelijke afsluitdatums zoeken

De datum van feitelijke voltooiing bevindt zich in de volgende gebieden van Workfront:

* De gebieden van project, van de Taak, en van de Details van de Kwestie
* De vakken Project, Taak en Uitgave bewerken
* Het gebied van de Updates van het project, van de Taak, en van de Uitgave als Update van het Systeem.
* Lijst of rapporten met projecten, taken of uitgaven.

Voor meer informatie over het creëren van rapporten, zie het artikel [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.
