---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Verslag: Budgeted Hour"
description: "Verslag: Budgeted Hour"
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# Verslag: Budgeted Hour

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

Wanneer u de informatie van het BoedgetedUur met andere gebruikers wilt delen die geen toegang tot de Planner van het Middel hebben, kunt u dit doen door een Boedgeted rapport van het Uur te bouwen. U kunt het rapport dan met hen delen.

>[!IMPORTANT]
>
>De begrote Uren worden normaal elk uur bijgewerkt (zelden, kan het een maximum van drie uren) in het gegevensbestand van Adobe Workfront vergen. Het verfrissen van het rapport verfrist noodzakelijk niet de uurinformatie in het. U kunt de tijd bekijken die sinds de laatste update in de hoger-juiste hoek van elk Boekgeted rapport van het Uur is verlopen. Als u het rapport vernieuwt, wordt de informatie in het rapport alleen vernieuwd als er meer dan een uur is verstreken sinds de laatste update.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Een rapport over een &#39;Budgeted Hour&#39; maken

1. Klik het **Belangrijkste Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek, dan klik **Rapporten**.

1. Klik **Nieuw Rapport > Gegreneerde Uur**.

   De standaardmening wordt toegepast op het rapport.

1. (Facultatief) om het rapport gemakkelijker te maken om te lezen, klik de **Beoogde kolom van Uren**, toen **Schakelaar aan de Wijze van de Tekst**, dan verandert

   ```
   valuefield
   ```

   lijn naar

   ```
   valueexpreesion
   ```

   en voert u de afrondingsexpressie in.

   Hiermee wordt het aantal begrotingsuren afgerond op een aantal decimalen dat u opgeeft.

   Voor informatie over hoe te om een aantal in Workfront te afronden, zie het artikel [ Overzicht van berekende gegevensuitdrukkingen ](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. (Facultatief) klik **Kolom** toevoegen om extra kolommen toe te voegen.
1. (Optioneel) Om het rapport beter leesbaar te maken, raden we u aan een groep aan het rapport toe te voegen. Wij stellen de volgende groepering voor:

   Klik het **lusje van Groepen**, dan doe één of verscheidene van het volgende:

   1. Klik **toevoegen Groepering** en beginnen &quot;Naam van het Project&quot;te typen, dan het te selecteren wanneer het in de lijst verschijnt.
   1. Klik **toevoegen Groepering** en beginnen &quot;Naam van de Rol van de Taak&quot;te typen, dan het te selecteren wanneer het in de lijst verschijnt.
   1. Klik **toevoegen Groepering** en beginnen **Datum van de Toewijzing** te typen, selecteer het wanneer het in de lijst verschijnt, en selecteer dan timeframe u door van de **Datums van de Groep door** gebied wilt groeperen.

1. (Facultatief) klik **Filters** om filters aan het rapport toe te voegen.
1. (Facultatief) klik **Grafiek** om een grafiek aan het rapport toe te voegen.
1. Klik **sparen + Sluiten**.

## Herzie het verslag over het begrote uur

De volgende informatie is standaard beschikbaar in het rapport Boedgeted Hour:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Project </td> 
   <td>Dit is de naam van het project verbonden aan het Boedgeted Uour.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Functie</p> </td> 
   <td>Dit is de naam van de functie die verbonden is aan de begrotingsuren. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gebruiker</td> 
   <td>Dit is de naam van de gebruiker verbonden aan de Begrotingshuur.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alloc. Datum</td> 
   <td> <p>Dit is de toewijzingsdatum. Het is de eerste dag (een zondag) van de week waarvoor u de uren in de begroting heeft opgenomen.</p> <p>Tip:  <p>Als een week twee maanden omvat, genereert dit twee rijen in het rapport: een rij die overeenkomt met de eerste dag van de week (de zondag van de week die de eerste maand is) en een tweede rij die overeenkomt met de eerste dag van de tweede maand (en die een willekeurige dag van de week kan zijn).</p> <p>Als u bijvoorbeeld 8 uur begroot voor een gebruiker voor de week van 30 juni (zondag) - 6 juli (zaterdag), geven de twee rijen een toewijzingsdatum van 30 juni en 1 juli weer.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bud. Uren</td> 
   <td>Dit zijn de begrotingsuren die aan de Gebruiker in de Planner van het Middel worden toegewezen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pln. Bud. Uren</td> 
   <td>Dit zijn de begrotingsuren die aan de Rol van de Baan of het Project in de Planner van het Middel worden toegewezen.</td> 
  </tr> 
 </tbody> 
</table>
