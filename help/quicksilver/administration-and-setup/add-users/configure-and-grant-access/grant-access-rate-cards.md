---
title: Toegang verlenen tot betaalkaarten
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-beheerder kunt u de toegang van een gebruiker tot financiële gegevens in Workfront definiëren via hun toegangsniveau.
author: Becky and Lisa
feature: System Setup and Administration
role: Admin
exl-id: b21e65d3-3c9f-4f3d-95d3-de4c09199622
source-git-commit: 627d59c8c8296e5b6c8b6da53705a1c3d7633751
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Toegang verlenen tot betaalkaarten

{{highlighted-preview-article-level}}

Als beheerder van Adobe Workfront, kunt u de toegang van een gebruiker tot tariefkaarten door het de toegangsniveau van de gebruiker bepalen, zoals die in [ wordt verklaard het niveauoverzicht van de Toegang ](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Voor informatie over tariefkaarten, zie [ tariefkaarten beheren ](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het verlenen van toegang tot betaalkaarten

Houd rekening met het volgende wanneer u gebruikers toegang biedt tot betaalkaarten in Workfront:

* De gebruikers moeten toegang tot de Kaarten van het Tarief, Projecten, en Financiële Gegevens hebben uitgeven om een tariefkaart aan een project vast te maken.
* De gebruikers zonder Toegang tot Kaarten van het Tarief en geven toegang tot Financiële Gegevens uit kunnen geen tariefkaart aan een project vastmaken, maar zij kunnen andere het facturerings tarieven op het project uitgeven die uit andere bronnen kwamen.

## Gebruikerstoegang tot tariefkaarten configureren met behulp van een aangepast toegangsniveau

1. Beginnen creërend of het uitgeven van het toegangsniveau, zoals die in [ wordt verklaard creeer of wijzig douanetoegangsniveaus ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klik het tandwielpictogram ![](assets/gear-icon-settings.png) op de **Mening** of **geef** knoop aan het recht van de Kaarten van het Tarief uit, dan selecteer de capaciteiten u onder **wilt verlenen - verbeter uw montages**.

   ![ Fijne toegang van de tariefkaart ](assets/rate-card-access-fine-tune.png)

1. (Facultatief) om toegangsmontages voor andere voorwerpen en gebieden op het toegangsniveau te vormen u aan werkt, ga met één van de artikelen voort die in [ worden vermeld toegang tot Adobe Workfront ](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) zoals [ toegang van de Verlening tot taken ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Wanneer u wordt gebeëindigd, klik **sparen**.

   Nadat het toegangsniveau wordt gecreeerd, kunt u het aan een gebruiker toewijzen. Voor meer informatie, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

## Toegang tot kaarten met gedeelde tarieven

U kunt een tariefkaart met andere gebruikers delen door hen toestemmingen aan het te verlenen, zoals die in [ wordt verklaard een tariefkaart van het Aandeel ](/help/quicksilver/administration-and-setup/manage-enterprise-operations/share-rate-cards.md).

Wanneer u een object met een andere gebruiker deelt, worden de rechten van de ontvanger op het object bepaald door een combinatie van twee dingen:

* De machtigingen die u aan de ontvanger toekent voor het object
* De instellingen van het toegangsniveau van de ontvanger voor het objecttype
