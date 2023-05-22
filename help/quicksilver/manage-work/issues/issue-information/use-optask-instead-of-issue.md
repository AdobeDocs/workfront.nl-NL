---
product-area: projects
navigation-topic: issue-information
title: Gebruik "opTask" en "issue" bij het verwijzen naar problemen
description: De naam van een uitgave wordt weergegeven als opTask in de Adobe Workfront-database. Hoewel er tijden zijn wanneer u de naam van het uitgiftegebied moet gebruiken om naar kwesties te verwijzen, moet u de meeste tijd u de opTask gebiedsnaam in plaats van kwestie gebruiken wanneer het van verwijzingen voorzien van kwesties.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: 813b97ee0979e29a90293d9ddaba12a33c99f64d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Gebruik &quot;opTask&quot; en &quot;issue&quot; bij het verwijzen naar problemen

De naam van een uitgave wordt weergegeven als `opTask` in de Adobe Workfront-database. Hoewel er momenten zijn waarop u het `issue` veldnaam om naar problemen te verwijzen, meestal moet u de optie `opTask` veldnaam in plaats van `issue` bij het verwijzen naar kwesties.

Raadpleeg voor meer informatie over hoe objecten worden weergegeven in de Workfront-database de [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

## `opTask` filename

Gebruik de `opTask` veldnaam bij het verwijzen naar kwesties in de volgende context:

* Wanneer u een aangepast rapport voor problemen maakt in de tekstmodus, en u wilt verwijzen naar problemen in weergaven, filters, groepen of aanwijzingen.

   Voor meer informatie over het gebruiken van tekstwijze in een rapport, zie [Overzicht van de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* Wanneer u de gebieden van de uitgave in een Kick-Begin- gegevensimporter bijwerkt.

   Ga voor meer informatie over het importeren van gegevens in Workfront met een Kick-start naar [Gegevens naar Adobe Workfront importeren met een Kick-startsjabloon](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` veldnaam

Gebruik de `issue` de naam van het gebied aan verwijzingskwesties in de volgende context:

* Wanneer u in een inzameling van verwijzingen voorziet gebruikend tekstwijze in een rapport.
* Wanneer u verwijst naar een uitgavemonzameling met de Workfront API.

Voor informatie over het rapporteren van verzamelingen raadpleegt u [Referentieverzamelingen in een rapport](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
