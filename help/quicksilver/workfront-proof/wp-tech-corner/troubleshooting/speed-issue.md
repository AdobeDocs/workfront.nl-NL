---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problemen met snelheid in  [!DNL Workfront Proof]
description: Deze hulppagina kan u helpen bepalen als om het even welke snelheidskwesties die u zou kunnen ervaren wanneer het gebruiken van  [!DNL Workfront Proof]  met uw ISP of  [!DNL Workfront Proof] het netwerk van de inhoudslevering van de inhoud verwant zijn.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 20fcf4dd07c1058559533501f7e297d78c43a70b
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Problemen met snelheid in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [&#x200B; het Bewijzen &#x200B;](../../../review-and-approve-work/proofing/proofing.md).

Deze Help-pagina kan u helpen bepalen of eventuele snelheidsproblemen die u kunt ondervinden bij het gebruik van [!DNL Workfront Proof] betrekking hebben op uw ISP of het netwerk voor inhoudslevering van [!DNL Workfront Proof] .

De problemen van de snelheid zijn over het algemeen toe te schrijven aan de lokale ISP verbinding of de lokale opstelling van de internettoegang (bijvoorbeeld, waar een volmachtsserver wordt gebruikt) en zijn jammer genoeg buiten de controle van [!DNL Workfront Proof].

Dit gezegd zijnde, zijn er een paar stappen u kunt nemen om uw verbindingssnelheid te controleren die voor de worteloorzaak van de kwesties zal toestaan worden bepaald u ervaart. Al deze stappen zijn even belangrijk voor het het oplossen van problemenproces en wij zouden u willen aanmoedigen om de tijd te nemen om informatie over alle vermelde stappen te verzamelen om de nauwkeurigste diagnose van het probleem te verzekeren.

Als u alle details hebt verzameld, raden we u aan contact op te nemen met uw lokale IT-afdeling om eventuele lokale problemen te identificeren.

## Vaststellen welk onderdeel van het systeem traag is

Wanneer u [!DNL Workfront Proof] gebruikt, werkt u mogelijk met het dashboard, bijvoorbeeld voor het beheer van de inhoud van mappen en gebruikers of met de [!DNL Workfront Proof] Viewer: een proefrevisie uitvoeren, de opmerkingen controleren die al zijn gemaakt, enzovoort.

Het bepalen van welk precies deel van het systeem langzaam is is de eerste stap in de kwesties van de het oplossen van problemensnelheid. Wanneer u rapporteert dat [!DNL Workfront Proof] traag is, moet u het volgende beschrijven:

* Wordt u traag op andere webpagina&#39;s?
* Komt het probleem voor in het dashboard of de [!DNL Workfront Proof] Viewer?
* Welk exact deel van het systeem is traag? (bijvoorbeeld een nieuwe proefdruk verwerken of een opmerking openen in de [!DNL Workfront Proof] Viewer)

## Traceroute in werking stellen en tests pingelen

Wanneer u prestatieskwesties ervaart is het belangrijk om het traceroutebevel in werking te stellen om de verbinding te verifiëren. Open hiertoe de opdrachtprompt in uw systeem (Terminal in Mac/Linux) en voer de volgende stappen uit:

1. Typ één van het volgende, dan wacht op tracerout om te worden voltooid:

   * Vensters: **tracert app.proofhq.com**
   * Mac/Linux: **traceroute app.proofhq.com**

1. (Vensters slechts) Type **pingelt app.proofhq.com**.
1. Wanneer pingel voltooit, klik in de bevelherinnering met de rechtermuisknop aan en selecteer allen.
1. Kopieer en plak de resultaten in het antwoord op uw e-mail.
Zorg ervoor u traceroute toestaat en pingel om te beëindigen alvorens de resultaten naar het Team van de Steun te verzenden.

## Verbindingssnelheid testen met Speedtest.net

1. Open een browser en ga naar Speedtest.net
1. Volg de instructies in de kennisbank Sneltoets om de snelheid van uw internetverbinding te testen.
1. Kopieer en plak de resultaten in een e-mail naar ons ondersteuningsteam.

## Het tabblad Netwerk in de browserconsole controleren

De webconsole die beschikbaar is in de moderne browsers verzamelt nuttige informatie over netwerkwachttijden. Deze laatste is nuttig om de oorzaak van de snelheidsproblemen die u ondervindt vast te stellen.

U kunt als volgt de laadtijden voor een webpagina controleren:

1. Open de console van uw browser en het tabblad Netwerk.
1. Laad de pagina opnieuw.
1. Neem screenshots of neem een screencast van de resultaten op.
1. Deel de resultaten met het Ondersteuningsteam.

Controleer of in de schermafbeelding alle gegevens worden weergegeven. U kunt het consolevenster uitvouwen wanneer u een schermafbeelding maakt of omlaag schuift in een screencast.

U kunt ook de documentatie van uw browser controleren op gedetailleerdere instructies.

## Controleer uw verbinding op een ander netwerk en een machine

Het controleren of u het zelfde probleem met verbindingssnelheid gebruikend een verschillend apparaat of een netwerk ervaart is een cruciale stap in het het oplossen van problemenproces. Probeer over te schakelen op een andere computer of een ander mobiel apparaat en probeer een alternatief netwerk (bijvoorbeeld mobiele gegevens) te gebruiken.

Vergelijk de verbinding in verschillende combinaties: gebruikend een verschillende machine op het zelfde netwerk, gebruikend de zelfde machine op een verschillend netwerk en gebruikend zowel alternatieve machine als netwerk, dan deel de resultaten met het Team van de Steun.
