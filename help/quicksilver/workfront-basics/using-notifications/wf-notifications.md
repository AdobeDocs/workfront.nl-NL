---
content-type: overview;reference
navigation-topic: notifications
title: Overzicht van meldingen
description: Adobe Workfront verzendt e-mailmeldingen, meldingen in de app en meldingen op uw mobiele apparaat.
author: Courtney
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '1355'
ht-degree: 0%

---

# Overzicht van meldingen

<!--Audited: 12/2023-->

[!DNL Adobe Workfront] verzendt e-mailmeldingen, meldingen in de app en meldingen op uw mobiele apparaat.

## E-mailmeldingen

[!DNL Workfront] verzendt e-mailmeldingen om gebruikers te waarschuwen over activiteiten in Workfront en geeft nuttige informatie en koppelingen.

Om de voorkeur voor uw e-mailberichten te veranderen, zie [&#x200B; uw eigen e-mailberichten wijzigen &#x200B;](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Als u e-mailmeldingen wilt ontvangen vanuit de Sandbox-omgeving, moet u e-mails inschakelen vanuit uw gebruikersprofiel in die omgeving.

U kunt de volgende e-mailmeldingen ontvangen van [!DNL Workfront] :

* [Gebeurtenismeldingen](#event-notifications)
* [Dagelijkse samenvattingsberichten](#daily-digest-notifications)
* [Kennisgeving van geposte opmerkingen](#notification-of-posted-comments)
* [Automatische herinneringen](#automatic-reminders)
* [Herinneringsmeldingen](#reminder-notifications)
* [Boekberichten](#boards-notifications)
* [Andere  [!DNL Workfront]  e-mails](#other-workfront-emails)

### Gebeurtenismeldingen

Gebeurtenismeldingen die gewoonlijk worden geactiveerd door bepaalde vooraf gedefinieerde gebeurtenissen, zoals het hebben van een taak die aan u is toegewezen of het krijgen van een antwoord op een opmerking die u hebt gemaakt.

Nadat de [!DNL Workfront] -beheerder of groepsbeheerder gebeurtenismeldingen in uw [!DNL Workfront] -systeem heeft geactiveerd, kunt u selecteren welke meldingen u wilt ontvangen door uw [!UICONTROL Notifications] -voorkeuren in uw gebruikersprofiel te bewerken. U kunt ook kiezen of u meldingen wilt ontvangen terwijl er gebeurtenissen plaatsvinden, of dat u gebeurtenissen wilt ontvangen die zijn samengevat in één e-mailoverzicht voor dagelijkse controlesamenvatting.

Afhankelijk van de manier waarop de [!DNL Workfront] -beheerder gebeurtenismeldingen voor uw [!DNL Workfront] -systeem heeft geconfigureerd, ziet u mogelijk alleen een subset van deze meldingen in uw instellingen. Voor meer informatie, zie [&#x200B; gebeurtenisberichten voor iedereen in het systeem &#x200B;](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md) vormen.

In de standaardstatus wordt aangegeven welke meldingen (dagelijks, direct of beide) standaard zijn ingeschakeld voor nieuwe gebruikers wanneer u de nieuwe gebruikers maakt.

Voor een volledige lijst van de gebeurtenisberichten, en informatie over hoe zij op het systeemniveau, groepsniveau, of gebruikersniveau worden toegelaten en gevormd, zie [&#x200B; de berichten van de Gebeurtenis beschikbaar in  [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Voor informatie over hoe te om te kiezen welke gebeurtenisberichten u wilt ontvangen, zie [&#x200B; uw eigen e-mailberichten wijzigen &#x200B;](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Gebeurtenismeldingen zijn de enige meldingen die kunnen worden geconfigureerd voor levering in dagelijkse samenvattingsupdates.

### Dagelijkse samenvattingsberichten

Een dagelijkse overzichtsmelding is een e-mail die alle berichten van een bepaald type bevat die u in de 24 uur vóór e-mail hebt ontvangen.

Voor een volledige lijst van welke e-mailberichten voor een dagelijkse samenvatting e-maillevering evenals informatie over alle categorieën voor e-mailberichten zijn toegelaten, zie [&#x200B; de berichten van de Gebeurtenis &#x200B;](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] verzendt geen dagelijkse samenvattingsmeldingen voor de categorieën [!UICONTROL Miscellaneous] en [!DNL Goals] van gebeurtenissen. U kunt de Dagelijkse meldingen voor deze categorieën niet uitschakelen.

Bij het ontvangen van dagelijkse samenvattingsmeldingen moet u rekening houden met een aantal dingen:

* Elke sectie [!UICONTROL notifications] in het deelvenster **[!UICONTROL My Settings]** genereert een eigen dagelijkse samenvatting-e-mail. U kunt elke dag zo veel e-mails met een overzicht hebben als meldingsinstellingen die zijn ingeschakeld voor dagelijkse e-mails met een overzicht.\
   Als u bijvoorbeeld hebt opgegeven dat u een dagelijkse samenvatting per e-mail wilt ontvangen voor verschillende acties onder **[!UICONTROL Information about Projects I]Eigen,** , ontvangt u één e-mailmelding met alle gebeurtenissen waaraan voor dit gebied is voldaan.

* Meldingen in een e-mailbericht met een dagelijkse samenvatting worden op verschillende criteria gegroepeerd. In het geval van **[!UICONTROL Information about Projects I Own]** worden de gebeurtenissen bijvoorbeeld gegroepeerd op de projectnaam.

  Voor de categorie **[!UICONTROL Communication]** worden de meldingen gegroepeerd door het object waar de communicatie heeft plaatsgevonden.

  >[!NOTE]
  >
  >Voor de categorie Communicatie kunt u afzonderlijke berichten selecteren die u direct wilt afleveren. Als u meldingen in een dagelijkse samenvatting wilt laten verzenden, moet u ze allemaal selecteren.

* De dagelijkse samenvatting e-mail maakt een lijst van gebeurtenissen die voor de acties op één bepaald gebied (als **Informatie over projecten I Bezit**) binnen de 24 uren voorafgaand aan de tijd die voor levering wordt gekozen.
* De tijdzone voor de tijd die voor dagelijkse samenvattingslevering wordt geselecteerd past uw timezone aan, aangezien het op uw browser wordt gevormd.
* De dagelijkse samenvattingse-mails hebben de naam van de sectie in de onderwerpregel en de datum waarop ze worden bezorgd.
* Ten minste één gebeurtenis moet een melding activeren voordat de dagelijkse samenvatting kan worden geleverd. Dagelijkse samenvattingen worden niet verzonden als er aan geen gebeurtenissen is voldaan die zijn gemarkeerd voor dagelijkse samenvattingen van e-mails.

### Kennisgeving van geposte opmerkingen

De meldingen in de categorie [!UICONTROL Communication] geven een waarschuwing voor opmerkingen die zijn geplaatst in de [!UICONTROL Update] -stream van een specifiek item.

E-mails met dagelijkse samenvattingen voor de categorie [!UICONTROL Communication] worden geselecteerd voor alle beschikbare berichten.

De informatie wordt samengevat voor het voorwerp waar de mededeling voorkwam, en een totaal aantal communicatie berichten wordt getoond voor elk voorwerp.

Als u wilt reageren op de opmerking of deze wilt bekijken in Workfront:

1. Klik op de knop **[!UICONTROL Comment]** in de e-mail.

   Het [!UICONTROL Updates] -gebied van het object wordt geopend, met de specifieke opmerking in blauw.

   Er is een antwoordvenster geopend dat u kunt gebruiken om op de opmerking te reageren.

Voor meer informatie over het vormen van e-mailberichten, met inbegrip van het toelaten van dagelijkse samenvattingsberichten, zie [&#x200B; Mening en wijzig uw montages van het e-mailbericht &#x200B;](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view-and-modify-your-email-notification-settings) in [&#x200B; uw eigen e-mailberichten wijzigen &#x200B;](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Automatische herinneringen

Automatische herinneringen worden door de [!DNL Workfront] -beheerder ingeschakeld om u te waarschuwen voor taken en problemen die opeisbaar, te laat of bijna op de geplande voltooiingsdatum zijn. Voor late meldingen wordt de e-mail iedere avond verzonden totdat de taak of uitgave is voltooid. Nadat de beheerder deze vormt, kunt u hen niet onbruikbaar maken. U kunt ook de inhoud of het onderwerpregel van een e-mailbericht dat wordt geactiveerd door een automatische herinnering niet wijzigen.

Zij kunnen naar één of meerdere van het volgende worden verzonden:

* De gebruikers die aan een taak of kwestie worden toegewezen
* De directe manager van de gebruiker
* De manager van de directe manager

Automatische herinneringse-mails worden verzonden vanaf het e-mailadres dat de beheerder van [!DNL Workfront] heeft geselecteerd voor de verwerking van uitgaande e-mails.

Afhankelijk van welke automatische herinnering wordt geactiveerd, zijn de volgende soorten informatie beschikbaar in de automatische herinnering e-mail:

* De datum waarop de taak of uitgave is gemaakt
* Naam van taak of uitgave
* De naam van het project waar de taak of kwestie verblijft
* Beschrijving van taak of afgifte
* Een lijst met gebruikers die zijn toegewezen aan de taak of uitgave
* De naam van de gebruiker die de taak of uitgave heeft ingevoerd
* Prioriteit van de taak of kwestie
* Datum waarop de taak of uitgifte achterstallig werd

Voor informatie over het toelaten van automatische herinneringen, zie [&#x200B; Opstelling automatische herinneringen &#x200B;](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### Herinneringsmeldingen

Een [!DNL Workfront] -beheerder (of een gebruiker met een [!UICONTROL Planner] -toegangsniveau en beheertoegang tot herinneringsmeldingen) kan herinneringsmeldingen over het naderen van deadlines ontwerpen en deze handmatig koppelen aan projecten, taken, problemen en tijdbladen.

>[!IMPORTANT]
>
>Als de deadline verandert nadat een gebruiker een herinneringsbericht voor een van de hierboven vermelde objecten ontvangt, ontvangt de gebruiker geen ander herinneringsbericht.

Herinneringsberichten worden verzonden vanaf het e-mailadres dat de beheerder van [!DNL Workfront] heeft geselecteerd voor de verwerking van uitgaande e-mailberichten.

Voor informatie over vestiging en het toelaten van herinneringsberichten, zie [&#x200B; de herinneringsberichten van de Opstelling &#x200B;](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

Voor informatie over hoe u de vereiste administratieve toegang kunt krijgen, zie [&#x200B; gebruikers administratieve toegang van de Verlening tot bepaalde gebieden &#x200B;](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

### Boekberichten

[!DNL Adobe Workfront] [!UICONTROL Boards] stuurt u een e-mail wanneer u aan een bord wordt toegevoegd en wanneer een kaart aan u wordt toegewezen. U kunt selecteren welke e-mails u wilt ontvangen in de voorkeursinstellingen voor de kamers.

Voor meer informatie, zie [&#x200B; Boards e-mailberichten en voorkeur &#x200B;](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### Overige [!DNL Workfront] e-mails

Er zijn andere e-mails die u ontvangt van [!DNL Workfront] en die niet kunnen worden geconfigureerd.

De volgende e-mails worden automatisch verzonden door [!DNL Workfront] als aan deze voorwaarden wordt voldaan:

* Een item herstellen: wanneer de [!DNL Workfront] -beheerder een object uit het [!UICONTROL Recycle] -vak herstelt, wordt een e-mail verzonden naar de [!DNL Workfront] -beheerder.
* Kan niet worden hersteld: wanneer de [!DNL Workfront] -beheerder een object probeert te herstellen vanuit de prullenbak en het herstellen is mislukt, wordt een e-mail verzonden naar de [!DNL Workfront] -beheerder.

De volgende e-mails kunnen alleen op gebruikersprofielniveau worden geconfigureerd. Ze kunnen niet worden in- of uitgeschakeld op systeemniveau:

* Voltooiing van persoonlijke taak: wanneer een persoonlijke taak die u aan iemand anders hebt toegewezen, is voltooid, ontvangt u een e-mail.
* Opmerking toegevoegd aan gebruiker: wanneer iemand opmerkingen maakt over uw gebruikersprofiel, ontvangt u een e-mail.

## Meldingen in apps

U kunt meldingen ontvangen in de [!DNL Workfront] -webtoepassing wanneer bepaalde gebeurtenissen plaatsvinden.

Voor meer informatie over in-app berichten, zie [&#x200B; Mening en beheer in-app berichten &#x200B;](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## E-mailmeldingen in de mobiele e-mailtoepassing

U kunt [!DNL Workfront] e-mailmeldingen ontvangen in uw mobiele e-mailtoepassing op uw mobiele apparaat.

Als u de [!DNL Workfront] Mobile-app op uw telefoon hebt geïnstalleerd, kunt u deze openen in de [!DNL Workfront] Mobile-app door op de koppelingen in de e-mail te tikken. U kunt bijvoorbeeld op een van de volgende actieknoppen tikken:

* [!UICONTROL Work On It]
* [!UICONTROL Comment]
* [!UICONTROL Make Approval Decision]
* [!UICONTROL See All Notifications]
* [!UICONTROL Add]
* [!UICONTROL Get Started]
* [!UICONTROL See More Details]

Voor meer informatie over [!DNL Workfront] Mobiele App, zie [&#x200B; Gebruik  [!DNL Adobe Workfront]  mobiele app &#x200B;](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
