---
product-area: documents
navigation-topic: approvals
title: AppBuilder in Workfront-documentgegevens
description: U kunt AppBuilder installeren via Documentdetails
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 74e0a85b-a8aa-4e39-9c2e-0f09957ebafa
source-git-commit: dcdae47ffd4a02ac9a0bbd3cd9bd1418f6c59e1a
workflow-type: tm+mt
source-wordcount: '1357'
ht-degree: 0%

---

# AppBuilder in Workfront-documentgegevens

U kunt AppBuilder installeren via Documentdetails.

## Vereisten

U moet het volgende hebben:

* Een Workfront-account voor IMS
* Een dev-machine met knooppunt v18 en npm

## Ontwikkelaars toevoegen aan de beheerconsole

>[!IMPORTANT]
>
>Controleer of u de juiste IMS-organisatie hebt geselecteerd voor alle volgende stappen. Als u tot veelvoudige organisaties behoort, is het mogelijk om verkeerde te selecteren. Let erop dat u onder de juiste organisatie werkt. Deze wordt meestal in de rechterbovenhoek weergegeven.


1. Navigeer naar een van de volgende opties:

* Stadium: [&#x200B; https://stage.adminconsole.adobe.com/](https://stage.adminconsole.adobe.com/)
* Prod: [&#x200B; https://adminconsole.adobe.com/](https://adminconsole.adobe.com/)

1. In de sectie van Gebruikers, klik **Ontwikkelaars** > **ontwikkelaars** toevoegen.

   ![&#x200B; leidt ontwikkelaars in Admin Console &#x200B;](assets/manage-users-admin-console.png)

   >[!NOTE]
   >
   >Als u geen optie ziet om Ontwikkelaars te beheren, hebt u geen product dat voor ontwikkelaars toegang toestaat. Workfront biedt ontwikkelaars geen toegang, maar AEM wel. Als u dit niet ziet, moeten we erachter komen hoe we Workfront kunnen opnemen in de lijst met toepassingen die ontwikkelaars toestaat.

1. Voeg de e-mail van de gebruiker toe. Het zou bestaande gebruikers moeten zoeken die reeds van binnen de admin console zijn toegevoegd.

1. Voeg noodzakelijke producten aan het ontwikkelaarprofiel toe, en klik **sparen**.

![&#x200B; voeg ontwikkelaar &#x200B;](assets/add-developer.png) toe

## Toegang tot AppBuilder verkrijgen

Organisaties moeten met hun accountmanagers samenwerken om AppBuilder te kunnen aanschaffen. Het exacte proces hiervoor is niet begrepen omdat we dit niet hoefden te doen voor de concepttest.

Als u de integratie met AppBuilder wilt testen, kunt u hier een gratis proefversie aanvragen voor IMS org:
[https://developer.adobe.com/app-builder/docs/overview/getting_access/#](https://developer.adobe.com/app-builder/docs/get_started/app_builder_get_started/set-up#access-and-credentials)

Ik heb de indruk dat hoewel het een gratis 30-daagse rechtszaak is, ze het proces na die tijd niet echt zullen deactiveren.

Als AppBuilder behoorlijk wordt gevormd, zou u &quot;project van malplaatje&quot;als deel van het creëren van een nieuw project moeten zien (dat in de volgende sectie wordt behandeld).

## Een nieuw project maken in de Dev Console

1. Klik **creeer project van malplaatje**.

   >[!IMPORTANT]
   >
   >Als deze optie niet wordt weergegeven, is de configuratie in de beheerconsole onjuist en hebt u geen toegang tot de catalogus van de App Builder. Deze optie wordt alleen weergegeven wanneer u toegang hebt tot AppBuilder.

   ![&#x200B; creeer project van malplaatje &#x200B;](assets/create-from-template.png)

1. Selecteer **App Builder**.

1. Ga de titel van het a **Project** en **App naam** in. Beide hebben gebreken, maar het zal gemakkelijker zijn om het Project te identificeren u later wilt als u de waarde aanpast.

   >[!NOTE]
   >
   >Er is een optie om extra werkruimten aan deze stap toe te voegen. Er werd ons voorgesteld een werkruimte te creëren voor elke ontwikkelaar. Dit houdt geheimen en plaatsingen gescheiden van elkaar aangezien devs werken. Geef de werkruimte een naam met de naam van de ontwikkelaar die de werkruimte gebruikt. De AIO-clip heeft opties voor het schakelen tussen de werkruimte, die we later zullen behandelen.


1. Laat **omvatten runtime** geselecteerd.

1. Klik **sparen**.

## Adobe IO (aio) CLI

Adobe biedt een open-source CLI die kan worden gebruikt om de App Builder-toepassingen te maken. De documentatie kan hier worden gevonden: [&#x200B; https://github.com/adobe/aio-cli &#x200B;](https://github.com/adobe/aio-cli) evenals de Instructies van Adobe App Builder [&#x200B; https://developer.adobe.com/app-builder/docs/getting_started/first_app/ &#x200B;](https://developer.adobe.com/app-builder/docs/get_started/app_builder_get_started/first-app).

1. Installatie
   1. Als u het gereedschap wilt installeren, voert u het volgende uit (zorg dat u zich eerst op knooppunt v18 bevindt): `npm install -g @adobe/aio-cli ` .

1. Verifiëren in terminal
   1. Start de terminal en meld u aan bij AIO met de opdracht: `aio login` .

1. Uw toepassing initialiseren
   1. Start het instellen van de app door: `aio app init example-app` .

1. Configuratieselectie
   1. Ga door om uw Organisatie en Project van de verstrekte opties te selecteren.\
      ![&#x200B; Uitgezochte org &#x200B;](assets/select-org.png)
      ![&#x200B; Uitgezochte project &#x200B;](assets/select-project.png)

1. Sjabloonselectie en -instellingen
   1. Blader door alle beschikbare sjablonen en kies de sjabloon **@adobe/aem-cf-editor-ui-ext-tpl** voor uw project.
      ![&#x200B; malplaatje van het Onderzoek &#x200B;](assets/search-template.png)
      ![&#x200B; Uitgezochte malplaatje &#x200B;](assets/select-template.png)

1. Uw extensie definiëren
   1. Geef de extensie een naam.
   1. Geef een beschrijvend overzicht van de functionaliteit van uw extensie.
   1. Selecteer een eerste versienummer waarmee u wilt beginnen.
   1. Bevestig voltooiing door **te selecteren wordt ik gedaan**.
      ![&#x200B; bepalen uitbreiding &#x200B;](assets/define-extension.png)

1. Ga naar uw projectmap
   1. De map src openen
   1. Wijzig de naam van de map `aem-cf-editor-1` in `workfront-doc-details-1` .

1. Configuratiebestanden wijzigen
   1. App.config.yaml openen
   1. Werk de regel bij van `aem/cf-editor/1` naar `workfront/doc-details/1` .
   1. Pas het include-pad aan van `src/aem-cf-editor-1/ext.config.yaml` naar `src/workfront-doc-details-1/ext.config.yaml` .

1. De Extension Registration Component bewerken
   1. Open `src/workfront-doc-details-1/web-src/src/components/ExtensionRegistration.js`.
   1. Voeg in de sectie Methoden een functie `secondaryNav` toe die een asynchrone functie `getButtons` bevat.
   1. `getButtons` ontvangt een object met de volgende structuur:

      ```
          {
          docId: "String",  // Document ID
          docvId: "String", // Document version ID
          sharedContext: {
              hostname: "String",
              protocol: "String",
              auth: {
              imsOrgID: "String",    // Customer's IMS Org ID
              imsToken: "String",    // User's IMS token
              imsClientId: "String"
              }
          }
          }
      ```

1. Deze functie retourneert een array met knopobjecten die in de navigatie worden weergegeven:

   ```
       methods: {
       secondaryNav: {
           async getButtons({docId, docvId, sharedContext}) {
           return [
               { label: 'Registration', url: '/index.html' },
               { label: 'Review', url: '/index.html#review' }
           ];
           }
       }
       }
   ```

1. Toepassingsroutering configureren
   1. Open uw dossier App.js en vorm de routes om de onlangs ontwikkelde functionaliteit te omvatten. U zult aan opstellingsroutes voor de standaardmening en om het even welke extra meningen zoals de overzichtspagina moeten. Hier is hoe u deze routes zou kunnen bepalen:

      ```
          <Route index element={<ExtensionRegistration />} />
          <Route exact path="index.html" element={<ExtensionRegistration />} />
          <Route exact path="review" element={<Review />} />
      ```

1. Documentgegevens openen
   1. Voer de geleverde functie `document.getDocumentDetails` in uw toepassing uit om essentiële documentspecificaties op te halen. Deze functie haalt een object op dat `docId` en `docvId` bevat, naast een `sharedContext` -object met `hostname` , `protocol` en verificatiegegevens. Zorg ervoor dat de toepassing deze gegevens op de juiste wijze verwerkt.

1. Gegevens ophalen in uw componenten integreren
   1. Voeg een nieuwe component aan de componentenomslag van uw toepassing toe. Stel binnen deze component een verbinding met Workfront tot stand om documentgegevens en verificatiegegevens op te halen via de verbinding die met de hosttoepassing is gemaakt. Hier is een voorbeeld van hoe u uw component kunt structureren om dit te behandelen:

      ```
          import { useEffect, useState } from 'react';
          import { attach } from "@adobe/uix-guest";
          import { extensionId } from "./Constants";
      
          function Review() {
              const [conn, setConn] = useState();
      
              useEffect(() => {
              const iife = async () => {
                  // "attach" the guest application to the host. This creates a "tunnel" from the host app that allows data to be passed to the iframe running this app.
                  const connection = await attach({
                  id: extensionId,
                  });
                  setConn(connection);
              };
      
              iife();
              }, []);
      
              useEffect(() => {
                  if (conn) {
                      // Using the connection created above, grab the document details from the host tunnel.
                      conn?.host?.document?.getDocumentDetails().then(setDocDetails);
                      // Pull the auth tokens from the sharedContext (see host app for details)
                      setAuth(conn?.sharedContext?.get("auth"));
                      setHostname(conn?.sharedContext?.get("hostname"));
                      setProtocol(conn?.sharedContext?.get("protocol"));
                  }
              }, [conn]);
      
          return (<>Text</>);
          }
      
          export default Review;
      ```

## Configuratie voor bestaande AIO-projecten

1. Configuratiebestanden bijwerken
   1. Open `app.config.yaml`.
   1. Wijzig de configuratie door de verwijzing van `aem/cf-editor/1` naar `workfront/doc-details/1` bij te werken. Met deze aanpassing worden de bestandspaden uitgelijnd op de huidige projectstructuur.

1. De Extension Registration Component herzien
   1. Zoek en open het bestand met de naam `ExtensionRegistration.js` .
   1. Voeg in de sectie Methoden een functie `secondaryNav` toe die een asynchrone functie `getButtons` bevat.
   1. `getButtons` ontvangt een object met de volgende structuur:

      ```
          {
          docId: "String",  // Document ID
          docvId: "String", // Document version ID
          sharedContext: {
              hostname: "String",
              protocol: "String",
              auth: {
              imsOrgID: "String",    // Customer's IMS Org ID
              imsToken: "String",    // User's IMS token
              imsClientId: "String"
              }
          }
          }
      ```

1. Deze functie retourneert een array met knopobjecten die in de navigatie worden weergegeven:

   ```
       methods: {
       secondaryNav: {
           async getButtons({docId, docvId, sharedContext}) {
           return [
               { label: 'Registration', url: '/index.html' },
               { label: 'Review', url: '/index.html#review' }
           ];
           }
       }
       }
   ```

1. Toepassingsroutering configureren
   1. Open uw `App.js` dossier en vorm de routes om de onlangs ontwikkelde functionaliteit te omvatten. U zult aan opstellingsroutes voor de standaardmening en om het even welke extra meningen zoals de overzichtspagina moeten. Hier is hoe u deze routes zou kunnen bepalen:

      ```
          <Route index element={<ExtensionRegistration />} />
          <Route exact path="index.html" element={<ExtensionRegistration />} />
          <Route exact path="review" element={<Review />} />
      ```

1. Documentgegevens openen
   1. Voer de geleverde functie `document.getDocumentDetails` in uw toepassing uit om essentiële documentspecificaties op te halen. Deze functie haalt een object op dat `docId` en `docvId` bevat, naast een `sharedContext` -object met `hostname` , `protocol` en verificatiegegevens. Zorg ervoor dat de toepassing deze gegevens op de juiste wijze verwerkt.

1. Gegevens ophalen in uw componenten integreren
   1. Voeg een nieuwe component aan de componentenomslag van uw toepassing toe. Stel binnen deze component een verbinding met Workfront tot stand om documentgegevens en verificatiegegevens op te halen via de verbinding die met de hosttoepassing is gemaakt. Hier is een voorbeeld van hoe u uw component kunt structureren om dit te behandelen:

      ```
          import { useEffect, useState } from 'react';
          import { attach } from "@adobe/uix-guest";
          import { extensionId } from "./Constants";
      
          function Review() {
              const [conn, setConn] = useState();
      
              useEffect(() => {
              const iife = async () => {
                  // "attach" the guest application to the host. This creates a "tunnel" from the host app that allows data to be passed to the iframe running this app.
                  const connection = await attach({
                  id: extensionId,
                  });
                  setConn(connection);
              };
      
              iife();
              }, []);
      
              useEffect(() => {
                  if (conn) {
                      // Using the connection created above, grab the document details from the host tunnel.
                      conn?.host?.document?.getDocumentDetails().then(setDocDetails);
                      // Pull the auth tokens from the sharedContext (see host app for details)
                      setAuth(conn?.sharedContext?.get("auth"));
                      setHostname(conn?.sharedContext?.get("hostname"));
                      setProtocol(conn?.sharedContext?.get("protocol"));
                  }
              }, [conn]);
      
          return (<>Text</>);
          }
      
          export default Review;
      ```

## Toepassingen publiceren

>[!IMPORTANT]
>
>Zorg ervoor dat u de juiste IMS org voor elk van de volgende stappen hebt geselecteerd.

Als een gasttoepassing in Workfront moet worden geladen, moet de toepassing naar de productiewerkruimte worden geduwd en ter goedkeuring worden ingediend.

1. De toepassing implementeren in de werkruimte Productie
   1. `aio app use -w Production `
   1. `aio app deploy `

1. Navigeer aan [&#x200B; https://developer-stage.adobe.com/ &#x200B;](https://developer-stage.adobe.com/) of [&#x200B; https://developer.adobe.com/ &#x200B;](https://developer.adobe.com/).
   1. Klik **Console** in de hogere juiste hoek.

1. Vind het project dat u gebruikte om de toepassing te creëren AppBuilder.

1. Selecteer de Productie-Workspace.
   ![&#x200B; Uitgezochte productiewerkruimte &#x200B;](assets/find-application.png)

1. Verzend de toepassing voor privérevisie (u krijgt waarschuwingen die we niet publiceren naar de marketplace van de app-uitwisseling, wat prima is).

1. Vul het formulier in (titel, beschrijving, pictogram en opmerking voor de controleur).
   ![&#x200B; Vul vorm voor privé overzicht &#x200B;](assets/submission-details.png) in

>[!IMPORTANT]
>
>Na indiening moet een systeembeheerder voor de organisatie de indiening goedkeuren.

## De verzending goedkeuren

1. Als systeembeheerder, navigeer aan [&#x200B; https://stage.exchange.adobe.com/ &#x200B;](https://stage.exchange.adobe.com/) of [&#x200B; https://exchange.adobe.com/ &#x200B;](https://exchange.adobe.com/).

1. Klik **leiden** > **Toepassingen van Experience Cloud**. De verzonden toepassingen worden weergegeven met opties voor goedkeuren/afwijzen.
Nadat de gepubliceerde toepassingsextensies zijn goedgekeurd, worden deze automatisch in uw Workfront-omgeving geladen.

   ![&#x200B; Goedgekeurde voorlegging &#x200B;](assets/approve-submission.png)

## Aanvullende Help

Adobe heeft geweldige documentatie over hoe u apps voor AppBuilder kunt gaan ontwikkelen en hoe u deze kunt implementeren.

Hier volgen enkele handige koppelingen:

* [&#x200B; https://developer.adobe.com/app-builder/docs/getting_started/first_app/#4-bootstrapping-new-app-using-the-cli](https://developer.adobe.com/app-builder/docs/get_started/app_builder_get_started/first-app#bootstrap-the-new-app-using-the-cli)

* [&#x200B; https://developer.adobe.com/uix/docs/guides/publication/](https://developer.adobe.com/uix/docs/guides/publication/)

* [&#x200B; https://developer.adobe.com/uix/docs/services/aem-cf-console-admin/extension-development/](https://developer.adobe.com/uix/docs/services/aem-cf-console-admin/extension-development/)

## Lokale ontwikkeling

Wanneer u uw App Builder-toepassing voor Workfront ontwikkelt, is het mogelijk dat u uw app in Workfront moet testen zonder deze te publiceren. Gelukkig hebben we daarvoor een oplossing.

In uw App Builder-app kunt u `aio app run` starten voor lokale ontwikkeling. Hierdoor krijgt u een URL, meestal iets als `https://localhost:9080` . U kunt `aio app deploy` ook uitvoeren om een statisch Adobe-domein te verkrijgen. Noteer deze URL&#39;s voor toekomstig gebruik.

Navigeer vervolgens naar de specifieke pagina met documentdetails die u wilt ontwikkelen in uw browser. Open de tools voor ontwikkelaars en open de Local Storage voor workfront.com of workfront.adobe.com. Hier, moet u een ingang toevoegen. Gebruik `appBuilderDocDetailsOverride` als de sleutel en de eerder vermelde URL van de App Builder als de waarde.

Wanneer u de pagina opnieuw laadt, worden de knoppen uit uw App Builder-toepassing weergegeven. Als u op deze knoppen klikt, kunt u uw app in actie bekijken.
