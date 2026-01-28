---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Toegang tot objecten en gebieden per licentietype (verouderd)
description: In de onderstaande tabel ziet u het hoogste toegangsniveau (Bewerken of Weergave) dat door elk van de Adobe Workfront-licenties wordt toegestaan voor de objecten en gebieden in Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# Toegang tot objecten en gebieden per licentietype (verouderd)

<!-- Audited: 11/2025 -->

>[!NOTE]
>
>De informatie in dit artikel verwijst naar de oudere toegangsniveaus. Voor informatie over de huidige toegangsniveaus, zie [ Nieuw overzicht van toegangsniveaus ](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

In de onderstaande tabel ziet u het hoogste toegangsniveau (Bewerken of Weergave) dat door elk van de Adobe Workfront-licenties wordt toegestaan voor de objecten en gebieden in Workfront.

* Weergave: de gebruiker kan items controleren en delen.
* Bewerken: de gebruiker kan items maken, bewerken, verwijderen en delen.

  >[!NOTE]
  >
  >Wanneer een andere gebruiker een object deelt, kan de deler machtigingen opgeven die hun mogelijkheid beperken om het object te bewerken. Voor meer informatie over de nieuwe vergunningstypes, zie [ Overzicht van het delen van toestemmingen op voorwerpen ](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

  >[!NOTE]
  >
  >Dit artikel bevat informatie over objecttoegang voor de oudere licentietypen. Voor informatie over de nieuwe licentietypen, zie [ Nieuw overzicht van toegangsniveaus ](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) en [ Nieuw overzicht van vergunningen ](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

|   | Plan | Werk | Controleren | Verzoek | Extern |
|---|---|---|---|---|---|
| Projecten | Bewerken | Bewerken (zonder Maken-machtigingen) | Weergave | Weergeven (alleen de pagina Details) | Geen toegang |
| Taken | Bewerken | Bewerken | Weergave | Weergave | Geen toegang |
| Problemen | Bewerken | Bewerken | Bewerken | Bewerken | Geen toegang |
| Portfolio&#39;s | Bewerken | Weergave | Weergave | Geen toegang | Geen toegang |
| Programma&#39;s | Bewerken | Weergave | Weergave | Geen toegang | Geen toegang |
| Rapporten, dashboards en kalenders | Bewerken | Weergave | Weergave | Weergave &#42; | Weergeven (alleen voor kalenders, geen machtigingen voor delen) |
| Filters, weergaven en groepen | Bewerken | Bewerken | Bewerken | Bewerken | Geen toegang |
| Documenten | Bewerken | Bewerken | Bewerken | Bewerken | Weergave (geen machtigingen voor delen) |
| Gebruikers | Bewerken | Weergave | Weergave | Weergave | Weergave |
| Teams | Bewerken | Bewerken | Weergave | Weergave | Geen toegang |
| Sjablonen | Bewerken | Geen toegang | Geen toegang | Geen toegang | Geen toegang |
| Financiële gegevens | Bewerken | Weergave (alleen het gedeelte Financiën in projectdetails) | Weergave | Geen toegang | Geen toegang |
| Bronbeheer | Bewerken | Weergave | Weergave | Geen toegang | Geen toegang |
| Scenario Planner | Bewerken | Bewerken | Bewerken | Geen toegang | Geen toegang |
| Workfront-doelen | Bewerken | Bewerken | Bewerken | Bewerken | Geen toegang |

&#42; Gebruikers met een aanvraaglicentie kunnen alleen rapporten, dashboards en kalenders weergeven die met hen worden gedeeld.

>[!NOTE]
>
>Gebruikers met een revisielicentie of een aanvraaglicentie hebben beperkte mogelijkheden voor delen. Voor meer informatie, zie [ overzicht van Vergunningen ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).
>
>Externe gebruikers kunnen niet zoeken naar items in Workfront. Ze kunnen documenten en kalenders weergeven die specifiek met hen worden gedeeld. Ze kunnen ook de gebruikers zien die items met hen delen.

In de volgende artikelen vindt u gedetailleerde informatie over wat de toegangsniveaus voor elk object en gebied toestaan:

* [ de toegang van de Verlening tot projecten ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [ de toegang van de Verlening tot taken ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [ de toegang van de Verlening tot kwesties ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [ de toegang van de Verlening tot documenten ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [ de toegang van de Verlening tot portefeuilles ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [ de toegang van de Verlening tot programma&#39;s ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [ de toegang van de vergunning tot rapporten, dashboards, en kalenders ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [ de toegang van de Verlening tot filters, meningen, en groeperingen ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [ de toegang van de Verlening tot gebruikers ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [Toegang verlenen aan teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [ de toegang van de Verlening tot malplaatjes ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [ de toegang van de Verlening tot financiële gegevens ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [ de toegang van de Verlening tot het Beheer van het Middel ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [ de toegang van de Verlening tot de Planner van het Scenario ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Toegang tot Adobe Workfront-doelen verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
