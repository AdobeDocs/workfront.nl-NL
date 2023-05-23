---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Werken in tijdzones
description: Het kan nuttig zijn om te begrijpen hoe [!DNL Adobe Workfront] gebruikt tijdzones om tijdvelden te berekenen voor objecten en tijden in andere gebieden, zoals e-mails.
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 0%

---

# Werken in tijdzones

Het kan nuttig zijn om te begrijpen hoe [!DNL Adobe Workfront] gebruikt tijdzones om het volgende te berekenen:

* Tijdvelden voor objecten
* Andere tijden [!DNL Workfront] gebieden, zoals automatische e-mails van Workfront

## Tijdzones in [!DNL Workfront]

Tijd die je ziet in [!DNL Workfront] zijn gebaseerd op configuraties van tijdzones voor uw organisatie [!DNL Workfront] en voor uw gebruikersprofiel. Als deze twee tijdzones verschillend zijn, ziet u mogelijk tijdverschillen in de verschillende gebieden en functies die u gebruikt in [!DNL Workfront].

>[!NOTE]
>
>In een douaneformulier in bijlage aan een voorwerp, worden de datum en de tijdverklaringen in berekende douanevelden berekend en bewaard door Coordinated Universal Time (UTC), niet door de configuraties van de tijdzone die voor de instantie van uw organisatie en uw gebruikersprofiel worden geplaatst. Berekeningen in een aangepast formulier worden gegenereerd en weergegeven op basis van de afzonderlijke tijdzones van elke gebruiker.

