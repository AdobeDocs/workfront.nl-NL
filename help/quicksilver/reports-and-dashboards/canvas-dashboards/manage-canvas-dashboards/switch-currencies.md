---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Valutavelden gebruiken in canvasdashboards
description: U kunt de valutavelden op een Canvasdashboard gebruiken.
author: Courtney
feature: Reports and Dashboards
source-git-commit: 3e4ab2dfc66efd262c0c2ad30a9c62758084f8ce
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---


# Valutavelden gebruiken in canvasdashboards

>[!IMPORTANT]
>
>De functie Canvasdashboards is momenteel alleen beschikbaar voor gebruikers die deelnemen aan de bètafase. Onderdelen van het onderdeel zijn mogelijk niet compleet of werken niet zoals bedoeld in deze fase. Gelieve te dienen om het even welke terugkoppelen betreffende uw ervaring door de instructies in [ te volgen verstrekt ](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) sectie in het de bètaoverzichtsartikel van de dashboards van het Canvas.<br>
>Als u feedback hebt over een mogelijk probleem met een probleem of een technisch probleem, stuurt u een ticket naar Workfront Support. Voor meer informatie, zie [ de Steun van de Klant van het Contact ](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Deze bètaversie is niet beschikbaar op de volgende cloudproviders:
>
>* Je eigen sleutel voor Amazon Web Services
>* Azure
>* Google Cloud Platform

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Alle </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td> 
<p>Standard</p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td> 
   <td><p>Toegang tot rapporten, dashboards en kalenders bewerken</p>
   <p>Toegang tot financiële gegevens weergeven</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td><p>Rechten voor het dashboard beheren</p>
  </td> 
  </tr> 
</tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Vereisten

1. U moet meerdere valutatypen hebben ingesteld in uw Workfront-instantie om de in dit artikel beschreven functionaliteit te kunnen gebruiken. Voor meer informatie, zie [ de wisselkoersen van de Opstelling ](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   >[!IMPORTANT]
   >
   >De in dit artikel beschreven functionaliteit is alleen van toepassing op native valutavelden. Ondersteuning voor aangepaste valutavelden wordt binnenkort beschikbaar.


## Een standaardvaluta instellen voor een Canvasdashboard

Wanneer u een Canvasdashboard maakt, kunt u een standaardvaluta voor het dashboard instellen. Deze valuta wordt gebruikt om alle native valutavelden weer te geven in rapporten op het dashboard, tenzij het valutaveld op rapportniveau is vergrendeld.

1. In het linkerpaneel, klik **de Dashboards van het Canvas**.

1. Klik **Nieuw Dashboard** in de hoger-juiste hoek.

1. In **creeer dashboard** doos,

1. Geef het volgende op:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Naam</strong></td>
      <td><p>Voer een naam in voor het dashboard. We raden u aan alleen UTF-8-tekens te gebruiken om compatibiliteitsproblemen te voorkomen.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Beschrijving (optioneel)</strong></td>
      <td>Voer een beschrijving van het dashboard in.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>Valuta</strong></td>
      <td>Kies het standaardvalutatype voor het dashboard. <br>
      <br> de Gebruikers kunnen tussen verschillende munttypes schakelen wanneer het filtreren van het dashboard.</td>
     </tr>
    </tbody>
   </table>


## Schakelen tussen valuta&#39;s op een Canvasdashboard

U kunt schakelen tussen verschillende valutatypen op dashboardniveau. Rapporten met valutavelden worden bijgewerkt met het geselecteerde valutatype.

De gebieden van de munteenheid kunnen op het rapportniveau worden gesloten. Als een valutaveld is vergrendeld, verandert het valutatype voor dat rapport niet wanneer u het valutatype voor het dashboard wijzigt.

Het valutatype voor het dashboard wijzigen,

1. Klik op het vervolgkeuzemenu Valuta in de rechterbovenhoek van de pagina met dashboarddetails.
1. Selecteer het gewenste valutatype in de lijst.

   ![ daling van de veranderingsmunt neer ](assets/filter-by-currency.png)


## Beperkingen

De volgende tabel geeft de beperkingen aan wanneer valuta&#39;s zijn gedefinieerd in het gedeelte Wisselkoersen in Setup.

<table> 
<tr>
<td></td>
<td>Gebruikers kunnen</td>
<td>Gebruikers kunnen</td>
</tr>
<tr> 
<td>Eén valuta is gedefinieerd</td>
<td>
<ul>
<li>Native valutavelden gebruiken in canvasdiagram, KPI- en tabelrapporten</li>
<li>Aangepaste valutavelden gebruiken in canvasgrafiek-, KPI- en diagramrapporten</li>
</ul>
</td>
<td>
<ul>
<li>Een standaardvaluta toewijzen aan het dashboard (bij het maken of bewerken van het dashboard)</li>
<li>De valutatransactie op dashboardniveau bekijken en gebruiken</li>
<li>Een specifieke valuta vergrendelen voor weergave in een canvasdiagram, KPI of tabelrapport</li>
<li>De gebieden van de Valuta van de Planning van het gebruik in een canvasgrafiek, KPI, en lijstrapporten</li>
</ul>
</td> 
</tr>
</td> 
</tr> 
<tr>
<td>Meerdere valuta's zijn gedefinieerd</td>
<td>
<ul>
  <li>Native valutavelden gebruiken in canvasdiagram, KPI- en tabelrapporten</li>
  <li>Een standaardvaluta voor het dashboard instellen (bij het maken of bewerken van het dashboard)</li>
  <li>De valutatransactie op dashboardniveau bekijken en gebruiken</li>
  <li>Vergrendel een specifieke valuta voor weergave in een canvasgrafiek, KPI of tabelrapport om de voorkeur voor het schakelen tussen dashboardvaluta's te negeren</li>
</ul>
</td>
<td><ul>
  <li>Aangepaste velden voor gegevensvaluta gebruiken in canvasdiagram, KPI- en tabelrapporten</li>
  <li>De gebieden van de Valuta van de Planning van het gebruik in een canvasgrafiek, KPI, en lijstrapporten</li>
</ul>
</td>
</tr></table>





