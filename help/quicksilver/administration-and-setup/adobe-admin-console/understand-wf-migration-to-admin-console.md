---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: De Workfront-migratie naar de Adobe Admin Console begrijpen
description: Dit artikel beschrijft in algemene termen het proces om een organisatie naar Adobe Admin Console te bewegen, zodat u als beheerder van Workfront kunt weten wat te verwachten.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '1114'
ht-degree: 0%

---

# De Workfront-migratie naar de Adobe Admin Console begrijpen

Adobe wijzigt de manier waarop u uw Adobe Workfront-gebruikers beheert, waardoor u en uw organisatie meer productiviteit krijgen. Als onderdeel van deze wijziging migreert Adobe uw Workfront-exemplaar en gebruikers naar de Adobe Admin Console. Dit is een noodzakelijke migratie en heeft geen invloed op rapporten, goedkeuringspaden, inhoud of elementen. Dit is van invloed op de manier waarop u gebruikerstoegang beheert en de manier waarop uw gebruikers zich aanmelden.

Dit artikel beschrijft in algemene termen het proces om een organisatie naar Adobe Admin Console te bewegen, zodat u als beheerder van Workfront kunt weten wat te verwachten.

Leren hoe u Adobe Admin Console kunt gebruiken om uw rechten van Adobe over uw volledige organisatie te beheren, zie [ gebruikers in Adobe Admin Console ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md) leiden.

## Wat verandert er?

Als onderdeel van de migratie gaat uw gebruikersbeheer van de Workfront-toepassing naar de Adobe Admin Console, met de volgende beheertaken:

* **de beheerders van het Systeem** zijn super gebruikers met voorrechten van alle beheerders. Zij wijzen alle administratieve rollen toe, en leiden gebruikers voor de volledige organisatie voor alle producten.

* **de beheerders van het Profiel van het Product (het systeembeheerders van Workfront)** beheren welke gebruikers in de organisatie toegang tot Workfront krijgen.

* **de Gebruikers zullen binnen met de Identiteit van Adobe ondertekenen.** Nadat Adobe bestaande gebruikers heeft gemigreerd naar de Adobe Admin Console, zullen gebruikers zich aanmelden bij hun Workfront-instanties met hun nieuwe Adobe Identity - een Adobe ID of Adobe Federated ID (SSO).

* **Er is geen verandering in hoe u alle andere functionaliteit** binnen de toepassing van Workfront zelf, met inbegrip van beheer van eigenschappen, gebruikersrollen, werkruimten, functionaliteit, en gedrag beheert.

## Tijdlijn migratiepad

Adobe migreert uw Workfront-exemplaar eerst naar de Adobe Admin Console en migreert vervolgens alle bestaande gebruikers met geverifieerde e-mailadressen. Als u systeembeheerder of beheerder van het Productprofiel van Workfront (de beheerder van het Systeem van Workfront) bent, zult u e-mail ontvangen die u door de migratiereis begeleidt. Hier volgt een tijdlijn van wat u kunt verwachten:

### Workfront-migratie naar Adobe Admin Console voltooid

Systeembeheerders ontvangen een e-mail wanneer de migratie van Workfront naar Adobe Admin Console is voltooid. Op dit ogenblik, kunnen de beheerders van het Systeem sommige vereiste stappen **moeten voltooien alvorens de gebruikersmigratie** begint, om invloed aan de gebruikers van Workfront te minimaliseren.

* **als uw gebruikers van Workfront momenteel login met SSO**, u opstelling SSO op Adobe Admin Console zodat kunnen uw gebruikers blijven het programma openen met SSO. Als uw Workfront-gebruikers momenteel geen SSO gebruiken, maar u wilt deze instellen op Adobe Admin Console, kunt u dit op dit moment doen tijdens de migratiereis.
* **als u reeds andere producten van Adobe in uw Adobe Admin Console** beheert, kan Adobe uw toestemming vragen om gebruikers aan uw bestaande console automatisch te migreren. Klik **krijgen Begonnen** knoop in e-mail om aan de toestemmingspagina te navigeren.
* **als u eerder het de vergunningstype van de Aanvrager** hebt geschrapt, zal het aan uw systeem worden toegevoegd. Er worden geen gebruikers toegewezen aan dit licentietype, maar dit is nodig voor de synchronisatie tussen Workfront en de Adobe Admin Console. U hoeft geen actie te ondernemen met betrekking tot het type licentie voor de aanvrager.

