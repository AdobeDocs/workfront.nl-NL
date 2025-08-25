---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Voorbereiden op het aan boord nemen van uw organisatie bij de Adobe Admin Console
description: Omdat Adobe Workfront een Adobe-product is, kunt u het openen via de Adobe Admin Console. Zo kunt u Workfront samen met andere Adobe-accounts en -producten voor uw gebruikers centraal beheren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: a25eb28800ca8bbeeffedb521b3d72c8df71c697
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Voorbereiden om aan boord van uw organisatie te gaan naar de Adobe Admin Console

<!-- Audited: 12/2023 -->

Omdat Adobe Workfront een Adobe-product is, kunt u het openen via de Adobe Admin Console. Zo kunt u Workfront samen met andere Adobe-accounts en -producten voor uw gebruikers centraal beheren.

Alle Workfront-klanten worden uiteindelijk naar de Adobe Admin Console verplaatst. Nadat uw organisatie naar de Adobe Admin Console is gegaan, wordt de Workfront-verificatie beheerd door de Console. Door deze stap sneller voor te bereiden en uit te voeren, wordt de basis gelegd voor efficiëntie in het werkbeheer en wordt uw organisatie geplaatst voor snellere innovatie in de toekomst

Voor een overzicht van Adobe Admin Console, zie [ Overzicht van Admin Console ](https://helpx.adobe.com/nl/enterprise/using/admin-console.html).

## Controlelijst voor migratie

Om ervoor te zorgen dat uw organisatie naar de Adobe Admin Console kan migreren, moet u de volgende acties uitvoeren.

1. Geef de gewenste Adobe Admin Console op waaraan u Workfront wilt toevoegen.

   * Als uw organisatie geen bestaande Adobe Admin Console heeft of als u geen bestaande Adobe Admin Console wilt gebruiken, kan de Steun van Workfront u bij het creëren van een nieuwe helpen.

   * Neem contact op met de ondersteuning van Workfront als u meerdere Adobe-beheerconsoles hebt en u niet zeker weet aan welke consoles Workfront het meest geschikt is om toe te voegen.

1. Bevestig met Workfront-ondersteuning dat je een bestaande Adobe Admin Console wilt gebruiken of een nieuwe wilt maken.

1. Stel identiteitsbeheer in op de Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Ben bereid om met de Steun van Workfront en uw team van IT betreffende authentificatievoorkeur zoals Enige Sign-On (SSO) of niet-SSO te spreken.

   Voor instructies, zie de sectie van Identity Management van de [ Gids van de Plaatsing voor Adobe Admin Console ](https://helpx.adobe.com/enterprise/using/deployment-planning.html).

1. (Voorwaardelijk) Als u Single Sign-On gebruikt, sluit u de nieuwe Adobe Admin Console aan op uw bestaande SSO-provider.

   Voor meer informatie en instructies, zie [ identiteit van de Opstelling ](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >Als uw organisatie Single Sign-On niet gebruikt, ontvangen gebruikers die naar de Adobe Admin Console zijn gemigreerd een e-mail om hun account en wachtwoord te maken.

1. Zorg ervoor dat de e-mailadressen van de gebruiker klaar zijn voor migratie:

   1. Dubbele e-mails verwijderen uit Workfront.

      Voor instructies, zie [ de e-mailadressen van de Update van bestaande gebruikers in uw instantie van Workfront ](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md#update-email-addresses-of-existing-users-in-your-workfront-instance) in [ verhinderen dubbele gebruikers ](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md).

      Als uw organisatie een dubbel e-mailadres heeft, wordt de gebruiker die wordt vertegenwoordigd door het e-mailadres met de meest recente `lastLoginDate` , verplaatst naar de Adobe Admin Console-organisatie. Andere gebruikers met dat e-mailadres worden gedeactiveerd.

      >[!NOTE]
      >
      >Omdat slechts één gebruiker met een bepaald e-mailadres op een bepaald ogenblik actief kan zijn, als u een andere gebruiker met het zelfde e-mailadres moet activeren zoals een momenteel actieve gebruiker, moet u de momenteel actieve gebruiker eerst deactiveren alvorens de gedeactiveerde gebruiker te activeren.

   1. (Voorwaardelijk) Als u de integratie van de douaneAPI gebruikt, bevestig die gebruikers een geldig e-mailadres hebben dat zij kunnen toegang hebben.

   1. (Optioneel) We raden u aan gebruikers die geen toegang meer nodig hebben tot Workfront, te deactiveren, zodat ze niet aan de Adobe Admin Console worden toegevoegd.

   >[!IMPORTANT]
   >
   >Deze acties met betrekking tot e-mails van gebruikers moeten zijn voltooid voordat uw organisatie naar de Adobe Admin Console gaat.

1. (Optioneel) Werk alle aangepaste integratie bij om OAuth2 te gebruiken.

   Voor instructies bij vestiging integratie OAuth2, zie [ tot toepassingen OAuth2 voor de integratie van Workfront ](../../administration-and-setup/configure-integrations/create-oauth-application.md) leiden.

   >[!NOTE]
   >
   >Deze stap is optioneel, maar wordt sterk aanbevolen, omdat andere vormen van API-verificatie en -autorisatie in de toekomst afgekeurd zullen worden.

Nadat uw Adobe Admin Console is geconfigureerd met Workfront, kunt u deze gebruiken om uw Workfront-systeembeheerders te maken.

Voor meer informatie, zie [ gebruikers in Adobe Admin Console ](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md) leiden.

Voor een lijst van andere acties die verschillend zijn gebaseerd op of uw organisatie aan Adobe Admin Console is genegeerd, zie [ Op platform-gebaseerde beleidsverschillen (Adobe Workfront/Adobe Bedrijfs Platform) ](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
