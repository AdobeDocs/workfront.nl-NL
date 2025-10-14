---
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Privacy en rechten in Workfront voor Google Workspace
description: Privacy en rechten in Workfront voor Google Workspace
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Privacy en rechten in Workfront voor Google Workspace

>[!IMPORTANT]
>
>Om stabielere en scalable integratie te leveren, verschuiven wij naar een moderne, flexibele integratiebenadering gebruikend Workfront Automation and Integration (Fusion). Als deel van dit overgangsproces, zal volgende Workfront voor de functionaliteit van Google Workspace niet beschikbaar na **28 Februari, 2026** zijn:
>
>* Google Workspace-functionaliteit openen vanuit Workfront
>
>* Workfront-taken weergeven en beheren vanuit Gmail of het Google Calendar-sitevenster
>
>We raden u aan Workfront Automation and Integration te gebruiken voor de integratiebehoeften van uw organisatie met Google Workspace.
>
>Voor een overzicht van de Automatisering en de Integratie van Workfront, zie [&#x200B; het overzicht van de Fusie van Adobe Workfront &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Voor informatie over de specifieke mogelijkheden van de modules van de Automatisering en van de Integratie van Workfront voor Google Workspace, zie [&#x200B; modules van Gmail &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) en [&#x200B; modules van de Kalender van Google &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Omdat de privacy van klanten belangrijk is, slaat Adobe Workfront geen identificerende klantgegevens op of verzamelt deze die het resultaat zijn van toestemming van derden voor een Google-plug-in. Workfront for Google Workspace dat het gebruik en de overdracht van informatie van Google APIs aan een andere app wordt ontvangen zal met het [&#x200B; beleid van de Gegevens van de Gebruiker van de Diensten van Google API &#x200B;](https://developers.google.com/terms/api-services-user-data-policy), met inbegrip van de Beperkte vereisten van het Gebruik naleven.

We hebben de volgende machtigingen nodig, zodat de Workfront for Google Workspace plug-in zijn maximale waarde kan leveren:

* **Mening uw e-mailberichten wanneer toe:voegen-op** loopt: De insteekmodule van Workfront voor Google Workspace kan gebruikers ontelbare uren van dubbel werk besparen door e-mails in nieuwe taken in Workfront om te zetten en automatisch de titel en de beschrijving van de taak met het onderwerp en het lichaam van e-mail te bevolken. Met de insteekmodule kunt u uw e-mails als nieuwe opmerkingen op Workfront plaatsen. De insteekmodule moet uw e-mailberichten weergeven wanneer de invoegtoepassing wordt uitgevoerd om deze waarde te kunnen leveren.
* **looppas als toe:voegen-op Gmail/niet-gevoelig**: De toestemmingen zijn nodig voor Workfront voor Google Workspace toe:voegen-op aan functie in het milieu van Gmail. Voor de insteekmodule is een Gmail-omgeving vereist. Hiervoor is de machtiging `Run as a Gmail add-on / non-sensitive` vereist.
* **Bekijk uw e-mailberichtmeta-gegevens wanneer toe:voegen-op loopt**: Om werkschema&#39;s te verbeteren, bevestigt de elektrisch toestel van Workfront voor Google Workspace als een e-mail een bericht van Workfront is, en identificeert het type van Workfront bericht (nieuw het werkverzoek, goedkeuringsverzoek, nieuwe commentaar enz.). Voor de insteekmodule is toestemming van `View your email message metadata when the add-on is running` vereist om deze waarde te leveren.
* **Plug-in moet als toe:voegen-op/niet-gevoelig van de Kalender** lopen: De Workfront voor Workspace stop-binnen van Google verbindt met uw kalender, zodat kunt u visualiseren hoe de taken programma&#39;s beïnvloeden. De plug-in heeft hiervoor de toestemming van `Run as a Calendar add-on / non-sensitive` nodig.
* **verbind met een externe de diensttoestemming:** uiteindelijk, moet het elektrische toestel met Workfront API verbinden, die de backbone van de stop-in waarde is. De Workfront API is een service buiten Google, dus de plug-in heeft de `Connect to an external service permission` nodig om de plug-in te laten werken.

Voor meer informatie over de toewijding van Adobe Workfront aan klantenprivacy, zie {het Bericht van de Privacy van 0} Workfront [.](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf)

Voor meer informatie, zie [&#x200B; het Beleid van de Gegevens van de Gebruiker van de Diensten van Google API &#x200B;](https://developers.google.com/terms/api-services-user-data-policy).
