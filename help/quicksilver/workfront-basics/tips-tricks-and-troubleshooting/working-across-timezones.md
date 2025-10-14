---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Werken in tijdzones
description: Het kan nuttig zijn om te begrijpen hoe  [!DNL Adobe Workfront]  tijdstreken gebruikt om tijdgebieden voor voorwerpen en tijden op andere gebieden zoals e-mails te berekenen.
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: 7697bb68e2042291e5290048cfc2f626145979af
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 0%

---

# Werken in tijdzones

<!-- Audited: 2/2024 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Het kan handig zijn om te begrijpen hoe [!DNL Adobe Workfront] tijdzones gebruikt om het volgende te berekenen:

* Tijdvelden voor objecten
* Tijden in andere [!DNL Workfront] gebieden, zoals geautomatiseerde Workfront-e-mails

>[!WARNING]
>
>Als u uw nauwkeurige tijdzone in de lijst niet kunt vinden wij verstrekken, vind de tijdzone die aan van u het dichtst is en werk het voor uw instantie bij.
>
>Bedenk ook dat een vergelijkbare tijdzone mogelijk niet perfect overeenkomt met die van u.
>
>Sommige landen of gebieden kunnen bijvoorbeeld de zomertijd in acht nemen, maar uw land misschien niet. Mogelijk moet u de tijdzones van uw systeem aanpassen aan deze wijzigingen.


## Tijdzones in [!DNL Workfront]

De tijden u in [!DNL Workfront] ziet zijn gebaseerd op de configuraties van de tijdzone voor de instantie van uw organisatie [!DNL Workfront] en voor uw gebruikersprofiel. Als deze twee tijdzones verschillend zijn, ziet u mogelijk tijdverschillen in de verschillende gebieden en functies die u in [!DNL Workfront] gebruikt.

>[!NOTE]
>
>In een douaneformulier in bijlage aan een voorwerp, worden de datum en de tijdverklaringen in berekende douanevelden berekend en bewaard door Coordinated Universal Time (UTC), niet door de configuraties van de tijdzone die voor de instantie van uw organisatie en uw gebruikersprofiel worden geplaatst. Berekeningen in een aangepast formulier worden gegenereerd en weergegeven op basis van de afzonderlijke tijdzones van elke gebruiker.

