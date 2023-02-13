---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: SAML 2.0-metagegevens bijwerken in uw identiteitsprovider
description: U kunt SAML 2.0-metagegevens bijwerken in uw identiteitsprovider.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 96f1d50024605328713ca2019f3b726e27dc569c
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---

# SAML 2.0-metagegevens bijwerken in uw identiteitsprovider

{{important-admin-console-onboard}}

De volgende secties beschrijven hoe te om uw meta-gegevens van de Prijsverhoging van de Bevestiging van de Veiligheid (SAML) 2.0 bij te werken wanneer het gebruiken van de Actieve Diensten van de Federatie van de Folder (ADFS) als uw identiteitsleverancier.

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

## ADFS gebruiken als uw identiteitsprovider

U kunt uw ADFS-metagegevens bijwerken voordat of nadat Adobe Workfront het SAML 2.0-certificaat heeft bijgewerkt. Als u ervoor kiest de ADFS-metagegevens bij te werken voordat het SAML 2.0-certificaat door Workfront wordt bijgewerkt, zijn extra stappen vereist.

* [ADFS-metagegevens bijwerken](#update-your-adfs-metadata)
* [Uw ADFS-metagegevens bijwerken forceren](#force-your-adfs-metadata-to-update)

### ADFS-metagegevens bijwerken {#update-your-adfs-metadata}

Voer de stappen in deze sectie uit als u de ADFS-metagegevens automatisch wilt bijwerken.

ADFS is standaard geconfigureerd om automatisch te controleren op updates van alle vertrouwensmetagegevens van de vertrouwde partij; de standaard is echter ingesteld op een opiniepeiling om de 24 uur . U kunt deze waarde wijzigen met powershell-opdrachten.

1. Meld u aan bij de ADFS-server en open de ADFS Management Console.
1. Vouw in het deelvenster aan de linkerkant de selectie uit **ADFS 2.0** vervolgens uitvouwen **Betrouwbaarheidsrelaties.**

1. Klik op de knop **Vertrouwden op een partij** map.
1. Selecteer het vertrouwen van de betrouwbare partij dat u eerder om met Workfront vormde te worden gebruikt, dan in het juiste paneel, klik **Bijwerken van metagegevens van Federatie**.
1. (Voorwaardelijk) Als deze optie grijs wordt weergegeven (wat betekent dat het vertrouwen van de betrouwbare partij eerder is geconfigureerd met een metagegevensbestand), voert u het volgende in.

   1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

   1. Klikken **Systeem** > **Single Sign On (SSO)**.

   1. Klikken **Instellingen bewerken.**
   1. Klikken **Configuratie bewerken** selecteert u vervolgens **SAML 2.0** in de **Type** vervolgkeuzelijst.

   1. Kopieer de **URL metagegevens**, die op het volgende moet lijken:

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Voor de server ADFS, klik op het vertrouwen van de afhankelijke partij die u eerder vormde met de rechtermuisknop aan, dan klik **Eigenschappen.**
   1. Klik op de knop **Toezicht** plakken, plakt u vervolgens de URL die u uit Workfront hebt gekopieerd in de **URL van metagegevens van de federatie van de partij** veld.

   1. Controleer de opties om **Hoofdkantoor** en **Opnieuw vertrouwde partij automatisch bijwerken**.

   1. Klikken **OK.**
   1. Selecteer het vertrouwen van de betrouwbare partij die u eerder om met Workfront vormde te worden gebruikt; klikt u vervolgens in het rechterdeelvenster op **Bijwerken vanuit federatiemetagegevens.**

1. Klikken **OK** om het bericht te negeren dat een deel van de inhoud in de metagegevens van de federatie niet wordt ondersteund door ADFS 2.0.
1. Openen **Windows PowerShell-modules.**
1. Nadat alle modules laden, stel het volgende bevel in powershell in werking:

   `Get-ADFSProperties`

1. Zoek de waarde naast **Monitoringinterval.**

   Het wordt een getal dat het aantal minuten tussen opiniepeilingen aangeeft. De standaardwaarde moet 1440 zijn (1440 minuten = 24 uur).

1. Plaats een nieuwe waarde door het volgende bevel in powershell in werking te stellen:

   `Set-ADFSProperties -MonitoringInterval 1`

   Dit verandert het controleinterval van om de 24 uur in elke minuut. U kunt de waarde 1 wijzigen in een andere hogere waarde als u wilt dat deze minder vaak wordt opiniepeild.

1. Om te controleren dat dit correct werkt, gebruik **Gebeurtenisviewer** om de volgende informatie in de logboeken van ADFS2.0 te zoeken:

   **Gebeurtenis ID 156 en 157**

### Uw ADFS-metagegevens bijwerken forceren {#force-your-adfs-metadata-to-update}

Voer de stappen in de volgende sectie uit om uw ADFS-metagegevens bij te werken.

Om meta-gegevens te dwingen die tussen Workfront en uw leverancier SAML 2.0 worden geruild wanneer het gebruiken van de Actieve Diensten van de Federatie van de Folder (ADFS):

>[!NOTE]
>
>Sommige van deze veranderingen zouden door uw afdeling van IT kunnen moeten worden gedaan.

1. Meld u aan bij de ADFS-server en open het dialoogvenster **ADFS-beheerconsole**.
1. Vouw in het deelvenster aan de linkerkant de selectie uit **ADFS 2.0** vervolgens uitvouwen **Betrouwbaarheidsrelaties**.

1. Klik op de knop **Vertrouwden op een partij** map.
1. Selecteer het vertrouwen van de betrouwbare partij dat u eerder om met Workfront vormde te worden gebruikt, dan in het juiste paneel, klik **Bijwerken van metagegevens van Federatie**.

   Als deze optie grijs wordt weergegeven en niet kan worden geselecteerd, voert u het volgende in:

   (De optie wordt alleen grijs weergegeven wanneer het vertrouwen van de betrouwbare partij eerder is geconfigureerd met een metagegevensbestand.)

   1. In Workfront, in het gebied van de Opstelling, kopieer **URL metagegevens** vanuit het Workfront-scherm Single Sign-On (Single Sign On).

      Om toegang te krijgen tot de informatie voor de **URL metagegevens**:

      1. Klikken **Instellen** in de rechterbovenhoek van Adobe Workfront op de algemene navigatiebalk.
      1. Klik > **Systeem** > **Single Sign On (SSO)**.
      1. Klikken **Instellingen bewerken.**
      1. Klikken **Configuratie bewerken** selecteert u vervolgens **SAML 2.0** in de **Type** vervolgkeuzelijst.
      1. Kopieer de **URL metagegevens**, die op het volgende moet lijken:

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`
   1. Voor de server ADFS, klik op het vertrouwen van de afhankelijke partij die u eerder vormde met de rechtermuisknop aan, dan klik **Eigenschappen.**
   1. Klik op de knop **Toezicht** plakken, plakt u vervolgens de URL die u uit Workfront hebt gekopieerd in de **URL van metagegevens van de federatie van de partij** veld.
   1. Controleer de opties om **Hoofdkantoor** en **Opnieuw vertrouwde partij automatisch bijwerken**.
   1. Klikken **OK**.
   1. Selecteer het vertrouwen van de betrouwbare partij dat u eerder om met Workfront vormde te worden gebruikt, dan in het juiste paneel, klik **Bijwerken vanuit federatiemetagegevens.**


1. Klikken **OK** om het bericht te negeren dat een deel van de inhoud in de metagegevens van de federatie niet wordt ondersteund door ADFS 2.0.
1. Klikken **Bijwerken** om het bijwerken van de metagegevens van uw federatie te voltooien.

Gebruikers die via het native aanmeldingsscherm toegang hebben tot Workfront, maken gebruik van de aanmeldingsgegevens van Workfront (dit kan worden geconfigureerd vanaf de profielpagina van elke gebruiker in het dialoogvenster **Toegang** -sectie) kunt u zich aanmelden met hun Workfront-gebruikersnaam en -wachtwoord door naar de volgende URL te navigeren: `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## Andere identiteitsproviders gebruiken

Wanneer u andere identiteitsproviders dan ADFS gebruikt (zoals Ping, Okta of Centrify), moet u de Workfront-metagegevens opnieuw uploaden naar uw identiteitsprovider.

Ga voor meer informatie over het verkrijgen van een nieuwe URL met metagegevens van Workfront naar [ADFS-metagegevens bijwerken](#update-your-adfs-metadata).

Voor extra informatie over het gebruiken van de Actieve Diensten van de Federatie van de Folder (ADFS) met SAML 2.0 in Workfront, zie [Adobe Workfront configureren met SAML 2.0 met behulp van ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
