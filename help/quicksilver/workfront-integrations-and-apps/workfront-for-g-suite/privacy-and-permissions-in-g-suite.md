---
product-area: workfront-integrations
keywords: google,doc,document,sheet,slide
navigation-topic: workfront-for-g-suite
title: Privacy en rechten in Workfront for G Suite
description: Privacy en rechten in Workfront for G Suite
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: a156092bf2b6cca70d09b76a65d755fbe05ec8da
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# Privacy en rechten in Workfront for G Suite

Omdat de privacy van klanten belangrijk is, slaat Adobe Workfront geen identificerende klantgegevens op of verzamelt deze die het resultaat zijn van toestemming van derden voor een Google-plug-in. Het gebruik en de overdracht van informatie die Workfront for G Suite van Google API&#39;s heeft ontvangen naar een andere app, voldoen aan het gebruikersgegevensbeleid van Google API Services, inclusief de gebruiksvereisten.

De volgende machtigingen zijn vereist, zodat de Workfront for G Suite-plug-in de maximale waarde kan leveren:

* **Uw e-mailberichten weergeven wanneer de invoegtoepassing wordt uitgevoerd**: Met de insteekmodule Workfront for G Suite kunnen gebruikers ontelbare uren dubbel werk besparen door e-mails om te zetten in nieuwe taken in Workfront en de titel en beschrijving van de taak automatisch te vullen met het onderwerp en de tekst van de e-mail. Met de insteekmodule kunt u uw e-mails als nieuwe opmerkingen op Workfront plaatsen. De insteekmodule moet uw e-mailberichten weergeven wanneer de invoegtoepassing wordt uitgevoerd om deze waarde te kunnen leveren.
* **Als Gmail-invoegtoepassing/niet-gevoelig uitvoeren**: De Workfront for G Suite-invoegtoepassing heeft machtigingen nodig om te kunnen functioneren in de Gmail-omgeving. Voor de insteekmodule is een Gmail-omgeving vereist. Hiervoor is de `Run as a Gmail add-on / non-sensitive` toestemming.
* **Metagegevens van uw e-mailbericht weergeven wanneer de invoegtoepassing wordt uitgevoerd**: Om de workflows te verbeteren, bevestigt de Workfront for G Suite-plug-in of een e-mailbericht een Workfront-melding is en geeft het type Workfront-melding aan (nieuwe werkaanvraag, goedkeuringsaanvraag, nieuwe opmerking enz.). Voor de insteekmodule is de `View your email message metadata when the add-on is running` toestemming om deze waarde te leveren.
* **Plug-in moet worden uitgevoerd als invoegtoepassing voor kalender/niet-gevoelig**: De insteekmodule Workfront for G Suite maakt verbinding met uw agenda, zodat u kunt visualiseren hoe taken van invloed zijn op schema&#39;s. De plug-in heeft de `Run as a Calendar add-on / non-sensitive` toestemming om dit te doen.
* **Verbinden met een externe de diensttoestemming:** Uiteindelijk moet de insteekmodule verbinding maken met de Workfront API, de ruggengraat van de waarde van de insteekmodule. De Workfront API is een externe service van Google, dus voor de insteekmodule is het `Connect to an external service permission` om de insteekmodule te laten werken.

Voor meer informatie over de toewijding van Adobe Workfront aan de privacy van klanten, zie [Privacykennisgeving voor Workfront](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

Zie voor meer informatie [Gebruikersgegevensbeleid Google API Services](https://developers.google.com/terms/api-services-user-data-policy).
