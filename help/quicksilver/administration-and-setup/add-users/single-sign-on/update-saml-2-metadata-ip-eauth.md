---
title: SAML 2.0-metagegevens bijwerken in uw IDP wanneer uitgebreide verificatie wordt gebruikt
description: Als beheerder van Adobe Workfront, kunt u Workfront enig sign-on (SSO) met om het even welke identiteitsleverancier integreren die het protocol van de Prijsverhoging van de Bevestiging van de Veiligheid (SAML) 2.0 steunt.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 55d7d8a8-0dfe-45bc-a23a-47111347e9ca
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 75fea812b4574191522af4721a013b57aa5d609f
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 0%

---

# De meta-gegevens van SAML 2.0 van de update in uw IDP wanneer het gebruiken van verbeterde authentificatie

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Als beheerder van Adobe Workfront, kunt u Workfront enig sign-on (SSO) met om het even welke identiteitsleverancier integreren die het protocol van de Prijsverhoging van de Bevestiging van de Veiligheid (SAML) 2.0 steunt.

In de volgende secties wordt het integratieproces beschreven wanneer uw Workfront-account is bijgewerkt naar de uitgebreide verificatieervaring (nog niet beschikbaar voor alle organisaties). Voor meer informatie over de verbeterde authentificatieervaring, zie [ Verbeterd overzicht van de Authentificatie ](../../../administration-and-setup/manage-workfront/security/get-started-enhanced-authentication.md).

Voor informatie over het vormen van SAML voorafgaand aan uw migratie aan de verbeterde authentificatieervaring, zie [ de meta-gegevens van SAML 2.0 van de Update in uw identiteitsleverancier ](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).


## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Okta gebruiken als uw identiteitsprovider

Okta is een voorbeeld van een identiteitsleverancier die SAML 2.0 steunt. In deze sectie wordt beschreven hoe u Okta kunt gebruiken als uw identiteitsprovider. De gelijkaardige stappen zouden worden vereist wanneer het vormen van een andere identiteitsleverancier die SAML 2.0 steunt.

>[!NOTE]
>
>Gebruikers worden toegewezen op basis van hun e-mailadres. Als u zich met Okta wilt aanmelden bij Workfront, moet u een gebruiker hebben met hetzelfde (niet-hoofdlettergevoelig) e-mailadres dat in uw Workfront-klant is gemaakt.

Voer de volgende secties in om Okta te configureren als uw identiteitsprovider in Workfront.