* [De [!DNL Workfront] instance](#your-organization-s-workfront-instance)
* [Uw gebruikersprofiel](#your-user-profile)

### De [!DNL Workfront] instance {#your-organization-s-workfront-instance}

De tijdzone voor de [!DNL Workfront] instantie wordt meestal ingesteld voor de locatie van het hoofdkantoor. Dit bepaalt het volgende:

* De tijd die wordt getoond in e-mailberichten die worden gegenereerd door [!DNL Workfront]
* De tijdzone voor nieuwe gebruikers (vóór de [!DNL Workfront] beheerder vormt een verschillende tijdzone voor hen die op waar worden gebaseerd zij)

   Zie voor meer informatie over deze twee voorbeelden [Basisinformatie voor uw systeem configureren](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Het begin of einde van een overschreven factureringspercentage voor een project. Zie voor meer informatie [De Factureringstarieven van de Rol van de Opheffing van de Taak op het projectniveau](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Uw gebruikersprofiel {#your-user-profile}

De tijdzone in uw gebruikersprofiel zou voor de plaats moeten worden gevormd waar u werkt. Dit bepaalt het volgende:

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* Tijdstippen voor een object waaraan u werkt, zoals begin- en eindtijd

   Als gebruikers in meerdere tijdzones zijn toegewezen aan een object, [!DNL Workfront] converteert de objecten tijden voor iedereen betrokken, gebruikend de tijdzone die in elk gebruikersprofiel wordt gevormd.

   **Voorbeeld:** In de Oost Standaardstreek van de Tijd (EST) waar u werkt, plaatst u een taak om bij 4:00 PM te beginnen en het toe te wijzen aan gebruikers die in de StandaardTijd van de Stille Oceaan (PST) streek werken. Voor die gebruikers wordt de begintijd weergegeven als 1:00 PM. Als het om 16:00 uur zou worden weergegeven, zouden ze er drie uur te laat aan beginnen te werken.

   Als de maker van het object het verschil tussen de tijdzones van de toewijzing niet opmerkt en de benodigde aanpassingen doorvoert bij het instellen van objecttijden, of als de toewijzen niet opmerken dat het verschil is, kan het moeilijk zijn om de timing goed te krijgen terwijl iedereen aan het object meewerkt.

   **Voorbeeld:** U vormt een eendaagse taak om bij 9:00 AM EST te beginnen, vergeten dat sommige gebruikers op het taakwerk in de streek PST. Voor hen, de begintijd 6:00 AM. Omdat ze er pas 9:00 uur aan beginnen te werken (12 uur &#39;s middags), begint de taak en eindigt deze drie uur later.

Voor informatie die uw tijdzone in uw gebruikersprofiel vormen, zie [Mijn instellingen configureren](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Voor informatie over hoe een [!DNL Workfront] beheerder (of iemand met [!UICONTROL Edit] toegang tot gebruikers) kan de tijdzone in een gebruikersprofiel vormen, zie [Gebruikersprofiel bewerken](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Hoe u het voor gebruikers gemakkelijker kunt maken om over tijdzones te werken

U kunt gebruikers helpen die gemakkelijker in verschillende tijdzones werken op verschillende manieren:

* [Planningen gebruiken](#use-schedules)
* [Berekende tijdvelden gebruiken in een aangepast formulier](#use-calculated-time-fields-in-a-custom-form)
* [Gebruik tekstvelden in plaats van datumvelden in een aangepast formulier](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Planningen gebruiken {#use-schedules}

[!DNL Workfront] beheerders creëren afzonderlijke programma&#39;s voor elke tijdzone binnen uw organisatie om ervoor te zorgen dat het werk geschikt voor iedereen, waar zij zijn gepland. Zodra de beheerder de programma&#39;s creeert, kunnen zij met bepaalde projecten en gebruikers worden geassocieerd:

* **[!UICONTROL Projects]**: Een projectmaker kan een programma voor een individueel project selecteren. Dit bepaalt het plannen van de taken in het project, dat op de werkuren wordt gebaseerd die voor de de tijdstreken van de ontvangers worden geplaatst.
* **[!UICONTROL Users]**: A [!DNL Workfront] beheerder (of iemand met [!UICONTROL Edit] (toegang tot gebruikers) kan een programma voor individuele gebruiker in het profiel van de gebruiker selecteren.

   Dit programma kan van een projectprogramma verschillend zijn. Bijvoorbeeld, wanneer iemand een taak in het project creeert en nog niemand aan het heeft toegewezen, gebruikt de taak het projectprogramma. Wanneer een gebruiker aan de taak wordt toegewezen, gebruikt de taak het programma van die gebruiker.

   Als de veelvoudige gebruikers aan een taak worden toegewezen, gebruikt het systeem één van het volgende, zoals die in de systeembrede projectvoorkeur wordt gevormd:

   * De tijdzone voor het programma van de primaire eigenaar van de taak
   * De tijdzone voor het programma van het project.

   Hierdoor kunnen taakdatums veranderen.

   **Voorbeeld:** Een EST-gebruiker wordt toegewezen aan een eendaagse taak die om 9:00 uur PST wordt gepland, dat is 12.00 uur EST. Omdat de EST-gebruiker slechts twee werkuren voor de dag heeft, loopt de datum waarop de taak is voltooid met ongeveer zes uur door tot de volgende werkdag.

   Voor informatie over de [!UICONTROL Project Preferences] gebied van [!UICONTROL Setup], zie [Projectvoorkeuren voor het hele systeem configureren](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   Voor instructies bij het toewijzen van een programma aan een project of een gebruiker, zie [Een schema maken](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   Voor informatie over hoe de tijdzone die in uw programma wordt gevormd de distributie van beïnvloedt [!UICONTROL Planned Hours] in de [!DNL Workload Balancer], zie [Gebruikerstoewijzingen beheren in het dialoogvenster [!DNL Workload Balancer]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### Berekende tijdvelden gebruiken in een aangepast formulier {#use-calculated-time-fields-in-a-custom-form}

U kunt een reeks berekende douanevelden op een douaneformulier gebruiken om de huidige tijd voor gebruikers in uw organisatie, zoals een rij van luchthavenklokken te tonen die de tijd in veelvoudige steden tonen. U zou een gebied voor elk van de tijdstreken kunnen tot stand brengen waar uw gebruikers werken, elk die de tijd voor zijn tijdzone berekenen.

Zie voor meer informatie [Berekende gegevens toevoegen aan een aangepast formulier](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)en de sectie [Berekende datum en tijd, aangepaste velden](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) in het artikel [Berekende gegevensexpressies](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Gebruik tekstvelden in plaats van datumvelden in een aangepast formulier {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Als u niet wilt [!DNL Workfront] als u de tijd wilt converteren die u voor in een object configureert voor gebruikers in verschillende tijdzones, kunt u een tekstveld in een aangepast formulier gebruiken dat u aan een object koppelt, in plaats van een datumveld. Op deze manier wordt de tijd weergegeven die u voor iedereen in het project typt.

Als u dit doet, raden we u aan de gebruikers van het formulier eraan te herinneren het verschil tussen hun tijdzone en die van u te berekenen, zodat ze kunnen bepalen wanneer het werk moet beginnen en eindigen. Dit kunt u opnemen in de instructies die u voor het aangepaste formulier typt of in de knopinfo voor dat veld. Zie voor meer informatie [Een aangepast veld toevoegen aan een aangepast formulier](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
