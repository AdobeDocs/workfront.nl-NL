---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Een externe webpagina insluiten in een dashboard
description: U kunt een externe webpagina in een dashboard insluiten om toegang te bieden tot gerelateerde informatie van andere systemen in Adobe Workfront of andere Workfront-pagina's.
author: Nolan
feature: Reports and Dashboards
exl-id: 04b623b5-38b0-4c32-b54e-204f1d422e45
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Een externe webpagina insluiten in een dashboard

U kunt een externe webpagina in een dashboard insluiten om toegang te bieden tot gerelateerde informatie van andere systemen in Adobe Workfront of andere Workfront-pagina&#39;s.

Als uw organisatie bijvoorbeeld een op het web gebaseerde opslagplaats voor documenten, wiki of een ander contentbeheersysteem heeft dat projectinformatie bevat die regelmatig via een URL wordt benaderd, kunt u die informatie in Workfront weergeven door een externe pagina op een dashboard te maken.

>[!IMPORTANT]
>
>Vanwege beveiligingsredenen kunt u met bepaalde websites geen webpagina&#39;s insluiten als een iframe. Als de webpagina die u in een dashboard wilt insluiten dit niet toestaat, wordt de pagina niet weergegeven in het dashboard. U kunt de externe pagina echter nog steeds openen door op de naam van het dashboard te klikken.\
>![](assets/qs-empty-external-page-report-350x165.png)\
>Als u insluiten wilt toestaan voor een website die u bezit, werkt u samen met uw webbeheerder om de instelling **X-frame-opties** instellen. Zie voor meer informatie [X-frame-opties](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-abonnement*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>Toegang tot rapporten, dashboards en kalenders bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Rechten voor het dashboard beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

U moet een dashboard maken voordat u er een externe pagina in kunt insluiten.

Voor informatie over het maken van dashboards raadpleegt u [Een dashboard maken](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Een externe pagina insluiten in een dashboard

>[!IMPORTANT]
>
>U kunt een externe pagina van een dashboard verwijderen als het niet meer nodig is. U kunt een externe pagina echter niet verwijderen nadat u deze hebt gemaakt in Workfront. U kunt een externe pagina alleen verwijderen met behulp van de API. Zie voor meer informatie [Een externe pagina verwijderen van een dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).

1. Zoek de URL van de pagina die u wilt weergeven in Workfront en kopieer de URL in de adresbalk.

   >[!NOTE]
   >
   >Als u URL&#39;s deelt met Workfront-objecten, moet u niet vergeten dat sommige URL&#39;s in de loop der tijd verlopen. Document-URL&#39;s verlopen bijvoorbeeld nadat ze zijn geopend. Dit wordt gevormd als veiligheidsmaatregel, en door ontwerp worden zij beschouwd als niet-statische URLs en zouden niet moeten worden gedeeld.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png)en klik vervolgens op **Dashboards**.

1. Als u een bestaand dashboard wilt bewerken, selecteert u het dashboard waarin u de websitepagina wilt insluiten en klikt u op **Dashboardhandelingen** en selecteert u **Bewerken** in het menu.\
   of\
   Als u een nieuw dashboard wilt maken, klikt u op **Nieuw dashboard**.\
   Ga voor meer informatie over het maken van een dashboard naar [Een dashboard maken](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

1. Klikken **Externe pagina toevoegen**.

   ![](assets/qs-add-external-page-350x239.png)

1. Geef een **Naam** voor de externe pagina.
1. Geef een **Beschrijving**.
1. Plak de URL die u eerder hebt gekopieerd in het dialoogvenster **URL** veld.\
   U kunt de volgende typen URL&#39;s opgeven:

   * Een (gecodeerde) https-URL naar een webpagina.\
      Alleen https-pagina&#39;s (versleuteld) worden met de URL geladen.\
      ![](assets/add-external-page-dialog-qs-350x247.png)

   * Een sjabloon-URL die sessiegegevens voor een specifieke website bevat.\
      Bijvoorbeeld: *https://localhost/?session={!$$SESSION}*
U moet zijn aangemeld bij de opgegeven website om de externe pagina weer te geven.\
      Voor informatie over hoe u een SessionID kunt verkrijgen van Workfront raadpleegt u [Basisbeginselen van API](../../../wf-api/general/api-basics.md).\
      Uw Workfront-beheerder kan uw systeemvoorkeuren zodanig configureren dat sessiegegevens uit beveiligingsoverwegingen niet kunnen worden gebruikt in externe pagina&#39;s. In dit geval wordt de externe pagina niet op het dashboard geladen.\
      Voor meer informatie over de voorkeuren voor systeembeveiliging raadpleegt u [Beveiligingsvoorkeuren voor het systeem configureren](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).\
      ![external_page_with_session_id_example.png](assets/external-page-with-session-id-example-350x134.png)

1. Klikken **Opslaan**.\
   De pagina wordt automatisch toegevoegd aan het dashboard. Als er toekomstige dashboards worden gemaakt, kan de externe pagina worden toegevoegd. De externe pagina is te vinden onder Beschikbare rapporten.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Alina: *** This is linked to: Creating Dashboards, and Editing Dashboards.)
   </MadCap:conditionalText>
   -->

## Een externe pagina in een dashboard bijwerken

De gegevens bijwerken voor een externe pagina die in een dashboard wordt gebruikt:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png)en klik vervolgens op **Dashboards**.
1. Selecteer het dashboard dat u wilt bijwerken, en klik dan **Bewerken** ![](assets/edit-icon.png).

   ![Selecteer het pictogram Bewerken.](assets/nwe-editdashboard2021-350x188.png)

1. Zoek aan de rechterkant van het scherm de externe pagina die u wilt bijwerken en klik op de knop **Bewerken** pictogram.\
   ![](assets/nwe-inline-edit-external-page-350x226.png)

1. In de **Externe pagina bewerken** , werkt u de velden bij die u wilt wijzigen en klikt u vervolgens op **Opslaan**.
1. (Optioneel) Klik op de knop **Verwijderen** pictogram ![](assets/delete.png) om de externe pagina uit het dashboard te verwijderen. Zie voor meer informatie [Een externe pagina verwijderen van een dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).
1. Klik in de linkerbenedenhoek op **Opslaan + Sluiten**.

## Externe pagina&#39;s in een rapport weergeven

U kunt alle externe pagina&#39;s in Workfront weergeven in een rapport Externe pagina.

1. Ga naar de **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) > **Rapporten**.
1. Klikken **Nieuw rapport** > selecteren **Externe pagina**.

   ![](assets/external-page-new-report-in-dropdown-nwe.png)

1. (Optioneel) Werk de tabbladen Weergave, Filters of Groepen van het rapport bij.

   Zie voor meer informatie [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Klikken **Opslaan en sluiten**.

   U kunt de naam en de URL die aan de externe pagina&#39;s in uw systeem zijn gekoppeld in het nieuwe rapport bekijken.

   ![](assets/external-page-report-name-url-columns-nwe-350x213.png)
