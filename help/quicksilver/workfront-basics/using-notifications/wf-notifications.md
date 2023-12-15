---
content-type: overview;reference
navigation-topic: notifications
title: Overzicht van meldingen
description: Adobe Workfront verzendt e-mailmeldingen, meldingen in de app en meldingen op uw mobiele apparaat.
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 6d2144732e5f47b670c2281d042a2dc950a2928f
workflow-type: tm+mt
source-wordcount: '1355'
ht-degree: 0%

---

# Overzicht van meldingen

<!--Audited: 12/2023-->

[!DNL Adobe Workfront] verzendt e-mailmeldingen, meldingen in de app en meldingen op uw mobiele apparaat.

## E-mailmeldingen

[!DNL Workfront] stuurt e-mailmeldingen naar gebruikers met informatie over activiteiten in Workfront en voeg nuttige informatie en koppelingen toe.

Als u de voorkeuren voor uw e-mailberichten wilt wijzigen, raadpleegt u [Uw eigen e-mailmeldingen wijzigen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Als u e-mailmeldingen wilt ontvangen vanuit de Sandbox-omgeving, moet u e-mails inschakelen vanuit uw gebruikersprofiel in die omgeving.

U kunt de volgende e-mailmeldingen ontvangen van [!DNL Workfront]:

* [Gebeurtenismeldingen](#event-notifications)
* [Dagelijkse samenvattingsberichten](#daily-digest-notifications)
* [Kennisgeving van geposte opmerkingen](#notification-of-posted-comments)
* [Automatische herinneringen](#automatic-reminders)
* [Herinneringsmeldingen](#reminder-notifications)
* [Boekberichten](#boards-notifications)
* [Overige [!DNL Workfront] e-mail](#other-workfront-emails)

### Gebeurtenismeldingen

Gebeurtenismeldingen die gewoonlijk worden geactiveerd door bepaalde vooraf gedefinieerde gebeurtenissen, zoals het hebben van een taak die aan u is toegewezen of het krijgen van een antwoord op een opmerking die u hebt gemaakt.

Nadat gebeurtenismeldingen zijn geactiveerd in uw [!DNL Workfront] door uw [!DNL Workfront] beheerder of groepsbeheerder, kunt u selecteren welke degenen u wilt ontvangen door uw uit te geven [!UICONTROL Notifications] in uw gebruikersprofiel. U kunt ook kiezen of u meldingen wilt ontvangen terwijl er gebeurtenissen plaatsvinden, of dat u gebeurtenissen wilt ontvangen die zijn samengevat in één e-mailoverzicht voor dagelijkse controlesamenvatting.

Afhankelijk van de manier waarop de [!DNL Workfront] de beheerder heeft gebeurtenisberichten voor uw gevormd [!DNL Workfront] systeem. Zie voor meer informatie [Gebeurtenismeldingen configureren voor iedereen in het systeem](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

In de standaardstatus wordt aangegeven welke meldingen (dagelijks, direct of beide) standaard zijn ingeschakeld voor nieuwe gebruikers wanneer u de nieuwe gebruikers maakt.

Voor een volledige lijst van de gebeurtenisberichten, en informatie over hoe zij op het systeemniveau, groepsniveau, of gebruikersniveau worden toegelaten en gevormd, zie [Gebeurtenismeldingen beschikbaar in [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Ga voor informatie over hoe u kunt kiezen welke gebeurtenismeldingen u wilt ontvangen naar [Uw eigen e-mailmeldingen wijzigen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Gebeurtenismeldingen zijn de enige meldingen die kunnen worden geconfigureerd voor levering in dagelijkse samenvattingsupdates.

### Dagelijkse samenvattingsberichten

Een dagelijkse overzichtsmelding is een e-mail die alle berichten van een bepaald type bevat die u in de 24 uur vóór e-mail hebt ontvangen.

Voor een volledige lijst van welke e-mailberichten voor een dagelijkse samenvatting e-maillevering evenals informatie over alle categorieën voor e-mailberichten zijn toegelaten, zie [Gebeurtenismeldingen](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] verzendt geen dagelijkse samenvattingsmeldingen voor de [!UICONTROL Miscellaneous] en [!DNL Goals] categorieën gebeurtenissen. U kunt de Dagelijkse meldingen voor deze categorieën niet uitschakelen.

Bij het ontvangen van dagelijkse samenvattingsmeldingen moet u rekening houden met een aantal dingen:

* Elk [!UICONTROL notifications] in uw **[!UICONTROL My Settings]** genereert een eigen dagelijkse samenvatting-e-mail. U kunt elke dag zo veel e-mails met een overzicht hebben als meldingsinstellingen die zijn ingeschakeld voor dagelijkse e-mails met een overzicht.\
   Als u bijvoorbeeld hebt geselecteerd om een dagelijkse samenvatting per e-mail te ontvangen voor verschillende acties onder de **[!UICONTROL Information about Projects I]Eigen,** u ontvangt één e-mailbericht met alle gebeurtenissen die voor dit gebied zijn ontvangen.

* Meldingen in een e-mailbericht met een dagelijkse samenvatting worden op verschillende criteria gegroepeerd. Bijvoorbeeld in het geval van **[!UICONTROL Information about Projects I Own]**, worden de gebeurtenissen gegroepeerd op de projectnaam.

  Voor de **[!UICONTROL Communication]** categorie, worden de meldingen gegroepeerd door het object waar de communicatie heeft plaatsgevonden.

  >[!NOTE]
  >
  >Voor de categorie Communicatie kunt u afzonderlijke berichten selecteren die u direct wilt afleveren. Als u meldingen in een dagelijkse samenvatting wilt laten verzenden, moet u ze allemaal selecteren.

* De dagelijkse samenvatting in de e-mail bevat gebeurtenissen die zijn opgetreden voor de acties op één bepaald gebied (zoals **Informatie over eigen projecten**) binnen 24 uur vóór de gekozen leveringstermijn.
* De tijdzone voor de tijd die voor dagelijkse samenvattingslevering wordt geselecteerd past uw timezone aan, aangezien het op uw browser wordt gevormd.
* De dagelijkse samenvattingse-mails hebben de naam van de sectie in de onderwerpregel en de datum waarop ze worden bezorgd.
* Ten minste één gebeurtenis moet een melding activeren voordat de dagelijkse samenvatting kan worden geleverd. Dagelijkse samenvattingen worden niet verzonden als er aan geen gebeurtenissen is voldaan die zijn gemarkeerd voor dagelijkse samenvattingen van e-mails.

### Kennisgeving van geposte opmerkingen

De meldingen in het [!UICONTROL Communication] rubriek Je waarschuwt voor opmerkingen die zijn geplaatst in het [!UICONTROL Update] stroom van een specifiek item.

Dagelijkse samenvattingse-mails voor de [!UICONTROL Communication] de categorie is geselecteerd voor alle beschikbare meldingen.

De informatie wordt samengevat voor het voorwerp waar de mededeling voorkwam, en een totaal aantal communicatie berichten wordt getoond voor elk voorwerp.

Als u wilt reageren op de opmerking of deze wilt bekijken in Workfront:

1. Klik op de knop **[!UICONTROL Comment]** in de e-mail.

   De [!UICONTROL Updates] wordt het gebied van het object geopend, met de specifieke opmerking in blauw.

   Er is een antwoordvenster geopend dat u kunt gebruiken om op de opmerking te reageren.

Voor meer informatie over het configureren van e-mailmeldingen, waaronder het inschakelen van dagelijkse digest-meldingen, raadpleegt u [De instellingen voor e-mailmeldingen weergeven en wijzigen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view-and-modify-your-email-notification-settings) in [Uw eigen e-mailmeldingen wijzigen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Automatische herinneringen

Automatische herinneringen worden ingeschakeld door uw [!DNL Workfront] beheerder om u van taken en kwesties op de hoogte te brengen die, laat, of dichtbij de geplande voltooiingsdatum te zijner tijd zijn. Voor late meldingen wordt de e-mail iedere avond verzonden totdat de taak of uitgave is voltooid. Nadat de beheerder deze vormt, kunt u hen niet onbruikbaar maken. U kunt ook de inhoud of het onderwerpregel van een e-mailbericht dat wordt geactiveerd door een automatische herinnering niet wijzigen.

Zij kunnen naar één of meerdere van het volgende worden verzonden:

* De gebruikers die aan een taak of kwestie worden toegewezen
* De directe manager van de gebruiker
* De manager van de directe manager

Automatische herinneringse-mails worden verzonden vanaf het e-mailadres dat uw [!DNL Workfront] beheerder geselecteerd om uitgaande e-mailberichten te verwerken.

Afhankelijk van welke automatische herinnering wordt geactiveerd, zijn de volgende soorten informatie beschikbaar in de automatische herinnering e-mail:

* De datum waarop de taak of uitgave is gemaakt
* Naam van taak of uitgave
* De naam van het project waar de taak of kwestie verblijft
* Beschrijving van taak of afgifte
* Een lijst met gebruikers die zijn toegewezen aan de taak of uitgave
* De naam van de gebruiker die de taak of uitgave heeft ingevoerd
* Prioriteit van de taak of kwestie
* Datum waarop de taak of uitgifte achterstallig werd

Voor informatie over het inschakelen van automatische herinneringen raadpleegt u [Automatische herinneringen instellen](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### Herinneringsmeldingen

A [!DNL Workfront] beheerder (of een gebruiker met een [!UICONTROL Planner] toegang tot niveau en administratieve toegang tot herinneringsberichten) kan herinneringsberichten over het naderen van termijnen ontwerpen en hen manueel associëren met projecten, taken, kwesties, en timesheets.

>[!IMPORTANT]
>
>Als de deadline verandert nadat een gebruiker een herinneringsbericht voor een van de hierboven vermelde objecten ontvangt, ontvangt de gebruiker geen ander herinneringsbericht.

Herinneringsmeldingen worden verzonden vanaf het e-mailadres dat de [!DNL Workfront] beheerder geselecteerd om uitgaande e-mailberichten te verwerken.

Voor informatie over het instellen en inschakelen van herinneringsmeldingen raadpleegt u [Herinneringsmeldingen instellen](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

Voor informatie over hoe u de vereiste administratieve toegang kunt krijgen, zie [Gebruikers administratieve toegang verlenen tot bepaalde gebieden](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

### Boekberichten

[!DNL Adobe Workfront] [!UICONTROL Boards] stuurt u een e-mail wanneer u aan een bord wordt toegevoegd en wanneer een kaart aan u wordt toegewezen. U kunt selecteren welke e-mails u wilt ontvangen in de voorkeursinstellingen voor de kamers.

Zie voor meer informatie [E-mailmeldingen en voorkeuren worden verzonden](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### Overige [!DNL Workfront] e-mail

Er zijn andere e-mails die je ontvangt van [!DNL Workfront] die niet kunnen worden geconfigureerd.

De volgende e-mails worden automatisch verzonden door [!DNL Workfront] wanneer aan deze voorwaarden is voldaan:

* Een item herstellen: wanneer de [!DNL Workfront] de beheerder herstelt een voorwerp van [!UICONTROL Recycle] Bak, er wordt een e-mail verzonden naar de [!DNL Workfront] beheerder.
* Kan niet herstellen: Wanneer de [!DNL Workfront] beheerder probeert een object te herstellen vanuit de prullenbak en het terugzetten is mislukt. Er wordt een e-mail verzonden naar de [!DNL Workfront] beheerder.

De volgende e-mails kunnen alleen op gebruikersprofielniveau worden geconfigureerd. Ze kunnen niet worden in- of uitgeschakeld op systeemniveau:

* Voltooiing van persoonlijke taak: wanneer een persoonlijke taak die u aan iemand anders hebt toegewezen, is voltooid, ontvangt u een e-mail.
* Opmerking toegevoegd aan gebruiker: wanneer iemand opmerkingen maakt over uw gebruikersprofiel, ontvangt u een e-mail.

## Meldingen in apps

U kunt meldingen ontvangen in het dialoogvenster [!DNL Workfront] webtoepassing, wanneer bepaalde gebeurtenissen plaatsvinden.

Zie voor meer informatie over meldingen in de app [Meldingen in apps weergeven en beheren](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## E-mailmeldingen in de mobiele e-mailtoepassing

U kunt [!DNL Workfront] e-mailmeldingen in uw mobiele e-mailtoepassing, op uw mobiele apparaat.

Als u de [!DNL Workfront] De mobiele toepassing die op uw telefoon is geïnstalleerd, en die op de verbindingen in e-mail tikt opent hen in [!DNL Workfront] Mobiele app. U kunt bijvoorbeeld op een van de volgende actieknoppen tikken:

* [!UICONTROL Work On It]
* [!UICONTROL Comment]
* [!UICONTROL Make Approval Decision]
* [!UICONTROL See All Notifications]
* [!UICONTROL Add]
* [!UICONTROL Get Started]
* [!UICONTROL See More Details]

Voor meer informatie over de [!DNL Workfront] Mobile App, zie [Gebruik de [!DNL Adobe Workfront] mobiele app](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
