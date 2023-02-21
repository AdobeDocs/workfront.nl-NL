---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Toegang [!DNL Adobe Workfront] van [!DNL Slack]
description: Integreren [!DNL Adobe Workfront] with [!DNL Slack] geeft u toegang tot [!DNL Workfront] van Slack of bepaalde handelingen uitvoeren in [!DNL Workfront] gebruiken van een schuine streep bevel. De integratie kan vanaf elk [!DNL Slack] milieu, met inbegrip van [!DNL Slack] mobiele app.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '1040'
ht-degree: 0%

---

# Toegang [!DNL Adobe Workfront] van [!DNL Slack]

Integreren [!DNL Adobe Workfront] with [!DNL Slack] geeft u toegang tot [!DNL Workfront] van [!DNL Slack]of bepaalde handelingen uit te voeren in [!DNL Workfront] gebruiken van een schuine streep bevel. De integratie kan vanaf elk [!DNL Slack] milieu, met inbegrip van [!DNL Slack] mobiele app.

U of uw [!DNL Slack] de beheerder moet [!DNL Workfront] in uw [!DNL Slack] instantie voordat u kunt gebruiken [!DNL Workfront] van [!DNL Slack]. Zie voor meer informatie [Adobe Workfront for Slack configureren](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Informatie over slashopdrachten {#about-slash-commands}

Wanneer u [!DNL Slack], typt u berichten in een berichtveld. Wanneer u uw bericht met een schuine streep begint, wordt het een bevel en het gedraagt zich anders dan een eenvoudig bericht. De opdracht vertelt [!DNL Slack] om een handeling uit te voeren.

U hebt toegang tot uw [!DNL Workfront] instantie van [!DNL Slack] door een slash-opdracht in te voeren [!DNL Slack] kanaal.

Onthoud het volgende wanneer u een slash-opdracht gebruikt in [!DNL Slack] toegang [!DNL Workfront]:

* Slash-opdrachten zijn hoofdlettergevoelig.
* De opdrachten voor [!DNL Workfront] zijn alleen zichtbaar voor u, ongeacht het kanaal waarin u de bestanden typt.
* De opdracht moet altijd beginnen met `/workfront` of `/wf`, gevolgd door een spatie en de naam van een handeling waarin u wilt uitvoeren [!DNL Workfront].

   Dit wijst erop dat uw bevel voor wordt bedoeld [!DNL Workfront] app. De opdrachten voor [!DNL Workfront] werk slechts wanneer u reeds gevormd hebt [!DNL Workfront] app met uw [!DNL Slack] -instantie.

Voor een lijst van alle bevelen kunt u van Slack voor lopen [!DNL Workfront], zie [Toegang [!DNL Workfront] van een slash-opdracht in [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## Aanmelden bij [!DNL Workfront] van [!DNL Slack] {#log-in-to-workfront-from-slack}

Wanneer u om het even welk bevel op het berichtgebied in Slack typt, zult u worden gevraagd login aan [!DNL Workfront] eerst.\
Voor een volledige lijst met [!DNL Workfront] opdrachten van [!DNL Slack], zie de [Toegang [!DNL Workfront] van een slash-opdracht in [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) in dit artikel.

Aanmelden bij [!DNL Workfront] van [!DNL Slack]:

1. Meld u aan bij uw [!DNL Slack] -instantie.
1. Typ een van de volgende opdrachten vanuit een willekeurig kanaal:\
   `/workfront log in`

   of

   `/wf log in`

1. Klik op de knop [!DNL Workfront] **[!UICONTROL Log In]** wordt weergegeven in de reactie.\
   Er wordt een nieuw tabblad geopend met velden voor [!DNL Workfront] referenties.

1. Volg de aanwijzingen om u aan te melden [!DNL Workfront] het gebruiken van Verbeterde Authentificatie, OAuth 2.0, of uw Taal van de Prijsverhoging van de Veiligheid (SAML) URL.

   >[!NOTE]
   >
   >* Wanneer u wordt gevraagd om de gastheer van uw in te gaan [!DNL Workfront] -account, typt u deze notatie: *yourCompany&#39;sDomain.my.workfront.com*. Het domein van uw bedrijf is gewoonlijk de naam van uw bedrijf.
   >* Verbeterde verificatie is pas beschikbaar na een [!DNL Workfront] de beheerder laat het voor deze integratie toe.



   De configuratiepagina voor [!DNL Workfront] meldingen in [!DNL Slack] wordt geopend.

1. (Optioneel) Alle [!DNL Workfront] meldingen die u niet wilt ontvangen in [!DNL Slack].

   Voor informatie over het configureren [!DNL Workfront] instellingen voor [!DNL Slack], zie de [Instellingen configureren](#configure-settings-configure-settings) in dit artikel

1. Ga terug naar uw [!DNL Slack] kanaal.

   U bent aangemeld bij [!DNL Workfront] van uw [!DNL Slack] -instantie.

## Toegang [!DNL Workfront] van [!DNL Slack]

* [Informatie over slashopdrachten](#about-slash-commands-about-slash-commands)
* [Toegang [!DNL Workfront] vanuit een gedeelde koppeling in [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## Toegang [!DNL Workfront] van een slash-opdracht in [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. Meld u aan bij uw [!DNL Slack] instantie en aanmelden bij [!DNL Workfront] van [!DNL Slack].\
   Voor meer informatie over aanmelden bij [!DNL Workfront] van [!DNL Slack], zie [Aanmelden bij [!DNL Workfront] van [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. Typ de volgende opdracht in het berichtveld vanaf een willekeurig kanaal:

   `/workfront help`

   of

   `/wf help`

1. Selecteer een van de volgende opdrachten:

   * `/wf home`

      De knopen van vertoningen waarvan u tot lijsten van uw taken, kwesties, en goedkeuringen kunt toegang hebben. Wanneer u op een van de knoppen klikt, worden de eerste 20 items van elke lijst weergegeven in [!DNL Slack].

      Voor meer informatie over het beheren [!DNL Workfront] tijdelijke items van [!DNL Slack], zie [Uw werk en goedkeuringen beheren vanuit [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

      De naam van de taak opnemen zoals deze wordt weergegeven in het dialoogvenster [!DNL Workfront] interface.

      Hiermee voegt u een taak toe aan [!DNL Workfront].

      Voor meer informatie over het toevoegen van taken aan [!DNL Workfront] van Slack, zie &quot;het Creëren van Taken van [!DNL Slack]&quot; sectie in [Taken en uitgaven maken van [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

      Neem de naam van het probleem op zoals dit wordt weergegeven in het dialoogvenster [!DNL Workfront] interface.

      Hiermee voegt u een uitgave toe aan [!DNL Workfront]

      Voor meer informatie over het toevoegen van problemen aan [!DNL Workfront] van [!DNL Slack], zie &quot;Problemen maken van [!DNL Slack]&quot; sectie in [Taken en uitgaven maken van [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

      Hiermee geeft u de lijst met uw [!DNL Workfront] Favorieten.

      Voor meer informatie over de toegang tot van uw Favorieten van [!DNL Slack], zie de [Toegang tot uw [!UICONTROL Favorites] Lijst van [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) in de [Uw favorieten en recente objecten openen vanuit [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) artikel.

   * `/wf recent`

      Hiermee geeft u de lijst met onlangs geopende items weer in [!DNL Workfront].

      Voor meer informatie over toegang tot je recente objecten van [!DNL Slack], zie de [Toegang tot uw [!UICONTROL Recent Items] Lijst van [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] en [!UICONTROL recent items from [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) artikel.

   * `wf tasks`

      Hiermee geeft u een lijst met uw taken weer.

      Voor meer informatie over het beheren van uw taken van [!DNL Slack], zie &quot;Uw Taken beheren van [!DNL Slack]&quot; sectie in [Uw werk en goedkeuringen beheren vanuit [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

      Hier wordt een lijst met uw problemen weergegeven.

      Voor meer informatie over het beheer van uw uitgaven van [!DNL Slack], zie &quot;Uw problemen beheren van [!DNL Slack]&quot; sectie in [Uw werk en goedkeuringen beheren vanuit [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` Hiermee geeft u [!DNL Workfront] goedkeuringen.\

      Voor meer informatie over het beheren van uw goedkeuringen van [!DNL Slack], zie &quot;Uw Goedkeuringen beheren van [!DNL Slack]&quot; sectie in [Uw werk en goedkeuringen beheren vanuit [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

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

         Meer informatie over zoeken in [!DNL Slack], zie [Zoeken naar [!DNL Adobe Workfront] items van Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

      Aanmelden bij [!DNL Workfront] van [!DNL Slack].

   * `/wf log out `

      Meldt u af van [!DNL Workfront] van [!DNL Slack]. U bent aangemeld bij [!DNL Workfront] als u een aparte [!DNL Workfront] -instantie in een andere browsertab in een andere toepassing wordt geopend.
   * `/wf settings`

      Biedt u toegang tot het configureren van uw [!DNL Workfront] instellingen in [!DNL Slack].

      Voor informatie over het configureren [!DNL Workfront] instellingen in Slack, zie [Instellingen configureren](#configure-settings-configure-settings).

   * `/wf help`
Hiermee geeft u een volledige lijst met opdrachten weer voor [!DNL Workfront].


   * `Visit Workfront Help`: Hiermee opent u de [!UICONTROL Slack] de [!DNL Workfront] Help Site in een nieuw browsertabblad.


1. (Optioneel) Als u het bericht van een opdracht wilt verwijderen, beweegt u de muisaanwijzer over de rechterbovenhoek van het Slack-bericht dat de opdracht bevat en klikt u op &#x200B;**[!UICONTROL Show message actions]** en klik vervolgens op **[!UICONTROL Delete message]**.

1. (Optioneel en voorwaardelijk) Klik op **[!UICONTROL Delete]** om te bevestigen dat u dit bericht wilt verwijderen.

### Toegang [!DNL Workfront] vanuit een gedeelde koppeling in [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

U hebt toegang tot [!DNL Workfront] objecten van een koppeling naar de objecten die met u worden gedeeld in [!DNL Slack].

Voor meer informatie over toegang tot [!DNL Workfront] van een gedeelde koppeling, zie [Toegang [!DNL Adobe Workfront] objecten van een gedeelde koppeling in [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## Instellingen configureren {#configure-settings}

1. Binnen een [!DNL Slack] berichtgebied, typ het volgende bevel:

   `/workfront settings`

   of

   `/wf settings`

   Alle instellingen zijn standaard ingeschakeld.

1. Schakel een van de volgende opties uit om de instellingen voor Workfront uit te schakelen:

   * In de **[!UICONTROL General Settings]** gebied uitschakelen **[!UICONTROL When pasting a [!DNL Workfront] URL in a [!DNL Slack] channel, show additional description, due date, or requestor name]**&#x200B; instellen als u dat niet wilt [!DNL Slack] als u aanvullende informatie wilt toevoegen over uw [!DNL Workfront] objecten wanneer u een URL deelt naar het object in [!UICONTROL Slack].

   * In de **[!UICONTROL Notifications Settings]** in, schakelt u meldingen uit die u niet meer wilt ontvangen van Workfront.\

      Voor informatie over ontvangen [!DNL Workfront] meldingen in [!DNL Slack], zie [Ontvangen [!DNL Adobe Workfront] meldingen in [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Afmelden bij [!DNL Workfront] van [!DNL Slack]

1. Binnen een [!DNL Slack] berichtgebied, typ het volgende bevel:\
   `/workfront log out` of\
   `/wf log out`\
   U ontvangt een bevestiging dat u bent afgemeld van [!DNL Workfront].\
   U bent aangemeld bij [!DNL Workfront] als u een aparte [!DNL Workfront] -instantie in een andere browsertab in een andere toepassing wordt geopend.