* [ creeer een app van Workfront in Okta ](#create-a-workfront-app-in-okta)
* [Voeg uw instantie Okta als identiteitsprovider in Workfront toe](#add-your-okta-instance-as-an-identity-provider-in-workfront)

### Een Workfront-app maken in Okta {#create-a-workfront-app-in-okta}

1. Meld u aan bij uw Okta-omgeving.
1. Zorg ervoor dat **Klassieke UI** in de upper-left hoek van de interface Okta wordt geselecteerd.
1. In het menu, klik **Toepassingen** > **Toepassingen**.

1. Klik **toevoegen Toepassing**, dan klik **creeer Nieuwe App**.

1. In **creeer een Nieuwe de dialoogdoos van de Integratie van de Toepassing**, uitgezochte **SAML 2.0**, dan klik **creeer**.

1. Specificeer een naam voor uw Workfront app, dan klik **daarna**.
1. Zoek op de pagina met SAML-instellingen die wordt weergegeven de informatie die vereist is voor de pagina SAML-instellingen:

   1. Open zonder het browsertabblad te verlaten waar de interface Okta wordt weergegeven, een apart browsertabblad of venster.
   1. Geef de volgende URL op in de browser:

      `https://[your_customer_subdomain].my.workfront.com/auth/saml2/metadata`

   1. In het resulterende dossier van XML, identificeer de waarden voor **entityID** en **Plaats**.

      ![ sso-okta.png ](assets/sso-okta.png)

   1. Kopieer de waarde van het **entityID** gebied aan uw systeemklembord. Sluit dit browsertabblad niet.

1. Ga terug naar de pagina van de Montages van SAML die u in Stap 6 opende.
1. Plak de waarde van het **entityID** gebied in het **Soortpubliek URI (identiteitskaart van de Entiteit van SP)** gebied.

1. In het dossier van XML op uw andere browser lusje, kopieer de waarde van het **gebied van de Plaats**.
1. Plak de waarde van het **gebied van de Plaats** in het **Enige teken op** **URL** gebied.

1. De rol aan de **Verklaringen van Attributen (Facultatieve)** sectie.
1. Op het **gebied van de Naam**, specificeer **e-mail**.

1. Op het **gebied van de Waarde**, specificeer **user.email**.

1. (Optioneel) Voeg geavanceerde waarden toe.
1. Klik **daarna**.
1. Selecteer, **ik ben een klant van Okta toevoegend een interne app**, dan klik **Afwerking**.

### Voeg uw instantie Okta als identiteitsprovider in Workfront toe {#add-your-okta-instance-as-an-identity-provider-in-workfront}

Deze procedure biedt essentiële informatie voor het configureren van Okta als een identiteitsprovider in Workfront. Voor extra informatie over andere afbeeldingen of configuratieopties, zie [ Adobe Workfront met SAML 2.0 ](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md) vormen.

1. Download de metagegevens van de identiteitsprovider voor uw Okta-instantie:

   1. Meld u aan bij uw Okta-omgeving.
   1. Zorg ervoor dat **Klassieke UI** in de upper-left hoek van de interface Okta wordt geselecteerd.
   1. In het menu, klik **Toepassingen** > **Toepassingen**.

   1. Klik Workfront app die u creeerde, zoals die in de sectie wordt beschreven, [ creeer een app van Workfront in Okta ](#create-a-workfront-app-in-okta)
   1. Voor het **Teken** lusje, klik **meta-gegevens van de Leverancier van de Identiteit**.

      ![ idp_okta_metadata.png ](assets/idp-okta-metadata.png)

      De metagegevens worden geopend als XML in een nieuw browsertabblad.

   1. Kopieer de URL die wordt weergegeven in het URL-veld van de browser.

1. Meld u aan bij Workfront als Workfront-beheerder.

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Systeem** > **Enige Sign-On (SSO)**.

1. (Voorwaardelijk) als u twee lusjes ziet, klik de **Nieuwe Leveranciers SSO** tabel.

   ![ sso_idp_halflife.png ](assets/sso-idp-halflife-350x234.png)

   >[!IMPORTANT]
   >
   >Schrap niet uw bestaande SSO configuratiemontages in het **Huidige Sso- Leverancier** lusje tot uw rekening aan de verbeterde authentificatieervaring wordt bijgewerkt en de nieuwe configuratie SSO volledig functioneel is.

1. Klik **Nieuwe Leverancier SSO**.
1. Geef een naam op, bijvoorbeeld Okta IDP, en geef vervolgens een beschrijving op.
1. In **bevolkt gebieden van de Meta-gegevens van Identiteitsprovider** sectie, kleef URL die u in Stap 1 in het **Meta-gegevens URL** gebied kopieerde.\
   Alternatief, kunt u **kiezen Dossier** klikken om een .xml- dossier te uploaden, maar wij adviseren dat u URL kleeft.

1. In de **sectie van de Attributen van de Gebruiker van de Kaart**, op het **3} gebied van het Attribuut van de Folder, type** e-mail **.** (**E-mailAdres** is reeds bevolkt op het **gebied van het Attribuut van de Gebruiker van Workfront**.)

1. (Optioneel) Schakel **Standaard SSO-provider maken** in om onbevoegde gebruikers naar het aanmeldingsscherm van de identiteitsprovider te verzenden in plaats van naar het Workfront-aanmeldingsscherm voor verificatie. We raden u aan deze optie alleen in te schakelen als alle gebruikers in uw systeem via de identiteitsprovider toegang hebben tot Workfront.
1. Selecteer **toelaten** checkbox. Voordat u dit doet, moet u ervoor zorgen dat gebruikers in uw systeem op de hoogte zijn van de nieuwe aanmeldervaring om ervoor te zorgen dat ze geen toegang verliezen tot het Workfront-systeem.
1. Klik **Verbinding van de Test**.\
   Er wordt een bericht weergegeven waarin wordt gemeld dat de verbinding is gelukt.

1. Klik **sparen**.

## Andere identiteitsproviders gebruiken

Wanneer u andere identiteitsproviders dan Okta gebruikt (zoals Ping of Centrify), moet u de Workfront-metagegevens opnieuw uploaden naar uw identiteitsprovider.
