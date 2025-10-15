---
product-area: projects
navigation-topic: issue-information
title: Gebruik "opTask" en "issue" bij het verwijzen naar problemen
description: De naam van een uitgave wordt weergegeven als opTask in de Adobe Workfront-database. Hoewel er tijden zijn wanneer u de naam van het uitgiftegebied moet gebruiken om naar kwesties te verwijzen, moet u de meeste tijd u de opTask gebiedsnaam in plaats van kwestie gebruiken wanneer het van verwijzingen voorzien van kwesties.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Gebruik &quot;opTask&quot; en &quot;issue&quot; bij het verwijzen naar problemen

<!--Audited: 08/2025-->

De naam van een uitgave wordt weergegeven als `opTask` in de Adobe Workfront-database. Hoewel er momenten zijn waarop u de veldnaam `issue` moet gebruiken om naar problemen te verwijzen, moet u meestal de `opTask` veldnaam gebruiken in plaats van `issue` wanneer u naar problemen verwijst.

Voor meer informatie over hoe de voorwerpen in het gegevensbestand van Workfront verschijnen, verwijs naar de [ API Ontdekkingsreiziger ](https://developer.adobe.com/workfront/api-explorer/).

## `opTask` veldnaam

Gebruik de veldnaam `opTask` wanneer u in de volgende context naar problemen verwijst:

* Wanneer u een aangepast rapport voor problemen maakt in de tekstmodus, en u wilt verwijzen naar problemen in weergaven, filters, groepen of aanwijzingen.

  Voor meer informatie over het gebruiken van tekstwijze in een rapport, zie [ Overzicht van de Wijze van de Tekst ](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* Wanneer u de gebieden van de uitgave in een Kick-Begin- gegevensimporter bijwerkt.

  Voor meer informatie over het invoeren van gegevens in Workfront die een Kick-Begin gebruiken, zie [ Gegevens van de Invoer in Adobe Workfront gebruikend een Kick-Begin malplaatje ](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` veldnaam

Gebruik de veldnaam `issue` om te verwijzen naar problemen in de volgende context:

* Wanneer u in een inzameling van verwijzingen voorziet gebruikend tekstwijze in een rapport.
* Wanneer u verwijst naar een uitgavemonzameling met de Workfront API.

Voor informatie over het melden van inzamelingen, zie [ inzamelingen van de Verwijzing in een rapport ](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
