---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Toegang tot objecten en gebieden door nieuwe licenties
description: In de onderstaande tabel ziet u het hoogste toegangsniveau (Bewerken of Weergave) dat door elk van de Adobe Workfront-licenties wordt toegestaan voor de objecten en gebieden in Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: b333ea67bb909ca55306f6474832c275ebad590c
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Toegang tot objecten en gebieden met nieuwe licenties

<!-- Audited: 2/2024 -->

In de onderstaande tabel ziet u het hoogste toegangsniveau (Bewerken of Weergave) dat door elk van de Adobe Workfront-licenties wordt toegestaan voor de objecten en gebieden in Workfront.

* **Mening**: De gebruiker kan punten herzien en delen.
* **geeft uit**: De gebruiker kan, punten creëren uitgeven schrappen en delen.

  >[!NOTE]
  >
  >Wanneer een andere gebruiker een object deelt, kan de deler machtigingen opgeven die hun mogelijkheid beperken om het object te bewerken. Voor meer informatie, zie [ Overzicht van het delen van toestemmingen op voorwerpen ](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

<table style="table-layout:auto">
    <tr>
        <td></td>
        <td>Standaard</td>
        <td>Licht</td>
        <td>Medewerker</td>
        <td>Extern</td>
    </tr>
    <tr>
        <td>Projecten</td>
        <td>Bewerken</td>
        <td>Weergave</td>
        <td>Weergave</td>
        <td>Geen toegang</td>
    </tr>
    <tr>
        <td>Taken</td>
        <td>Bewerken</td>
        <td>Weergave</td>
        <td>Weergave</td>
        <td>Weergave</td>
    </tr>
    <tr>
        <td>Problemen</td>
        <td>Bewerken</td>
        <td>Bewerken</td>
        <td>Bewerken</td>
        <td>Geen toegang</td>
    </tr>
    <tr>
        <td>Portfolio's</td>
        <td>Bewerken</td>
        <td>Weergave</td>
        <td>Weergave</td>
        <td>Geen toegang</td>
    </tr>
    <tr>
        <td>Programma's</td>
        <td>Bewerken</td>
        <td>Weergave</td>
        <td>Weergave</td>
        <td>Geen toegang</td>
    </tr>
    <tr>
        <td>Rapporten, dashboards en kalenders</td>
        <td>Bewerken</td>
        <td>Weergave</td>
        <td>Weergeven*</td>
        <td>Weergeven (alleen voor kalenders, geen machtigingen voor delen)</td>
    </tr>
    <tr>
        <td>Filters, weergaven en groepen</td>
        <td>Bewerken</td>
        <td>Bewerken</td>
        <td>Bewerken</td>
        <td>Geen toegang</td>
    </tr>
    <tr>
        <td>Documenten</td>
        <td>Bewerken</td>
        <td>Bewerken</td>
        <td>Bewerken</td>
        <td>Weergave (geen machtigingen voor delen)</td>
    </tr>
    <tr>
        <td>Gebruikers</td>
        <td>Bewerken</td>
        <td>Weergave</td>
        <td>Weergave</td>
        <td>Weergave</td>
    </tr>
    <tr>
        <td>Teams</td>
        <td>Bewerken</td>
        <td>Weergave</td>
        <td>Weergave</td>
        <td>Geen toegang</td>
    </tr>
    <tr>
        <td>Sjablonen</td>
        <td>Bewerken</td>
        <td>Geen toegang</td>
        <td>Geen toegang</td>
        <td>Geen toegang</td>
    </tr>
    <tr>
        <td>Financiële gegevens</td>
        <td>Bewerken</td>
        <td>Geen toegang</td>
        <td>Geen toegang</td>
        <td>Geen toegang</td>
    </tr>
    <tr>
        <td>Bronbeheer</td>
        <td>Bewerken</td>
        <td>Weergave</td>
        <td>Geen toegang</td>
        <td>Geen toegang</td>
    </tr>
    <tr>
        <td>Scenario Planner</td>
        <td>Bewerken</td>
        <td>Weergave</td>
        <td>Geen toegang</td>
        <td>Geen toegang</td>
    </tr>
    <tr>
        <td>Workfront-doelen</td>
        <td>Bewerken</td>
        <td>Bewerken</td>
        <td>Bewerken</td>
        <td>Geen toegang</td>
    </tr>
</table>

&#42; Gebruikers met een licentie voor contribuanten kunnen alleen rapporten, dashboards en kalenders weergeven die met hen worden gedeeld.

>[!NOTE]
>
>* Gebruikers met een Light-licentie of een Contributor-licentie hebben beperkte mogelijkheden voor delen. Voor meer informatie, zie [ overzicht van Vergunningen ](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
>
>* Externe gebruikers kunnen niet zoeken naar items in Workfront. Ze kunnen documenten en kalenders weergeven die specifiek met hen worden gedeeld. Ze kunnen ook de gebruikers zien die items met hen delen.
>
>* Gebruikers van de contribuant en externe gebruikers kunnen geen inhoud zien die voor het hele systeem wordt gedeeld.  Het moet expliciet met hen worden gedeeld.

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
