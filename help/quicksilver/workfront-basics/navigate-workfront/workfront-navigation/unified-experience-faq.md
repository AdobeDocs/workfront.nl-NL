---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Veelgestelde vragen over Adobe Unified Experience
description: Enkele functies verschillen van [!DNL Workfront] en Adobe Experience Cloud, en je hebt misschien vragen zoals je [!DNL Workfront] -instantie wordt gemigreerd naar de uniforme ervaring.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 019a1b61cd97d5d61f9a4fbf3f98eccab50809a8
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] Veelgestelde vragen

De [!DNL Adobe Unified Experience] for [!DNL Workfront] staat u toe om al uw [!DNL Adobe] toepassingen op één plaats met één enkele login. De [!DNL Adobe] het navigatiegebied is naadloos geïntegreerd met [!DNL Workfront]. Een aantal functies verschillen en u hebt wellicht enkele vragen als uw [!DNL Workfront] -instantie wordt gemigreerd naar de uniforme ervaring.

Voor informatie over hoe u zich bij de [!DNL Adobe Unified Experience], zie [[!DNL Adobe Unified Experience] for [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Vergelijking van [!DNL Adobe Unified Experience] en [!DNL Workfront only] ervaring

Alleen klanten die de [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] heeft toegang tot [!DNL Adobe Unified Experience]. Klanten die nog niet zijn gemigreerd, zien de [!DNL Workfront only] ervaring, zonder de mogelijkheid om te schakelen tussen [!DNL Adobe] toepassingen.

In deze tabel worden enkele functies beschreven die verschillen tussen de twee ervaringen.

| [!DNL Adobe Unified Experience] | [!DNL Workfront] alleen ervaring |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Main Menu] staat links ![Hoofdmenu](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Main Menu] staat aan de rechterkant ![Hoofdmenu](assets/main-menu-icon.png) |
| Eén aanmeldings-URL is beschikbaar voor alle [!DNL Adobe Experience Cloud] toepassingen | Aanmelden bij [!DNL Workfront] met een aangepaste [!DNL Workfront] URL |
| Met een &quot;organisatieswitch&quot; kunt u schakelen tussen [!DNL Workfront] organisaties en omgevingen | De &quot;organisatieschakeloptie&quot; is niet beschikbaar |
| Navigatie omvat een navigatiegebied van het hoogste niveau voor [!DNL Adobe] producten, [!DNL Adobe] meldingen, Help en uw gebruikersprofiel, naast de [!DNL Workfront] navigatiebalk | Navigatie omvat de [!DNL Workfront] alleen navigatiebalk |
| De Help is toegankelijk via de [!UICONTROL Main Menu] en het bovenste navigatiegebied | De Help is toegankelijk via de [!UICONTROL Main Menu] en [!DNL Workfront] navigatiebalk |

{style="table-layout:auto"}

## Veelgestelde vragen

### Hoe kan ik bepalen of ik Adobe Verenigde Ervaring of Adobe Workfront gebruik?

Om te bepalen of uw organisatie op de Adobe Verenigde Ervaring is, onderzoek URL die u gebruikt om tot Workfront toegang te hebben.

| URL | Ervaring met Adobe |
|------------|------------|
| (Bedrijfsnaam).my.workfront.com | Workfront-ervaring |
| experience.adobe.com | Adobe Unified Experience |

### Hoe kan ik meer leren over de [!DNL Adobe Admin Console]?

Voor informatie over de [!DNL Admin Console]Lees de volgende artikelen:

* [Voorbereiden op de [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Verschillen in beheer op basis van platforms ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] overzicht](https://helpx.adobe.com/nl/enterprise/using/admin-console.html)

### Wat moet ik als klant doen om de migratie te vergemakkelijken?

Er wordt contact opgenomen met bestaande klanten om migraties te plannen. De collega&#39;s van de steun van het migratieteam zullen klanten door het proces lopen, adviseren over [!DNL Admin Console] instellen en koppelingen verschaffen naar documentatie die nodig is om de beweging zo eenvoudig en probleemloos mogelijk te maken.

* [[!DNL Adobe Workfront] Ondersteuningsoverzicht](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] informatie](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] en [!DNL Admin Console] Veelgestelde vragen](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

### Hoe omgaat u met [!DNL Adobe Admin Console] voor bedrijven die dit al hebben ingeschakeld voor gefedereerde id&#39;s anders dan [!DNL Workfront] SSO is ingesteld?

[!DNL Adobe Admin Console] heeft de optie om [!DNL Workfront], waarbij SSO wordt vervangen door IMS. Alle gebruikersprovisioning vindt plaats in het dialoogvenster [!DNL Admin Console]en de gebruikers de [!DNL Adobe] aanmeldingsscherm om [!DNL Experience Cloud] waar zij zullen zien [!DNL Workfront] als optie (als zij toegang krijgen tot het netwerk).

### Hoe beïnvloedt dit klanten die reeds het AEM beheerpaneel voor hebben [!DNL Adobe Assets] - maar de SSO is anders geconfigureerd dan [!DNL Workfront?]

Eenmaal [!DNL Workfront] wordt toegevoegd als een [!DNL Admin Console] toepassing, moet u niets anders doen [!DNL Workfront] om de bestaande SSO-instelling te benutten die u hebt [!DNL Adobe Assets].

### Hoe beïnvloedt dit degenen die met SSO worden opgezet?

SSO is ingesteld in het dialoogvenster [!DNL Admin Console] en door de [!DNL Workfront] toepassing.

### Is SSO met onze interne [!DNL Active Directory] nog steeds een optie met IMS?

IMS is een vervanging voor SSO en functies die meestal hetzelfde zijn. Alle gebruikerstoestemmingen worden verleend en provisioned in [!DNL Adobe Admin Console]en ziet de gebruiker de [!DNL Adobe] aanmeldingsscherm waar ze kunnen kiezen &quot;[!UICONTROL Personal Account]&quot; of &quot;[!UICONTROL Company Account]&quot; aan login (als u hebt [!DNL Active Directory], zullen de meesten login met een bedrijfrekening).

### Voor degenen die geen SSO gebruiken, doet het [!DNL Workfront] wijziging aanmeldings-URL?

De aanmeldings-URL wordt gewijzigd. De oude URL wordt echter doorgestuurd naar de nieuwe aanmeldings-URL, zodat u de gebruikers opnieuw moet trainen waar ze naartoe moeten.

### Zullen aliassen die we hebben ingesteld nog steeds werken, of zijn de [!DNL Workfront] koppelingen die veranderen met deze migratie?

[!DNL Workfront] Er zijn omleidingen/aliassen beschikbaar om naar de startpagina te gaan.

### Zal er een tijd zijn waarin de omleidingen zijn uitgeschakeld? Of kunnen we altijd in my.company.workfront.com typen?

U kunt altijd aangepaste URL&#39;s gebruiken. Nadat u op een van deze koppelingen hebt geklikt, wordt u doorgestuurd naar [!DNL Workfront] en een andere URL tonen. Het is echter beter [!DNL experience] om u aan te melden bij experience.adobe.com, en bladwijzerkoppelingen van binnenuit [!DNL Experience Cloud]. Minder omleiding betekent minder vertraging/laadtijd.

### Zullen directe verbindingen aan verzoekrijen worden gebroken?

Alle directe koppelingen moeten worden omgeleid naar de nieuwe URL-patronen. Als u echter koppelingen naar personen hebt gedistribueerd, moet u een update verzenden om de directe koppeling te benutten en vertragingen bij het bereiken van de verwachte pagina te voorkomen.

### Zullen we migreren naar [!DNL Experience Cloud] wereldwijd of kunnen we voor bepaalde gebruikers kiezen ( niet alle gebruikers gebruiken zelfs andere Adobe producten ) ?

De gehele [!DNL Workfront] klantaccount wordt gemigreerd. Dit kan niet per gebruiker gebeuren.

### Will all [!DNL Workfront] gebruikers moeten zich aanmelden via [!DNL Experience Cloud]? Of alleen beheerders?

Ja, alle gebruikers kunnen zich aanmelden via [!DNL Experience Cloud]. De IMS-aanmelding vervangt de SSO. Het is een zeer gelijkaardige ervaring, enkel een verschillend login scherm.

### Zullen gebruikers hun [!DNL Adobe] rekeningen aan hun [!DNL Workfront] of ze beide al hebben?

Ja, er is een proces voor dit, en meer details zullen worden verstrekt wanneer het tijd voor uw organisatie is om zich aan IMS te bewegen.

### Wat gebeurt er met de [!DNL Workfront] gebruikers die geen [!DNL Adobe] account?

Gebruikers die geen toegang hebben gekregen in [!DNL Adobe Admin Console] om in te gaan [!DNL Workfront] moet een &quot;[!UICONTROL personal account]&quot; of een [!DNL Adobe] ID-account om u aan te kunnen melden. Dit verzendt een e-mail naar de beheerder om hun verzoek goed te keuren of te verwerpen, en het laat extra admin toe om te vormen welk type van toegang die gebruiker heeft. Wanneer ze zich aanmelden, gaan ze naar experience.adobe.com, voeren ze hun e-mailadres in en kiezen [!UICONTROL Personal Account]. Vanaf dat moment kunnen ze toegang krijgen [!DNL Workfront].

### Wat gebeurt er als we geen [!DNL Adobe] andere producten dan [!DNL Workfront?]

Het wordt nog steeds aanbevolen dat uw organisatie naar de [!DNL Adobe Unified Experience]. U ontvangt een [!DNL Adobe] ID en de hierboven vermelde voordelen.

### We hebben externe gebruikers opgenomen in onze [!DNL Workfront] -instantie. Wij zouden niet willen dat zij toegang hebben tot andere producten inbegrepen in [!DNL Adobe]. Hoe zouden wij hun toegang binnen de console beperken?

[!DNL Admin Console] geeft beheerders veel controle over wat de gebruikers kunnen en kunnen toegang hebben. Wanneer een externe gebruiker toegang wil, moet hij een [!DNL Adobe] ID, die een e-mail naar de beheerder verzendt. De beheerder kan dan toegang tot een product goedkeuren of verwerpen en bepalen wat zij kunnen/niet tot voor producten kunnen toegang hebben die door die organisatie worden bezeten. Vervolgens worden de [!DNL Workfront] Systeembeheerder kan naar de [!UICONTROL Users] gebied van [!DNL Workfront] om het even welke meer korrelige toestemmingen voor de externe gebruiker te maken.

### Groepbeheerders worden gebruikt om personen te maken in [!DNL Workfront]. Met de overgang naar [!DNL Experience Cloud], zullen groepsbeheerders nog steeds mensen kunnen aanmaken?

Ja, het maken van gebruikers is nog steeds mogelijk via [!DNL Workfront]. Deze gebruikers kunnen worden toegevoegd aan [!DNL Experience Cloud] automatisch. U kunt ook groepsbeheerders instellen als producteigenaars in het dialoogvenster [!DNL Admin Console] om hen toe te staan om [!DNL Workfront] aan gebruikers.

### Wat is de deadline om over te schakelen naar [!DNL Experience Cloud]?

Er is momenteel geen deadline voor het verplaatsen naar [!DNL Adobe Experience Cloud]. We werken samen met klanten om ze te laten kiezen wanneer ze klaar zijn om de stap te zetten.

### Moet ons ondersteuningsteam iets doen voor deze wijziging?

Als het ondersteuningsteam verantwoordelijk is voor het maken van nieuwe gebruikers, moeten zij vertrouwd raken met het [!DNL Admin Console] interfaces die worden gebruikt om gebruikers te maken en een machtiging aan Workfront toe te wijzen. Anders is er waarschijnlijk geen belangrijke wijziging voor uw interne ondersteuningsteam.

### Hoe beïnvloedt deze integratie wij door de API functie?

Het bestaande URL-pad blijft beschikbaar voor API-verkeer. U zou niets moeten doen om de eindpunten in uw integratie bij te werken. Directe aanmelding via gebruikersnaam en wachtwoord wordt echter niet ondersteund - u moet een API-sleutel gebruiken, met als uitzondering [!DNL Workfront Fusion] connectors.

### Wat over [!DNL Creative Cloud] gebruikers? Hoe beïnvloedt de migratie hen? Zijn er voordelen voor hen?

Er zijn geen gevolgen voor [!DNL Creative Cloud] gebruikers met de migratie naar [!DNL Adobe Unified Experience].

### Will logins change for [!DNL Workfront] mobiele gebruikers?

[!DNL Workfront] mobiele gebruikers mogen niet worden beïnvloed door de migratie naar [!DNL Adobe Unified Experience].
