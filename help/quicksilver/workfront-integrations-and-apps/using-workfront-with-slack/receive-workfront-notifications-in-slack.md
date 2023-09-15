---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Ontvangen [!DNL Adobe Workfront] meldingen in [!DNL Slack]
description: Ontvangen [!DNL Adobe Workfront] meldingen in [!DNL Slack]
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 0%

---

# Ontvangen [!DNL Adobe Workfront] meldingen in [!DNL Slack]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

Nadat u [!DNL Adobe Workfront for Slack], u kunt [!DNL Workfront] meldingen in [!DNL Slack].\
Voor informatie over installeren [!DNL Workfront for Slack], zie [Configureren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

U kunt een geselecteerd aantal van [!UICONTROL notifications] die worden weergegeven in de meldingsballon in de [!DNL Workfront] interface, ook te leveren in [!DNL Slack].

E-mailmeldingen werken onafhankelijk van [!DNL Workfront] interfacemeldingen. U of uw [!DNL Workfront] de beheerder kan e-mailberichten onbruikbaar maken, terwijl de interfaceberichten niet kunnen worden onbruikbaar gemaakt in [!DNL Workfront].\
U kunt deze optie echter uitschakelen [!DNL Workfront] meldingen die u ontvangt [!DNL Slack], als u zich alleen op deze meldingen wilt concentreren in het dialoogvenster [!DNL Workfront] interface.

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

Voordat je [!DNL Workfront] meldingen in [!DNL Slack], moet u

* Configureren [!DNL Workfront for Slack]\
   Voor instructies over het configureren [!DNL Workfront for Slack], zie [Configureren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Configureren [!DNL Workfront] meldingen voor [!DNL Slack] {#configure-workfront-notifications-for-slack}

1. (Voorwaardelijk) Na [!DNL Workfront] is toegevoegd aan uw [!DNL Slack] instantie, aanmelden [!DNL Workfront] van [!DNL Slack].\
   Voor informatie over het aanmelden [!DNL Workfront] van [!DNL Slack], zie [Toegang [!DNL Adobe Workfront] van [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

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

   De wijzigingen die u aanbrengt in de [!UICONTROL notifications] opties worden onmiddellijk van kracht.\
   De meldingen die u hebt ingeschakeld, worden geleverd in het dialoogvenster [!DNL Workfront] [!DNL Slack] kanaal. Wanneer u hier meldingen uitschakelt, worden deze alleen uitgeschakeld voor [!DNL Slack]en niet voor de [!DNL Workfront] interface. U blijft ze ontvangen in het dialoogvenster [!DNL Workfront] de berichten bellen in het hogere recht van de interface.

## Beheren [!DNL Workfront] meldingen van [!DNL Slack]

Je kunt ontvangen en reageren op [!DNL Workfront] meldingen van [!DNL Slack].

U kunt e-mailmeldingen uitschakelen voor meldingen die u inschakelt [!DNL Slack], om dubbele meldingen te voorkomen.\
Voor informatie over het configureren van uw e-mailmeldingen raadpleegt u [Uw eigen e-mailmeldingen wijzigen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

In- of uitschakelen [!DNL Workfront] meldingen in [!DNL Slack] heeft geen invloed op de meldingen die u ontvangt in het dialoogvenster [!DNL Workfront] interface.\
Meldingen binnen het dialoogvenster [!DNL Workfront] interface kan niet worden uitgeschakeld.

Om uw [!DNL Workfront] meldingen voor [!DNL Slack]:

1. Aanmelden bij [!UICONTROL Slack].
1. Aanmelden bij [!DNL Workfront] van [!DNL Slack].\
   Voor informatie over aanmelden bij [!DNL Workfront] van [!DNL Slack], zie &quot;Aanmelden bij [!DNL Workfront] van [!DNL Slack]&quot; sectie in [Toegang [!DNL Adobe Workfront] van [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Zorg ervoor dat uw [!DNL Workfront] meldingen voor [!DNL Slack] zijn ingeschakeld.\
   Voor meer informatie over [!DNL Workfront] meldingen kunnen zo worden geconfigureerd dat ze ook worden verzonden naar [!DNL Slack], zie [Configureren [!DNL Workfront] meldingen voor [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack).

1. Ga naar de **[!DNL Workfront]** kanaal om uw [!DNL Workfront] meldingen.
1. (Voorwaardelijk en optioneel) Voer een van de volgende handelingen uit:

   * Klikken **[!UICONTROL Work on it]** aanvaarden om aan een taak te werken.

   * (Voorwaardelijk en optioneel) Klik op **[!UICONTROL Reply in [!DNL Workfront]]** Als u wilt reageren op een opmerking, typt u uw antwoord en klikt u op **[!UICONTROL Reply]**.

   * (Voorwaardelijk en optioneel) Klik op **[!UICONTROL Approve]** of **[!UICONTROL Reject]** om een taak, kwestie, of project goed te keuren of te verwerpen die uw goedkeuring in afwachting zijn.

   * (Voorwaardelijk en optioneel) Klik op **[!UICONTROL Approve]**, **[!UICONTROL Changes]**, of **[!UICONTROL Reject]**, een document goed te keuren, met wijzigingen goed te keuren of af te wijzen.

     U kunt de muis ook boven de miniatuur van het document houden en op het vergrootglaspictogram klikken om een grotere voorvertoning van het document weer te geven voordat u het goedkeurt.\
      Alleen de goedgekeurde Slack [bestandstypen](https://api.slack.com/types/file) kan worden voorvertoond.

   * (Voorwaardelijk en optioneel) Klik op **[!UICONTROL Grant]** of **[!UICONTROL Ignore]** om het verzoek om meer toegang van een andere gebruiker te verlenen of te negeren.\

     Je ontvangt een bevestiging dat je actie is uitgevoerd in [!DNL Workfront], voor elk besluit dat u neemt in uw berichten.
