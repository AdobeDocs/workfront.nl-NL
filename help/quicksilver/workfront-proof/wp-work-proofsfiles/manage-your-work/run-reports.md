---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Rapporten uitvoeren in  [!DNL Workfront Proof]
description: Met Workfront Proof kunt u rapporten weergeven, zodat u de voortgang van het werk en de efficiëntie van uw teams kunt bijhouden.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 342f9282-b6f5-425e-a7ef-e23bd011d284
source-git-commit: a0d76692f9e9d12ed0d538c1344638dbc208d625
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 0%

---

# Rapporten uitvoeren in [!DNL Workfront Proof]


>[!IMPORTANT]
>
>* <span class="previe"> de functionaliteit van de Rapportering is niet meer beschikbaar in [!DNL Workfront Proof]. Het rapporterende lusje toont nog, maar de gegevens zijn niet nauwkeurig.</span>
> 
>* Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [ het Bewijzen ](../../../review-and-approve-work/proofing/proofing.md).

Met Workfront Proof kunt u rapporten weergeven, zodat u de voortgang van het werk en de efficiëntie van uw teams kunt bijhouden.

U kunt eenvoudig het aantal proefdrukken weergeven dat is gemaakt in uw [!DNL Workfront Proof] -account, het aantal versies dat is gekoppeld aan elke proefdruk, de doorlooptijd en meer.

## Vereisten

Of rapporten beschikbaar zijn, is afhankelijk van het type [!DNL Workfront Proof] -account en de machtigingsniveaus van de gebruiker.

* [Accountvereisten](#account-prerequisites)
* [Gebruikersvereisten](#user-prerequisites)

### Accountvereisten {#account-prerequisites}

Rapportinformatie is alleen beschikbaar bij Premium-abonnementen.

### Gebruikersvereisten {#user-prerequisites}

Het melden van informatie is beschikbaar slechts aan gebruikers met volledige toegang tot alle proeven op uw rekening (d.w.z. gebruikers met minstens [ Profielen van de Toestemmingen van de Bewijs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

In dit deelvenster kunt u

* De tijdspanne bepalen van de weergegeven gegevens
* Wijzigingen in metriek in de loop der tijd analyseren
* Controleer de details van een geselecteerd punt in de tijd door er boven te houden
* Controleer het totale aantal proefdrukken dat in het geselecteerde tijdbereik is gemaakt
* Controleer het gemiddelde aantal versies dat is opgenomen in de voltooide proefdrukken

## Rapporten weergeven {#viewing-reports}

1. Ga naar de pagina **[!UICONTROL Dashboards]** .
1. Klik op de tab **[!UICONTROL Reports]** .\
   ![ proof_reports.png ](assets/proof-reports-350x193.png)

1. Selecteer in het vervolgkeuzemenu **[!UICONTROL Time frame]** of u informatie wilt weergeven over proefdrukken die zijn gemaakt in de afgelopen 24 uur, 7 dagen, 30 dagen, 90 dagen of een aangepaste tijdsperiode.\
   Als u een aangepaste tijdsperiode selecteert, selecteert u de begin- en einddatum en klikt u op **[!UICONTROL Apply]** .\
   De volgende informatie wordt weergegeven voor de tijdsperiode die u hebt geselecteerd:\
   **Gemaakte Bewijs:** Aantal proeven die binnen de geselecteerde tijdspanne worden gecreeerd.\
   **Versies per Bewijs:** Gemiddeld aantal versies per proef voor alle voltooide (Goedgekeurd of Goedgekeurd met Veranderingen) binnen de geselecteerde tijdspanne.\
   **Draai rond Tijd:** Gemiddelde tijd van toen de eerste versie werd gecreeerd aan de tijd het besluit op de definitieve versie werd genomen.\
   **Eerste Tijd van de Activiteit:** Gemiddelde tijd van toen het bewijs tot de tijd van de eerste activiteit op de proef werd gecreeerd.\
   **Bewijzen laat:** Gemiddeld percentage voltooide (Goedgekeurd of Goedgekeurd met Veranderingen) die minstens één versie hadden die binnen de geselecteerde tijdspanne laat was.\
   **Commentaren en Reacties:** Gemiddeld aantal commentaren en antwoorden die op alle proeven binnen de geselecteerde tijdspanne werden gemaakt.

1. (Optioneel) Schakel de optie **[!UICONTROL Show min-max range]** in of uit om te bepalen of minimum- en maximumwaarden in de grafiek worden weergegeven.\
   Als u deze optie selecteert, wordt een blauwe schaduw weergegeven tussen de minimale en maximale geregistreerde waarden.

1. (Optioneel) U kunt de gegevens filteren die worden weergegeven, zoals beschreven in [ Rapporten filteren ](#filtering-reports) .

## Filterrapporten {#filtering-reports}

Standaard bevatten de gegevens in rapporten alle gegevens van uw [!DNL Workfront Proof] -systeem. U kunt filters gebruiken om alleen informatie weer te geven die relevant is voor uw behoeften.

Rapportgegevens filteren:

1. Ga naar de pagina **[!UICONTROL Dashboards]** .
1. Klik op de tab **[!UICONTROL Reports]** .\
   ![ proof_reports.png ](assets/proof-reports-350x193.png)

1. Stel een rapport in werking, zoals die in [ wordt beschreven het Bekijken Rapporten ](#viewing-reports).
1. Klik op **[!UICONTROL Filter]**.

1. Selecteer links op de pagina een van de volgende filteropties:\
   **[!UICONTROL Proof Type]:** selecteer het type proef u in het rapport wilt worden omvat.\
   **[!UICONTROL Decisions]:** selecteer opties om te bepalen of slechts proefdrukken die bepaalde besluiten bevatten zijn gemaakt.\
   **[!UICONTROL Recipients]:** selecteer individuele gebruikers om informatie te bekijken over proeven die met de geselecteerde gebruikers worden gedeeld.\
   **[!UICONTROL Proof Owners]:** selecteer individuele gebruikers om informatie over proeven te bekijken die door de geselecteerde gebruikers worden bezeten.\
   **[!UICONTROL Proof Creators]:** selecteer individuele gebruikers om informatie over proeven te bekijken die door de geselecteerde gebruikers worden gecreeerd.\
   **[!UICONTROL Accounts]:** selecteer welke rekeningen u in het rapport wilt omvatten.

1. Klik op **[!UICONTROL Apply]**.
1. (Optioneel) Schakel de optie **[!UICONTROL Show min-max range]** in of uit om te bepalen of minimum- en maximumwaarden in de grafiek worden weergegeven.\
   Als u deze optie selecteert, wordt een blauwe schaduw weergegeven tussen de minimale en maximale geregistreerde waarden.

## Rapporten afdrukken

1. Ga naar de pagina **[!UICONTROL Dashboards]** .
1. Klik op de tab **[!UICONTROL Reports]** en klik vervolgens op **[!UICONTROL Print]** .\
   ![ proof_reports_print.png ](assets/proof-reports-print-350x191.png)

1. Maak een keuze uit de verschillende beschikbare afdrukopties.\
   De afdrukopties variëren afhankelijk van de gebruikte browser- en browserversie.
