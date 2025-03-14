---
product-area: enterprise-scenario-planner-product-area
keywords: plan, toestemmingen, aandeel, initiatieven, scenario's, scenario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Een abonnement delen in de Scenario-planner
description: U kunt een abonnement dat u hebt gemaakt in de Adobe Workfront Scenario Planner delen met andere gebruikers.
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# Een abonnement delen in de [!DNL Scenario Planner]

<!--Audited: 07/2024-->

U kunt een abonnement in de [!DNL Adobe Workfront Scenario Planner] delen met andere gebruikers, zodat zij aan het werk kunnen samenwerken dat u doet.

>[!TIP]
>
>Als u een koppeling naar een plan naar anderen stuurt, moet u het plan ook met hen delen opdat zij het kunnen bekijken.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>Nieuw: Ultimate </p></li>
   <p>De Scenario Planner is niet beschikbaar voor de nieuwe Workfront Select- of Workfront Prime-plannen. </p>
   <li><p>Huidig: [!UICONTROL Business] of hoger</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licentie*</p> </td> 
   <td> <p>Nieuw: Licht of hoger</p> 
   <p>Huidig: [!UICONTROL Review] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>Voor de nieuwe plannen van Workfront:</p><p> Adobe Workfront</li></p>
   <li><p>Voor de huidige plannen van Workfront: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>

