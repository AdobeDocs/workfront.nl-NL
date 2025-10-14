---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: Integreer  [!DNL Workfront Proof]  met  [!DNL Basecamp]
description: Als u  [!DNL Basecamp]  voor projectbeheer gebruikt kunt u uw overzicht en goedkeuringshulpmiddelen van het projectteam aanbieden rijker gebruikend  [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---

# [!DNL Workfront Proof] integreren met [!DNL Basecamp]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [&#x200B; het Bewijzen &#x200B;](../../../review-and-approve-work/proofing/proofing.md).

Als u [!DNL Basecamp] gebruikt voor projectbeheer, kunt u met [!DNL Workfront Proof] de uitgebreidere revisie- en goedkeuringsgereedschappen voor uw projectteam bieden.

## De [!DNL Basecamp] integratie met [!DNL Workfront]

Dankzij de integratie met [!DNL Basecamp] kunnen gebruikers proefdrukken weergeven, bekijken en goedkeuren in [!DNL Basecamp] . Gebruikers kunnen proefdrukken indienen bij uw [!DNL Workfront Proof] -account en deze verbinden met uw [!DNL Basecamp] -project. Uw revisoren kunnen opmerkingen maken en beslissingen nemen via [!DNL Basecamp] en daarbij de mini-proefdruk gebruiken die is ingesloten in uw Basecamp-bericht.

Wanneer [!DNL Workfront Proof] is geïntegreerd, heeft [!DNL Basecamp] de volgende proefdrukfunctionaliteit:

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

* Vorm [!DNL Basecamp] in [&#x200B; montages van de Rekening:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) dit laat de integratie Basecamp voor uw gehele organisatie toe. Voor meer informatie, zie [&#x200B; Toelatend de Integratie Basecamp met  [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).

* Vorm [!DNL Basecamp] in [&#x200B; Persoonlijke montages &#x200B;](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Dit laat proefscheppers en eigenaars toe om met hun persoonlijke rekening van Basecamp te verbinden en [!DNL Workfront Proof] toegang toe te machtigen. Voor meer informatie, zie [&#x200B; Vormend Persoonlijke Montages &#x200B;](#configuring-personal-settings).

U kunt [!DNL Workfront] integreren met [!DNL Basecamp] of [!DNL Basecamp Classic] . Elke versie van [!DNL Basecamp] gebruikt een andere API en vereist daarom verschillende configuratieprocedures.

Voor informatie bij het vormen [!DNL Basecamp Classic], zie [&#x200B; Integrerend  [!DNL Workfront Proof]  met  [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## [!DNL Basecamp] Integratie met [!DNL Workfront Proof] inschakelen

Als Profielen van de Toestemmingen van de a [&#x200B; Bewijs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) of [&#x200B; Profielen van de Toestemmingen van de Bewijs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), kunt u opstelling de [!DNL Basecamp] integratie voor de volledige rekening in uw [&#x200B; montages van de Rekening &#x200B;](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Verzamel in [!UICONTROL Basecamp] de volgende informatie:

   * De URL voor uw [!DNL Basecamp] -account
   * De URL gevonden in de sectie &quot;[!UICONTROL My info]&quot;

1. Log uit van [!DNL Basecamp] .
1. Klik op **[!UICONTROL Account settings]** in de rechterbovenhoek.
1. Klik op de tab **[!UICONTROL Integrations]** .
1. Klik in de sectie **[!UICONTROL [!DNL Basecamp]]** rechts van **[!UICONTROL [!DNL Basecamp] integration]** op **[!UICONTROL Enable]** .

1. Controleer of **[!UICONTROL Classic version]** de versie is waarmee u wilt integreren naast **[!UICONTROL [!DNL Basecamp] version]** .

1. (Voorwaardelijk) Als er geen URL van [!DNL Basecamp] wordt weergegeven, klikt u op **[!UICONTROL Edit]** , typt u de URL voor uw [!DNL Basecamp] -account, zonder &quot;http://&quot; op te nemen en klikt u vervolgens op **[!UICONTROL Save]** .

1. Klik in de rechterbovenhoek van het venster op **[!UICONTROL Settings]** > **[!UICONTROL Personal settings]** .

1. Klik op de tab **[!UICONTROL Integrations]** .
1. Klik onder **[!DNL Basecamp]** rechts van **[!UICONTROL Basecamp integration]** op **[!UICONTROL Enable]** .

1. Klik rechts van **[!UICONTROL [!DNL Basecamp] API Token]** in de weergegeven opties op **[!UICONTROL Edit]** .

1. Typ in het vak dat wordt weergegeven de URL in de sectie &quot;[!UICONTROL My info]&quot; in [!DNL Basecamp] en klik vervolgens op **[!UICONTROL Save]** .\
   Nadat u [!DNL Workfront Proof] met [!DNL Basecamp] hebt geïntegreerd, kunnen uw gebruikers hun persoonlijke instellingen configureren. Voor informatie bij vestiging persoonlijke montages, zie [&#x200B; Vormend Persoonlijke Montages &#x200B;](#configuring-personal-settings)

1. Als u [!DNL Basecamp] -integratie niet kunt inschakelen, is de [!DNL Workfront Proof] -account-id mogelijk niet dezelfde als de account-id die u gebruikt in [!DNL Basecamp] .
1. Nadat u [!DNL Workfront Proof] met [!DNL Basecamp] hebt geïntegreerd, kunnen uw gebruikers hun persoonlijke instellingen configureren. Voor informatie bij vestiging persoonlijke montages, zie [&#x200B; het Vormen Persoonlijke Montages &#x200B;](#configuring-personal-settings).

## Persoonlijke instellingen configureren

Nadat u opstelling [&#x200B; de montages van de Rekening &#x200B;](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) voor uw Organisatie, elk van uw auteurs die creeert/voorlegt zouden hun [&#x200B; persoonlijke montages moeten plaatsen.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. Ga naar **[!UICONTROL Personal**&#x200B;**settings]** .

1. Open de tab **[!UICONTROL Integrations]** (1).
1. Klik op **[!UICONTROL Enable]** (2) om de [!DNL Basecamp] -integratie in te schakelen.
1. Klik op **[!UICONTROL Connect to your [!DNL Basecamp] account]** (3).\
   ![&#x200B; Basecamp_Personal_settings-integration.png &#x200B;](assets/basecamp-personal-settings-integration-350x174.png)

1. Log in bij uw [!DNL Basecamp] account (1).\
   ![&#x200B; Basecamp_login_page.png &#x200B;](assets/basecamp-login-page-350x107.png)

1. Klik op **[!UICONTROL Yes, I'll allow access]** om [!DNL Workfront Proof] toegang tot uw account te verlenen (2).\
   ![&#x200B; Basecamp_authentication_page.png &#x200B;](assets/basecamp-authorization-page-350x173.png)

1. (Optioneel) Wanneer uw persoonlijke integratie actief is (3), kunt u eenvoudig schakelen tussen uw [!DNL Basecamp] -accounts.

   1. Klik op **[!UICONTROL Switch [!DNL Basecamp] account]** (4).\

      ![&#x200B; Basecamp_switching_accounts__1_.png &#x200B;](assets/basecamp-switching-accounts--1--350x179.png)\
      De [!UICONTROL Switch Basecamp Account] gaat naar de [!UICONTROL Personal Settings] -pagina, waar u kunt kiezen welke [!DNL Basecamp] -accounts u wilt integreren met uw [!DNL Workfront Proof] -account.

   1. Klik op **[!UICONTROL Re-Integrate with [!DNL Basecamp]]** (5) voordat u de [!DNL Basecamp] account\

      Hiermee vernieuwt u de pagina [!UICONTROL Personal Settings] en geeft u de meest actuele lijst met [!DNL Basecamp] -accounts weer.

   1. Klik op **[!UICONTROL Integrate with this account]** om er verbinding mee te maken met [!DNL Workfront Proof] .\

      ![&#x200B; Basecamp_switching_accounts_2.png &#x200B;](assets/basecamp-switching-accounts-2-350x138.png)\
      U kunt nu proefdrukken toevoegen aan [!DNL Basecamp] -projecten.
