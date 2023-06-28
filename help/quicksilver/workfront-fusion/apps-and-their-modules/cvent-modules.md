---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Cilummodules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die Cvent gebruiken, evenals het verbinden met veelvoudige derdetoepassingen en de diensten.
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---

# [!DNL Cvent] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Cvent]en deze verbinding maken met meerdere toepassingen en services van derden.

Als u instructies bij het creëren van een scenario nodig hebt, zie [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Voor informatie over modules, zie [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] of hoger</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereisten: Als u de [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Oudere productvereisten: Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Te gebruiken [!DNL Cvent] modules, moet u een [!DNL Cvent] account.

## Verbinden [!DNL Cvent] tot [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>De [!DNL Cvent] modules werken via een [!UICONTROL SOAP] API. Verbinding maken met [!DNL Cvent]moet u het volgende doen:
>
>* U hebt [!UICONTROL SOAP] toegang tot de [!DNL Cvent] API.
>* De [!DNL Workfront Fusion] IP de adressen zijn toegevoegd aan de lijst van gewenste personen van uw organisatie.
>
>  Voor een lijst met [!DNL Workfront Fusion] IP-adressen, zie [IP Adressen voor de toegang tot [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


U kunt een verbinding maken met uw [!DNL Cvent] rechtstreeks vanuit een [!DNL Cvent] module.

1. In alle [!DNL Cvent] module, klikt u op **[!UICONTROL Add]** naast de [!UICONTROL Connection] veld.
1. Selecteer het gebied waarmee u verbinding wilt maken.

   * [!UICONTROL North America]
   * [!UICONTROL Europe]
   * [!UICONTROL Sandbox]

1. Klikken **[!UICONTROL Continue]** om de verbinding tot stand te brengen en terug naar de module te gaan.

## [!DNL Cvent] modules en hun velden

Wanneer u [!DNL Cvent] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Cvent] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Handelingen](#actions)
* [Zoekopdrachten](#searches)

### Handelingen

* [[!UICONTROL Custom API Call]](#create-meeting-request)
* [[!UICONTROL Read a record]](#read-a-record)
* [[!UICONTROL Register Invitee]](#register-invitee)
* [[!UICONTROL Add Invitee]](#add-invitee)
* [[!UICONTROL Delete Contact]](#delete-contact)
* [[!UICONTROL Update Contact]](#update-contact)
* [[!UICONTROL Create meeting request]](#create-meeting-request)

#### [!UICONTROL Custom API Call]

Deze actiemodule laat u een douane voor authentiek verklaarde vraag aan het maken [!DNL Cvent] API. Op deze manier kunt u een automatisering van de gegevensstroom maken die niet door de ander kan worden uitgevoerd [!DNL Cvent] modules.

Als u deze module configureert, worden de volgende velden weergegeven.

De module keert een statuscode, samen met de kopballen en het lichaam van de API vraag terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Cvent] account aan [!DNL Workfront Fusion], zie <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Cvent] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewerking</td> 
   td&gt; <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Hoofdtekst (XML)</td> 
   <td> <p>Ga of kaart het lichaam van de API vraag in. Dit mag alleen de XML bevatten. De module zal automatisch authentificatiekopballen omvatten. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Read a record]

Deze actiemodule leest informatie over een specifieke record.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Cvent] account aan [!DNL Workfront Fusion], zie <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Cvent] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Record type]</p> </td> 
   <td>Selecteer het itemtype van de record die u wilt lezen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact] / [!UICONTROL Event] / [!UICONTROL Invitee ID]</td> 
   <td> <p>Voer de id in van het item dat u wilt lezen of wijs deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Selecteer de velden die u in de uitvoer van de module wilt opnemen. De velden zijn beschikbaar op basis van het geselecteerde itemtype.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Register Invitee]

In deze actiemodule wordt een genodigde voor een gebeurtenis geregistreerd.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Cvent] account aan [!DNL Workfront Fusion], zie <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Cvent] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Id genodigde</p> </td> 
   <td> <p>Voer de id in van de genodigde die u voor een gebeurtenis wilt registreren of wijs deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gebeurtenis-id</td> 
   <td> <p>Voer de id in van de gebeurtenis waarvoor u de genodigde wilt registreren of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add Invitee]

Deze actiemodule nodigt een contactpersoon voor een gebeurtenis uit.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Cvent] account aan [!DNL Workfront Fusion], zie <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Cvent] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contact ID]</p> </td> 
   <td> <p>Voer de id in van de contactpersoon die u aan een gebeurtenis wilt toevoegen of wijs deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Voer de id in van de gebeurtenis waaraan u de contactpersoon wilt toevoegen of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete Contact]

Deze actiemodule schrapt één enkel contact in Gebeurtenis.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Cvent] account aan [!DNL Workfront Fusion], zie <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Cvent] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Contact ID]</td> 
   <td> <p>Ga of kaart identiteitskaart van het contact in u wilt schrappen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update Contact]

Deze actiemodule werkt een bestaand contact bij gebruikend zijn identiteitskaart

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Cvent] account aan [!DNL Workfront Fusion], zie <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Cvent] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contact ID]</p> </td> 
   <td> <p>Ga of kaart identiteitskaart van het contact in u wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>Selecteer de velden waarvoor u informatie wilt invoeren en vul vervolgens de gewenste waarden voor die velden in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
   <td> <p>Selecteer de velden waarvoor u informatie wilt invoeren en vul vervolgens de gewenste waarden voor die velden in.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create meeting request]

Met deze actiemodule voegt u een verzoek voor een vergadering toe aan uw account.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Cvent] account aan [!DNL Workfront Fusion], zie <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Cvent] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Form ID]</p> </td> 
   <td> <p>Voer de id in van het formulier dat u wilt gebruiken om de nieuwe vergaderingsaanvraag te maken of wijs deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Meeting Request Fields]</td> 
   <td> <p>Selecteer de velden voor vergaderingsverzoeken waarvoor u informatie wilt invoeren en vul vervolgens de gewenste waarden voor die velden in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event Request Fields]</td> 
   <td> <p>Selecteer de velden met gebeurtenisaanvragen waarvoor u informatie wilt invoeren en vul vervolgens de gewenste waarden voor die velden in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL RFP Request Fields]</td> 
   <td> <p>Selecteer het verzoek om voorstellen gebieden die u informatie voor wilt invoeren, dan vult de gewenste waarden voor die gebieden in.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Zoekopdrachten

#### [!UICONTROL List records]

Deze onderzoeksmodule wint informatie over alle verslagen van een specifiek type terug.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Cvent] account aan [!DNL Workfront Fusion], zie <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Cvent] tot [!DNL Adobe Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Record type]</p> </td> 
   <td> <p>Selecteer het type record dat u wilt weergeven.</p> 
    <ul> 
     <li> <p>Alle gebeurtenissen van uw [!DNL Cvent] account</p> </li> 
     <li> <p>Alle sessies voor een gebeurtenis</p> </li> 
     <li> <p>Alle genodigden voor een gebeurtenis</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Als u genodigden of sessies opsomt, voert u de id in of wijst u deze toe aan de gebeurtenis waaraan deze genodigden of sessies zijn gekoppeld.</p> </td> 
  </tr> 
 </tbody> 
</table>
