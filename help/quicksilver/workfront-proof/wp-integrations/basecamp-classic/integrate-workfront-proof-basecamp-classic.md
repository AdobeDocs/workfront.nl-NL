---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Integreer  [!DNL Workfront Proof]  met Klassiek Basecamp
description: Als u  [!DNL Basecamp]  voor projectbeheer gebruikt kunt u uw overzicht en goedkeuringshulpmiddelen van het projectteam aanbieden rijker gebruikend  [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 0%

---

# [!DNL Workfront Proof] integreren met [!DNL Basecamp Classic]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [&#x200B; het Bewijzen &#x200B;](../../../review-and-approve-work/proofing/proofing.md).

Als u [!DNL Basecamp] gebruikt voor projectbeheer, kunt u met [!DNL Workfront Proof] de uitgebreidere revisie- en goedkeuringsgereedschappen voor uw projectteam bieden.

## De [!DNL Basecamp] integratie met [!DNL Workfront]

Dankzij de integratie met [!DNL Basecamp] kunnen gebruikers proefdrukken weergeven, bekijken en goedkeuren in [!DNL Basecamp] . Gebruikers kunnen proefdrukken indienen bij uw [!DNL Workfront Proof] -account en deze verbinden met uw [!DNL Basecamp] -project. Uw recensenten kunnen en maken [&#x200B; een besluit over een proef in de het proeven kijker &#x200B;](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) via [!DNL Basecamp] nemen, gebruikend de mini proef ingebed in uw bericht Basecamp.

Wanneer [!DNL Workfront Proof] is geïntegreerd, kunnen gebruikers in [!DNL Basecamp] het volgende doen met proefdrukken:

* Gebruikers kunnen proefdrukken controleren en goedkeuren binnen [!DNL Basecamp Classic] .
* Gebruikers beschikken direct over revisiegereedschappen.
* Projectbeoordelingsteams ontvangen een bericht in [!DNL Basecamp] met een mini-proefdruk voor revisie en goedkeuring.
* Gebruikers kunnen overschakelen op een proefdruk van een volledige pagina voor controle en goedkeuring.
* Gebruikers kunnen opmerkingen en markeringen toevoegen aan proefdrukken op miniformaat en op volledige grootte.

  >[!NOTE]
  >
  >Nadat een opmerking is beantwoord, kan deze niet meer worden bewerkt of verwijderd.

* Revisoren kunnen reageren op de opmerkingen en markeringen die door andere revisoren zijn gemaakt.
* Gebruikers worden gewaarschuwd wanneer een nieuwe versie van het bewijs beschikbaar is.
* Gebruikers die geen [!DNL Workfront Proof] -gebruikers zijn, kunnen in [!DNL Basecamp] aan een proefdruk werken.

De integratie van [!DNL Workfront Proof] met [!DNL Basecamp] moet op twee niveaus worden ingesteld:

* Vorm [!DNL Basecamp] in [&#x200B; montages van de Rekening:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) dit laat de integratie Basecamp voor uw gehele organisatie toe.
* Voor meer informatie, zie [&#x200B; Toelatend de  [!DNL Basecamp]  Integratie met  [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).
* Vorm [!DNL Basecamp] in [&#x200B; Persoonlijke montages &#x200B;](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Dit laat proefscheppers en eigenaars toe om met hun persoonlijke [!DNL Basecamp] rekening te verbinden en [!DNL Workfront Proof] toegang te machtigen. Voor meer informatie, zie [&#x200B; Vormend Persoonlijke Montages &#x200B;](#configuring-personal-settings).

U kunt [!DNL Workfront] integreren met [!DNL Basecamp] of [!DNL Basecamp Classic] . Elke versie van [!DNL Basecamp] gebruikt een andere API en vereist daarom verschillende configuratieprocedures.

Voor informatie bij het vormen [!DNL Basecamp Classic], zie [&#x200B; toelatend de  [!DNL Basecamp]  Integratie met  [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) in dit artikel.

Voor informatie bij het vormen [!DNL Basecamp], zie [&#x200B;  [!DNL Workfront Proof]  met  [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md) integreren.

## [!DNL Basecamp] Integratie met [!DNL Workfront Proof] inschakelen

Als Profielen van de Toestemmingen van de a [&#x200B; Bewijs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) of [&#x200B; Profielen van de Toestemmingen van de Bewijs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), kunt u de integratie van Basecamp voor de volledige rekening in uw [&#x200B; montages van de Rekening &#x200B;](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) opstelling.

1. Ga naar [&#x200B; montages van de Rekening.](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)
1. Open de tab **[!UICONTROL Integrations]** (1).
1. Klik op **[!UICONTROL Enable]** (2) om de integratie met het basisstempel in te schakelen.
1. Controleer of [!DNL Basecamp Classic] de versie is waarmee u wilt integreren (3).
1. (Voorwaardelijk) Als er geen [!DNL Basecamp] URL wordt weergegeven (4), klikt u op **[!UICONTROL Edit]** en voert u de URL voor uw [!DNL Basecamp] -account in (zonder de map http://).
1. Klik op **[!UICONTROL Save]** (5).\
   ![&#x200B; Basecamp_account_settings_-_integration.png &#x200B;](assets/basecamp-account-settings---integration-350x192.png)

1. (Optioneel) Controleer de [!DNL Basecamp] URL in uw browser nadat u zich hebt aangemeld bij uw [!DNL Basecamp Classic] -account (6).

   ![&#x200B; Basecamp_URL.png &#x200B;](assets/basecamp-url-350x75.png)

   Nadat u [!DNL Workfront Proof] met [!DNL Basecamp] hebt geïntegreerd, kunnen uw gebruikers hun persoonlijke instellingen configureren. Voor informatie bij vestiging persoonlijke montages, zie [&#x200B; het Vormen Persoonlijke Montages &#x200B;](#configuring-personal-settings).

   Als u [!DNL Basecamp] -integratie niet kunt inschakelen, is de [!DNL Workfront Proof] -account-id mogelijk niet dezelfde als de account-id die u gebruikt in [!DNL Basecamp] .

## Persoonlijke instellingen configureren

Nadat u opstelling [&#x200B; de montages van de Rekening &#x200B;](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) voor uw Organisatie, elk van uw auteurs die creeert/voorlegt zouden hun [&#x200B; persoonlijke montages moeten plaatsen.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

>[!NOTE]
>
>U kunt deze stappen het gemakkelijkst uitvoeren als u de [!DNL Basecamp] -sessie hebt geopend in het ene browservenster en de [!DNL Workfront Proof] -sessie is geopend in een ander venster.

* [Het terugwinnen van Uw  [!DNL Basecamp]  API Token](#retrieving-your-basecamp-api-token)
* [Het toevoegen van Uw  [!DNL Basecamp]  API teken aan Uw Persoonlijke Montages](#adding-your-basecamp-api-token-to-your-personal-settings)

### Uw API-token [!DNL Basecamp] ophalen

Gebruikers hebben hun individuele verificatietoken voor de [!DNL Basecamp] API nodig om de integratie op het individuele niveau in [!DNL Workfront Proof] te voltooien.

U kunt als volgt uw API-token van [!DNL Basecamp] ophalen:

1. Meld u aan bij uw [!DNL Basecamp] -account.
1. Klik op **[!UICONTROL My Info]** (1) in de rechterbovenhoek van het scherm.\
   De pagina [!UICONTROL My Info] wordt weergegeven.\
   ![&#x200B; Basecamp_Integration_-_Token1.png &#x200B;](assets/basecamp-integration---token1-350x334.png)

1. Klik in de sectie [!UICONTROL Authentication tokens] op **[!UICONTROL Show your tokens]** (2) om uw persoonlijke verificatietokens weer te geven.
1. Selecteer **[!UICONTROL Token for feed readers]** of **[!UICONTROL Basecamp API]** (3), dan kopieer het teken aan uw klembord.

1. Plak de API-token [!DNL Basecamp] in het vak [!UICONTROL Token for feed readers] of [!UICONTROL Basecamp API] .\
   ![&#x200B; Basecamp_Integration_-_Token2.png &#x200B;](assets/basecamp-integration---token2-350x178.png)

### Uw [!DNL Basecamp] API-token toevoegen aan uw persoonlijke instellingen

Om het [!DNL Basecamp] API teken in uw [!DNL Workfront Proof] [&#x200B; Persoonlijke montages &#x200B;](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) te kleven:

1. Ga naar [[!UICONTROL Integrations] - de Opstelling van de Gebruiker &#x200B;](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md) in uw [&#x200B; Persoonlijke montages &#x200B;](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) (1).\
   Een beheerder moet eerst de [!DNL Basecamp Classic] -integratie inschakelen voordat u uw persoonlijke instellingen kunt inschakelen. Voor informatie bij vestiging de integratie, zie [&#x200B; toelatend de  [!DNL Basecamp]  Integratie met  [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) in dit artikel.

1. Plak in het tekstvak [!DNL Basecamp] API-token (2) de token die u net van de pagina [!DNL Basecamp] [!UICONTROL My Info] hebt gekopieerd naar het veld (3).\
   Voor informatie bij het kopiëren van uw [!DNL Basecamp] API teken, zie [&#x200B; het Terugwinnen van Uw  [!DNL Basecamp]  Symbolisch API &#x200B;](#retrieving-your-basecamp-api-token) in dit artikel.

1. Klik op **[!UICONTROL Save]** (4).

![&#x200B; Basecamp_Personal_settings_-_integration.png &#x200B;](assets/basecamp-personal-settings---integration-350x250.png)

Uw [!DNL Workfront Proof] [&#x200B; Persoonlijke montages &#x200B;](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) zijn nu geïntegreerd met uw [!DNL Basecamp Classic] rekening.
