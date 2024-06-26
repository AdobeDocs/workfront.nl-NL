---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Installeren [!DNL Adobe Workfront] for [!DNL Jira]
description: U kunt [!DNL Adobe Workfront] for [!DNL Jira] om uw [!DNL Jira] en [!DNL Workfront] systemen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Installeren [!DNL Adobe Workfront for Jira]

U kunt [!DNL Adobe Workfront for Jira] om uw [!DNL Jira] en [!DNL Workfront] systemen.

Nadat u de invoegtoepassing hebt geïnstalleerd, kunt u workflows definiëren die [!DNL Jira] automatisch uitgaven wanneer [!DNL Workfront] tijdelijke items worden gemaakt. De items in beide toepassingen worden gekoppeld en sommige van de gegevens ervan kunnen automatisch in beide systemen worden bijgewerkt.

Alle gebruikers in [!DNL Workfront] en [!DNL Jira] kan van deze integratie profiteren. Ze hebben alleen een licentie nodig voor het systeem waarin ze het meest werken, en niet voor beide systemen.

Deze invoegtoepassing is beschikbaar voor de [!UICONTROL Server] en [!UICONTROL OnDemand] (of [!UICONTROL Cloud]) versies van [!DNL Jira] Software. Deze invoegtoepassing is niet beschikbaar voor de [!DNL Data Center] versie van [!DNL Jira] Software.

Voor een lijst met [!DNL Jira] versies die [!DNL Workfront for Jira] momenteel wordt ondersteund, zie [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) op de Atlassiaanse markt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> 
   <p>Nieuw: alle</p>
   <p>Huidige: [!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] overzicht van licenties</td> 
   <td> 
   <p>Nieuw: Standaard</p>
   <p>Huidige: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] toegang</td> 
   <td> <p>Toegang tot systeembeheerder</p> <p>Belangrijk: wij adviseren dat u afzonderlijke rekeningen van de systeembeheerder in [!DNL Jira] en [!DNL Workfront] om aan deze integratie te wijden, eerder dan het gebruiken van bestaande degenen die aan gebruikers zouden kunnen worden vastgemaakt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td><p>U moet een [!DNL Workfront] beheerder.</p></td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Installeren [!DNL Workfront] for [!DNL Jira]

Installeren [!DNL Workfront] for [!DNL Jira] OnDemand is hetzelfde als het op een [!DNL Jira] Serverinstantie.

U moet een [!DNL Jira] beheerder om de [!DNL Workfront] invoegtoepassing.

Als u geen [!DNL Jira] beheerder, kunt u naar de [!DNL Workfront] add-on en verzoek om installatie ervan. Uw verzoek is verzonden naar de [!DNL Jira] beheerder voor goedkeuring en installatie.

Voor meer informatie over het vragen van om toe:voegen-op om op uw te installeren [!DNL Jira] toepassing, zie [Het beheren van gebruikersverzoeken om toe:voegen-ons.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Om te installeren [!DNL Workfront for Jira]:

1. Aanmelden bij [!DNL Jira] als [!DNL Jira] beheerder.
1. Zoek de **[!DNL Workfront for Jira]** toe:voegen-aan in [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. Klikken **[!UICONTROL Get it now]** om het te installeren.

   Nadat de installatie is voltooid, kunt u zich aanmelden bij [!DNL Workfront] van [!DNL Jira] en configureer uw integratie.

   Zie voor meer informatie [Adobe Workfront voor Jira configureren](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Overwegingen bij een [!DNL Jira Server] installatie

>[!NOTE]
>
>Deze voorschriften zijn niet van toepassing op [!UICONTROL OnDemand] ([!UICONTROL Cloud]) versie van [!DNL Jira] Software.

Hoewel u de [!DNL Workfront] invoegtoepassing in beide [!DNL Jira] omgevingen die vergelijkbaar zijn, moet u rekening houden met het volgende wanneer u met een [!DNL Jira Server] installatie:

* Bij het configureren van de invoegtoepassing [!DNL Jira], het adres dat in het **[!DNL JIRA Base URL]** het veld mag niet dezelfde URL zijn die u gebruikt om toegang te krijgen [!DNL Jira] op uw persoonlijke server. De **[!DNL JIRA Base URL]** moet een openbaar toegankelijk adres zijn dat met uw privé server gebruikend NATIONAAL of omgekeerde volmachtsprotocollen wordt verbonden, zodat [!DNL Workfront] heeft toegang tot de server om aanvragen bij de server in te dienen.

* U moet SSL-versleuteling gebruiken om de communicatie tussen [!DNL Jira] en [!DNL Workfront]. Wanneer u SSL inschakelt, moet u over een volledige SSL-certificaatstapel van een certificeringsinstantie beschikken. Wij ondersteunen zelfondertekende certificaten niet.
* U moet ervoor zorgen dat de [!DNL jira.workfront.com] domein is toegankelijk vanaf uw bedrijfsservers. Het dient als middleware milieu tussen [!DNL Workfront] en [!DNL Jira] en is vereist voor de invoegtoepassing.

  U moet ook de volgende statische IP adressen aan de lijst van gewenste personen op uw firewall voor uitgaande en binnenkomende verbindingen toevoegen.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  Voor meer informatie over het configureren van uw firewall voor optimale functionaliteit met [!DNL Workfront], zie [Uw firewall configureren](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
