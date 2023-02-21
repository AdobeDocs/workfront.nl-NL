---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Taken en problemen maken met Slack
description: Nadat u hebt geïnstalleerd en geconfigureerd [!DNL Adobe Workfront] voor Slack, kunt u taken en kwesties van Slack tot stand brengen en hen associëren met projecten in Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Taken en uitgaven maken van [!DNL Slack]

Nadat u hebt geïnstalleerd en geconfigureerd [!DNL Adobe Workfront for Slack], kunt u taken en problemen maken van [!DNL Slack] en associeer hen met projecten in [!DNL Workfront].

Voor meer informatie over het configureren [!DNL Workfront] with [!DNL Slack], zie [Configureren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

U moet toegang hebben om taken en kwesties in uw Niveau van de Toegang tot te creëren en u moet hebben [!UICONTROL Contribute] toestemmingen op het project dat u hen associeert met.

Voor meer informatie over de Niveaus van de Toegang, zie [Overzicht van toegangsniveaus](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). Zie voor meer informatie over machtigingen voor objecten [Overzicht van het delen van machtigingen voor objecten](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.\

## Vereisten

Voordat u taken en uitgaven kunt maken van [!DNL Slack]moet u

* Configureren [!DNL Workfront] voor Slack\
   Voor instructies over het configureren [!DNL Workfront for Slack], zie [Configureren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Taken maken van [!DNL Slack]

1. Meld u aan bij uw [!DNL Slack] instantie en aanmelden bij [!DNL Workfront] van [!DNL Slack].\
   Voor meer informatie over aanmelden bij Workfront vanaf [!DNL Slack], zie &quot;Aanmelden bij [!DNL Workfront] van [!DNL Slack]&quot; sectie in [Toegang [!DNL Adobe Workfront] van [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Typ de volgende opdracht in het berichtveld vanaf een willekeurig kanaal:

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >Opdrachten zijn hoofdlettergevoelig. U kunt uw opdracht starten met `/wf` in plaats van `/workfront`.
   >  
   >De naam van de Taak moet zijn ingegaan aangezien het in zal verschijnen [!DNL Workfront] interface, zonder haakjes of aanhalingstekens.

1. (Optioneel) Typ de naam van een project waaraan u de nieuwe taak wilt koppelen en selecteer de naam wanneer deze in de lijst wordt weergegeven.\
   U ontvangt een bevestiging die aangeeft dat de taak aan het geselecteerde project is toegevoegd.
1. (Optioneel) Klik op de naam van de taak in het bevestigingsbericht om de taak te openen in [!DNL Workfront], in een nieuw browsertabblad.

## Uitgaven maken van [!DNL Slack]

1. Meld u aan bij uw [!DNL Slack] instantie en aanmelden bij [!DNL Workfront] van [!DNL Slack].\
   Voor meer informatie over aanmelden bij [!DNL Workfront] van [!DNL Slack], zie &quot;Aanmelden bij [!DNL Workfront] van [!DNL Slack]&quot; sectie in [Toegang [!DNL Adobe Workfront] van [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Typ de volgende opdracht in het berichtveld vanaf een willekeurig kanaal:

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >Opdrachten zijn hoofdlettergevoelig. U kunt de opdracht starten met &#39;/wf&#39; in plaats van &#39;/workfront.&#39; \
   >De naam van de uitgave moet worden ingevoerd zoals deze wordt weergegeven in het dialoogvenster [!DNL Workfront] interface, zonder haakjes of aanhalingstekens.

1. (Optioneel) Typ de naam van een project waaraan u het nieuwe probleem wilt koppelen en selecteer het wanneer het in de lijst wordt weergegeven.\
   U ontvangt een bevestiging die aangeeft dat de uitgave aan het geselecteerde project is toegevoegd.
1. (Optioneel) Klik op de naam van het probleem in het bevestigingsbericht om het te openen in [!DNL Workfront], in een nieuw browsertabblad.
