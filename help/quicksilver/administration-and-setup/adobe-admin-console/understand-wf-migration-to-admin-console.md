---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: De Workfront-migratie naar de Adobe Admin Console begrijpen
description: Werken met Workfront-product- en gebruikersmigratie naar Adobe Admin Console
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
source-git-commit: 99b94c246f14110e37b23c95a178efd5b9042a9d
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 0%

---

# De Workfront-migratie naar de Adobe Admin Console begrijpen

Adobe wijzigt de manier waarop u uw Adobe Workfront-gebruikers beheert, waardoor u en uw organisatie meer productiviteit krijgen. Als onderdeel van deze wijziging migreert Adobe uw Workfront-exemplaar en gebruikers naar de Adobe Admin Console. Dit is een noodzakelijke migratie en heeft geen invloed op rapporten, goedkeuringspaden, inhoud of elementen. Dit is van invloed op de manier waarop u gebruikerstoegang beheert en de manier waarop uw gebruikers zich aanmelden.

Als u wilt weten hoe u de Adobe Admin Console kunt gebruiken om uw rechten voor Adoben in uw hele organisatie te beheren, raadpleegt u [Gebruikers beheren in de Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## Wat verandert er?

Als onderdeel van de migratie gaat uw gebruikersbeheer van de Workfront-toepassing naar de Adobe Admin Console, met de volgende beheertaken:

* **Systeembeheerders** zijn supergebruikers met rechten van alle beheerders. Zij wijzen alle administratieve rollen toe, en leiden gebruikers voor de volledige organisatie voor alle producten.

* **Productprofielbeheerders (Workfront-systeembeheerders)** beheren welke gebruikers in de organisatie toegang krijgen tot Workfront.

* **Gebruikers zullen zich aanmelden met Adobe Identity.** Nadat de Adobe bestaande gebruikers naar de Adobe Admin Console migreert, zullen de gebruikers binnen aan hun instanties van Workfront gebruikend hun nieuwe Identiteit van de Adobe - of Adobe ID of Federated ID van de Adobe (SSO) ondertekenen.

* **Er is geen wijziging in de manier waarop u alle andere functies beheert** binnen de Workfront-toepassing zelf, inclusief het beheer van functies, gebruikersrollen, werkruimten, functionaliteit en gedrag.

## Tijdlijn migratiepad

Adobe migreert uw Workfront-exemplaar eerst naar de Adobe Admin Console en migreert vervolgens alle bestaande gebruikers met geverifieerde e-mailadressen. Als u systeembeheerder of beheerder van het Productprofiel van Workfront (de beheerder van het Systeem van Workfront) bent, zult u e-mail ontvangen die u door de migratiereis begeleidt. Hier volgt een tijdlijn van wat u kunt verwachten:

### Workfront-migratie naar Adobe Admin Console voltooid

Systeembeheerders ontvangen een e-mail wanneer de migratie van Workfront naar Adobe Admin Console is voltooid. Op dit moment kunnen systeembeheerders enkele vereiste stappen moeten uitvoeren **voordat de migratie van gebruikers begint**, om de gevolgen voor Workfront-gebruikers te minimaliseren.

* **Als uw Workfront-gebruikers zich momenteel aanmelden bij SSO**, moet u SSO instellen op de Adobe Admin Console zodat uw gebruikers zich kunnen blijven aanmelden met SSO. Als uw Workfront-gebruikers momenteel geen SSO gebruiken, maar u wilt deze instellen op Adobe Admin Console, kunt u dit op dit moment doen tijdens de migratiereis.
* **Als u al andere Adobe producten beheert in uw Adobe Admin Console**, kan de Adobe uw toestemming vragen om gebruikers automatisch naar uw bestaande console te migreren. Klik op de knop **Aan de slag** in de e-mail om naar de toestemmingspagina te navigeren.

Er is momenteel geen wijziging in het gebruikersbeheer. Workfront-beheerders blijven gebruikers in Workfront beheren en gebruikers blijven zich aanmelden met hun Workfront-id of SSO totdat de gebruikersmigratie is voltooid.

### Gebruikersmigratie plannen

Nadat de systeembeheerder de voorwaarden voltooit die in de vorige sectie worden geschetst, zal de Adobe automatisch uw gebruikersmigratie plannen 30 dagen nadat deze eerste vereisten volledig zijn, en zal met de beheerders van het Profiel van het Product van Workfront (de beheerders van het Systeem van Workfront) communiceren om de gebruikersmigratie te beheren.

Workfront-productprofielbeheerders (Workfront-systeembeheerders) zullen:

* Een e-mail ontvangen met de geplande begindatum voor migratie van gebruikers (ongeveer 30 dagen nadat aan deze voorwaarden is voldaan)
* Toegang verkrijgen tot de aangewezen Workfront-beheerconsole, waar ze de migratiedatum kunnen wijzigen

  >[!NOTE]
  >
  >Vanwege de complexiteit van de migratie zijn datumwijzigingen beperkt tot maximaal 30 dagen na de geplande datum. Neem contact op met de technische ondersteuning als u een latere datum nodig hebt.

* Ontvang een herinnering per e-mail 1 dag vóór de Begindatum van de migratie van de Gebruiker

### Gebruikers voorbereiden voor migratiedag

Als beheerder van het Productprofiel van Workfront (de beheerder van het Systeem van Workfront), zijn verantwoordelijk voor het verzekeren van alle gebruikers voor migratiedag worden voorbereid.

* Bereid alle gebruikers voor de aanstaande migratie aan Identiteit van de Adobe voor door hen van het volgende op de hoogte te brengen:.

   * Terwijl gebruikers migreren, ontvangen ze een e-mail van de Adobe waarin ze op de hoogte worden gesteld van de wijziging in de manier waarop ze zich aanmelden bij Workfront. Gebruikers worden uitgenodigd een uitnodiging om zich voor het eerst aan te melden met Adobe Identity te accepteren, door zich aan te melden met een bestaande Adobe ID of door een nieuwe uitnodiging in te stellen met hetzelfde e-mailadres.

### Wat verwacht u op de migratiedag

* **De migratie van gebruikers begint om middernacht van het Workfront Datacenter dat als host fungeert voor de klant.**

* **Adobe migreert eerst automatisch Workfront-beheerders.** Wanneer Workfront-beheerders worden gemigreerd naar Adobe Identity, krijgen zij de rol van beheerder van het productprofiel van de Adobe (Workfront System Administrator) toegewezen. Bestaande rollen die een gebruiker vóór de migratie kan hebben, worden niet beïnvloed.

  >[!NOTE]
  >
  >Tijdens de migratie van gebruikers zal de toegang tot het product niet verloren gaan. Als een gebruiker tijdens de migratie van zijn gebruiker is aangemeld, heeft dit geen invloed. Bij hun volgende aanmelding moeten ze echter hun Adobe-id gebruiken.



* **Terwijl gebruikers worden gemigreerd, ontvangen ze een e-mail van de Adobe waarin ze op de hoogte worden gesteld van de wijziging in de manier waarop ze zich aanmelden bij Workfront.** Gebruikers worden uitgenodigd een uitnodiging om zich voor het eerst aan te melden met Adobe Identity te accepteren, door zich aan te melden met een bestaande Adobe ID of door een nieuwe Adobe ID in te stellen met hetzelfde e-mailadres.

  Ga voor informatie over hoe u zich bij Workfront kunt aanmelden met een Adobe ID naar [Aanmelden bij Adobe Experience Cloud](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud).

### Migratie van gebruiker voltooid

Adobe stelt alle systeembeheerders en productprofielbeheerders (Workfront System beheerders) via e-mail op de hoogte nadat alle beheerders en gebruikers zijn gemigreerd. Op dit moment zullen alle Workfront-gebruikers voor die instantie zich aanmelden bij Workfront met Adobe Identity. Systeembeheerders van Workfront en beheerders van productprofielen (Workfront-systeembeheerders) kunnen gebruikerstoegang in de Adobe Admin Console beheren. Als klanten geen vorm van foldersynchronisatie binnen de beheerderconsole gebruiken, kunnen zij toegang tot Workfront binnen de Toepassing van Workfront blijven beheren.

## Ondersteuning

Volg voor vragen of problemen de stappen die in het artikel worden beschreven [Contact opnemen met Klantenondersteuning](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).




