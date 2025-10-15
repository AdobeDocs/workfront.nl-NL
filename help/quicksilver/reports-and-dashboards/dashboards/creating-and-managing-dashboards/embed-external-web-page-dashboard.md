---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Een externe webpagina insluiten in een dashboard
description: U kunt een externe webpagina in een dashboard insluiten om toegang te bieden tot gerelateerde informatie van andere systemen in Adobe Workfront of andere Workfront-pagina's.
author: Nolan
feature: Reports and Dashboards
exl-id: 04b623b5-38b0-4c32-b54e-204f1d422e45
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 0%

---

# Een externe webpagina insluiten in een dashboard

<!--Audited: 01/2025-->

U kunt een externe webpagina in een dashboard insluiten om toegang te bieden tot gerelateerde informatie van andere systemen of vanuit Adobe Workfront.

Als uw organisatie bijvoorbeeld een op het web gebaseerde opslagplaats voor documenten, wiki of een ander contentbeheersysteem heeft dat projectinformatie bevat die regelmatig via een URL wordt benaderd, kunt u die informatie in Workfront weergeven door een externe pagina op een dashboard te maken.

>[!IMPORTANT]
>
>* Vanwege beveiligingsredenen kunt u met bepaalde websites geen webpagina&#39;s insluiten als een iframe. Als de webpagina die u in een dashboard wilt insluiten dit niet toestaat, wordt de pagina niet weergegeven in het dashboard. U kunt de externe pagina echter nog steeds openen door op de naam van het dashboard te klikken.\
>![ Leeg extern paginarapport ](assets/qs-empty-external-page-report-350x165.png)\
>Om het inbedden voor een website toe te staan u bezit, werk met uw Webbeheerder om **x-kader-Opties** het plaatsen aan te passen. Voor meer informatie, zie [ x-kader-Opties ](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).
>
>
>* Dashboardpagina&#39;s worden niet meer ondersteund als ingesloten externe pagina&#39;s in dashboards. Bestaande dashboards worden niet automatisch gewijzigd om deze externe pagina&#39;s te verwijderen, maar wijzigingen aan een dashboard die een dergelijke verwijzing bevat, kunnen pas worden opgeslagen wanneer de verwijzing wordt verwijderd of gewijzigd.
>  > De volgende Workfront.com-subdomeinen worden niet meer ondersteund:
>
>     * /dashboards &#x200B;
>     * /dashboard/:ID &#x200B;
>     * /portfolio/:ID/content-dashboard__:dashboardID &#x200B;
>     * /program/:ID/content-dashboard__:dashboardID &#x200B;
>     * /project/:ID/content-dashboard__:dashboardID &#x200B;
>     * /task/:ID/content-dashboard__:dashboardID &#x200B;
>     * /template/:ID/content-dashboard__:dashboardID &#x200B;
>     * /templatetask/:ID/content-dashboard__:dashboardID &#x200B;
>     * /resourcesManagement/:ID/
>     * content-dashboard_:dashboardID &#x200B;
>     * /team/:ID/content-dashboard__:dashboardID &#x200B;
>     * /iteration/:ID/content-dashboard__:dashboardID &#x200B;
>     * /Requests/:ID/content-dashboard__:dashboardID &#x200B;
>     * /group/:ID/content-dashboard__:dashboardID &#x200B;
>     * /billingrecord/:ID/content-dashboard__:dashboardID
>
>Als alternatieve oplossing, overweeg het omvatten van een lijstrapport in uw dashboard zoals verklaard in [ voeg een rapport aan een Dashboard ](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md) toe

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
      <p>Standard</p>
      <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards en kalenders bewerken</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang tot het dashboard bewerken</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Vereisten

U moet een dashboard maken voordat u er een externe pagina in kunt insluiten.

Voor informatie bij het creëren van dashboards, zie [ een dashboard ](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md) creëren.

## Een externe pagina insluiten in een dashboard

>[!IMPORTANT]
>
>U kunt een externe pagina van een dashboard verwijderen als het niet meer nodig is. U kunt een externe pagina echter niet verwijderen nadat u deze hebt gemaakt in Workfront. U kunt een externe pagina alleen verwijderen met de API. Voor meer informatie, zie [ een Externe Pagina uit een dashboard ](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md) verwijderen.

1. Zoek de URL van de pagina die u wilt weergeven in Workfront en kopieer de URL in de adresbalk.

   >[!NOTE]
   >
   >Als u URL&#39;s deelt met Workfront-objecten, moet u niet vergeten dat sommige URL&#39;s in de loop der tijd verlopen. Document-URL&#39;s verlopen bijvoorbeeld nadat ze zijn geopend. Dit wordt gevormd als veiligheidsmaatregel, en door ontwerp worden zij beschouwd als niet-statische URLs en zouden niet moeten worden gedeeld.

{{step1-to-dashboards}}

