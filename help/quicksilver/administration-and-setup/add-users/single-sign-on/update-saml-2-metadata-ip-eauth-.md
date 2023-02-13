---
title: De meta-gegevens van SAML 2.0 van de update in uw IDP wanneer het gebruiken van verbeterde authentificatie
description: Als beheerder van Adobe Workfront, kunt u Workfront enig sign-on (SSO) met om het even welke identiteitsleverancier integreren die het protocol van de Prijsverhoging van de Bevestiging van de Veiligheid (SAML) 2.0 steunt.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
source-git-commit: b6fc4775953e47a1b9d84d7537a6d9f5d35b1f2c
workflow-type: tm+mt
source-wordcount: '935'
ht-degree: 0%

---

# De meta-gegevens van SAML 2.0 van de update in uw IDP wanneer het gebruiken van verbeterde authentificatie

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Als beheerder van Adobe Workfront, kunt u Workfront enig sign-on (SSO) met om het even welke identiteitsleverancier integreren die het protocol van de Prijsverhoging van de Bevestiging van de Veiligheid (SAML) 2.0 steunt.

In de volgende secties wordt het integratieproces beschreven wanneer uw Workfront-account is bijgewerkt naar de uitgebreide verificatieervaring (nog niet beschikbaar voor alle organisaties). Voor meer informatie over de verbeterde authentificatieervaring, zie [Overzicht van uitgebreide verificatie](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

Voor informatie over het vormen van SAML voorafgaand aan uw migratie aan de verbeterde authentificatieervaring, zie [SAML 2.0-metagegevens bijwerken in uw identiteitsprovider](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Okta gebruiken als uw identiteitsprovider

Okta is een voorbeeld van een identiteitsleverancier die SAML 2.0 steunt. In deze sectie wordt beschreven hoe u Okta kunt gebruiken als uw identiteitsprovider. De gelijkaardige stappen zouden worden vereist wanneer het vormen van een andere identiteitsleverancier die SAML 2.0 steunt.

>[!NOTE]
>
>Gebruikers worden toegewezen op basis van hun e-mailadres. Als u zich met Okta wilt aanmelden bij Workfront, moet u een gebruiker hebben met hetzelfde (niet-hoofdlettergevoelig) e-mailadres dat in uw Workfront-klant is gemaakt.

Voer de volgende secties in om Okta te configureren als uw identiteitsprovider in Workfront.

* [Een Workfront-app maken in Okta](#create-a-workfront-app-in-okta)
* [Voeg uw Okta-instantie toe als een identiteitsprovider in Workfront](#add-your-okta-instance-as-an-identity-provider-in-workfront)

### Een Workfront-app maken in Okta {#create-a-workfront-app-in-okta}

1. Meld u aan bij uw Okta-omgeving.
1. Zorg ervoor dat **Klassieke interface** wordt in de linkerbovenhoek van de interface Okta geselecteerd.
1. Klik in het menu op **Toepassingen** > **Toepassingen**.

1. Klikken **Toepassing toevoegen** en klik vervolgens op **Nieuwe app maken**.

1. In de **Het dialoogvenster Nieuwe toepassingsintegratie maken** selecteert u **SAML 2.0** en klik vervolgens op **Maken**.

1. Geef een naam op voor uw Workfront-toepassing en klik vervolgens op **Volgende**.
1. Zoek op de pagina met SAML-instellingen die wordt weergegeven de informatie die vereist is voor de pagina SAML-instellingen:

   1. Open zonder het browsertabblad te verlaten waar de interface Okta wordt weergegeven, een apart browsertabblad of venster.
   1. Geef de volgende URL op in de browser:

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. Geef in het resulterende XML-bestand de waarden op voor **entityID** en **Locatie**.

      ![sso-okta.png](assets/sso-okta.png)

   1. Kopieer de waarde van de **entityID** aan uw systeemklembord. Sluit dit browsertabblad niet.

1. Ga terug naar de pagina van de Montages van SAML die u in Stap 6 opende.
1. Plak de waarde in het menu **entityID** in het veld **Audience URI (SP Entiteit ID)** veld.

1. Kopieer in het XML-bestand op het andere browsertabblad de waarde uit het dialoogvenster **Locatie** veld.
1. Plak de waarde in het menu **Locatie** in het veld **Single Sign On** **URL** veld.

1. Naar de **Kenmerkinstructies (optioneel)** sectie.
1. In de **Naam** veld, specificeren **email**.

1. In de **Waarde** veld, specificeren **user.email**.

1. (Optioneel) Voeg geavanceerde waarden toe.
1. Klikken **Volgende**.
1. Selecteren, **Ik ben een klant van Okta die een interne app toevoegt** en klik vervolgens op **Voltooien**.

### Voeg uw Okta-instantie toe als een identiteitsprovider in Workfront {#add-your-okta-instance-as-an-identity-provider-in-workfront}

Deze procedure biedt essentiële informatie voor het configureren van Okta als een identiteitsprovider in Workfront. Voor extra informatie over andere afbeeldingen of configuratieopties raadpleegt u [Adobe Workfront configureren met SAML 2.0](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

1. Download de metagegevens van de identiteitsprovider voor uw Okta-instantie:

   1. Meld u aan bij uw Okta-omgeving.
   1. Zorg ervoor dat **Klassieke interface** wordt in de linkerbovenhoek van de interface Okta geselecteerd.
   1. Klik in het menu op **Toepassingen** > **Toepassingen**.

   1. Klik op de Workfront-toepassing die u hebt gemaakt, zoals beschreven in de sectie. [Een Workfront-app maken in Okta](#create-a-workfront-app-in-okta)
   1. Op de **Aanmelden** tabblad, klikt u op **Metagegevens identiteitsprovider**.

      ![idp_okta_metadata.png](assets/idp-okta-metadata.png)

      De metagegevens worden geopend als XML in een nieuw browsertabblad.

   1. Kopieer de URL die wordt weergegeven in het URL-veld van de browser.

1. Meld u aan bij Workfront als Workfront-beheerder.
1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Systeem** > **Single Sign-On (SSO)**.

1. (Voorwaardelijk) Als u twee tabbladen ziet, klikt u op de knop **Nieuwe SSO-providers** tab.

   ![sso_idp_halflife.png](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >Verwijder de bestaande SSO-configuratie-instellingen niet uit het dialoogvenster **Huidige SSO-provider** tot uw account is bijgewerkt naar de verbeterde verificatie en de nieuwe SSO-configuratie volledig functioneert.

1. Klikken **Nieuwe SSO-provider**.
1. Geef een naam op, bijvoorbeeld Okta IDP, en geef vervolgens een beschrijving op.
1. In de **Velden vullen met metagegevens van identiteitsprovider** plakt u de URL die u in stap 1 hebt gekopieerd in de **URL metagegevens** veld.\
   U kunt ook op **Bestand kiezen** om een .xml- dossier te uploaden, maar wij adviseren dat u URL kleeft.

1. In de **Gebruikerskenmerken toewijzen** in de **Directory-kenmerk** veld, type **email**. (**E-mailadres** is al ingevuld in het dialoogvenster **Workfront-gebruikerskenmerk** veld.)

1. (Optioneel) Inschakelen **Standaard SSO-provider maken** ongeautoriseerde gebruikers naar het aanmeldingsscherm van de identiteitsprovider sturen in plaats van naar het Workfront-aanmeldingsscherm voor verificatie. We raden u aan deze optie alleen in te schakelen als alle gebruikers in uw systeem via de identiteitsprovider toegang hebben tot Workfront.
1. Selecteer **Inschakelen** selectievakje. Voordat u dit doet, moet u ervoor zorgen dat gebruikers in uw systeem op de hoogte zijn van de nieuwe aanmeldervaring om ervoor te zorgen dat ze geen toegang verliezen tot het Workfront-systeem.
1. Klikken **Verbinding testen**.\
   Er wordt een bericht weergegeven waarin wordt gemeld dat de verbinding is gelukt.

1. Klikken **Opslaan**.

## Andere identiteitsproviders gebruiken

Wanneer u andere identiteitsproviders dan Okta gebruikt (zoals Ping of Centrify), moet u de Workfront-metagegevens opnieuw uploaden naar uw identiteitsprovider.
