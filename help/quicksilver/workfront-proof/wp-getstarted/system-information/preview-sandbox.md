---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: Testomgeving voor sandbox voorvertonen [!DNL Workfront Proof]
description: De voorvertoningssandbox is een testomgeving die fungeert als replica van uw live omgeving en die elk weekend wordt vernieuwd [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Testomgeving voor sandbox voorvertonen [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

De voorvertoningssandbox is een testomgeving die fungeert als replica van uw live omgeving en die elk weekend wordt vernieuwd [!DNL Workfront Proof].

## De voorvertoningssandbox

De voorvertoningssandbox fungeert als een omgeving waarin gebruikers in uw organisatie veilig gegevens kunnen testen en bewerken uit de productieomgeving zonder dat dit van invloed is op de productieomgeving. Het is ideaal voor het uitvoeren van trainingssessies, het testen van nieuwe functies en het bepalen van de installatiefunctionaliteit.

Nieuwe productfuncties worden ook geüpload naar de voorvertoningssandbox-omgeving voordat ze worden geleverd aan de productieomgeving. Uw gebruikers kunnen daar nieuwe functionaliteit uitproberen zonder hun normale werkschema in het milieu van de Productie te beïnvloeden.

De voorvertoningssandbox bevat uw feitelijke productiegegevens. De gegevensstromen van Productie aan Voorproef, en niet in omgekeerde. Het verfrist zich elk weekend, zodat kunnen de gegevens tot één week achter de milieu van de Productie zijn. De punten die sinds laatste worden gecreeerd verfrissen tijd zijn in het milieu van de Sandbox van de Voorproef tot het volgende verfrist zich.

## De voorvertoningssandbox openen

Als systeembeheerder hebt u standaard toegang tot de omgeving van de voorvertoning van de sandbox. Neem contact op met uw [!DNL Workfront] beheerder of ons ondersteuningsteam.

* [De voorvertoningssandbox openen als een zelfstandige sandbox [!DNL Workfront Proof] Klant](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [De voorvertoningssandbox openen als een [!DNL Workfront]+[!DNL Workfront Proof] Klant](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### De voorvertoningssandbox openen als een zelfstandige sandbox [!DNL Workfront Proof] Klant

1. Ga naar deze URL:  `https://preview.proofhq.com`.
1. Meld u aan met uw voorvertoningsreferenties.\
   De voorvertoningsgegevens moeten dezelfde zijn als de gegevens voor de productie, tenzij u deze hebt gewijzigd in Productie nadat de voorvertoning is vernieuwd. Logins worden gesynchroniseerd slechts wanneer verfrist voorkomt, die elk weekend plaatsvindt. Ze worden niet automatisch gesynchroniseerd.

### De voorvertoningssandbox openen als een [!DNL Workfront+Workfront] Klant proefdrukken

Als systeembeheerder, kunt u tot [!DNL Workfront Proof] Sandbox voorvertonen via [!DNL Workfront] interface.

Om toegang te krijgen tot [!DNL Workfront Proof] Voorvertoning sandbox:

1. Meld u aan bij uw [!DNL Workfront] milieu.
1. Klikken **[!UICONTROL Setup]** in de algemene navigatiebalk.
1. Klik op **[!UICONTROL System]** >**[!UICONTROL Preferences]**.

1. In de **[!UICONTROL Test Environments]** sectie, klikt u op **[!UICONTROL Sandbox Preview]**.

1. Meld u aan met uw voorvertoningsreferenties.\
   Uw voorvertoningsgegevens moeten dezelfde zijn als uw productiegegevens, tenzij u deze in Productie hebt gewijzigd nadat de voorvertoning is vernieuwd. De logins worden alleen gesynchroniseerd wanneer het vernieuwen plaatsvindt. Ze worden niet automatisch gesynchroniseerd.
1. Klik op de knop [!DNL Workfront Proof] in de algemene navigatiebalk.\
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   De [!DNL Workfront Proof] Voorvertoningsomgeving wordt weergegeven.

## E-mails ontvangen vanuit de voorvertoningssandbox

E-mailmeldingen worden nooit geactiveerd door de [!DNL Workfront Proof] Voorvertoningsomgeving.
