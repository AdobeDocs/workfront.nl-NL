---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: De niveaus van toestemmingen voor  [!DNL Workfront]  voor Vooruitzichten
description: ' [!DNL Workfront for Outlook]  toe:voegen-binnen vereist gelezen/schrijf brievenbustoegang. De  [!DNL Workfront for Outlook]  integratie vereist de hoogste niveautoestemmingen omdat het de functionaliteit heeft om e-mailgehechtheid van de de uitwisselingsserver van Vooruitzichten te downloaden en hen te uploaden aan  [!DNL Workfront], wanneer de gebruiker een Verzoek van e-mail voorlegt die gehechtheid heeft.'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 177bf9271dca0310653b73b9100607a82290c326
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# Machtigingsniveaus voor [!DNL Workfront for Outlook]

[!DNL Workfront for Outlook] vereist de hoogste van de vier machtigingsniveaus die zijn toegestaan in [!DNL Outlook] add-ins.

Voor details betreffende toestemmingen in [!DNL Outlook] toe:voegen-ins, zie [ Privacy, toestemmingen en veiligheid voor  [!DNL Outlook]  toe:voegen-ins ](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) in de [!DNL Microsoft] documentatie.

[!DNL Workfront for Outlook] toe:voegen-binnen vereist lees-schrijf brievenbustoegang (`ReadWriteMailbox`), die het hoogste toestemmingswerkingsgebied is.
Voor de integratie met [!DNL Workfront for Outlook] zijn machtigingen op het hoogste niveau vereist, omdat deze de functionaliteit heeft om e-mailbijlagen te downloaden van de [!DNL Outlook] Exchange-server en deze te uploaden naar [!DNL Workfront] , wanneer de gebruiker een aanvraag indient via een e-mail met bijlagen. Deze functionaliteit werkt alleen als [!DNL Workfront for Outlook] de functie `mailbox.getCallbackTokenAsync()` from [!DNL Office] Add-in JavaScript API gebruikt om het token op te halen en dat te gebruiken om e-mailbijlagen van de Exchange-server te downloaden. De enige toestemming die het gebruik van die functie toestaat is `ReadWriteMailbox`. Voor meer informatie, zie [ Privacy, toestemmingen en veiligheid voor toe:voegen-ins van Vooruitzichten ](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) in de documentatie van Microsoft.

Voor de [!DNL Workfront for Outlook] add-in is ook `ReadWriteItem` permission (opgenomen in `ReadWriteMailbox` ) vereist, waarmee de hoofdtekst van de e-mail wordt gelezen en e-mailmetagegevens worden gelezen/bijgewerkt:

* Hoofdtekst van e-mail lezen:

  [!DNL Workfront for Outlook] leest de hoofdtekst van de e-mail wanneer een gebruiker de aanvraag indient of de hoofdtekst van de e-mail als een update naar [!DNL Adobe Workfront] Object verzendt.
* E-mailmetagegevens lezen/bijwerken:

  [!DNL Workfront for Outlook] werkt e-mailheaders bij wanneer een gebruiker een aanvraag via e-mail verzendt. Dit gebeurt om informatie op te slaan over het verzonden [!DNL Adobe Workfront] -object, zodat de volgende keer dat de gebruiker de invoegtoepassing voor dezelfde e-mail opent, de informatie over eerdere acties met die e-mail wordt weergegeven.

[!DNL Workfront for Outlook] heeft slechts toegang tot de Brievenbus van een gebruiker wanneer de gebruiker een actie binnen toe:voegen-op uitvoert. Deze heeft geen achtergrondfunctionaliteit. Workfront for Outlook opent alleen de mailbox van de gebruiker in het volgende scenario:

* De gebruiker probeert een aanvraag in te dienen, een taak te maken of een e-mail te verzenden als een update vanuit [!DNL Workfront for Outlook] (De invoegtoepassing openen en een actie selecteren)
   * [!DNL Workfront for Outlook] leest de hoofdtekst van de e-mail om het formulier in de invoegtoepassing in te vullen.
   * [!DNL Workfront for Outlook] leest e-mailmeta-gegevens om informatie over toe:voegen-binnen over de vorige acties te tonen die in toe:voegen-binnen met zelfde e-mail worden gedaan.
* Wanneer een gebruiker een aanvraag indient, een taak maakt of een e-mail verzendt als een update vanuit [!DNL Workfront for Outlook] (klik op de knop [!UICONTROL submit] op de invoegtoepassing):
   * [!DNL Workfront for Outlook] leest de hoofdtekst van de e-mail om deze naar Workfront te verzenden als een aanvraagbeschrijving of een opmerking.
   * [!DNL Workfront for Outlook] werkt de e-mailmetagegevens bij en slaat informatie op over de verzonden aanvragen of het bijgewerkte object.
   * [!DNL Workfront for Outlook] downloadt e-mailbijlagen van de Exchange-server om deze te uploaden naar verzonden aanvragen, gemaakte taken of bijgewerkte objecten.
