---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Taken en problemen maken vanuit Slack
description: Nadat u  [!DNL Adobe Workfront]  voor Slack hebt geïnstalleerd en gevormd, kunt u taken en kwesties van Slack tot stand brengen en hen associëren met projecten in Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Taken en problemen maken vanuit [!DNL Slack]

Nadat u [!DNL Adobe Workfront for Slack] hebt geïnstalleerd en geconfigureerd, kunt u taken en problemen maken vanuit [!DNL Slack] en deze koppelen aan projecten in [!DNL Workfront] .

Voor meer informatie over het vormen [!DNL Workfront] met [!DNL Slack], zie [&#x200B;  [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) vormen.

U moet toegang hebben om taken en kwesties in uw Niveau van de Toegang tot stand te brengen en u moet [!UICONTROL Contribute] toestemmingen op het project hebben dat u hen associeert met.

Voor meer informatie over de Niveaus van de Toegang, zie [&#x200B; overzicht van de Niveaus van de Toegang &#x200B;](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). Voor meer informatie over toestemmingen aan voorwerpen, zie [&#x200B; Overzicht van het delen van toestemmingen op voorwerpen &#x200B;](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/nl/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] plan] </a>*</td> 
   <td> <p>[!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, licentietype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.\

## Vereisten

Voordat u taken en problemen kunt maken vanuit [!DNL Slack] , moet u

* [!DNL Workfront] voor Slack configureren\
   Voor instructies bij het vormen [!DNL Workfront for Slack], zie [&#x200B; vormen  [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Taken maken van [!DNL Slack]

1. Meld u aan bij de [!DNL Slack] -instantie en meld u aan bij [!DNL Workfront] from [!DNL Slack] .\
   Voor meer informatie over het programma openen aan Workfront van [!DNL Slack], zie het &quot;Aanmelden aan [!DNL Workfront] van [!DNL Slack]&quot;sectie in [&#x200B; Toegang  [!DNL Adobe Workfront]  van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Typ de volgende opdracht in het berichtveld vanaf een willekeurig kanaal:

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >De bevelen zijn case sensitive. U kunt de opdracht starten met `/wf` in plaats van met `/workfront` .
   >  
   >De taaknaam moet worden ingevoerd zoals deze wordt weergegeven in de interface van [!DNL Workfront] , zonder haakjes of aanhalingstekens.

1. (Optioneel) Typ de naam van een project waaraan u de nieuwe taak wilt koppelen en selecteer de naam wanneer deze in de lijst wordt weergegeven.\
   U ontvangt een bevestiging die aangeeft dat de taak aan het geselecteerde project is toegevoegd.
1. (Optioneel) Klik in het bevestigingsbericht op de naam van de taak om deze te openen in [!DNL Workfront] , op een nieuw browsertabblad.

## Uitgaven maken van [!DNL Slack]

1. Meld u aan bij de [!DNL Slack] -instantie en meld u aan bij [!DNL Workfront] from [!DNL Slack] .\
   Voor meer informatie over het programma openen aan [!DNL Workfront] van [!DNL Slack], zie het &quot;Aanmelden aan [!DNL Workfront] van [!DNL Slack]&quot;sectie in [&#x200B; Toegang  [!DNL Adobe Workfront]  van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Typ de volgende opdracht in het berichtveld vanaf een willekeurig kanaal:

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >De bevelen zijn case sensitive. U kunt de opdracht starten met &#39;/wf&#39; in plaats van &#39;/workfront.&#39; \
   >De naam van de uitgave moet worden ingevoerd zoals deze wordt weergegeven in de interface [!DNL Workfront] , zonder haakjes of aanhalingstekens.

1. (Optioneel) Typ de naam van een project waaraan u het nieuwe probleem wilt koppelen en selecteer het wanneer het in de lijst wordt weergegeven.\
   U ontvangt een bevestiging die aangeeft dat de uitgave aan het geselecteerde project is toegevoegd.
1. (Optioneel) Klik in het bevestigingsbericht op de naam van het probleem om het te openen in [!DNL Workfront] op een nieuw browsertabblad.
