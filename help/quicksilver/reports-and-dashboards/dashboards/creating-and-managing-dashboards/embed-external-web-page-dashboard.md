---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Een externe webpagina insluiten in een dashboard
description: U kunt een externe webpagina in een dashboard insluiten om toegang te bieden tot gerelateerde informatie van andere systemen in Adobe Workfront of andere Workfront-pagina's.
author: Nolan
feature: Reports and Dashboards
exl-id: 04b623b5-38b0-4c32-b54e-204f1d422e45
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 0%

---

# Een externe webpagina insluiten in een dashboard

<!--Audited: 01/2024-->

U kunt een externe webpagina in een dashboard insluiten om toegang te bieden tot gerelateerde informatie van andere systemen of vanuit Adobe Workfront.

Als uw organisatie bijvoorbeeld een op het web gebaseerde opslagplaats voor documenten, wiki of een ander contentbeheersysteem heeft dat projectinformatie bevat die regelmatig via een URL wordt benaderd, kunt u die informatie in Workfront weergeven door een externe pagina op een dashboard te maken.

>[!IMPORTANT]
>
>* Vanwege beveiligingsredenen kunt u met bepaalde websites geen webpagina&#39;s insluiten als een iframe. Als de webpagina die u in een dashboard wilt insluiten dit niet toestaat, wordt de pagina niet weergegeven in het dashboard. U kunt de externe pagina echter nog steeds openen door op de naam van het dashboard te klikken.\
>![](assets/qs-empty-external-page-report-350x165.png)\
>Als u insluiten wilt toestaan voor een website die u bezit, werkt u samen met uw webbeheerder om de instelling **X-frame-opties** instellen. Zie voor meer informatie [X-frame-opties](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).
>
>
>* Dashboardpagina&#39;s worden niet meer ondersteund als ingesloten externe pagina&#39;s in dashboards. Bestaande dashboards worden niet automatisch gewijzigd om deze externe pagina&#39;s te verwijderen, maar wijzigingen aan een dashboard die een dergelijke verwijzing bevat, kunnen pas worden opgeslagen wanneer de verwijzing wordt verwijderd of gewijzigd.
> De volgende Workfront.com-subdomeinen worden niet meer ondersteund:
>
>     * /dashboards &#x200B;
>     * /dashboard/:ID-&#x200B;
>     * /portfolio/:ID/content-dashboard__:dashboardID-&#x200B;
>     * /program/:ID/content-dashboard__:dashboardID &#x200B;
>     * /project/:ID/content-dashboard__:dashboardID &#x200B;
>     * /task/:ID/content-dashboard__:dashboardID &#x200B;
>     * /template/:ID/content-dashboard__:dashboardID-&#x200B;
>     * /templatetask/:ID/content-dashboard__:dashboardID &#x200B;
>     * /resourcesManagement/:ID/
>     * content-dashboard__:dashboardID &#x200B;
>     * /team/:ID/content-dashboard__:dashboardID &#x200B;
>     * /iteration/:ID/content-dashboard__:dashboardID &#x200B;
>     * /Requests/:ID/content-dashboard__:dashboardID &#x200B;
>     * /group/:ID/content-dashboard__:dashboardID &#x200B;
>     * /billingrecord/:ID/content-dashboard__:dashboardID
>
>Als alternatieve oplossing kunt u overwegen een lijstrapport op te nemen in het dashboard, zoals wordt uitgelegd in [Een rapport toevoegen aan een dashboard](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md)

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td> <p>Huidig: Plan </p>
   of
   <p>Nieuw: Standaard </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau</strong></td> 
   <td> <p>Toegang tot rapporten, dashboards en kalenders bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt. Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

U moet een dashboard maken voordat u er een externe pagina in kunt insluiten.

