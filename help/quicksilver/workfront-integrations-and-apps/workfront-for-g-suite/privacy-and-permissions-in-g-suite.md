---
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Privacy en rechten in Workfront voor Google Workspace
description: Privacy en rechten in Workfront voor Google Workspace
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Privacy en rechten in Workfront voor Google Workspace

Omdat de privacy van klanten belangrijk is, slaat Adobe Workfront geen identificerende klantgegevens op of verzamelt deze die het resultaat zijn van toestemming van derden voor een Google-plug-in. Workfront for Google Workspace dat het gebruik en de overdracht van informatie van Google APIs aan een andere app wordt ontvangen zal met het [ beleid van de Gegevens van de Gebruiker van de Diensten van Google API ](https://developers.google.com/terms/api-services-user-data-policy), met inbegrip van de Beperkte vereisten van het Gebruik naleven.

We hebben de volgende machtigingen nodig, zodat de Workfront for Google Workspace plug-in zijn maximale waarde kan leveren:

* **Mening uw e-mailberichten wanneer toe:voegen-op** loopt: De insteekmodule van Workfront voor Google Workspace kan gebruikers ontelbare uren van dubbel werk besparen door e-mails in nieuwe taken in Workfront om te zetten en automatisch de titel en de beschrijving van de taak met het onderwerp en het lichaam van e-mail te bevolken. Met de insteekmodule kunt u uw e-mails als nieuwe opmerkingen op Workfront plaatsen. De insteekmodule moet uw e-mailberichten weergeven wanneer de invoegtoepassing wordt uitgevoerd om deze waarde te kunnen leveren.
* **looppas als toe:voegen-op Gmail/niet-gevoelig**: De toestemmingen zijn nodig voor Workfront voor Google Workspace toe:voegen-op aan functie in het milieu van Gmail. Voor de insteekmodule is een Gmail-omgeving vereist. Hiervoor is de machtiging `Run as a Gmail add-on / non-sensitive` vereist.
* **Bekijk uw e-mailberichtmeta-gegevens wanneer toe:voegen-op loopt**: Om werkschema&#39;s te verbeteren, bevestigt de elektrisch toestel van Workfront voor Google Workspace als een e-mail een bericht van Workfront is, en identificeert het type van Workfront bericht (nieuw het werkverzoek, goedkeuringsverzoek, nieuwe commentaar enz.). Voor de insteekmodule is toestemming van `View your email message metadata when the add-on is running` vereist om deze waarde te leveren.
* **Plug-in moet als toe:voegen-op/niet-gevoelig van de Kalender** lopen: De Workfront voor Workspace stop-binnen van Google verbindt met uw kalender, zodat kunt u visualiseren hoe de taken programma&#39;s beïnvloeden. De plug-in heeft hiervoor de toestemming van `Run as a Calendar add-on / non-sensitive` nodig.
* **verbind met een externe de diensttoestemming:** uiteindelijk, moet het elektrische toestel met Workfront API verbinden, die de backbone van de stop-in waarde is. De Workfront API is een service buiten Google, dus de plug-in heeft de `Connect to an external service permission` nodig om de plug-in te laten werken.

Voor meer informatie over de toewijding van Adobe Workfront aan klantenprivacy, zie {het Bericht van de Privacy van 0} Workfront [&#128279;](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

Voor meer informatie, zie [ het Beleid van de Gegevens van de Gebruiker van de Diensten van Google API ](https://developers.google.com/terms/api-services-user-data-policy).
