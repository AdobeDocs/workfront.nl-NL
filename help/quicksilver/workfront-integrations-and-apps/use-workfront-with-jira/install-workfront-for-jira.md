---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Installeren  [!DNL Adobe Workfront]  voor  [!DNL Jira]
description: U kunt  [!DNL Adobe Workfront]  voor  [!DNL Jira]  gebruiken om uw  [!DNL Jira]  en  [!DNL Workfront]  systemen te integreren.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 0%

---

# Installeren [!DNL Adobe Workfront for Jira]

>[!IMPORTANT]
>
>Om stabielere en scalable integratie te leveren, verschuiven wij naar een moderne, flexibele integratiebenadering gebruikend Workfront Automation and Integration (Fusion). Als deel van dit overgangsproces, zal Workfront voor de integratie van Jira niet beschikbaar na **28 Februari, 2026** zijn.
>
>We raden u aan Workfront Automation and Integration te gebruiken voor de integratiebehoeften van uw organisatie met Jira.
>
>Voor een overzicht van de Automatisering en de Integratie van Workfront, zie [&#x200B; het overzicht van de Fusie van Adobe Workfront &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Voor informatie over de specifieke mogelijkheden van de modules van de Automatisering en van de Integratie van Workfront voor Jira, zie {de modules van de Software van 0} Jira [.](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new)

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Met [!DNL Adobe Workfront for Jira] kunt u uw [!DNL Jira] - en [!DNL Workfront] -systemen integreren.

Nadat u de invoegtoepassing hebt geïnstalleerd, kunt u workflows definiëren waarmee automatisch [!DNL Jira] -problemen worden gemaakt wanneer [!DNL Workfront] -werkitems worden gemaakt. De items in beide toepassingen worden gekoppeld en sommige van de gegevens ervan kunnen automatisch in beide systemen worden bijgewerkt.

Alle gebruikers in [!DNL Workfront] en [!DNL Jira] kunnen van deze integratie profiteren. Ze hebben alleen een licentie nodig voor het systeem waarin ze het meest werken, en niet voor beide systemen.

Deze invoegtoepassing is beschikbaar voor de [!UICONTROL Server] - en [!UICONTROL OnDemand] (of [!UICONTROL Cloud] ) -versies van [!DNL Jira] Software. Deze invoegtoepassing is niet beschikbaar voor de [!DNL Data Center] -versie van [!DNL Jira] Software.

Voor een lijst van [!DNL Jira] versies die [!DNL Workfront for Jira] momenteel steunt, zie [[!DNL [!DNL Workfront for Jira]] &#x200B;](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) bij de Atlassiaanse Marketplace.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td><p>Alle</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard </p>
       <p>Plan </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Toegang tot Jira</td> 
   <td> <p>Toegang tot systeembeheerder</p> <p>Belangrijk: wij adviseren dat u afzonderlijke rekeningen van de systeembeheerder in Jira en Workfront creeert om aan deze integratie te wijden, eerder dan het gebruiken van bestaande die aan gebruikers zouden kunnen worden vastgemaakt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++## Installeren [!DNL Workfront] voor [!DNL Jira]

[!DNL Workfront] voor [!DNL Jira] OnDemand installeren is hetzelfde als op een [!DNL Jira] Server-instantie installeren.

U moet een [!DNL Jira] -beheerder zijn om de [!DNL Workfront] add-on te installeren.

Als u geen [!DNL Jira] beheerder bent, kunt u naar de [!DNL Workfront] add-on bladeren en vragen of deze kan worden geïnstalleerd. Uw verzoek wordt naar de [!DNL Jira] -beheerder verzonden voor goedkeuring en installatie.

Voor meer informatie over het verzoeken van om toe:voegen-op om op uw [!DNL Jira] toepassing te worden geïnstalleerd, zie [&#x200B; het Leiden gebruikersverzoeken om toe:voegen-ons.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Ga als volgt te werk om [!DNL Workfront for Jira] te installeren:

1. Meld u aan bij [!DNL Jira] als [!DNL Jira] -beheerder.
1. Vind **[!DNL Workfront for Jira]** toe:voegen-op in [[!DNL Atlassian Marketplace] &#x200B;](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview).

1. Klik op **[!UICONTROL Get it now]** om de toepassing te installeren.

   Nadat de installatie is voltooid, kunt u zich aanmelden bij [!DNL Workfront] vanuit [!DNL Jira] en uw integratie configureren.

   Voor meer informatie, zie [&#x200B; Adobe Workfront voor Jira &#x200B;](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) vormen.

## Overwegingen bij een [!DNL Jira Server] -installatie

>[!NOTE]
>
>Deze vereisten zijn niet van toepassing op de [!UICONTROL OnDemand] ([!UICONTROL Cloud]) versie van [!DNL Jira] Software.

Hoewel het installeren van de [!DNL Workfront] invoegtoepassing in de twee [!DNL Jira] -omgevingen vergelijkbaar is, moet u rekening houden met het volgende wanneer u werkt met een [!DNL Jira Server] -installatie:

* Wanneer u de invoegtoepassing configureert in [!DNL Jira] , is het adres dat is opgegeven in het veld **[!DNL JIRA Base URL]** mogelijk niet dezelfde URL die u gebruikt om [!DNL Jira] op uw persoonlijke server te openen. **[!DNL JIRA Base URL]** moet een openbaar-toegankelijk adres zijn dat met uw privé server gebruikend NATIONAAL of omgekeerde volmachtsprotocollen wordt verbonden, zodat [!DNL Workfront] tot het kan toegang hebben om verzoeken aan uw server te doen.

* U moet SSL-codering gebruiken om de communicatie tussen [!DNL Jira] en [!DNL Workfront] te beveiligen. Wanneer u SSL inschakelt, moet u over een volledige SSL-certificaatstapel van een certificeringsinstantie beschikken. Wij ondersteunen zelfondertekende certificaten niet.
* U moet ervoor zorgen dat het [!DNL jira.workfront.com] -domein toegankelijk is vanaf uw bedrijfsservers. Het dient als een middleware-omgeving tussen [!DNL Workfront] en [!DNL Jira] en is vereist voor de invoegtoepassing.

  U moet ook de volgende statische IP adressen aan de lijst van gewenste personen op uw firewall voor uitgaande en binnenkomende verbindingen toevoegen.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  Voor meer informatie over het vormen van uw firewall voor optimale functionaliteit met [!DNL Workfront], zie [&#x200B; Vormend Uw Firewall &#x200B;](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