Zie voor informatie over het maken van dashboards [Een dashboard maken](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Een externe pagina insluiten in een dashboard

>[!IMPORTANT]
>
>U kunt een externe pagina van een dashboard verwijderen als het niet meer nodig is. U kunt een externe pagina echter niet verwijderen nadat u deze hebt gemaakt in Workfront. U kunt een externe pagina alleen verwijderen met de API. Zie voor meer informatie [Een externe pagina verwijderen van een dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).

1. Zoek de URL van de pagina die u wilt weergeven in Workfront en kopieer de URL in de adresbalk.

   >[!NOTE]
   >
   >Als u URL&#39;s deelt met Workfront-objecten, moet u niet vergeten dat sommige URL&#39;s in de loop der tijd verlopen. Document-URL&#39;s verlopen bijvoorbeeld nadat ze zijn geopend. Dit wordt gevormd als veiligheidsmaatregel, en door ontwerp worden zij beschouwd als niet-statische URLs en zouden niet moeten worden gedeeld.

{{step1-to-dashboards}}

1. Als u een bestaand dashboard wilt bewerken, selecteert u het dashboard waarin u de websitepagina wilt insluiten en klikt u op **Dashboardhandelingen** en klik vervolgens op **Bewerken**
of\
   Als u een nieuw dashboard wilt maken, klikt u **Nieuw dashboard**.\
   Ga voor meer informatie over het maken van een dashboard naar [Een dashboard maken](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

1. Klikken **Externe pagina toevoegen** onder de **Selecteer Layout/Rapporten toevoegen/Kalenders toevoegen** gebied.

   ![](assets/qs-add-external-page-350x239.png)

   De **Externe pagina toevoegen** wordt weergegeven.

1. Geef de volgende informatie op over de externe pagina:

   * **Naam**: Voeg een naam voor het dashboard toe.
   * **Beschrijving**: Voeg meer informatie over het dashboard toe om de informatie te identificeren die het bevat. De beschrijving wordt op het dashboard weergegeven voor iedereen die toegang heeft om de beschrijving weer te geven, nadat u deze hebt opgeslagen.
   * **URL**: plak de URL die u eerder in dit veld hebt gekopieerd.

     U kunt de volgende typen URL&#39;s opgeven:

      * Een (gecodeerde) https-URL naar een webpagina.\
        Alleen https-pagina&#39;s (versleuteld) worden met de URL geladen.\
        ![](assets/add-external-page-dialog-qs-350x247.png)

      * Een sjabloon-URL die sessiegegevens voor een specifieke website bevat.\
        Bijvoorbeeld: *https://localhost/?session={!$$SESSION}*
U moet zijn aangemeld bij de opgegeven website om de externe pagina weer te geven.\
        Voor informatie over hoe u een SessionID kunt verkrijgen van Workfront raadpleegt u [Basisbeginselen van API](../../../wf-api/general/api-basics.md).\
        Uw Workfront-beheerder kan uw systeemvoorkeuren zodanig configureren dat sessiegegevens uit beveiligingsoverwegingen niet kunnen worden gebruikt in externe pagina&#39;s. In dit geval wordt de externe pagina niet op het dashboard geladen.\
        Zie voor meer informatie over de voorkeuren voor systeembeveiliging [Systeembeveiligingsvoorkeuren configureren](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).\
        ![external_page_with_session_id_example.png](assets/external-page-with-session-id-example-350x134.png)

     >[!WARNING]
     >
     >Het gebruik van de SessionID is onveilig en wordt niet aangeraden.
     >

   * **Hoogte**: Typ een getal groter dan 0 om de ruimte te definiëren die de externe pagina inneemt op het dashboard. De standaardhoogte is 500.

1. Klikken **Opslaan**.

   De pagina wordt automatisch toegevoegd aan het dashboard.

   Als u extra dashboards creeert, kunt u deze externe pagina vinden en het toevoegen aan andere dashboards. U kunt alle bestaande externe pagina&#39;s vinden in de lijst met beschikbare rapporten en kalenders wanneer u een dashboard maakt of bewerkt.

   <!--
    *** This is linked to: Creating Dashboards, and Editing Dashboards.
   -->

## Een externe pagina in een dashboard bijwerken

De gegevens bijwerken voor een externe pagina die in een dashboard wordt gebruikt:

{{step1-to-dashboards}}

1. Klik op de naam van het dashboard dat u wilt bijwerken om het te openen, en klik op **Dashboardhandelingen** vervolgens **Bewerken**.

   De **Details dashboard** wordt geopend.

1. In de **Selecteer Indeling / Rapporten toevoegen / Kalenders toevoegen** gebied van de **Details dashboard** , zoekt u de externe pagina die u wilt bijwerken, plaatst u de muis boven de pagina en klikt u op de knop **Bewerken** pictogram.\
   ![](assets/nwe-inline-edit-external-page-350x226.png)

1. In de **Externe pagina bewerken** , werkt u de velden bij die u wilt wijzigen en klikt u vervolgens op **Opslaan**.
1. (Optioneel) Klik op de knop **Verwijderen** pictogram ![](assets/delete.png) om de externe pagina uit het dashboard te verwijderen. Zie voor meer informatie [Een externe pagina verwijderen van een dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).
1. Klikken **Opslaan + Sluiten**.

## Externe pagina&#39;s in een rapport weergeven

U kunt alle externe pagina&#39;s in Workfront weergeven in een rapport Externe pagina.

{{step1-to-reports}}

1. Klikken **Nieuw rapport** > selecteren **Externe pagina**.

   ![](assets/external-page-new-report-in-dropdown-nwe.png)

1. (Optioneel) Werk de tabbladen Weergave, Filters of Groepen van het rapport bij.

   Zie voor meer informatie [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Klikken **Opslaan en sluiten**.

   U kunt de naam en de URL die aan de externe pagina&#39;s in uw systeem zijn gekoppeld in het nieuwe rapport bekijken.

   ![](assets/external-page-report-name-url-columns-nwe-350x213.png)
