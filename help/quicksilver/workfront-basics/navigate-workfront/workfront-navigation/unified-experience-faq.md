---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Veelgestelde vragen over Adobe Unified Experience
description: Enkele eigenschappen zijn verschillend tussen  [!DNL Workfront]  en Adobe Experience Cloud, en u zou sommige vragen kunnen hebben aangezien uw  [!DNL Workfront]  instantie aan de verenigde ervaring wordt gemigreerd.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 4ce69180b8f419ff5634d0dba802f9fb57cd758b
workflow-type: tm+mt
source-wordcount: '1378'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] Veelgestelde vragen

Met [!DNL Adobe Unified Experience] for [!DNL Workfront] kunt u al uw [!DNL Adobe] -toepassingen op één locatie beheren met één aanmelding. Het navigatiegebied van [!DNL Adobe] wordt naadloos geïntegreerd met [!DNL Workfront] . Enkele functies verschillen en u hebt mogelijk enkele vragen omdat uw [!DNL Workfront] -instantie naar de uniforme ervaring wordt gemigreerd.

Voor informatie over hoe te login aan [!DNL Adobe Unified Experience], zie [[!DNL Adobe Unified Experience]  voor  [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Vergelijking van [!DNL Adobe Unified Experience] - en [!DNL Workfront only] -ervaring

Alleen klanten die [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] gebruiken, hebben toegang tot de [!DNL Adobe Unified Experience] . Klanten die nog niet zijn gemigreerd, zien de [!DNL Workfront only] -ervaring zonder dat ze tussen [!DNL Adobe] -toepassingen kunnen schakelen.

In deze tabel worden enkele functies beschreven die verschillen tussen de twee ervaringen.

| [!DNL Adobe Unified Experience] | [!DNL Workfront] alleen ervaring |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Main Menu] is op het linker![&#x200B; Belangrijkste Menu &#x200B;](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Main Menu] is op het juiste ![&#x200B; Belangrijkste Menu &#x200B;](assets/main-menu-icon.png) |
| Er is één aanmeldings-URL beschikbaar voor alle [!DNL Adobe Experience Cloud] -toepassingen | Meld u aan bij [!DNL Workfront] met een aangepaste [!DNL Workfront] URL |
| Met een &quot;bedrijfsswitch&quot; kunt u schakelen tussen [!DNL Workfront] organisaties en omgevingen | De &quot;organisatieschakeloptie&quot; is niet beschikbaar |
| Navigatie omvat een navigatiegebied op hoofdniveau voor [!DNL Adobe] -producten, [!DNL Adobe] -meldingen, Help en uw gebruikersprofiel, naast de navigatiebalk van [!DNL Workfront] | Navigatie bevat alleen de navigatiebalk van [!DNL Workfront] |
| De Help is toegankelijk via het navigatiegebied [!UICONTROL Main Menu] en boven. | De Help is toegankelijk via de navigatiebalk [!UICONTROL Main Menu] en [!DNL Workfront] |
| De proefdrukviewer wordt geopend op een nieuw tabblad | De proefdrukviewer wordt geopend in Workfront |
| URL voor toegang tot Workfront is `experience.adobe.com` | URL voor toegang tot Workfront is `(CompanyName).my.workfront.adobe.com` |
| Datumnotatie (zoals MM/DD/JJJJ) is gebaseerd op de taalinstellingen voor Unified Experience. Als de gebruiker zijn taalinstellingen niet heeft bijgewerkt, worden `en-US` -instellingen gebruikt. | De datumnotatie (zoals DD-MM-JJJJ) is gebaseerd op de browservoorkeuren |

{style="table-layout:auto"}

## Veelgestelde vragen

### Hoe kan ik bepalen of ik Adobe Unified Experience of Adobe Workfront gebruik?

Om te bepalen of uw organisatie op de Adobe Verenigde Ervaring is, onderzoek URL die u gebruikt om tot Workfront toegang te hebben.

| URL | Adobe-ervaring |
|------------|------------|
| (Bedrijfsnaam).my.workfront.com | Workfront-ervaring |
| experience.adobe.com | Adobe Unified Experience |

### Hoe kan ik meer leren over de [!DNL Adobe Admin Console] ?

Lees de volgende artikelen voor meer informatie over [!DNL Admin Console] :

* [Voor  [!DNL Adobe Admin Console] voorbereiden](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Op platform-gebaseerde beleidsverschillen ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console]  overzicht &#x200B;](https://helpx.adobe.com/nl/enterprise/using/admin-console.html)

### Wat moet ik als klant doen om de migratie te vergemakkelijken?

Er wordt contact opgenomen met bestaande klanten om migraties te plannen. De collega&#39;s die ondersteuning bieden voor het migratieteam zullen klanten door het proces laten lopen, advies geven over [!DNL Admin Console] -installatie en koppelingen verschaffen naar documentatie die nodig is om de stap zo eenvoudig en probleemloos mogelijk te maken.

* [[!DNL Adobe Workfront]  Overzicht van de Steun &#x200B;](https://experienceleague.adobe.com/en/docs/support-resources/adobe-support-tools-guide/workfront/overview)
* [[!DNL Adobe Business Platform]  en  [!DNL Admin Console]  Veelgestelde vragen &#x200B;](https://experienceleague.adobe.com/en/docs/support-resources/adobe-support-tools-guide/workfront/faq)

### Hoe gaat u met [!DNL Adobe Admin Console] voor bedrijven die dit al hebben ingeschakeld voor gefedereerde id&#39;s anders dan met [!DNL Workfront] SSO is ingesteld?

[!DNL Adobe Admin Console] heeft de optie om [!DNL Workfront] op te nemen, waarbij SSO wordt vervangen door Adobe Identity Management System (IMS). Alle gebruikersprovisioning vindt plaats in [!DNL Admin Console] en gebruikers zien het [!DNL Adobe] aanmeldingsscherm om [!DNL Experience Cloud] te bereiken waar ze [!DNL Workfront] als optie zien (als ze toegang krijgen tot dit scherm).

### Hoe beïnvloedt dit klanten die reeds het AEM admin paneel voor [!DNL Adobe Assets] hebben - maar SSO wordt gevormd verschillend dan [!DNL Workfront?]

Als [!DNL Workfront] eenmaal is toegevoegd als een [!DNL Admin Console] -toepassing, hoeft u niets anders te doen om [!DNL Workfront] de bestaande SSO-instelling die u voor [!DNL Adobe Assets] hebt, te kunnen gebruiken.

### Hoe beïnvloedt dit degenen die met SSO worden opgezet?

SSO wordt ingesteld in de [!DNL Admin Console] en overgeërfd door de [!DNL Workfront] -toepassing.

### Is SSO met onze interne [!DNL Active Directory] nog steeds een optie met Adobe Identity Management System (IMS)?

IMS is een vervanging voor SSO en functies die meestal hetzelfde zijn. Alle gebruikerstoestemmingen worden verleend en provisioned in [!DNL Adobe Admin Console], en de gebruiker zal het [!DNL Adobe] login scherm zien waar zij &quot; [!UICONTROL Personal Account]&quot;kunnen kiezen of &quot; [!UICONTROL Company Account]&quot;aan login (als u [!DNL Active Directory] hebt, zullen de meesten login met een bedrijfrekening).

### Worden de aanmeldings-URL van [!DNL Workfront] gewijzigd voor gebruikers die geen SSO gebruiken?

De aanmeldings-URL wordt gewijzigd. De oude URL wordt echter doorgestuurd naar de nieuwe aanmeldings-URL, zodat u de gebruikers opnieuw moet trainen waar ze naartoe moeten.

### Werken aliassen die we hebben ingesteld nog steeds of veranderen de [!DNL Workfront] -koppelingen met deze migratie?

Er zijn [!DNL Workfront] omleidingen/aliassen beschikbaar om naar de startpagina te gaan.

### Zal er een tijd zijn waarin de omleidingen zijn uitgeschakeld? Of kunnen we altijd in my.company.workfront.com typen?

U kunt altijd aangepaste URL&#39;s gebruiken. Nadat u op een van deze koppelingen hebt geklikt, wordt u naar [!DNL Workfront] geleid en wordt een andere URL weergegeven. Het is echter beter [!DNL experience] om u aan te melden bij experience.adobe.com en bladwijzerkoppelingen te maken vanuit [!DNL Experience Cloud] . Minder omleiding betekent minder vertraging/laadtijd.

### Zullen directe verbindingen aan verzoekrijen worden gebroken?

Alle directe koppelingen moeten worden omgeleid naar de nieuwe URL-patronen. Als u echter koppelingen naar personen hebt gedistribueerd, moet u een update verzenden om de directe koppeling te benutten en vertragingen bij het bereiken van de verwachte pagina te voorkomen.

### Zullen we migreren naar [!DNL Experience Cloud] wereldwijd of kunnen we voor bepaalde gebruikers kiezen (niet alle gebruikers gebruiken zelfs andere Adobe-producten)?

De gehele [!DNL Workfront] klantenaccount wordt gemigreerd. Dit kan niet per gebruiker gebeuren.

### Moeten alle [!DNL Workfront] -gebruikers zich aanmelden via [!DNL Experience Cloud] ? Of alleen beheerders?

Ja, alle gebruikers kunnen zich aanmelden via [!DNL Experience Cloud] . De aanmelding bij Adobe Identity Management System (IMS) vervangt SSO. Het is een zeer gelijkaardige ervaring, enkel een verschillend login scherm.

### Moeten gebruikers hun [!DNL Adobe] -accounts koppelen aan hun [!DNL Workfront] -accounts als ze beide al hebben?

Ja, er is een proces voor dit, en meer details zullen worden verstrekt wanneer het tijd voor uw organisatie is om zich aan IMS te bewegen.

### Wat gebeurt er met [!DNL Workfront] -gebruikers die geen [!DNL Adobe] -account hebben?

Gebruikers die geen toegang hebben gekregen in [!DNL Adobe Admin Console] om lid te worden van [!DNL Workfront] , moeten een &quot;[!UICONTROL personal account]&quot;- of [!DNL Adobe] id-account maken om zich aan te melden. Dit verzendt een e-mail naar de beheerder om hun verzoek goed te keuren of te verwerpen, en het laat extra admin toe om te vormen welk type van toegang die gebruiker heeft. Wanneer ze zich aanmelden, gaan ze naar experience.adobe.com, voeren ze hun e-mailadres in en kiezen ze [!UICONTROL Personal Account] . Vanaf dat punt hebben ze toegang tot [!DNL Workfront] .

### Wat gebeurt er als we geen andere [!DNL Adobe] -producten hebben dan [!DNL Workfront?]

Het wordt nog steeds aangeraden dat uw organisatie migreert naar [!DNL Adobe Unified Experience] . U ontvangt een [!DNL Adobe] -id samen met de bovenstaande voordelen.

### We hebben externe gebruikers opgenomen in ons [!DNL Workfront] -exemplaar. We zouden niet willen dat ze toegang hebben tot andere producten die in [!DNL Adobe] zijn opgenomen. Hoe zouden wij hun toegang binnen de console beperken?

[!DNL Admin Console] geeft beheerders veel controle over wat gebruikers kunnen en kunnen benaderen. Wanneer een externe gebruiker toegang wil, moet hij of zij een [!DNL Adobe] id maken die een e-mail naar de beheerder stuurt. De beheerder kan dan toegang tot een product goedkeuren of verwerpen en bepalen wat zij kunnen/niet tot voor producten kunnen toegang hebben die door die organisatie worden bezeten. Vervolgens kan de [!DNL Workfront] Systeembeheerder naar het [!UICONTROL Users] gebied [!DNL Workfront] gaan om gedetailleerdere machtigingen voor de externe gebruiker te maken.

### Groepbeheerders worden gebruikt om personen te maken in [!DNL Workfront] . Zullen groepbeheerders met de verplaatsing naar [!DNL Experience Cloud] nog steeds personen kunnen maken?

Ja, het maken van gebruikers is nog steeds mogelijk via [!DNL Workfront] . Deze gebruikers kunnen automatisch aan [!DNL Experience Cloud] worden toegevoegd. U kunt uw groepbeheerders ook instellen als producteigenaars in de [!DNL Admin Console] , zodat ze [!DNL Workfront] aan gebruikers kunnen toewijzen.

### Wat is de deadline om over te schakelen naar [!DNL Experience Cloud]?

Er is momenteel geen deadline om naar [!DNL Adobe Experience Cloud] te gaan. We werken samen met klanten om ze te laten kiezen wanneer ze klaar zijn om de stap te zetten.

### Moet ons ondersteuningsteam iets doen voor deze wijziging?

Als het ondersteuningsteam verantwoordelijk is voor het maken van nieuwe gebruikers, moeten deze gebruikers vertrouwd raken met de [!DNL Admin Console] -interfaces die worden gebruikt om gebruikers te maken en een machtiging aan Workfront toe te wijzen. Anders is er waarschijnlijk geen belangrijke wijziging voor uw interne ondersteuningsteam.

### Hoe beïnvloedt deze integratie wij door de API functie?

Het bestaande URL-pad blijft beschikbaar voor API-verkeer. U zou niets moeten doen om de eindpunten in uw integratie bij te werken. Directe aanmelding via gebruikersnaam en wachtwoord wordt echter niet ondersteund. U moet een API-sleutel gebruiken, met als uitzondering [!DNL Workfront Fusion] -connectors.

### En [!DNL Creative Cloud] gebruikers? Hoe beïnvloedt de migratie hen? Zijn er voordelen voor hen?

[!DNL Creative Cloud] -gebruikers hebben geen invloed op de migratie naar [!DNL Adobe Unified Experience] .

### Worden aanmeldingsgegevens voor [!DNL Workfront] mobiele gebruikers gewijzigd?

[!DNL Workfront] mobiele gebruikers mogen niet worden beïnvloed door de migratie naar [!DNL Adobe Unified Experience] .

### JumpSeat werkt niet met de [!DNL Adobe Unified Experience] , hoe los ik dit op?

JumpSeat werkt met [!DNL Adobe Unified Experience], maar vereist een configuratieupdate. Wijzig de toepassings-URL met behulp van het JumpSeat-beheerdeelvenster van `workfront.com` om te eindigen met `.workfront.adobe.com`
