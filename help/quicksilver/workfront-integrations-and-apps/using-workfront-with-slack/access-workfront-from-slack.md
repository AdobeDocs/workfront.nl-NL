---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Toegang  [!DNL Adobe Workfront]  van  [!DNL Slack]
description: Het integreren  [!DNL Adobe Workfront]  met  [!DNL Slack]  staat u toe om  [!DNL Workfront]  van Slack toegang te hebben, of bepaalde acties in  [!DNL Workfront]  uit te voeren gebruikend een slash bevel. De integratie kan van om het even welk  [!DNL Slack]  milieu, met inbegrip van  [!DNL Slack]  mobiele app worden gebruikt.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 0%

---

# Toegang [!DNL Adobe Workfront] vanaf [!DNL Slack]

Door [!DNL Adobe Workfront] te integreren met [!DNL Slack] hebt u toegang tot [!DNL Workfront] vanuit [!DNL Slack] of kunt u bepaalde handelingen uitvoeren in [!DNL Workfront] met behulp van een slash-opdracht. De integratie kan vanuit elke [!DNL Slack] -omgeving worden gebruikt, inclusief de mobiele app van [!DNL Slack] .

Uw [!DNL Slack] -beheerder moet de [!DNL Workfront] app in uw [!DNL Slack] -instantie installeren voordat u [!DNL Workfront] from [!DNL Slack] kunt gebruiken. Voor meer informatie, zie [ Adobe Workfront voor Slack ](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) vormen.

## Informatie over slash-opdrachten {#about-slash-commands}

Wanneer u [!DNL Slack] gebruikt, typt u berichten in een berichtveld. Wanneer u uw bericht met een schuine streep begint, wordt het een bevel en het gedraagt zich anders dan een eenvoudig bericht. De opdracht geeft [!DNL Slack] de opdracht een handeling uit te voeren.

U hebt vanuit [!DNL Slack] toegang tot uw [!DNL Workfront] -instantie door een slash-opdracht in een willekeurig [!DNL Slack] -kanaal te typen.

Houd rekening met het volgende wanneer u een slash-opdracht in [!DNL Slack] gebruikt om toegang te krijgen tot [!DNL Workfront] :

* Slash-opdrachten zijn hoofdlettergevoelig.
* De opdrachten voor [!DNL Workfront] zijn alleen voor u zichtbaar, ongeacht in welk kanaal u de opdrachten typt.
* De opdracht moet altijd beginnen met `/workfront` of `/wf` , gevolgd door een spatie en de naam van een handeling die u wilt uitvoeren in [!DNL Workfront] .

  Dit geeft aan dat uw opdracht bedoeld is voor de [!DNL Workfront] -app. De opdrachten voor [!DNL Workfront] werken alleen wanneer u de [!DNL Workfront] app met uw [!DNL Slack] -instantie al hebt geconfigureerd.

