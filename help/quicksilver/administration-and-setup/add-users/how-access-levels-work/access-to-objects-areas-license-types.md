---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Toegang tot objecten en gebieden door licenties
description: In de onderstaande tabel ziet u het hoogste toegangsniveau (Bewerken of Weergave) dat door elk van de Adobe Workfront-licenties wordt toegestaan voor de objecten en gebieden in Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Toegang tot objecten en gebieden via licenties

<!-- Audited: 2/2024 -->

>[!NOTE]
>
>De informatie in dit artikel verwijst naar de huidige toegangsniveaus. Voor informatie over de niveaus van de erfenistoegang, zie [&#x200B; overzicht van de niveaus van de Toegang &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

In de onderstaande tabel ziet u het hoogste toegangsniveau (Bewerken of Weergave) dat door elk van de Adobe Workfront-licenties wordt toegestaan voor de objecten en gebieden in Workfront.

* **Mening**: De gebruiker kan punten herzien en delen.
* **geeft uit**: De gebruiker kan, punten creëren uitgeven schrappen en delen.

  >[!NOTE]
  >
  >Wanneer een andere gebruiker een object deelt, kan de deler machtigingen opgeven die hun mogelijkheid beperken om het object te bewerken. Voor meer informatie, zie [&#x200B; Overzicht van het delen van toestemmingen op voorwerpen &#x200B;](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

<table style="table-layout:auto">
    <tr>
        <td></td>
        <td>Standard</td>
        <td>Licht</td>
        <td>Medewerker</td>
        <td>Extern</td>
    </tr>
    <tr>
        <td>Projecten</td>
        <td>Bewerken</td>
        <td>Bewerken**</td>
        <td>Weergave</td>
        <td>Geen toegang</td>
    </tr>
    <tr>
        <td>Taken</td>
        <td>Bewerken</td>
        <td>Weergave</td>
        <td>Weergave</td>
        <td>Geen toegang</td>
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

&#42;&#42; De gebruikers met een Lichte vergunning kunnen slechts tijd op het projectniveau registreren wanneer Edit toegang wordt toegelaten. Ze kunnen geen projecten maken, bewerken, verwijderen of delen. Het standaard toegangsniveau op Projecten voor Lichte gebruikers is Mening.

>[!NOTE]
>
>* Gebruikers met een Light-licentie of een Contributor-licentie hebben beperkte mogelijkheden voor delen. Voor meer informatie, zie [&#x200B; overzicht van Vergunningen &#x200B;](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
>
>* Externe gebruikers kunnen niet zoeken naar items in Workfront. Ze kunnen documenten en kalenders weergeven die specifiek met hen worden gedeeld. Ze kunnen ook de gebruikers zien die items met hen delen.
>
>* Gebruikers van de contribuant en externe gebruikers kunnen geen inhoud zien die voor het hele systeem wordt gedeeld.  Het moet expliciet met hen worden gedeeld.

In de volgende artikelen vindt u gedetailleerde informatie over wat de toegangsniveaus voor elk object en gebied toestaan:

* [&#x200B; de toegang van de Verlening tot projecten &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [&#x200B; de toegang van de Verlening tot taken &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [&#x200B; de toegang van de Verlening tot kwesties &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [&#x200B; de toegang van de Verlening tot documenten &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [&#x200B; de toegang van de Verlening tot portefeuilles &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [&#x200B; de toegang van de Verlening tot programma&#39;s &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [&#x200B; de toegang van de vergunning tot rapporten, dashboards, en kalenders &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [&#x200B; de toegang van de Verlening tot filters, meningen, en groeperingen &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [&#x200B; de toegang van de Verlening tot gebruikers &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [Toegang verlenen aan teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [&#x200B; de toegang van de Verlening tot malplaatjes &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [&#x200B; de toegang van de Verlening tot financiële gegevens &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [&#x200B; de toegang van de Verlening tot het Beheer van het Middel &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [&#x200B; de toegang van de Verlening tot de Planner van het Scenario &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Toegang tot Adobe Workfront-doelen verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
