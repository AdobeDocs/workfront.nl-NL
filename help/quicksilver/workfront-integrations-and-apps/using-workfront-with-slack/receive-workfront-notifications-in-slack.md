---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Ontvang  [!DNL Adobe Workfront]  berichten in  [!DNL Slack]
description: Ontvang  [!DNL Adobe Workfront]  berichten in  [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# [!DNL Adobe Workfront] -meldingen ontvangen in [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

Nadat u [!DNL Adobe Workfront for Slack] hebt geïnstalleerd, kunt u [!DNL Workfront] meldingen ontvangen in [!DNL Slack] .\
Voor informatie over het installeren van [!DNL Workfront for Slack], zie [&#x200B;  [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) vormen.

U kunt een geselecteerd aantal [!UICONTROL notifications] inschakelen dat wordt weergegeven in de meldingsballon in de [!DNL Workfront] -interface en dat ook wordt geleverd in [!DNL Slack] .

E-mailmeldingen werken onafhankelijk van interfacemeldingen van [!DNL Workfront] . Uw [!DNL Workfront] -beheerder kan e-mailmeldingen uitschakelen, terwijl interfacemeldingen niet kunnen worden uitgeschakeld in [!DNL Workfront] .\
U kunt [!DNL Workfront] -meldingen die u ontvangt in [!DNL Slack] echter uitschakelen als u alleen binnen de interface van [!DNL Workfront] op deze meldingen wilt focussen.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] plan] </a>*</td> 
   <td> <p>[!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, licentietype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.\

## Vereisten

Voordat u [!DNL Workfront] meldingen kunt ontvangen in [!DNL Slack] , moet u

* Configureren [!DNL Workfront for Slack]\
   Voor instructies bij het vormen [!DNL Workfront for Slack], zie [&#x200B; vormen  [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## [!DNL Workfront] -meldingen configureren voor [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (Voorwaardelijk) Nadat [!DNL Workfront] aan uw [!DNL Slack] -instantie is toegevoegd, meldt u zich aan bij [!DNL Workfront] vanuit [!DNL Slack] .\
   Voor informatie over het registreren in [!DNL Workfront] van [!DNL Slack], zie [&#x200B; Toegang  [!DNL Adobe Workfront]  van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Typ een van de volgende opdrachten in het berichtveld vanaf een willekeurig kanaal:

   `/workfront settings`

   of

   `/wf settings`

1. Standaard zijn alle meldingen ingeschakeld.\
   Schakel een van de volgende meldingen uit:

   * [!UICONTROL I'm assigned to a new task or issue]
   * [!UICONTROL My team is assigned to a new task or issue]
   * [!UICONTROL I receive a new approval or access request]
   * [!UICONTROL Someone includes me on a directed update]
   * [!UICONTROL Someone comments on a thread I'm in]
   * [!UICONTROL An update is made to a task, issue or project I am subscribed to]
   * [!UICONTROL Someone comments on one of my work items]
   * [!UICONTROL Someone comments on my help request]

   De wijzigingen die u aanbrengt in de opties voor [!UICONTROL notifications] , worden direct van kracht.\
   De meldingen die u hebt ingeschakeld, worden via het kanaal [!DNL Workfront] [!DNL Slack] verzonden. Wanneer u hier meldingen uitschakelt, worden deze alleen uitgeschakeld voor [!DNL Slack] en niet voor de [!DNL Workfront] -interface. U blijft ze ontvangen in de meldingsballon [!DNL Workfront] rechtsboven in de interface.

## [!DNL Workfront] -meldingen beheren vanuit [!DNL Slack]

U kunt [!DNL Workfront] -meldingen van [!DNL Slack] ontvangen en erop reageren.

U kunt e-mailmeldingen uitschakelen voor meldingen die u inschakelt in [!DNL Slack] om ervoor te zorgen dat u geen dubbele meldingen ontvangt.\
Voor informatie over het vormen van uw e-mailberichten, zie [&#x200B; uw eigen e-mailberichten wijzigen &#x200B;](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Het in- of uitschakelen van [!DNL Workfront] -meldingen in [!DNL Slack] heeft geen invloed op de meldingen die u ontvangt in de [!DNL Workfront] -interface.\
Meldingen binnen de interface [!DNL Workfront] kunnen niet worden uitgeschakeld.

Uw [!DNL Workfront] -meldingen voor [!DNL Slack] beheren:

1. Meld u aan bij [!UICONTROL Slack] .
1. Meld u aan bij [!DNL Workfront] vanuit [!DNL Slack] .\
   Voor informatie over het aanmelden bij [!DNL Workfront] van [!DNL Slack], zie het &quot;Aanmelden aan [!DNL Workfront] van [!DNL Slack]&quot;sectie in [&#x200B; Toegang  [!DNL Adobe Workfront]  van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Zorg ervoor dat de [!DNL Workfront] meldingen voor [!DNL Slack] zijn ingeschakeld.\
   Voor meer informatie waarover [!DNL Workfront] berichten kunnen worden gevormd om ook naar [!DNL Slack] worden verzonden, zie [&#x200B;  [!DNL Workfront]  berichten voor  [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack) vormen.

1. Ga naar het kanaal **[!DNL Workfront]** om uw [!DNL Workfront] -meldingen te zoeken.
1. (Voorwaardelijk en optioneel) Voer een van de volgende handelingen uit:

   * Klik op **[!UICONTROL Work on it]** om aan een taak te werken.

   * (Voorwaardelijk en optioneel) Klik op **[!UICONTROL Reply in [!DNL Workfront]]** om te reageren op een opmerking, uw antwoord te typen en op **[!UICONTROL Reply]** te klikken.

   * (Voorwaardelijk en optioneel) Klik op **[!UICONTROL Approve]** of **[!UICONTROL Reject]** om een taak, uitgave of project goed te keuren of af te wijzen die in afwachting zijn van uw goedkeuring.

   * (Voorwaardelijk en optioneel) Klik op **[!UICONTROL Approve]** , **[!UICONTROL Changes]** of **[!UICONTROL Reject]** om een document goed te keuren, goed te keuren met wijzigingen of af te wijzen.

     U kunt de muis ook boven de miniatuur van het document houden en op het vergrootglaspictogram klikken om een grotere voorvertoning van het document weer te geven voordat u het goedkeurt.\
      Slechts kunnen de goedgekeurde Slack [&#x200B; dossiertypes &#x200B;](https://api.slack.com/types/file) worden voorvertoond.

   * (Voorwaardelijk en optioneel) Klik op **[!UICONTROL Grant]** of **[!UICONTROL Ignore]** om het verzoek om meer toegang van een andere gebruiker te verlenen of te negeren.\

     U ontvangt een bevestiging dat uw actie in [!DNL Workfront] is voltooid, voor elke beslissing die u in uw berichten maakt.
