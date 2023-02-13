---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Machtigingsniveaus voor [!DNL Workfront] voor Outlook
description: De [!DNL Workfront for Outlook] toe:voegen-binnen vereist gelezen/schrijven brievenbustoegang. De [!DNL Workfront for Outlook] de integratie vereist de hoogste niveautoestemmingen omdat het de functionaliteit heeft om e-mailgehechtheid van de server van de Uitwisseling van Vooruitzichten te downloaden en hen te uploaden aan [!DNL Workfront], wanneer de gebruiker een aanvraag indient via een e-mail met bijlagen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 177bf9271dca0310653b73b9100607a82290c326
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Machtigingsniveaus voor [!DNL Workfront for Outlook]

[!DNL Workfront for Outlook] vereist het hoogste van de vier niveaus van toestemmingen die in worden toegestaan [!DNL Outlook] invoegtoepassingen.

Voor meer informatie over machtigingen in [!DNL Outlook] add-ins, zie [Privacy, rechten en beveiliging voor [!DNL Outlook] add-ins](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) in de [!DNL Microsoft] documentatie.

De [!DNL Workfront for Outlook] add-in vereist lees-schrijf brievenbustoegang (`ReadWriteMailbox`), het hoogste machtigingsbereik.
De [!DNL Workfront for Outlook] voor integratie zijn machtigingen op het hoogste niveau vereist, omdat deze de functionaliteit heeft om e-mailbijlagen te downloaden van de [!DNL Outlook] server uitwisselen en uploaden naar [!DNL Workfront], wanneer de gebruiker een aanvraag indient via een e-mail met bijlagen. Deze functionaliteit werkt alleen als: [!DNL Workfront for Outlook] gebruikt de functie `mailbox.getCallbackTokenAsync()` van [!DNL Office] Voeg JavaScript API toe om het token op te halen en gebruik dat om e-mailbijlagen te downloaden van de Exchange-server. De enige toestemming die het gebruik van die functie toestaat is `ReadWriteMailbox`. Zie voor meer informatie [Privacy, toestemmingen en veiligheid voor toe:voegen-ins van Vooruitzichten](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) in de documentatie van Microsoft.

De [!DNL Workfront for Outlook] add-in vereist ook `ReadWriteItem` machtiging (opgenomen in `ReadWriteMailbox`), dat wordt gebruikt voor het lezen van de e-mailtekst en het lezen/bijwerken van e-mailmetagegevens:

* Hoofdtekst van e-mail lezen:

   [!DNL Workfront for Outlook] leest het e-maillichaam wanneer een gebruiker het verzoek indient of het e-maillichaam als update verzendt naar [!DNL Adobe Workfront] Object.
* E-mailmetagegevens lezen/bijwerken:

   [!DNL Workfront for Outlook] werkt e-mailkoppen bij wanneer een gebruiker een aanvraag via e-mail verzendt. Hiermee slaat u gegevens op over de verzonden [!DNL Adobe Workfront] -object, zodat de volgende keer dat de gebruiker de invoegtoepassing voor dezelfde e-mail opent, de informatie over eerdere acties met die e-mail wordt weergegeven.

[!DNL Workfront for Outlook] Toegang tot de Brievenbus van een gebruiker slechts wanneer de gebruiker een actie binnen toe:voegen-op uitvoert. Deze heeft geen achtergrondfunctionaliteit. Workfront for Outlook opent alleen de mailbox van de gebruiker in het volgende scenario:

* De gebruiker probeert een aanvraag in te dienen, een taak te maken of een e-mail te verzenden als update van [!DNL Workfront for Outlook] (De invoegtoepassing openen en een handeling selecteren)
   * [!DNL Workfront for Outlook] leest het e-maillichaam om in de vorm binnen toe:voegen-binnen te bevolken.
   * [!DNL Workfront for Outlook] leest e-mailmeta-gegevens om informatie over toe:voegen-binnen over de vorige acties te tonen die in toe:voegen-binnen met zelfde e-mail worden gedaan.
* Wanneer een gebruiker een verzoek indient, een taak creeert of een e-mail als update verzendt van [!DNL Workfront for Outlook] (klik op de knop [!UICONTROL submit] op de invoegtoepassing):
   * [!DNL Workfront for Outlook] leest de e-mailtekst die u naar Workfront wilt verzenden als een aanvraagbeschrijving of een opmerking.
   * [!DNL Workfront for Outlook] werkt de e-mailmeta-gegevens bij om informatie over de voorgelegde verzoeken of het bijgewerkte voorwerp op te slaan.
   * [!DNL Workfront for Outlook] Hiermee downloadt u e-mailbijlagen van de Exchange-server om deze te uploaden naar verzonden aanvragen, gemaakte taken of bijgewerkte objecten.
