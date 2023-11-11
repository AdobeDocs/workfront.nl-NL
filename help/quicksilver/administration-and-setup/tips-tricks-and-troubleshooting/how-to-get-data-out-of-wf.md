---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Historische gegevens exporteren uit Adobe Workfront: Pros en cons'
description: In dit artikel worden de voor- en nadelen beschreven van vier opties die u kunt gebruiken om historische gegevens uit Workfront te exporteren.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

# Historische gegevens exporteren uit [!DNL Adobe Workfron]t: Pros en cons

In dit artikel worden de voor- en nadelen uitgelegd van vier opties waarmee u historische gegevens kunt exporteren [!DNL Workfront].

## Gebruik één van onze partners

[!DNL AtAppStore], [!DNL Workfront] -gecertificeerde partner, beschikt over een gebruiksvriendelijke app waarmee u uw gegevens kunt downloaden. Deze app bevat ook een viewer waarmee u uw gegevens gemakkelijk kunt bekijken.

* **Pros:** Al uw [!DNL Workfront] objecten worden geëxporteerd, inclusief de aangepaste velden. De interface van de Viewer is eenvoudig te gebruiken en te lezen en kan gemakkelijk worden geïmporteerd in een [!DNL MS Access] Database.

* **Cons:** Documenten worden niet geëxporteerd. U moet de bestanden afzonderlijk downloaden. Ga voor meer informatie naar [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx.](https://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## Verzoek om een [!DNL Postgres] data dump file van ons Database team

Uw Account Executive kan een verzoek indienen bij ons databaseteam om een databasedumpbestand (.dmp [!DNL Postgres] ) met uw gegevens. Een extra aanvraag gaat naar ons AOS-team om alle opgeslagen documenten op te halen.

* **Pros**: U kunt de volledige gegevens laden, inclusief aangepaste velden, en documenten die in het systeem zijn opgeslagen.

* **Cons**: Het databasebestand is moeilijk leesbaar: u kunt dit bestand alleen lezen als u het uploadt naar een [!DNL Postgres] de relaties tussen de tabellen te herstellen. De documenten worden opgeslagen op een aparte bestandsserver en moeten door het AOS-team apart worden uitgepakt. Hierbij, is er geen organisatie aan de documenten, en zij worden allen van verwijzingen voorzien door hun GUID.
* **Kosten**: Er zijn kosten verbonden aan deze download, afhankelijk van hoe lang het team duurt om het dossier tot stand te brengen. Raadpleeg uw AE/CAE voor meer informatie of om dit proces op gang te brengen.

## Exporteren via [!UICONTROL Kick-Starts]

Of u nu externe consultinguren hebt of niet, u kunt een van onze consultants gebruiken om uw gegevens te exporteren in de vorm van rapporten of [!UICONTROL kick-starts]of u kunt deze rapporten zelf uitvoeren:

* **Pros**: De rapporten zijn gemakkelijk te lezen en kunnen in een verscheidenheid van toepassingen worden ingevoerd; zij kunnen worden aangepast om het even welke groeperingen en meningen te omvatten u zou willen.

* **Cons**: Documenten moeten afzonderlijk worden gedownload.

* **Kosten**: Het is gratis als u de rapporten zelf kunt uitvoeren (u hebt alleen een aanmeldingsgegevens voor systeembeheer nodig) of als u de resterende externe consultinguren kunt gebruiken. Neem contact op met uw AE/CAE als u hiervoor advies op afstand wilt aanschaffen.

  Voor meer informatie over het gebruiken van Kick-Begarts om gegevens uit te voeren, zie [Gegevens exporteren uit [!DNL Adobe Workfront] via [!UICONTROL Kick-Starts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Onze open API gebruiken

Als u beschikt over de juiste bronnen in uw organisatie, kunt u een aangepaste API maken om al uw gegevens op te halen uit Workfront:

* **Pros**: U hebt controle over de uitvoer van het systeem.

* **Cons**: De tijd wordt aan uw kant besteed, en u zult middelen aan code API moeten vinden en de uitvoer uitvoeren.

* **Kosten**: Intern aan uw organisatie.
