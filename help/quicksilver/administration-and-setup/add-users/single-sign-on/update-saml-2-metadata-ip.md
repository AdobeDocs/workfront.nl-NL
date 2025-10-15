---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: SAML 2.0-metagegevens bijwerken in uw identiteitsprovider
description: U kunt SAML 2.0-metagegevens bijwerken in uw identiteitsprovider.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 22ae8b489c63ba6eea1472cf415f95e375a94773
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 0%

---

# SAML 2.0-metagegevens bijwerken in uw identiteitsprovider

>[!IMPORTANT]
>
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet aan boord van de Adobe Admin Console zijn.
>
>Om gebruikersattributen in kaart te brengen in organisaties die aan Adobe Admin Console in kaart zijn gebracht, zie [ de gebruikersattributen van de Kaart in Adobe verenigde ervaring ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) in de gebruikersattributen van de artikel Kaart.

De volgende secties beschrijven hoe te om uw meta-gegevens van de Prijsverhoging van de Bevestiging van de Veiligheid (SAML) 2.0 bij te werken wanneer het gebruiken van de Actieve Diensten van de Federatie van de Folder (ADFS) als uw identiteitsleverancier.

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

## ADFS gebruiken als uw identiteitsprovider

U kunt uw ADFS-metagegevens bijwerken voordat of nadat Adobe Workfront het SAML 2.0-certificaat heeft bijgewerkt. Als u ervoor kiest de ADFS-metagegevens bij te werken voordat het SAML 2.0-certificaat door Workfront wordt bijgewerkt, zijn extra stappen vereist.

