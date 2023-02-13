---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Voorbereiden om aan boord van uw organisatie te gaan naar de Adobe Admin Console
description: Omdat Adobe Workfront een Adobe-product is, kunt u het openen via de Adobe Admin Console. Zo kunt u Workfront samen met andere Adobe-accounts en -producten voor uw gebruikers centraal beheren.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Voorbereiden om aan boord van uw organisatie te gaan naar de Adobe Admin Console

Omdat Adobe Workfront een Adobe-product is, kunt u het openen via de Adobe Admin Console. Zo kunt u Workfront samen met andere Adobe-accounts en -producten voor uw gebruikers centraal beheren.

Alle Workfront-klanten worden uiteindelijk naar de Adobe Admin Console verplaatst. Nadat uw organisatie naar de Adobe Admin Console is gegaan, wordt de Workfront-verificatie beheerd door de Adobe Admin Console. Door deze stap sneller voor te bereiden en uit te voeren, wordt de basis gelegd voor efficiëntie in het werkbeheer en wordt uw organisatie geplaatst voor snellere innovatie in de toekomst

Voor een overzicht van de Adobe Admin Console raadpleegt u [Overzicht van Admin Console](https://helpx.adobe.com/nl/enterprise/using/admin-console.html).

## Controlelijst voor migratie

Om ervoor te zorgen dat uw organisatie naar de Adobe Admin Console kan migreren, moet u de volgende acties uitvoeren

1. Geef de gewenste Adobe Admin Console op waaraan u Workfront wilt toevoegen.

   * Als uw organisatie geen bestaande Adobe Admin Console heeft of als u geen bestaande Adobe Admin Console wilt gebruiken, kan de Steun van Workfront u bij het creëren van een nieuwe helpen.

   * Als u meerdere Adobe-Admin Consoles hebt en u niet zeker weet welke het meest geschikt is om Adobe Workfront toe te voegen aan, neemt u contact op met de ondersteuning van Workfront.

1. Bevestig met Workfront-ondersteuning dat je een bestaande Adobe Admin Console wilt gebruiken of een nieuwe wilt maken.

1. Stel identiteitsbeheer in op de Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Ben bereid om met de Steun van Workfront en uw team van IT betreffende authentificatievoorkeur zoals Enige Sign-On (SSO) of niet-SSO te spreken.

   Zie de Identity Management-sectie van de Implementatiegids voor de Adobe Admin Console (https://helpx.adobe.com/enterprise/using/deployment-planning.html) voor instructies.

1. (Voorwaardelijk) Als u Single Sign-On gebruikt, sluit u de nieuwe Adobe Admin Console aan op uw bestaande SSO-provider.

   Zie voor meer informatie en instructies [Identiteit instellen](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >Als uw organisatie Single Sign-On niet gebruikt, ontvangen gebruikers die naar de Adobe Admin Console zijn gemigreerd een e-mail om hun account en wachtwoord te maken.

1. Zorg ervoor dat de e-mailadressen van de gebruiker klaar zijn voor migratie:

   1. Dubbele e-mails verwijderen uit Workfront

      Zie E-mailadressen van bestaande gebruikers in uw Workfront-exemplaar bijwerken om dubbele gebruikers te voorkomen voor instructies.

      Als uw organisatie een dubbel e-mailadres heeft, wordt de gebruiker vertegenwoordigd door het e-mailadres met het meest recente `lastLoginDate` wordt verplaatst naar de Adobe Admin Console-organisatie. Andere gebruikers met dat e-mailadres worden gedeactiveerd.

      >[!NOTE]
      >
      >Omdat slechts één gebruiker met een bepaald e-mailadres op een bepaald tijdstip actief kan zijn, moet u eerst de huidige actieve gebruiker deactiveren voordat u de gedeactiveerde gebruiker activeert als u een andere gebruiker met hetzelfde e-mailadres als een momenteel actieve gebruiker wilt activeren.

   2. (Voorwaardelijk) Als u de integratie van de douaneAPI gebruikt, bevestig die gebruikers een geldig e-mailadres hebben dat zij kunnen toegang hebben.

   3. (Optioneel) We raden u aan gebruikers die geen toegang meer nodig hebben tot Workfront, te deactiveren, zodat ze niet aan de Adobe Admin Console worden toegevoegd.
   >[!IMPORTANT]
   >
   >Deze acties met betrekking tot e-mails van gebruikers moeten zijn voltooid voordat uw organisatie naar de Adobe Admin Console gaat.

1. (Optioneel) Werk alle aangepaste integratie bij om OAuth2 te gebruiken.

   Voor instructies over het instellen van OAuth2-integratie raadpleegt u [OAuth2-toepassingen maken voor Workfront-integratie](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   Het maken van OAuth2-integratie is alleen beschikbaar in de nieuwe Workfront-ervaring.

   >[!NOTE]
   >
   >Deze stap is optioneel, maar wordt sterk aanbevolen, omdat andere vormen van API-verificatie en -autorisatie in de toekomst afgekeurd zullen worden.

Nadat uw Adobe Admin Console met Workfront is geconfigureerd, kunt u deze gebruiken om uw gebruikers te beheren.

Zie voor meer informatie [Gebruikers beheren in de Adobe Admin Console](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Voor een lijst met andere acties die verschillend zijn op basis van het feit of uw organisatie al dan niet is aangemeld bij de Adobe Admin Console, raadpleegt u [Op Platform gebaseerde verschillen in beheer (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