Voor een lijst van alle bevelen u van Slack voor [!DNL Workfront] kunt in werking stellen, zie [ Toegang  [!DNL Workfront]  van een schuine streep bevel in  [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## Aanmelden bij [!DNL Workfront] vanuit [!DNL Slack] {#log-in-to-workfront-from-slack}

Wanneer u een opdracht in het berichtveld in Slack typt, wordt u gevraagd zich eerst aan te melden bij [!DNL Workfront] .\
Voor een volledige lijst van [!DNL Workfront] bevelen van [!DNL Slack], zie [ Toegang  [!DNL Workfront]  van een slash bevel in  [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) sectie in dit artikel.

Als u zich wilt aanmelden bij [!DNL Workfront] vanaf [!DNL Slack] :

1. Meld u aan bij uw [!DNL Slack] -instantie.
1. Typ een van de volgende opdrachten vanuit een willekeurig kanaal:\
   `/workfront log in`

   of

   `/wf log in`

1. Klik op de koppeling [!DNL Workfront] **[!UICONTROL Log In]** die in het antwoord wordt weergegeven.\
   Er wordt een nieuw tabblad geopend met velden voor [!DNL Workfront] -referenties.

1. Volg de aanwijzingen om u aan te melden bij [!DNL Workfront] via Enhanced Authentication, OAuth 2.0 of de URL voor de markering van beveiligingsinstellingen (SAML).

   >[!NOTE]
   >
   >* Wanneer u wordt ertoe aangezet om de gastheer van uw [!DNL Workfront] rekening in te gaan, typ het gebruikend dit formaat: *yourCompany&#39;sDomain.my.workfront.com*. Het domein van uw bedrijf is gewoonlijk de naam van uw bedrijf.
   >* Verbeterde verificatie is pas beschikbaar als een [!DNL Workfront] -beheerder deze heeft ingeschakeld voor deze integratie.


   De configuratiepagina voor [!DNL Workfront] -meldingen in [!DNL Slack] wordt geopend.

1. (Optioneel) Schakel alle [!DNL Workfront] -meldingen uit die u niet wilt ontvangen in [!DNL Slack] .

   Voor informatie over het vormen van [!DNL Workfront] montages voor [!DNL Slack], zie [ montages ](#configure-settings-configure-settings) sectie in dit artikel vormen

1. Ga terug naar het kanaal [!DNL Slack] .

   U bent aangemeld bij [!DNL Workfront] vanuit uw [!DNL Slack] -instantie.

## Toegang [!DNL Workfront] vanaf [!DNL Slack]

* [Informatie over slash-opdrachten](#about-slash-commands-about-slash-commands)
* [Toegang  [!DNL Workfront]  van een gedeelde verbinding in  [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## Toegang [!DNL Workfront] via een slash-opdracht in [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. Meld u aan bij de [!DNL Slack] -instantie en meld u aan bij [!DNL Workfront] from [!DNL Slack] .\
   Voor meer informatie over het programma openen aan [!DNL Workfront] van [!DNL Slack], zie [ Login aan  [!DNL Workfront]  van  [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. Typ de volgende opdracht in het berichtveld vanaf een willekeurig kanaal:

   `/workfront help`

   of

   `/wf help`

1. Selecteer een van de volgende opdrachten:

   * `/wf home`

     De knopen van vertoningen waarvan u tot lijsten van uw taken, kwesties, en goedkeuringen kunt toegang hebben. Wanneer u op een van de knoppen klikt, worden de eerste 20 items van elke lijst in [!DNL Slack] weergegeven.

     Voor meer informatie over het beheren van [!DNL Workfront] het werkpunten van [!DNL Slack], zie [ uw werk en goedkeuringen van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md) leiden.

   * `/wf add task <TaskName>`

     Neem de naam van de taak op zoals deze wordt weergegeven in de interface van [!DNL Workfront] .

     Voegt een taak toe aan [!DNL Workfront].

     Voor meer informatie over het toevoegen van taken aan [!DNL Workfront] van Slack, zie de &quot;Creërende Taken van [!DNL Slack]&quot;sectie in [ tot taken en kwesties van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md) leiden.

   * `/wf add issue <Issue Name>`

     Neem de naam van de uitgave op zoals deze wordt weergegeven in de interface van [!DNL Workfront] .

     Hiermee voegt u een uitgave toe aan [!DNL Workfront]

     Voor meer informatie over het toevoegen van kwesties aan [!DNL Workfront] van [!DNL Slack], zie de &quot;Creërende Kwesties van [!DNL Slack]&quot;sectie in [ creeer taken en kwesties van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

     Geeft de lijst met uw [!DNL Workfront] favorieten weer.

     Voor meer informatie over de toegang tot van uw Favorieten van [!DNL Slack], zie [ tot Uw [!UICONTROL Favorites] Lijst van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) sectie in [ toegang hebbend tot Uw Favorieten en Recente Punten van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) artikel.

   * `/wf recent`

     Hiermee geeft u de lijst weer van de laatst geopende items in [!DNL Workfront] .

     Voor meer informatie over de toegang tot van uw Recente Punten van [!DNL Slack], zie [ Toegang tot Uw [!UICONTROL Recent Items] Lijst van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites]  en [!UICONTROL recent items from [!DNL Slack]] ](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) artikel.

   * `wf tasks`

     Hiermee geeft u een lijst met uw taken weer.

     Voor meer informatie over het beheren van uw taken van [!DNL Slack], zie &quot;het Leiden Uw Taken van [!DNL Slack]&quot;sectie in [ het Leiden Uw Werk en Goedkeuringen van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

     Hier wordt een lijst met uw problemen weergegeven.

     Voor meer informatie over het beheren van uw kwesties van [!DNL Slack], zie &quot;het Leiden Uw Kwesties van [!DNL Slack]&quot;sectie in [ het Leiden Uw Werk en Goedkeuringen van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` Geeft uw [!DNL Workfront] -goedkeuringen weer.\

     Voor meer informatie over het beheren van uw goedkeuringen van [!DNL Slack], zie &quot;het Leiden Uw Goedkeuringen van [!DNL Slack]&quot;sectie in [ uw werk en goedkeuringen van  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md) leiden.

   * `/wf search <keyword>`

     Trefwoord opnemen.

     Zoeken naar een specifiek trefwoord. U kunt de volgende typen objecten zoeken:

      * Project
      * Taak
      * Probleem
      * Rapport
      * Mensen
      * Sjabloon
      * Document
      * Portfolio
      * Programma
      * Dashboard
      * Bedrijf
      * Notitie \

        Voor meer informatie over het zoeken in [!DNL Slack], zie [ Onderzoek naar  [!DNL Adobe Workfront]  punten van Slack ](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

     Hiermee meldt u zich aan bij [!DNL Workfront] vanuit [!DNL Slack] .

   * `/wf log out `

     Hiermee meldt u zich af van [!DNL Workfront] van [!DNL Slack] . U blijft aangemeld bij [!DNL Workfront] als u een aparte [!DNL Workfront] -instantie hebt geopend op een ander browsertabblad in een andere toepassing.
   * `/wf settings`

     Biedt u toegang tot het configureren van uw [!DNL Workfront] -instellingen in [!DNL Slack] .

     Voor informatie over het vormen van [!DNL Workfront] montages in Slack, zie [ montages ](#configure-settings-configure-settings) vormen.

   * `/wf help`
Hiermee geeft u een volledige lijst met opdrachten voor [!DNL Workfront] weer.


   * `Visit Workfront Help`: opent de [!UICONTROL Slack] -sectie op de [!DNL Workfront] Help-site in een nieuw browsertabblad.


1. (Optioneel) Als u het bericht van een opdracht wilt verwijderen, klikt u met de muis in de rechterbovenhoek van het bericht met de opdracht in de Slack en klikt u op &#x200B; **[!UICONTROL Show message actions]** . Klik vervolgens op **[!UICONTROL Delete message]** .

1. (Optioneel en voorwaardelijk) Klik op **[!UICONTROL Delete]** om te bevestigen dat u dit bericht wilt verwijderen.

### Toegang [!DNL Workfront] via een gedeelde koppeling in [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

U hebt toegang tot [!DNL Workfront] -objecten via een koppeling naar de objecten die u in [!DNL Slack] deelt.

Voor meer informatie over de toegang tot van [!DNL Workfront] van een gedeelde verbinding, zie [ Toegang  [!DNL Adobe Workfront]  voorwerpen van een gedeelde verbinding in  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Instellingen configureren {#configure-settings}

1. Typ in een berichtveld van het type [!DNL Slack] de volgende opdracht:

   `/workfront settings`

   of

   `/wf settings`

   Alle instellingen zijn standaard ingeschakeld.

1. Schakel een van de volgende opties uit om de instellingen voor Workfront uit te schakelen:

   * Schakel in het gebied **[!UICONTROL General Settings]** de instelling **[!UICONTROL When pasting a [!DNL Workfront] URL in a [!DNL Slack] channel, show additional description, due date, or requestor name]** &#x200B; uit als u niet wilt dat [!DNL Slack] aanvullende informatie over uw [!DNL Workfront] -objecten toevoegt wanneer u een URL deelt naar het object in [!UICONTROL Slack] .

   * Schakel in het gebied **[!UICONTROL Notifications Settings]** de meldingen uit die u niet meer van Workfront wilt ontvangen.\

     Voor informatie over het ontvangen van [!DNL Workfront] berichten in [!DNL Slack], zie [ ontvangen  [!DNL Adobe Workfront]  berichten in  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Log uit van [!DNL Workfront] van [!DNL Slack]

1. Typ in een berichtveld van het type [!DNL Slack] de volgende opdracht:\
   `/workfront log out` Of\
   `/wf log out`\
   U ontvangt een bevestiging dat u bent afgemeld van [!DNL Workfront] .\
   U blijft aangemeld bij [!DNL Workfront] als u een aparte [!DNL Workfront] -instantie hebt geopend op een ander browsertabblad in een andere toepassing.
