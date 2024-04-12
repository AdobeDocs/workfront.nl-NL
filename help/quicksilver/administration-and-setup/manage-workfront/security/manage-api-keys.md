---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: API-sleutels beheren
description: Adobe Workfront-beheerders kunnen de API-sleutels beheren die worden gebruikt om toepassingen in staat te stellen om namens een gebruiker toegang te krijgen tot Workfront, om zo kwetsbaarheden op het gebied van API-beveiliging tot een minimum te beperken.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: f504013e202c57245a2edc3dff2b71d19bcfdbee
workflow-type: tm+mt
source-wordcount: '1386'
ht-degree: 0%

---

# API-sleutels beheren

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

Adobe Workfront-beheerders kunnen de API-sleutels beheren die worden gebruikt om toepassingen in staat te stellen om namens een gebruiker toegang te krijgen tot Workfront, om zo kwetsbaarheden op het gebied van API-beveiliging tot een minimum te beperken.

U kunt de huidige API-sleutel voor beheerders opnieuw instellen of verwijderen, API-sleutels configureren voor verlopen en de API-sleutels voor alle gebruikers verwijderen.

Voorbeelden van toepassingen die gebruikmaken van de Workfront API zijn:

* Documentintegratie zoals Dropbox, Google Drive en Workfront DAM
* Workfront mobiele toepassingen

>[!IMPORTANT]
>
>Wanneer u een API-sleutel opnieuw instelt of verwijdert, moet elke toepassing die gebruikmaakt van de Workfront API en die via deze API-sleutel voor verificatie bij Workfront zorgt, opnieuw worden geconfigureerd om toegang tot Workfront te herstellen.

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
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront API-toetsen

Elke gebruiker in Workfront heeft een unieke API-sleutel. Deze sleutel wordt per gebruiker gegenereerd op het moment dat de gebruiker toegang krijgt tot een integratie die gebruikmaakt van de Workfront API (zoals de mobiele Workfront-app of documentintegratie).

>[!NOTE]
>
> API-sleutels die u genereert in de productieomgeving, worden tijdens de wekelijkse vernieuwing gekopieerd naar de voorbeeldomgeving. Alle API-sleutels die u genereert in de voorvertoningsomgeving, worden tijdens de wekelijkse vernieuwing overschreven met uw productie-API-sleutels.

Workfront-beheerders hebben ook een unieke API-sleutel. Wanneer een toepassing een beheerder-API-sleutel gebruikt om toegang te krijgen tot Workfront, heeft de toepassing beheerderstoegang tot Workfront.

## De API-sleutel voor beheerders beheren

U kunt de API-sleutel voor uw beheerdersgebruikersaccount genereren, opnieuw instellen of verwijderen.

>[!NOTE]
>
>U kunt ook een API-sleutel genereren via de API. Zie de klasse [API voor abonnementen voor gebeurtenissen](../../../wf-api/general/event-subs-api.md) sectie in [API voor abonnementen voor gebeurtenissen](../../../wf-api/general/event-subs-api.md).

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Systeem >** **Klantgegevens.**
1. (Voorwaardelijk) Voer een van de volgende handelingen uit:

   Een API-sleutel genereren: in het dialoogvenster **Instellingen API-sleutel** sectie, klikken **API-sleutel genereren**.

   of\
   Een API-sleutel opnieuw instellen: in het dialoogvenster **Instellingen API-sleutel** sectie, klikken **Herstellen** vervolgens **Herstellen.**

   of

   De API-sleutel verwijderen: in het dialoogvenster **Instellingen API-sleutel** sectie, klikken **Verwijderen** vervolgens **Verwijderen**.

## Een API-sleutel genereren voor gebruikers die geen beheerder zijn

U kunt API-sleutels voor gebruikers in andere rollen dan Workfront-beheerders genereren en beheren.

>[!NOTE]
>
>Dit is niet beschikbaar als het Workfront-exemplaar van uw organisatie is ingeschakeld met Adobe IMS. Zie uw netwerk of beheerder van IT als u meer informatie nodig hebt.

1. (Voorwaardelijk) als uw organisatie Single Sign-On (SSO) toegangsbeheer gebruikt, maak tijdelijk de optie onbruikbaar die authentificatie SSO vereist.

   1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

   1. Uitbreiden **Systeem** en klik vervolgens op **Single Sign-On (SSO)**.
   1. In de **Type** in het veld selecteert u het type SSO dat uw organisatie gebruikt.
   1. Met het geselecteerde type, scrol neer en ontruim **Inschakelen** selectievakje.
      ![](assets/sysadmin-security-sso-disable-31620-350x320.png)
   1. Klikken **Opslaan**.


1. Voer in de adresbalk van een browser de volgende API-aanroep in:

   `<domain>`**.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**gebruikersnaam**&amp;password=**password**&amp;method=PUT

   Vervangen `<domain>` met uw Workfront-domeinnaam en gebruikersnaam en wachtwoord.

1. (Voorwaardelijk) laat de optie toe die authentificatie vereist SSO als u het in Stap 1 onbruikbaar maakte.

   1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

   1. Uitbreiden **Systeem** en klik vervolgens op **Single Sign-On (SSO)**.

   1. Selecteer de SSO-methode in het dialoogvenster **Type** vervolgkeuzelijst.
   1. Schakel het selectievakje in waarvoor SSO-verificatie is vereist.

## Configureren wanneer API-sleutels verlopen

