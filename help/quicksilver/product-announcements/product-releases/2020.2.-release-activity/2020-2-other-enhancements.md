---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2 andere verbeteringen
description: Op deze pagina worden alle andere verbeteringen beschreven die zijn aangebracht met de release 2020.2 voor de productieomgeving. Deze verbeteringen zijn in de productieomgeving beschikbaar gesteld in de week van 11 mei 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 46ed705e-b966-4ae9-a602-a5a73a3de3aa
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 2020.2 andere verbeteringen

Op deze pagina worden alle andere verbeteringen beschreven die zijn aangebracht met de release 2020.2 voor de productieomgeving. Deze verbeteringen zijn in de productieomgeving beschikbaar gesteld in de week van 11 mei 2020.

Voor een lijst van alle veranderingen beschikbaar met versie 2020.2, zie [Overzicht van de release 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## Voor Workfront-beheerders: nieuwere lay-outsjablonen die in Workfront Classic zijn gemaakt, zijn nu beschikbaar in de nieuwe Workfront-ervaring

Layoutsjablonen die na Herfst 2019 in Workfront Classic zijn gemaakt, zijn nu beschikbaar in de nieuwe Workfront-ervaring. Het is raadzaam deze lay-outsjablonen bij te werken in de nieuwe Workfront-ervaring om te profiteren van de nieuwe functionaliteit en deze zo nuttig mogelijk te maken voor gebruikers in die omgeving.

Zie voor meer informatie [Lay-outsjablonen](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

**Beschikbaar in deze omgevingen:**

* De nieuwe Adobe Workfront-ervaring

## Voor alle objecten zijn groepsspecifieke goedkeuringsprocessen beschikbaar

Als u volledig gebruik wilt maken van groepsspecifieke goedkeuringsprocessen, kunt u deze nu toevoegen aan taken, problemen en projecten wanneer u deze objecten bewerkt.

U kunt een groep-specifiek goedkeuringsproces aan een taak op het gebied van Taken van het Edit vakje van het Project, evenals aan kwesties automatisch vastmaken, wanneer het vormen van verzoekrijen of de Onderwerpen van de Rij op een project.

Raadpleeg de volgende artikelen voor informatie over het toevoegen van goedkeuringsprocessen aan projecten, taken en problemen:

* [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md)
* [Taken bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [Problemen bewerken](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
* [Werkvoorraadonderwerpen maken](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)

## Goedkeuringsprocessen maken voor groepen die aangepaste statussen gebruiken

Om het voor groepen gemakkelijker te maken om hun eigen unieke werkschema&#39;s te beheren, kunt u groep-specifieke douanestatus in goedkeuringsprocessen nu gebruiken.

Eerder kon een groep zijn eigen douanestatus niet gebruiken met zijn groep-specifieke goedkeuringsprocessen. Alleen statussen voor het hele systeem waren beschikbaar en deze werkten niet altijd in de goedkeuringsprocessen voor groepen.

Aangepaste statussen kunnen nu worden gebruikt in goedkeuringsprocessen voor eenmalig gebruik en voor het hele systeem:

* Maak een goedkeuringsproces voor één gebruik voor een object (project, taak of uitgave) en baseer dit op statussen die zijn gekoppeld aan de groep die aan dat object werkt. Dit omvat alle aangepaste statussen die aan de groep zijn gekoppeld.
* Maak een algemeen goedkeuringsproces en stel dit alleen beschikbaar voor de groep of voor iedereen in het systeem.

Voor gebruikers met administratieve toegang tot goedkeuringsprocessen is informatie over het configureren van goedkeuringsprocessen beschikbaar in [Een goedkeuringsproces voor werkitems maken](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (of als u Adobe Workfront Classic gebruikt, zie [Goedkeuringsprocessen maken](https://one.workfront.com/s/article/Creating-Approval-Processes-1001577410)).

Voor gebruikers is informatie over het koppelen van goedkeuringsprocessen aan werkitems beschikbaar in [Een nieuw of bestaand goedkeuringsproces koppelen aan werk](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (of als u Adobe Workfront Classic gebruikt, zie [Een nieuw of bestaand goedkeuringsproces koppelen aan werk](https://one.workfront.com/s/article/Associating-a-New-or-Existing-Approval-Process-with-Work-708455630)).

**Beschikbaar in deze omgevingen:**

* Adobe Workfront Classic
* De nieuwe Adobe Workfront-ervaring

## Nieuwe overlaypagina&#39;s voor zoeken

Om gebruikers in staat te stellen gemakkelijker heen en weer te navigeren tussen zoekpagina&#39;s en vorige pagina&#39;s in de nieuwe Workfront-ervaring, hebben we een pagina met zoekopdrachten toegevoegd die het scherm gedeeltelijk bedekt.

Wanneer u nu op Geavanceerd zoeken in het menu Zoeken klikt of een standaardzoekopdracht uitvoert, wordt een pagina vanaf de rechterkant van het scherm geopend.

Zie voor meer informatie [Zoeken in Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

**Beschikbaar in deze omgevingen:**

* De nieuwe Adobe Workfront-ervaring

## Updates voor abonnementen op gebeurtenissen

We hebben gedrag gewijzigd en meer gegevens toegevoegd aan de API voor abonnementen voor gebeurtenissen om gebruikers beter in staat te stellen problemen op te lossen, problemen op te lossen en op te lossen. We hebben ook de volgende wijzigingen aangebracht:

* Gemigreerde onderliggende overseinentechnologieën
* Herbouwde de dienst om minder complexe gebiedsdelen te hebben en zo efficiënter te schrapen
* Verbeterde controle en waarschuwingen

Zie voor meer informatie [Veelgestelde vragen - Abonnementen voor gebeurtenissen](../../../wf-api/general/event-subs-faq.md) en [Aanbevolen werkwijzen voor abonnementen op gebeurtenissen](../../../wf-api/general/event-sub-best-practice.md).