1. Om een bestaand dashboard uit te geven, selecteer het dashboard u de website binnen wilt inbedden pagina, dan klik **Acties van het Dashboard**, dan klik **uitgeven**
of\
   Om een nieuw dashboard tot stand te brengen, klik **Nieuw Dashboard**.\
   Voor meer informatie over het creëren van een dashboard, zie [ een dashboard ](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md) creëren.

1. Klik **toevoegen Externe Pagina** onder **Uitgezochte Lay-out/voeg Rapporten/toevoegt Calendars** gebied toe.

   ![ voeg externe pagina ](assets/qs-add-external-page-350x239.png) toe

   **voegt Externe de vakvertoningen van de Pagina** toe.

1. Geef de volgende informatie op over de externe pagina:

   * **Naam**: Voeg een naam voor het dashboard toe.
   * **Beschrijving**: Voeg meer informatie over het dashboard toe om de informatie te identificeren het bevat. De beschrijving wordt op het dashboard weergegeven voor iedereen die toegang heeft om de beschrijving weer te geven, nadat u deze hebt opgeslagen.
   * **URL**: Deeg URL u vroeger op dit gebied kopieerde.

     U kunt de volgende typen URL&#39;s opgeven:

      * Een (gecodeerde) https-URL naar een webpagina.\
        Alleen https-pagina&#39;s (versleuteld) worden met de URL geladen.\
        ![ voeg externe paginadialoog ](assets/add-external-page-dialog-qs-350x247.png) toe

      * Een sjabloon-URL die sessiegegevens voor een specifieke website bevat.\
        Bijvoorbeeld: *https://localhost/?session={!$$SESSION}*
U moet zijn aangemeld bij de opgegeven website om de externe pagina weer te geven.\
        Voor informatie over hoe te om een SessionID van Workfront te verkrijgen, zie [ API basissen ](../../../wf-api/general/api-basics.md).\
        Uw Workfront-beheerder kan uw systeemvoorkeuren zodanig configureren dat sessiegegevens uit beveiligingsoverwegingen niet kunnen worden gebruikt in externe pagina&#39;s. In dit geval wordt de externe pagina niet op het dashboard geladen.\
        Voor meer informatie over de voorkeur van de systeemveiligheid, zie [ de voorkeur van de systeemveiligheid ](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md) vormen.\
        ![ external_page_with_session_id_example.png ](assets/external-page-with-session-id-example-350x134.png)

     >[!WARNING]
     >
     >Het gebruik van de SessionID is onveilig en wordt niet aangeraden.
     >

   * **Hoogte**: Type een aantal groter dan 0 om de ruimte te bepalen die de externe pagina op het dashboard bezet. De standaardhoogte is 500.

1. Klik **sparen**.

   De pagina wordt automatisch toegevoegd aan het dashboard.

   Als u extra dashboards creeert, kunt u deze externe pagina vinden en het toevoegen aan andere dashboards. U kunt alle bestaande externe pagina&#39;s vinden in de lijst met beschikbare rapporten en kalenders wanneer u een dashboard maakt of bewerkt.

   <!--
    *** This is linked to: Creating Dashboards, and Editing Dashboards.
   -->

## Een externe pagina in een dashboard bijwerken

De gegevens bijwerken voor een externe pagina die in een dashboard wordt gebruikt:

{{step1-to-dashboards}}

1. Klik de naam van het dashboard dat u wilt bijwerken om het te openen, en **Acties Dashboard** te klikken, dan **geeft** uit.

   Het **vakje van de Details van het Dashboard** opent.

1. In **Uitgezochte Lay-out/voeg het gebied van Rapporten** van de **doos van de Details van het Dashboard** toe, bepaal de plaats van de externe pagina u, over het wilt bijwerken en **klikken geeft** pictogram uit.\
   ![ Inline geeft externe pagina uit ](assets/nwe-inline-edit-external-page-350x226.png)

1. In **geef Externe de doos van de Pagina** uit, werk de gebieden bij u wilt veranderen, dan klik **sparen**.
1. (Facultatief) klik het **pictogram van de Schrapping** pictogram van de Schrapping ![ om de externe pagina uit het dashboard te verwijderen. ](assets/delete.png) Voor meer informatie, zie [ een Externe Pagina uit een dashboard ](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md) verwijderen.
1. Klik **sparen + Sluiten**.

## Externe pagina&#39;s in een rapport weergeven

U kunt alle externe pagina&#39;s in Workfront weergeven in een rapport Externe pagina.

{{step1-to-reports}}

1. Klik **Nieuw Rapport** > selecteren **Externe Sectie**.

   ![ Externe sectie ](assets/external-page-new-report-in-dropdown-nwe.png)

1. (Optioneel) Werk de tabbladen Weergave, Filters of Groepen van het rapport bij.

   Voor meer informatie, zie [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

1. Klik **sparen + Sluiten**.

   In het nieuwe rapport kunt u de naam en de URL weergeven die aan externe pagina&#39;s in uw systeem zijn gekoppeld.