<p>Voor meer informatie, zie <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref"> Toegang nodig om [!DNL Scenario Planner]</a> te gebruiken. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Toegangsniveau </td> 
   <td> <p>[!UICONTROL Edit] toegang tot de [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objectmachtigingen </p> </td> 
   <td> <p>[!UICONTROL Manage] machtigingen voor een abonnement</p> <p>Voor informatie bij het vragen van om extra toegang tot een plan, zie <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref"> de toegang van het Verzoek tot een plan in [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang tot de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

* De gebruikers die machtigingen voor het abonnement hebben, moeten toegang hebben tot het [!DNL Scenario Planner] -gebied in hun toegangsniveaus, zoals toegestaan door uw [!DNL Workfront] -beheerder, om machtigingen voor een abonnement te kunnen ontvangen.

  [!UICONTROL Requestors] kan bijvoorbeeld geen plannen weergeven, maken of bewerken. Houd dit in gedachten wanneer u een abonnement deelt met een gebruiker die een licentie voor de aanvrager heeft.

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

Voor meer informatie over toegang tot [!DNL Scenario Planner] voor diverse licentietypen, zie [ de toegang van de Verlening tot  [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## Overwegingen bij het delen van plannen

* Alle gebruikers, met inbegrip van systeembeheerders, hebben toegang slechts tot plannen die zij creeerden.
* U kunt één enkel plan delen, of u kunt veelvoudige plannen, in bulk delen.
* U kunt geen plannen bekijken die u niet creeerde of die niet met u worden gedeeld.
* U kunt een abonnement alleen met andere gebruikers delen. U kunt geen plannen met groepen, teams, of bedrijven delen.
* U moet een abonnement eerst opslaan voordat u het kunt delen.
* U kunt een URL naar een abonnement met een andere gebruiker delen. Als de gebruiker geen toestemmingen heeft om het plan minstens te bekijken, kunnen zij om toegang tot het plan van een andere gebruiker verzoeken wanneer zij URL ontvangen. Voor informatie over het verzoeken van toegang tot een plan, zie [ toegang van het Verzoek tot een plan in  [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
* Wanneer u meerdere plannen deelt die al met anderen zijn gedeeld, worden de gebruikers met wie u deelt niet vervangen, maar toegevoegd aan de bestaande gebruikers op elk abonnement dat u hebt geselecteerd.

## Opties voor overzichtsmachtigingen

De volgende lijst maakt een lijst van de toestemmingen die u kunt verlenen wanneer het delen van een plan. Voor meer informatie over de toegangsgebruikers die op hun vergunning worden gebaseerd, zie [ toegang van de Verlening tot  [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong> Acties </strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Manage]</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL View]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Plan weergeven </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Initiatieven weergeven </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Weergavescenario's</td> 
   <td>✓</td> 
   <td><span style="font-weight: normal;"> ✓ </span> </td> 
  </tr> 
  <tr> 
   <td>Taakrollen weergeven</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Kosten en begrotingsgegevens weergeven*</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>Kosten en begrotingsgegevens beheren*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Initiatieven maken</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Scènes maken</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Initiatieven of scenario's verwijderen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>scenario's kopiëren</td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Publicatiescenario's**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*U moet toegang tot Financiële Gegevens hebben om financiële informatie over plannen te kunnen bekijken of beheren, zelfs als u toestemmingen aan plannen beheert. Voor informatie over toegang tot financiële gegevens, zie [ Toegang van de Verlening tot financiële gegevens ](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

**U moet toegang hebben tot creëren en toestemmingen om projecten te beheren om scenario&#39;s te kunnen publiceren.

Voor informatie over het niveau van de projecttoegang, zie [ Toegang van de Verlening tot projecten ](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Voor informatie over projecttoestemmingen, zie [ een project in  [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md) delen.

## Abonnementen delen

{{step1-to-scenario-planner}}

1. Klik op de naam van een abonnement om het te openen

   of

   Selecteer verschillende plannen om deze in bulk te delen.

   >[!TIP]
   >
   >U kunt een plan delen door de avatars van gebruikers te klikken met wie het plan in de hoger-juiste hoek van de plankopbal wordt gedeeld.

1. (Voorwaardelijk) als u een plan opende, klik het **[!UICONTROL More]** pictogram ![ Meer pictogram ](assets/more-icon.png) rechts van de [!UICONTROL Plan] naam, dan klik **[!UICONTROL Share]**

   of

   Als u meerdere plannen hebt geselecteerd om deze in bulk te delen, klikt u op het pictogram **[!UICONTROL Share]** ![](assets/share-icon-26x26.png) boven aan de lijst met plannen om het toegangsvak [!UICONTROL Plan] te openen.

   >[!TIP]
   >
   >* Gebruikers die machtigingen hebben voor alle plannen die u selecteert, worden in het toegangsvak [!UICONTROL Plan] weergegeven.
   >* Eventuele extra gebruikers worden toegevoegd aan en vervangen de bestaande gebruikers op alle geselecteerde plannen niet.

1. Typ in het veld **[!UICONTROL Give plan access to]** de naam van de gebruikers met wie u het abonnement wilt delen en selecteer de gebruikers in de lijst.
1. Van het drop-down menu van toestemmingen rechts van de gebruikersnaam, selecteer het niveau van toestemming u hen aan het plan wilt verlenen.
1. Selecteer een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL View]</td> 
      <td>De gebruikers u het plan met deelt zullen toestemmingen hebben om het plan te bekijken. Zij kunnen geen informatie over het plan uitgeven, initiatieven toevoegen, scenario's, of scenario's publiceren. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Manage]</td> 
      <td> <p>De gebruikers u het plan met deelt hebben toestemmingen om het plan te beheren, dat omvat uitgeven informatie, voegt initiatieven, scenario's toe, en publiceert het plan. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >U kunt een abonnement alleen verwijderen wanneer u het hebt gemaakt. U kunt geen plannen schrappen die met u worden gedeeld.

1. Klik op **[!UICONTROL Save]**.

   Het abonnement wordt nu gedeeld met de gebruikers die u hebt opgegeven.

   U kunt gebruikers bekijken die toestemmingen aan het plan in Gedeeld met me kolom in een lijst van plannen of in de hoger-juiste hoek van de plankopbal hebben.

   >[!TIP]
   >
   >U kunt plannen weergeven die met u worden gedeeld door het filter [!UICONTROL Shared with me] toe te passen in een lijst met plannen.