* [De instantie van uw organisatie  [!DNL Workfront] &#x200B;](#your-organization-s-workfront-instance)
* [Uw gebruikersprofiel](#your-user-profile)

### De [!DNL Workfront] -instantie van uw organisatie {#your-organization-s-workfront-instance}

De tijdzone voor de [!DNL Workfront] -instantie van uw organisatie wordt meestal ingesteld op de locatie van het hoofdkantoor. Dit bepaalt het volgende:

* De tijd die wordt weergegeven in e-mailberichten die worden gegenereerd door [!DNL Workfront]
* De tijdzone voor nieuwe gebruikers (voordat de beheerder van [!DNL Workfront] een andere tijdzone configureert op basis van waar ze werken)

  Voor meer informatie over deze twee voorbeelden, zie [&#x200B; basisinformatie voor uw systeem &#x200B;](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md) vormen.

* Het begin of einde van een overschreven factureringspercentage voor een project. Voor meer informatie, zie [&#x200B; het Facturerings van de Rol van de Opheffing van de Baan op het projectniveau &#x200B;](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Uw gebruikersprofiel {#your-user-profile}

Het veld Tijdzone in het gebruikersprofiel bepaalt de tijd die in de uitgaande e-mailberichten wordt weergegeven.

De tijdzone beïnvloedt ook wat vertoningen in een PTO kalenderrapport tonen.

Voor informatie die uw tijdzone in uw gebruikersprofiel vormen, zie [&#x200B; Mijn Montages &#x200B;](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) vormen.

Voor informatie over hoe een [!DNL Workfront] beheerder (of iemand met [!UICONTROL Edit] toegang tot gebruikers) de tijdzone in een gebruikersprofiel kan vormen, zie [&#x200B; het profiel van een gebruiker &#x200B;](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

### Tijdzone van uw browser

De tijdzone in uw browser zou voor de plaats moeten worden gevormd waar u werkt. Dit bepaalt het volgende:

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* Tijdstippen voor een object waaraan u werkt, zoals begin- en eindtijd.

  Als gebruikers in meerdere tijdzones aan een object zijn toegewezen, zet [!DNL Workfront] de objecttijden voor alle betrokkenen om met de tijdzone die in de browser van elke gebruiker is geconfigureerd.

  **VOORBEELD**
In de oostelijke Standaardstreek van de Tijd (EST) waar u werkt, plaatst u een taak om bij 4 :00 PM te beginnen en het toe te wijzen aan gebruikers die in de Standaardstreek van de Stille Oceaan werken (PST). Voor die gebruikers, de vertoningen van de begintijd als 1 :00 PM. Als het het als 4 :00 PM zou tonen, zouden zij beginnen aan het drie uren te werken te laat.

  Als de maker van het object het verschil niet weet tussen de tijdzones van de toewijzing en niet de benodigde aanpassingen aanbrengt bij het instellen van objecttijden, of als de toewijzen dat verschil niet weten, kan het moeilijk zijn om de timing goed te krijgen terwijl iedereen aan het object werkt.

  **VOORBEELD**

  U vormt een eendaagse taak om bij 9 :00 TE beginnen AM EST, vergeten dat sommige gebruikers op het taakwerk in de streek PST. Voor hen, de begintijd 6 :00 AM. Omdat zij niet aan het beginnen te werken tot 9 :00 hun tijd (middags uw tijd), begint de taak en eindigt drie uur te laat.

De configuratie van de tijdzone verschilt per browser. Raadpleeg de documentatie of Help van elke browser voor meer informatie.

## Hoe u het voor gebruikers gemakkelijker kunt maken om over tijdzones te werken

U kunt gebruikers helpen die gemakkelijker in verschillende tijdzones werken op verschillende manieren:

* [Planningen gebruiken](#use-schedules)
* [Berekende tijdvelden gebruiken in een aangepast formulier](#use-calculated-time-fields-in-a-custom-form)
* [Gebruik tekstvelden in plaats van datumvelden in een aangepast formulier](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Planningen gebruiken {#use-schedules}

[!DNL Workfront] beheerders creëren afzonderlijke programma&#39;s voor elke tijdzone binnen uw organisatie om ervoor te zorgen dat het werk geschikt voor iedereen wordt gepland, waar zij zijn. Zodra de beheerder de programma&#39;s creeert, kunnen zij met bepaalde projecten en gebruikers worden geassocieerd:

* **[!UICONTROL Projects]**: Een projectmaker kan een schema voor een afzonderlijk project selecteren. Dit bepaalt het plannen van de taken in het project, dat op de werkuren wordt gebaseerd die voor de de tijdstreken van de ontvangers worden geplaatst.
* **[!UICONTROL Users]**: een [!DNL Workfront] beheerder (of iemand met [!UICONTROL Edit] toegang tot gebruikers) kan een schema voor een individuele gebruiker selecteren in het gebruikersprofiel.

  Dit programma kan van een projectprogramma verschillend zijn. Bijvoorbeeld, wanneer iemand een taak in het project creeert en nog niemand aan het heeft toegewezen, gebruikt de taak het projectprogramma. Wanneer een gebruiker aan de taak wordt toegewezen, gebruikt de taak het programma van die gebruiker.

  Als de veelvoudige gebruikers aan een taak worden toegewezen, gebruikt het systeem één van het volgende, zoals die in de systeem of groepsbrede projectvoorkeur wordt gevormd:

   * De tijdzone voor het programma van de primaire eigenaar van de taak
   * De tijdzone voor het programma van het project.

  Als één gebruiker aan een taak wordt toegewezen, gebruikt het systeem één van het volgende, zoals die in de systeem of groep brede projectvoorkeur wordt gevormd:

   * De tijdzone voor het tijdschema van de taaktoewijzing
   * De tijdzone voor het programma van het project.

  Hierdoor kunnen taakdatums veranderen.

>[!BEGINSHADEBOX]

**VOORBEELD:**
Een gebruiker EST wordt toegewezen aan een eendagtaak die om bij 9 :00 wordt gepland te beginnen AM PST, die niet EST is. Omdat de EST-gebruiker slechts twee werkuren voor de dag heeft, loopt de datum waarop de taak is voltooid met ongeveer zes uur door tot de volgende werkdag.


>[!ENDSHADEBOX]

Voor informatie over het [!UICONTROL Project Preferences] gebied van [!UICONTROL Setup], zie [&#x200B; systeem-brede projectvoorkeur &#x200B;](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

Voor instructies bij het toewijzen van een programma aan een project of een gebruiker, zie [&#x200B; een programma &#x200B;](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

Voor informatie over hoe de tijdzone die in uw programma wordt gevormd de distributie van [!UICONTROL Planned Hours] in [!UICONTROL Workload Balancer] beïnvloedt, zie [&#x200B; gebruikerstoewijzingen in [!UICONTROL Workload Balancer]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md) beheren.


### Berekende tijdvelden gebruiken in een aangepast formulier {#use-calculated-time-fields-in-a-custom-form}

U kunt een reeks berekende douanevelden op een douaneformulier gebruiken om de huidige tijd voor gebruikers in uw organisatie, zoals een rij van luchthavenklokken te tonen die de tijd in veelvoudige steden tonen. U zou een gebied voor elk van de tijdstreken kunnen tot stand brengen waar uw gebruikers werken, elk die de tijd voor zijn tijdzone berekenen.

Voor meer informatie, zie [&#x200B; berekende gebieden aan een vorm &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) toevoegen, evenals de sectie [&#x200B; Datum &amp; tijd berekende douanevelden &#x200B;](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) in het artikel [&#x200B; Overzicht van berekende gegevensuitdrukkingen &#x200B;](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Gebruik tekstvelden in plaats van datumvelden in een aangepast formulier {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Als u niet wilt dat [!DNL Workfront] de tijden omzet u voor in een voorwerp voor gebruikers in verschillende tijdstreken vormt, kunt u een tekstgebied in een douaneformulier gebruiken dat u aan een voorwerp, eerder dan een datumgebied vastmaakt. Op deze manier wordt de tijd weergegeven die u voor iedereen in het project typt.

Als u dit doet, raden we u aan de gebruikers van het formulier eraan te herinneren het verschil tussen hun tijdzone en die van u te berekenen, zodat ze kunnen bepalen wanneer het werk moet beginnen en eindigen. Dit kunt u opnemen in de instructies die u voor het aangepaste formulier typt of in de knopinfo voor dat veld. Voor meer informatie, zie [&#x200B; een douaneformulier &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.
