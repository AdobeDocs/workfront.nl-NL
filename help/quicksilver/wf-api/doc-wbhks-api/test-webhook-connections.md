---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhaak-verbindingen testen
description: Webhaak-verbindingen testen
author: John
feature: Workfront API
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: a62ae524f922326811423cd17d0656920b7cc9d3
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---


# Webhaak-verbindingen testen

Voer de handtests in deze sectie uit om te controleren of de implementatie van uw documentwebhaak correct werkt. Deze stappen gaan door de Webinterface van Adobe Workfront en raken indirect de eindpunten voor uw Web-haakimplementatie.

## Vereisten

Voor het uitvoeren van de tests zijn de volgende voorwaarden vereist:

* Een Workfront-account met ADM (Advanced Document Management) ingeschakeld

* Een Workfront-gebruiker voor dit account met System Admin Rights

* Een WebHaak-instantie van Document met HTTP-eindpunten die toegankelijk zijn voor Workfront

Bij deze tests wordt er ook van uitgegaan dat de instantie WebHaak van het document is geregistreerd. (U kunt uw exemplaar in Workfront registreren onder Setup > Documenten > Aangepaste integratie.)

**Test 1: Verstrek de dienst van Webhaak van het Document voor een gebruiker**

Test URL van de Authentificatie en Symbolische Eindpunt URL voor op OAuth-Gebaseerde Leveranciers van Webhaken.

1. Ga in Workfront naar de hoofdpagina Documenten door op de koppeling Documenten in de bovenste navigatiebalk te klikken.
1. Klik op Add de drop-down Documenten en selecteer uw dienst van Webhaak van het Document onder Add de Dienst.
1. (Alleen OAuth-services) Nadat u de vorige stap hebt voltooid, wordt de OAuth2-verificatiepagina van uw service geladen in een pop-upvenster. (Opmerking: u wordt mogelijk eerst gevraagd u aan te melden bij uw service.) Via de verificatiepagina geeft u Workfront toegang tot de account van de gebruiker door op de knop Vertrouwd of Toestaan te klikken.
1. Controleer of uw service is toegevoegd aan de vervolgkeuzelijst Documenten toevoegen. Vernieuw de browser als deze standaard niet wordt weergegeven.

**Test 2: Een document koppelen aan Workfront Test de volgende eindpunten: /bestanden, /metadata**

1. Ga in Workfront naar de hoofdpagina Documenten door op de koppeling Documenten in de bovenste navigatiebalk te klikken.
1. Selecteer de documentservice Webhaak onder Documenten toevoegen.
1. Navigeer in het modaal door de mappenstructuur.
1. Controleer of u door de mapstructuur kunt navigeren.
1. Een document selecteren en koppelen naar Workfront

**Test 3: Naar een document navigeren in het inhoudsbeheersysteem**

Test de volgende eindpunten: /metadata (in het bijzonder viewLink)

1. Een document koppelen aan Workfront
1. Selecteer het document en klik op de koppeling Openen.
1. Controleer of het document op een nieuw tabblad wordt geopend.

**Test 4: Naar een document in het inhoudsbeheersysteem navigeren (met aanmelding)**

Test de volgende eindpunten: /metadata (in het bijzonder viewLink)

1. Zorg ervoor dat u bent afgemeld bij het inhoudsbeheersysteem.
1. Koppel een document aan Workfront.
1. Selecteer het document en klik op de koppeling Openen.
1. Controleer of het aanmeldingsscherm van het inhoudsbeheersysteem op een nieuw tabblad wordt geladen.
1. Aanmelden en controleren of u naar het document bent gegaan

**Test 5: Het document downloaden van het contentbeheersysteem**

Test de volgende eindpunten (in het bijzonder de downloadkoppeling): /metadata 

1. Koppel een document aan Workfront.
1. Selecteer het document en klik op de koppeling Downloaden.
1. Controleer of het downloaden begint.

**Test 6: Inhoud zoeken**

Test de volgende eindpunten: /search

1. Ga in Workfront naar de hoofdpagina Documenten door op de koppeling Documenten in de bovenste navigatiebalk te klikken.
1. Selecteer de documentservice Webhaak onder Documenten toevoegen.
1. Voer een zoekopdracht uit vanuit het modaal.
1. Controleer of de zoekresultaten correct zijn.

**Test 7: Document van Workfront naar inhoudsbeheersysteem verzenden**

Test de volgende eindpunten: /files, /uploadInit, /upload

1. Ga in Workfront naar de hoofdpagina Documenten door op de koppeling Documenten in de bovenste navigatiebalk te klikken.
1. Een document vanaf uw computer uploaden naar Workfront
1. Ga naar de pagina met documentdetails
1. Selecteer in het vervolgkeuzemenu Documenthandelingen de documentservice onder Verzenden naar...
1. Ga naar de gewenste doelmap en klik op de knop Opslaan.
1. Controleer of het document naar de juiste locatie in het inhoudsbeheersysteem is geüpload.

**Test 8: Miniaturen weergeven in Workfront**

Test de volgende eindpunten: /miniatuur

1. Koppel een document aan Workfront.
1. Selecteer het document in de lijst.
1. Controleer of de miniatuur in het rechterdeelvenster wordt weergegeven.

**Test 9: De inhoudbytes ophalen**

Test de volgende eindpunten: /download

1. Koppel een document aan Workfront.
1. Ga naar de pagina met documentdetails.
1. Het document naar Workfront verzenden door Documenthandelingen > Verzenden naar te selecteren.. > Workfront. Hiermee wordt een nieuwe documentversie in Workfront gemaakt.
1. Download het document vanuit Workfront door op de koppeling Downloaden te klikken.

**Test 10: Toegangstoken vernieuwen (alleen OAuth2 Webhaak-providers)**

Test de volgende eindpunten: URL van token-eindpunt

1. Verricht de dienst van Webhaak van het Document voor een gebruiker
1. Maak het toegangstoken van de gebruiker ongeldig door 1 te wachten op time-out, of 2) het manueel ongeldig te maken in het externe systeem.
1. Vernieuw het toegangstoken in Workfront. U kunt dit bijvoorbeeld doen door een document aan Workfront te koppelen. Het toegangstoken is vernieuwd als u naar een document kunt navigeren en er een koppeling naar kunt maken.

>[!NOTE]
>
>De optie Verzenden naar.. is niet beschikbaar voor gekoppelde documenten. Dit wordt door Workfront toegevoegd. U kunt het /download eindpunt testen door het eindpunt manueel te raken gebruikend een cliënt REST, zoals Postman. Alternatief, kan het /download eindpunt worden getest door een digitaal bewijs te produceren. Neem contact op met Workfront om digitale proefdrukken in te schakelen.
