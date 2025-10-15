---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Uw werk en goedkeuringen beheren vanuit Slack
description: U kunt uw thuiswerklijst openen, taken en problemen controleren en direct vanuit Slack beslissingen nemen over goedkeuringen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 0%

---

# Uw werk en goedkeuringen beheren vanuit [!DNL Slack]

Nadat u [!DNL Adobe Workfront for Slack] hebt geïnstalleerd, kunt u het volgende doen:

* Lijsten met uw [!UICONTROL Home] items openen vanuit [!DNL Slack]
* Controleren en accepteren om te werken aan taken en problemen vanuit [!DNL Slack]
* Goedkeuringen beoordelen en beslissen via [!DNL Slack]

Voor meer informatie over het vormen [!DNL Workfront] met [!DNL Slack], zie [  [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) vormen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Alle</p>
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat u uw werk en goedkeuringen kunt beheren vanuit [!DNL Slack] , moet u

* Configureren [!DNL Workfront for Slack]\
  Voor instructies bij het vormen [!DNL Workfront for Slack], zie [ vormen  [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Uw werk beheren vanuit [!DNL Slack]

1. Meld u aan bij de [!DNL Slack] -instantie en meld u aan bij [!DNL Workfront] from [!DNL Slack] .\
   Voor meer informatie over het programma openen aan [!DNL Workfront] van [!DNL Slack], zie het &quot;Aanmelden aan [!DNL Workfront] van [!DNL Slack]&quot;sectie in [ Toegang  [!DNL Adobe Workfront]  van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Typ de volgende opdracht in het berichtveld vanaf een willekeurig kanaal:

   `/workfront home`

   >[!NOTE]
   >
   >* De bevelen zijn case sensitive.
   >* U kunt de opdracht starten met `/wf` in plaats van met `/workfront` .

   De knopen waarvan u tot lijsten van uw taken, kwesties, en goedkeuringsvertoning kunt toegang hebben. Wanneer u op een van de knoppen klikt, worden de eerste 20 items van elke lijst in [!DNL Slack] weergegeven.

1. (Optioneel) Klik op **[!UICONTROL Tasks]** om al uw taken weer te geven.

   Voor meer informatie over het beheren van taken in [!DNL Slack], zie [ het Leiden Uw Taken van  [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack).

1. (Optioneel) Klik op **[!UICONTROL Issues]** om al uw problemen weer te geven.

   Voor meer informatie over het beheren van kwesties in [!DNL Slack], zie [ het Leiden Uw Kwesties van  [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack).

1. (Optioneel) Klik op **[!UICONTROL Approvals]** om alle goedkeuringen weer te geven die op uw beslissing wachten.\
   Voor meer informatie over het beheren van uw goedkeuringen in [!DNL Slack], zie [ uw goedkeuringen van  [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack) leiden.

## Uw taken beheren vanuit [!DNL Slack] {#manage-your-tasks-from-slack}

1. Meld u aan bij de [!DNL Slack] -instantie en meld u aan bij [!DNL Workfront] from [!DNL Slack] .\
   Voor informatie over het aanmelden bij [!DNL Workfront] van [!DNL Slack], zie het &quot;Aanmelden aan [!DNL Workfront] van [!DNL Slack]&quot;sectie in [ Toegang  [!DNL Adobe Workfront]  van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Typ een van de volgende opdrachten in het berichtveld vanaf een willekeurig kanaal:

   `/workfront home` en klik vervolgens op **[!UICONTROL Tasks]**

   of

   `/workfront tasks`

   >[!NOTE]
   >
   >* De bevelen zijn case sensitive.
   >* U kunt de opdracht starten met `/wf` in plaats van met `/workfront` .

   De eerste 20 taken op uw lijstvertoning.

1. Klik **[!UICONTROL +`<remaining number>`meer]** om extra taken te tonen.
1. Overweeg de volgende informatie over je werk te bekijken:

   * **[!UICONTROL Name]**
   * **[!UICONTROL Project Name]** of **[!DNL Parent Object Name]**

   * **[!DNL Planned Completion Date]** van het werkitem.
   * **[!DNL Assigned By Name]**: dit is de naam van de gebruiker die de taak aan u heeft toegewezen.
   * **[!UICONTROL Status]**

1. (Optioneel) Klik op de naam van een item om dit in Workfront te openen op een apart browsertabblad.
1. (Optioneel) Selecteer een nieuwe status in het veld **[!UICONTROL Status]** .
1. (Optioneel) Klik op **[!UICONTROL Log Time]** en selecteer vervolgens een **[!UICONTROL Hour Type]** en een uur om de tijd voor het aanmelden bij het onderdeel in te stellen.

   >[!NOTE]
   >
   >* U kunt slechts uren in toename van een volledig of half uur, tot 12 uren en 30 minuten registreren.
   >* De uren u registreert hebben een Datum van de Ingang van vandaag. U kunt geen tijd voor een vroegere of toekomstige datum van [!DNL Slack] registreren.

   U ontvangt een bevestiging dat de tijd is geregistreerd.

1. (Optioneel) Klik op **[!UICONTROL Work on it]** om een taak te accepteren. De knop [!UICONTROL Work on it] verdwijnt.

## Uw uitgaven beheren vanuit [!DNL Slack] {#manage-your-issues-from-slack}

1. Meld u aan bij de [!DNL Slack] -instantie en meld u aan bij [!DNL Workfront] from [!DNL Slack] .\
   Voor meer informatie over het programma openen aan [!DNL Workfront] van [!DNL Slack], zie [ het Aanmelden aan  [!DNL Workfront]  van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront]  van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Typ een van de volgende opdrachten in het berichtveld vanaf een willekeurig kanaal:

   `/workfront home` en klik vervolgens op **[!UICONTROL Issues]**

   of

   `/workfront issues`

   >[!NOTE]
   >
   >* De bevelen zijn case sensitive.
   >* U kunt de opdracht starten met `/wf` in plaats van met `/workfront` .

   De eerste 20 uitgaven in uw lijstvertoning.

1. Klik **[!UICONTROL + remaining `<number>`meer]** om extra punten te tonen.
1. Overweeg de volgende informatie over je werk te bekijken:

   * **[!UICONTROL Name]**
   * **[!UICONTROL Project]** Naam of naam bovenliggend object
   * **[!UICONTROL Due on]** Datum: Dit is de geplande voltooiingsdatum van het werkitem.
   * **[!DNL Requested by]** Naam: Dit is de primaire contactpersoon (voor uitgaven) of de gebruiker die de toewijzing heeft uitgevoerd (voor taken).

1. (Optioneel) Klik op de naam van de uitgave om deze in Workfront te openen op een apart browsertabblad.
1. (Optioneel) Klik op **[!DNL Work on it]** om te gaan werken aan problemen die u nog niet hebt geaccepteerd.

   De knop [!UICONTROL Work on it] verdwijnt.

## Uw goedkeuringen beheren vanuit [!DNL Slack] {#manage-your-approvals-from-slack}

1. Meld u aan bij de [!DNL Slack] -instantie en meld u aan bij [!DNL Workfront] from [!DNL Slack] .\
   Voor meer informatie over het programma openen aan [!DNL Workfront] van [!DNL Slack], zie het &quot;Aanmelden aan [!DNL Workfront] van [!DNL Slack]&quot;sectie in [ Toegang  [!DNL Adobe Workfront]  van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Typ een van de volgende opdrachten in het berichtveld vanaf een willekeurig kanaal:

   `/workfront home` en klik vervolgens op **[!UICONTROL Approvals]**

   of

   `/workfront approvals`

   >[!NOTE]
   >
   >* De bevelen zijn case sensitive.
   >* U kunt de opdracht starten met `/wf` in plaats van met `/workfront` .

   De eerste 20 items in de lijstweergave van **[!UICONTROL Approvals]** . De extra informatie over de punten toont ook, zoals de naam van de gebruiker die het of de naam van het project verzocht het punt tot behoort.

1. Klik **[!UICONTROL + remaining `<number>`meer]** om extra punten te tonen.

1. Overweeg goedkeuringen voor de volgende objecten te beheren:

   * **Projecten**

     Klik op **[!UICONTROL Approve]** of **[!UICONTROL Reject]** om de statuswijziging van een project te accepteren of te negeren.

   * **Taken**

     Klik op **[!UICONTROL Approve]** of **[!UICONTROL Reject]** om de statuswijziging van een taak te accepteren of te negeren.

   * **Kwesties**

     Klik op **[!UICONTROL Approve]** of **[!DNL Reject]** om de statuswijziging van een uitgave te accepteren of te negeren.

   * **Documenten**

     Klik op **[!UICONTROL Approve]** om een document goed te keuren, op **[!UICONTROL Reject]** om het te negeren of op **[!UICONTROL Changes]** om aan te geven dat u het goedkeurt, maar dat het document aanvullende wijzigingen nodig heeft.\
     (Optioneel) Plaats de muisaanwijzer op de documentminiatuur om op het vergrootglas te klikken en een voorvertoning van het document weer te geven.

   * **proef** &#x200B; klik de proefdruk naam om het in [!DNL Workfront] in een afzonderlijk lusje te openen en de goedkeuring te beheren.
   * **Verzoeken van de Toegang**

     Klik op **[!UICONTROL Grant Access]** om het gevraagde object uitgebreide machtigingen te geven of op **[!UICONTROL Ignore]** om het verzoek om meer toegang te negeren.

1. (Optioneel) Klik op de naam van het object dat ter goedkeuring is ingediend om het te openen in [!DNL Workfront] op een nieuw browsertabblad.