Er is momenteel geen wijziging in het gebruikersbeheer. Workfront-beheerders blijven gebruikers in Workfront beheren en gebruikers blijven zich aanmelden met hun Workfront-id of SSO totdat de gebruikersmigratie is voltooid.

### Gebruikersmigratie plannen

Nadat de systeembeheerder de voorwaarden voltooit die in de vorige sectie worden beschreven, zal Adobe automatisch uw gebruikersmigratie plannen gedurende 30 dagen nadat deze voorwaarden volledig zijn, en zal met de beheerders van het Profiel van het Product van Workfront (de beheerders van het Systeem van Workfront) communiceren om de gebruikersmigratie te beheren.

Workfront-productprofielbeheerders (Workfront-systeembeheerders) zullen:

* Een e-mail ontvangen met de geplande begindatum voor migratie van gebruikers (ongeveer 30 dagen nadat aan deze voorwaarden is voldaan)
* Toegang verkrijgen tot de aangewezen Workfront-beheerconsole, waar ze de migratiedatum kunnen wijzigen

  >[!NOTE]
  >
  >Vanwege de complexiteit van de migratie zijn datumwijzigingen beperkt tot maximaal 30 dagen na de geplande datum. Neem contact op met de technische ondersteuning als u een latere datum nodig hebt.

* Ontvang een herinnering per e-mail 1 dag vóór de Begindatum van de migratie van de Gebruiker

### Gebruikers voorbereiden voor migratiedag

Als beheerder van het Productprofiel van Workfront (de beheerder van het Systeem van Workfront), zijn verantwoordelijk voor het verzekeren van alle gebruikers voor migratiedag worden voorbereid.

* Bereid alle gebruikers voor op de komende migratie naar Adobe Identity door hen van het volgende op de hoogte te brengen:

   * Als gebruikers migreren, ontvangen ze een e-mail van Adobe waarin ze op de hoogte worden gesteld van de wijziging in de manier waarop ze zich aanmelden bij Workfront. Gebruikers worden uitgenodigd om voor het eerst een uitnodiging voor aanmelding met Adobe Identity te accepteren, hetzij door u aan te melden met een bestaande Adobe ID, hetzij door een nieuwe uitnodiging met hetzelfde e-mailadres in te stellen.

### Wat verwacht u op de migratiedag

* **de migratie van de Gebruiker zal bij middernacht van het ontvangen Workfront Datacenter van de klant beginnen.**

* **Adobe zal automatisch eerst de beheerders van Workfront migreren.** Wanneer Workfront-beheerders worden gemigreerd naar Adobe Identity, krijgen ze de rol Adobe Product Profile Administrator (Workfront System Administrator) toegewezen. Bestaande rollen die een gebruiker vóór de migratie kan hebben, worden niet beïnvloed.

  >[!NOTE]
  >
  >Tijdens de migratie van gebruikers zal de toegang tot het product niet verloren gaan. Als een gebruiker tijdens de migratie van zijn gebruiker is aangemeld, heeft dit geen invloed. Als ze zich opnieuw aanmelden, moeten ze echter hun Adobe-identiteit gebruiken.



* **aangezien de gebruikers worden gemigreerd, zullen zij een e-mail van Adobe ontvangen die hen op de hoogte brengt van de verandering in de manier zij binnen aan Workfront ondertekenen.** Gebruikers worden uitgenodigd een uitnodiging voor aanmelding met Adobe Identity voor het eerst te accepteren door u aan te melden met een bestaande Adobe ID of door een nieuwe Adobe ID in te stellen met hetzelfde e-mailadres.

  Voor informatie over hoe te om in Workfront met Adobe ID te registreren, zie [ Login aan Adobe Experience Cloud ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud).

### Migratie van gebruiker voltooid

Adobe stelt alle systeembeheerders en productprofielbeheerders (Workfront System beheerders) via e-mail op de hoogte nadat alle beheerders en gebruikers zijn gemigreerd. Op dit moment zullen alle Workfront-gebruikers voor die instantie zich aanmelden bij Workfront met Adobe Identity. Systeembeheerders van Workfront en beheerders van productprofielen (Workfront-systeembeheerders) kunnen gebruikerstoegang in de Adobe Admin Console beheren. Als klanten geen vorm van foldersynchronisatie binnen de beheerderconsole gebruiken, kunnen zij toegang tot Workfront binnen de Toepassing van Workfront blijven beheren.

## Ondersteuning

Voor vragen of zorgen gelieve de stappen te volgen die in het artikel [ worden geschetst de Steun van de Klant van het Contact ](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).




