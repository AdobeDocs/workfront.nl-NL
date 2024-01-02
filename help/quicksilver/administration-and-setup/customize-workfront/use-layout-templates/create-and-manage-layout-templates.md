---
title: Lay-outsjablonen maken en beheren
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: Als Workfront-beheerder of groepsbeheerder kunt u lay-outsjablonen maken en wijzigen om lay-outelementen in Workfront aan te passen voor uw gebruikers.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: cf044c8cff6b1172ec460ae232cd07c9b7c808b7
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# Lay-outsjablonen maken en beheren

<!--Audited: 12/2023-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Als Adobe Workfront-beheerder of groepsbeheerder kunt u lay-outsjablonen maken en wijzigen om de volgende lay-outelementen in Workfront voor uw gebruikers aan te passen:

* Hoofdmenu
* Linkernavigatievenster
* Thuisgebied
* Weergaven, filters en groepen die mensen gebruiken met lijsten en rapporten.
* Schermterminologie
* Project-, taak- en uitgavekoppen

Nadat u een lay-outmalplaatje creeert of wijzigt, kunt u het aan individuele gebruikers, teams, groepen, of baanrollen toewijzen.

De standaard Workfront-indeling van elke gebruiker is afhankelijk van het toegangsniveau en het type licentie. Sommige gebruikers zien bepaalde gebieden bijvoorbeeld niet in het hoofdmenu. Zie voor meer informatie [De standaard Adobe Workfront-lay-out](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
   of
   <p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Om deze stappen op systeemniveau uit te voeren, hebt u het toegangsniveau van de Beheerder van het Systeem nodig.</p>
<p>Om hen voor een groep uit te voeren, moet u een manager van die groep zijn.</p> <p><b>OPMERKING</b>:</p> <p>Als u geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt.

Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## Overwegingen bij het maken en beheren van lay-outsjablonen

* Gebruikers kunnen een aantal onderdelen van hun eigen indeling aanpassen. Wanneer u een lay-outmalplaatje verandert, voegen uw veranderingen met om het even welke aanpassingen samen zij, zonder hen te beschrijven of opnieuw in te stellen. Dit geldt ook als u gebruikers toewijst aan een nieuwe lay-outsjabloon.
* Beheerders en gebruikers met een licentie voor abonnementen die andere gebruikers kunnen bewerken, kunnen lay-outsjablonen op systeemniveau en op groepsniveau toevoegen aan de gebruikers die ze kunnen beheren tijdens het bewerken van hun profiel.
* Groepbeheerders kunnen geen lay-outsjablonen toewijzen aan taakrollen of teams.

Zie voor meer informatie over lay-outsjablonen [Lay-outsjablonen](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

<!--removed this from above, but keeping it for a bit, in case it will be needed - known issue around old templates still visible at time:
* Your older layout templates created in Adobe Workfront Classic have been automatically available in your instance of the new Adobe Workfront experience since they were migrated in early Fall 2019. Layout templates created in Adobe Workfront Classic after that time were migrated in April 2020. We recommend that you update these layout templates in the new Adobe Workfront experience to take advantage of new functionality and to make them even more useful in that environment.
-->

## Een lay-outsjabloon maken of wijzigen

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **Interface** > **Layoutsjablonen**.

1. Klikken **Nieuwe lay-outsjabloon**.

   of

   Klik op de naam van de lay-outsjabloon die u wilt wijzigen.

1. Als u een nieuwe lay-outsjabloon maakt, typt u een **Naam van lay-outsjabloon** en (facultatief) a **Beschrijving** daarvoor.

1. Pas gebieden van de gebruikersinterface aan, zoals die in de volgende artikelen worden beschreven:

   * [Het hoofdmenu aanpassen met een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Het linkerdeelvenster aanpassen met een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Vastgezette pagina&#39;s aanpassen met behulp van een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [De weergave Details aanpassen met een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Home en overzicht aanpassen met een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [De landingspagina aanpassen met een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Filters, weergaven en groepen aanpassen met een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [De terminologie van de gebruikersinterface aanpassen met behulp van een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Test de lay-outsjabloon en stel deze ter beschikking van gebruikers, zoals in de volgende artikelen wordt beschreven:

   * [Een nieuwe lay-outsjabloon testen](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Administratieve toegang verlenen voor een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Gebruikers toewijzen aan een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>U kunt ook een lay-outsjabloon maken door deze te kopiëren en de kopie te wijzigen. Zie voor meer informatie [Een lay-outsjabloon kopiëren](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).

