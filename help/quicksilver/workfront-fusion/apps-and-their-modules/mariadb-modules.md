---
title: MariaDB-modules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die gebruiken [!DNL MariaDB]en deze verbinding maken met meerdere toepassingen en services van derden.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# [!DNL MariaDB] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL MariaDB]en deze verbinding maken met meerdere toepassingen en services van derden.

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

Te gebruiken [!DNL MariaDB] modules, moet u een [!DNL MariaDB] account.

## Verbinden [!DNL MariaDB] tot [!DNL Workfront Fusion]

U kunt een verbinding maken met uw [!DNL MariaDB] rechtstreeks vanuit een [!DNL MariaDB] module.

1. In alle [!DNL MariaDB] module, klikt u op **[!UICONTROL Add]** naast de [!UICONTROL Connection] veld.
1. Configureer de volgende velden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>Voer een naam in voor de nieuwe verbinding.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Host]</td> 
      <td> <p>Voer het IP-adres of de hostnaam van uw databaseinstantie in. Deze gastheer moet van buiten uw netwerk toegankelijk zijn.</p> <p>Voorbeeld: <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Port]</td> 
      <td>De standaardpoort is 3306. Als u een niet-standaardhaven gebruikt, plaats dit aantal aan uw haven. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Database Name]</td> 
      <td>Voer de naam in van de database waarmee u wilt communiceren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Username]</td> 
      <td>Voer uw gebruikersnaam in.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Password]</td> 
      <td>Voer uw wachtwoord in.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **[!UICONTROL Continue]** om de verbinding tot stand te brengen en terug naar de module te gaan.

## [!DNL MariaDB] Modules en hun velden

Wanneer u [!DNL MariaDB] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL MariaDB] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Een query uitvoeren (geavanceerd)

Deze actiemodule wint informatie van uw gegevensbestand terug, die op een vraag wordt gebaseerd u verstrekt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Voor instructies over het aansluiten van uw [!DNL MariaDB] account aan [!DNL Workfront Fusion], zie <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL MariaDB] tot [!DNL Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td> <p>Ga de SQL vraag in die u de module wilt gebruiken om gegevens terug te winnen.</p> <p>Belangrijk: Variabelen die in de query worden gebruikt, worden niet ontsmet. Zorg ervoor dat u variabelen goed ontsmet om SQL-injectie te voorkomen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Select rows from a table (advanced)]

Deze module leest verslag van uw gegevensbestand.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Voor instructies over het aansluiten van uw [!DNL MariaDB] account aan [!DNL Workfront Fusion], zie <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL MariaDB] tot [!DNL Workfront Fusion]</a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table]</td> 
   <td> <p>Selecteer de tabel die de records bevat die u wilt lezen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Het filter instellen waarmee u rijen wilt selecteren</p> 
    <ul> 
     <li> <p>Selecteer het veld waarnaar u wilt zoeken</p> </li> 
     <li> <p>Selecteer de operator die u voor de zoekopdracht wilt gebruiken</p> </li> 
     <li> <p>Voer de waarde in of wijs de waarde toe waarnaar u wilt zoeken.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort] </td> 
   <td> <p>Voor elk niveau waarop u de resultaten wilt sorteren, klikt u op <strong>[!UICONTROL Add item]</strong>selecteert u vervolgens het veld waarop u de resultaten wilt sorteren en of u oplopend of aflopend wilt sorteren</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>