U kunt API Toetsen vormen om voor alle gebruikers in uw systeem te verlopen. Wanneer de API-sleutel van een gebruiker vervalt, moet de gebruiker opnieuw worden geverifieerd voor toepassingen die de Workfront API gebruiken om toegang te krijgen tot Workfront. U kunt de frequentie wijzigen waarmee de API-toetsen verlopen. U kunt ook configureren of API-sleutels verlopen wanneer het wachtwoord van een gebruiker verloopt.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Systeem** > **Klantgegevens**.
1. In de **Instellingen API-sleutel** in het gebied **Na het maken**, **API-sleutels verlopen in** Selecteer de tijdlijn wanneer u de API-toetsen wilt laten verlopen.

   Wanneer u deze optie wijzigt, begint de nieuwe tijdlijn vanaf het moment dat u de wijziging aanbracht. Als u deze optie bijvoorbeeld wijzigt vanuit *1 maand* tot *6 maanden* verlopen de API-toetsen zes maanden vanaf het moment dat u de wijziging aanbrengt.

   API-sleutels verlopen standaard elke maand.

1. Selecteer **API-sleutel verwijderen wanneer het wachtwoord van een gebruiker vervalt**.

   Deze optie is standaard niet geselecteerd.

   Voor informatie over hoe te om gebruikerswachtwoorden te vormen om te verlopen, zie [Systeembeveiligingsvoorkeuren configureren](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Klikken **Opslaan**.

## De API-sleutels voor alle gebruikers verwijderen

Als u zich zorgen maakt over een bepaalde inbreuk op de beveiliging van uw Workfront-systeem, kunt u de API-sleutels voor alle gebruikers tegelijk verwijderen.

>[!IMPORTANT]
>
>Als u API-sleutels verwijdert voor alle gebruikers, worden ALLE API-sleutels voor alle gebruikers in het systeem ongeldig. Hierdoor zullen al uw integraties in Workfront mislukken totdat u een nieuwe API-sleutel genereert in Workfront en al uw integraties bijwerkt.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Uitbreiden **Systeem** en klik vervolgens op **Klantgegevens.**

1. In de **Instellingen API-sleutel** gebied, klikken **Alle API-sleutels verwijderen** en klik vervolgens op **Verwijderen** **Alles**.

## API-aanmeldingen beperken met een X.509-certificaat

>[!IMPORTANT]
>
>De in dit gedeelte beschreven procedure is alleen van toepassing op organisaties die nog niet aan boord zijn gegaan bij het Adobe Business Platform. Aanmelden bij Workfront via de Workfront API is niet beschikbaar als uw organisatie is aangemeld bij het Adobe Business Platform.
>
>Voor een lijst van procedures die verschillen gebaseerd op of uw organisatie aan het Bedrijfs Platform van de Adobe is geregistreerd, zie [Platformgebaseerde verschillen in beheer (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Toepassingen van derden kunnen met Workfront communiceren via de API. Om de beveiliging van uw Workfront-site te verhogen, kunt u Workfront zodanig configureren dat de aanmeldingsaanvragen voor de API worden beperkt door een X.509-certificaat naar Workfront te uploaden. Als deze optie is ingeschakeld, moeten alle aanmeldingsaanvragen via de API naast gebruikersnaam en wachtwoord ook een clientcertificaat bevatten.

>[!NOTE]
>
>Dit is niet beschikbaar als het Workfront-exemplaar van uw organisatie is ingeschakeld met Adobe IMS. Zie uw netwerk of beheerder van IT als u meer informatie nodig hebt.

* [Het X.509-certificaat ophalen](#obtain-the-x-509-certificate)
* [Het certificaat uploaden naar Workfront](#upload-the-certificate-to-workfront)
* [Verifieer API login vraag wordt beperkt](#verify-api-login-calls-are-restricted)

### Het X.509-certificaat ophalen {#obtain-the-x-509-certificate}

Vraag een geldig X.509-certificaat aan van een vertrouwde certificeringsinstantie (zoals Verisign) en plaats het op een tijdelijke locatie op uw werkstation.

### Het certificaat uploaden naar Workfront {#upload-the-certificate-to-workfront}

Nadat u het X.509-certificaat van uw certificeringsinstantie hebt ontvangen, moet u het uploaden naar Workfront.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Uitbreiden **Systeem** en klik vervolgens op **Klantgegevens**.

1. In de **Instellingen API-sleutel** gebied, selecteren **X.509-certificaat inschakelen**.
1. Blader op uw werkstation naar het X.509-certificaat dat u eerder hebt gedownload en selecteer dit certificaat.
1. (Optioneel) Klik op **Details weergeven** naast de certificaatnaam om de volgende details over het certificaat weer te geven:

   * Onderwerpnaam
   * Onderwerp Organisatie
   * Onderwerpeenheid
   * Algemene naam van uitgever
   * Uitgevende organisatie
   * Eenheid emittentenorganisatie
   * Serienummer
   * Datum van afgifte
   * Vervaldatum

1. Klikken **Opslaan**.

### Verifieer API login vraag wordt beperkt {#verify-api-login-calls-are-restricted}

Voordat u uw exemplaar van Workfront configureert voor een X.509-certificaat, moet u een API-aanvraag uitvoeren bij de `/login` eindpunt dat geldige gebruikersbenaming en wachtwoordparameters gebruikt. U zult een 200 reactie ontvangen die een sessionID bevat.

Nadat u van het X.509-certificaat een vereiste hebt gemaakt via de pagina met klantgegevens in uw exemplaar van Workfront, probeert u zich opnieuw aan te melden. Dit keer ontvangt u een 500-foutreactie met het volgende bericht: &quot;Niet-vertrouwd verzoek. Neem contact op met de systeembeheerder en voeg het certificaat bij.&quot;

Nadat u hebt bevestigd dat het X.509-certificaat vereist is, voert u hetzelfde aanmeldingsverzoek uit met een extra parameter voor apiCertificate die is ingesteld op de waarde van het certificaat. Als deze verrichting correct werd uitgevoerd zult u een 200 reactie ontvangen die geldige sessionID bevat.
