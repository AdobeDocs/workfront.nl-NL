---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Integreren [!DNL Workfront Proof] met Basecamp Classic
description: Als u [!DNL Basecamp] voor projectbeheer kunt u uw projectteam rijkere revisie- en goedkeuringsinstrumenten bieden met behulp van [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 0%

---

# Integreren [!DNL Workfront Proof] with [!DNL Basecamp Classic]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Als u [!DNL Basecamp] voor projectbeheer kunt u uw projectteam rijkere revisie- en goedkeuringsinstrumenten bieden met behulp van [!DNL Workfront Proof].

## De [!DNL Basecamp] Integratie met [!DNL Workfront]

Integreren met [!DNL Basecamp] staat gebruikers toe om proeven te bekijken, te herzien en goed te keuren allen binnen [!DNL Basecamp]. Gebruikers kunnen proefdrukken verzenden naar uw [!DNL Workfront Proof] en deze aan te sluiten op uw [!DNL Basecamp] project. Uw revisoren kunnen [Beslissen op een bewijs in de professionele drukker](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) via [!DNL Basecamp]met de mini-proefdruk die is ingesloten in uw Basecamp-bericht.

Indien geïntegreerd met [!DNL Workfront Proof], [!DNL Basecamp] Hiermee kunnen gebruikers het volgende doen met proefdrukken:

* Gebruikers kunnen proefdrukken controleren en goedkeuren binnen [!DNL Basecamp Classic].
* Gebruikers beschikken direct over revisiegereedschappen.
* Projectbeoordelingsteams ontvangen een bericht in [!DNL Basecamp] met een mini-bewijs voor controle en goedkeuring.
* Gebruikers kunnen overschakelen op een proefdruk van een volledige pagina voor controle en goedkeuring.
* Gebruikers kunnen opmerkingen en markeringen toevoegen aan proefdrukken op zowel miniformaat als op volledige grootte.

   >[!NOTE]
   >
   >Nadat een opmerking is beantwoord, kan deze niet meer worden bewerkt of verwijderd.

* Revisoren kunnen reageren op de opmerkingen en markeringen die door andere revisoren zijn gemaakt.
* Gebruikers worden gewaarschuwd wanneer een nieuwe versie van het bewijs beschikbaar is.
* Gebruikers die niet [!DNL Workfront Proof] gebruikers kunnen aan een proef werken in [!DNL Basecamp].

De integratie van [!DNL Workfront Proof] with [!DNL Basecamp] moeten op twee niveaus worden ingesteld:

* Configureren [!DNL Basecamp] in [Accountinstellingen:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Dit maakt de integratie met Basecamp mogelijk voor uw hele organisatie.
* Zie voor meer informatie [Het inschakelen van de [!DNL Basecamp] Integratie met [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).
* Configureren [!DNL Basecamp] in [Persoonlijke instellingen](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Hierdoor kunnen makers en eigenaars van proofings verbinding maken met hun persoonlijke [!DNL Basecamp] account en autoriseren [!DNL Workfront Proof] toegang. Zie voor meer informatie [Persoonlijke instellingen configureren](#configuring-personal-settings).

U kunt [!DNL Workfront] met [!DNL Basecamp] of [!DNL Basecamp Classic]. Elke versie van [!DNL Basecamp] gebruikt een andere API en vereist daarom verschillende configuratieprocedures.

Voor informatie over het configureren [!DNL Basecamp Classic], zie [Het inschakelen van de [!DNL Basecamp] Integratie met [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) in dit artikel.

Voor informatie over het configureren [!DNL Basecamp], zie [Integreren [!DNL Workfront Proof] with [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md).

## Het inschakelen van de [!DNL Basecamp] Integratie met [!DNL Workfront Proof]

Als [Profielen met proefmachtigingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) of [Profielen met proefmachtigingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), kunt u Basecamp-integratie instellen voor de gehele account in uw [Accountinstellingen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Ga naar [Accountinstellingen.](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)
1. Open de **[!UICONTROL Integrations]** tab (1).
1. Als u de integratie met Basecamp wilt inschakelen, klikt u op **[!UICONTROL Enable]** (2)
1. Controleren of [!DNL Basecamp Classic] is de versie u met (3) integreert.
1. (Voorwaardelijk) Indien niet [!DNL Basecamp] URL wordt weergegeven (4), klikt u op **[!UICONTROL Edit]** en voer de URL voor uw [!DNL Basecamp] account (zonder de map http://).
1. Klikken **[!UICONTROL Save]** 5.\
   ![Basecamp_account_settings_-_integration.png](assets/basecamp-account-settings---integration-350x192.png)

1. (Optioneel) Controleer uw [!DNL Basecamp] URL in uw browser nadat u zich hebt aangemeld bij uw [!DNL Basecamp Classic] rekening (6).

   ![Basecamp_URL.png](assets/basecamp-url-350x75.png)

   Eenmaal integreren [!DNL Workfront Proof] with [!DNL Basecamp]kunnen uw gebruikers hun persoonlijke instellingen configureren. Voor informatie over het instellen van persoonlijke instellingen raadpleegt u [Persoonlijke instellingen configureren](#configuring-personal-settings).

   Als u niet kunt [!DNL Basecamp] integratie, uw [!DNL Workfront Proof] account-id is mogelijk niet dezelfde als de account-id waarin u gebruikt [!DNL Basecamp].

## Persoonlijke instellingen configureren

Nadat u het programma hebt ingesteld [Accountinstellingen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) voor uw organisatie moet elke auteur die proefdrukken maakt/verzendt, zijn of haar  [persoonlijke instellingen.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

>[!NOTE]
>
>U kunt deze stappen het gemakkelijkst uitvoeren als u beschikt over uw [!DNL Basecamp] sessie geopend in één browservenster en uw [!DNL Workfront Proof] sessie geopend in een ander venster.

* [Uw [!DNL Basecamp] API-token](#retrieving-your-basecamp-api-token)
* [Uw [!DNL Basecamp] API-token voor uw persoonlijke instellingen](#adding-your-basecamp-api-token-to-your-personal-settings)

### Uw [!DNL Basecamp] API-token

Om de integratie op individueel niveau te voltooien [!DNL Workfront Proof], hebben gebruikers hun individuele verificatietoken nodig voor de [!DNL Basecamp] API.

Om uw [!DNL Basecamp] API-token:

1. Aanmelden bij uw [!DNL Basecamp] account.
1. Klikken **[!UICONTROL My Info]** (1) in de rechterbovenhoek van het scherm.\
   De [!UICONTROL My Info] wordt weergegeven.\
   ![Basecamp_Integration_-_Token1.png](assets/basecamp-integration---token1-350x334.png)

1. In de [!UICONTROL Authentication tokens] sectie, klikt u op **[!UICONTROL Show your tokens]** (2) om uw persoonlijke verificatietokens weer te geven.
1. Selecteer **[!UICONTROL Token for feed readers]** of de **[!UICONTROL Basecamp API]** (3), kopieert u de token naar het klembord.

1. Plak uw [!DNL Basecamp] API-token in de [!UICONTROL Token for feed readers] of de [!UICONTROL Basecamp API] doos.\
   ![Basecamp_Integration_-_Token2.png](assets/basecamp-integration---token2-350x178.png)

### Uw [!DNL Basecamp] API-token voor uw persoonlijke instellingen

Als u de opdracht [!DNL Basecamp] API-token in uw [!DNL Workfront Proof] [Persoonlijke instellingen](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings):

1. Ga naar de [[!UICONTROL Integrations] - Gebruikersinstelling](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md) in uw [Persoonlijke instellingen](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) (1)\
   Een beheerder moet eerst de [!DNL Basecamp Classic] integratie zodat u uw persoonlijke instellingen kunt inschakelen. Voor informatie over het instellen van de integratie raadpleegt u [Het inschakelen van de [!DNL Basecamp] Integratie met [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) in dit artikel.

1. In de [!DNL Basecamp] API-token box (2), plakt u de token die u net van uw [!DNL Basecamp] [!UICONTROL My Info] in het veld (3).\
   Voor informatie over het kopiëren van uw [!DNL Basecamp] API-token, zie [Uw [!DNL Basecamp] API-token](#retrieving-your-basecamp-api-token) in dit artikel.

1. Klikken **[!UICONTROL Save]** (4).

![Basecamp_Personal_settings_-_integration.png](assets/basecamp-personal-settings---integration-350x250.png)

Uw [!DNL Workfront Proof] [Persoonlijke instellingen](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) zijn nu geïntegreerd met uw [!DNL Basecamp Classic] account.