* [ werk uw meta-gegevens ADFS ](#update-your-adfs-metadata) bij
* [Uw ADFS-metagegevens bijwerken forceren](#force-your-adfs-metadata-to-update)

### ADFS-metagegevens bijwerken {#update-your-adfs-metadata}

Voer de stappen in deze sectie uit als u de ADFS-metagegevens automatisch wilt bijwerken.

Door gebrek, wordt ADFS gevormd om updates aan elk van zijn het vertrouwen van de partij meta-gegevens automatisch te controleren; nochtans, wordt het gebrek geplaatst aan opiniepeiling slechts om de 24 uur. U kunt deze waarde wijzigen met powershell-opdrachten.

1. Meld u aan bij de ADFS-server en open de ADFS-beheerconsole.
1. In het linkerpaneel, breid **ADFS 2.0 uit,** breid dan **Vertrouwensrelaties uit.**

1. Klik de **Relying Partij vertrouwt** omslag.
1. Selecteer het vertrouwen van de afhankelijke partij dat u eerder om met Workfront, dan in het rechterpaneel werd gevormd te worden gebruikt, **Update van Metagegevens van de Federatie** klikken.
1. (Voorwaardelijk) Als deze optie grijs wordt weergegeven (wat betekent dat het vertrouwen van de betrouwbare partij eerder is geconfigureerd met een metagegevensbestand), voert u het volgende in.

   1. Klik het **pictogram 1} van het Belangrijkste Menu** Belangrijkste menupictogram ![ in de hoger-juiste hoek van Adobe Workfront, dan klik ](assets/main-menu-icon.png) de montages van de Opstelling **** Gear pictogram ![.](assets/gear-icon-settings.png)

   1. Klik **Systeem** > **Enig Teken (SSO)**.

   1. Klik **uitgeven Montages.**
   1. Klik **uitgeven Configuratie**, dan uitgezocht **SAML 2.0** in de **Type** drop-down lijst.

   1. Kopieer **Meta-gegevens URL**, die aan het volgende gelijkaardig zouden moeten zijn:

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Voor de server ADFS, klik op het vertrouwende partijvertrouwen met de rechtermuisknop aan dat u eerder vormde, dan klik **Eigenschappen.**
   1. Klik het **Controle** lusje, dan kleef URL die u van Workfront in het **Van de federatie afhankelijke URL van de partij** gebied kopieerde.

   1. Controleer de opties aan **Monitor die partij** vertrouwt en **automatisch bijwerken die partij** vertrouwt.

   1. Klik **O.K.**
   1. Selecteer het vertrouwen van de afhankelijke partij die u eerder om met Workfront vormde te worden gebruikt; dan, in het rechterpaneel, klik **Update van Metagegevens van de Federatie.**

1. Klik **O.K.** om het bericht over enkele inhoud in de federatie meta-gegevens te negeren die niet door ADFS 2.0 worden gesteund.
1. Open **Powershell Modules van Vensters.**
1. Nadat alle modules laden, stel het volgende bevel in powershell in werking:

   `Get-ADFSProperties`

1. Zoek de waarde naast **het Interval van de Controle.**

   Het wordt een getal dat het aantal minuten tussen opiniepeilingen aangeeft. De standaardwaarde moet 1440 zijn (1440 minuten = 24 uur).

1. Plaats een nieuwe waarde door het volgende bevel in powershell in werking te stellen:

   `Set-ADFSProperties -MonitoringInterval 1`

   Dit verandert het controleinterval van om de 24 uur in elke minuut. U kunt de waarde 1 wijzigen in een andere hogere waarde als u wilt dat deze minder vaak wordt opgevraagd.

1. Om te verifiëren dat dit correct werkt, gebruik de **Kijker van de Gebeurtenis** om de volgende informatie in de logboeken te zoeken ADFS2.0:

   **identiteitskaart van de Gebeurtenis 156 en 157**

### Uw ADFS-metagegevens bijwerken forceren {#force-your-adfs-metadata-to-update}

Voer de stappen in de volgende sectie uit om uw ADFS-metagegevens bij te werken.

Om meta-gegevens te dwingen die tussen Workfront en uw leverancier SAML 2.0 worden geruild wanneer het gebruiken van de Actieve Diensten van de Federatie van de Folder (ADFS):

>[!NOTE]
>
>Sommige van deze veranderingen zouden door uw afdeling van IT kunnen moeten worden gedaan.

1. Login aan de server ADFS en open de **Console van het Beheer ADFS**.
1. In het linkerpaneel, breid **ADFS 2.0** uit, dan breid **Vertrouwensrelaties** uit.

1. Klik de **Relying Partij vertrouwt** omslag.
1. Selecteer het vertrouwen van de afhankelijke partij dat u eerder om met Workfront, toen in het rechterpaneel werd gevormd te worden gebruikt, **Update van Metagegevens van de Federatie** klikken.

   Als deze optie grijs wordt weergegeven en niet kan worden geselecteerd, voert u het volgende in:

   (De optie wordt alleen grijs weergegeven wanneer het vertrouwen van de betrouwbare partij eerder is geconfigureerd met een metagegevensbestand.)

   1. In Workfront, in het gebied van de Opstelling, kopieer **Meta-gegevens URL** van uw Workfront Enige Sign-On opstellingsscherm.

      Om tot de informatie voor **Meta-gegevens URL** toegang te hebben:

      1. Klik **Opstelling** dichtbij de hoger-juiste hoek van Adobe Workfront op de Globale Bar van de Navigatie.
      1. Klik > **Systeem** > **Enig Teken (SSO)**.
      1. Klik **uitgeven Montages.**
      1. Klik **uitgeven Configuratie**, dan uitgezocht **SAML 2.0** in de **Type** drop-down lijst.
      1. Kopieer **Meta-gegevens URL**, die aan het volgende gelijkaardig zouden moeten zijn:

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Voor de server ADFS, klik op het vertrouwende partijvertrouwen met de rechtermuisknop aan dat u eerder vormde, dan klik **Eigenschappen.**
   1. Klik het **Controle** lusje, dan kleef URL die u van Workfront in het **Van de federatie afhankelijke URL van de partij** gebied kopieerde.
   1. Controleer de opties aan **Monitor die partij** vertrouwt en **automatisch bijwerken die partij** vertrouwt.
   1. Klik **OK**.
   1. Selecteer het vertrouwen van de afhankelijke partij dat u eerder om met Workfront, toen in het rechterpaneel, **Update van Meta-gegevens van de Federatie vormde te worden gebruikt.**

1. Klik **O.K.** om het bericht over enkele inhoud in de federatie meta-gegevens te negeren die niet door ADFS 2.0 worden gesteund.
1. Klik **Update** om het bijwerken van uw federatie meta-gegevens te voltooien.

De gebruikers die tot Workfront via het inheemse login scherm toegang hebben gebruikend de login van Workfront geloofsbrieven (dit kan van de het profielpagina van elke gebruiker in de **sectie van de Toegang** worden gevormd) kunnen login gebruikend hun gebruikersnaam en wachtwoord van Workfront door aan volgende URL te navigeren: `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## Andere identiteitsproviders gebruiken

Wanneer u andere identiteitsproviders dan ADFS gebruikt (zoals Ping, Okta of Centrify), moet u de Workfront-metagegevens opnieuw uploaden naar uw identiteitsprovider.

Voor meer informatie over hoe te om een nieuwe Meta-gegevens URL van Workfront te verkrijgen, zie [ Update uw meta-gegevens ADFS ](#update-your-adfs-metadata).

Voor extra informatie over het gebruiken van de Actieve Diensten van de Federatie van de Folder (ADFS) met SAML 2.0 in Workfront, zie [ Adobe Workfront met SAML 2.0 vormen gebruikend ADFS ](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
