---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: Testomgeving voor sandbox voorvertonen- [!DNL Workfront Proof]
description: De zandbak van de Voorproef is een testend milieu dat als replica van uw levende milieu dient en elk weekend door  [!DNL Workfront Proof] verfrist.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Testomgeving voor sandbox voorvertonen- [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [ het Bewijzen ](../../../review-and-approve-work/proofing/proofing.md).

De voorvertoningssandbox is een testomgeving die fungeert als replica van uw live omgeving en die elk weekend wordt vernieuwd door [!DNL Workfront Proof] .

## De voorvertoningssandbox

De voorvertoningssandbox fungeert als een omgeving waarin gebruikers in uw organisatie veilig gegevens kunnen testen en bewerken uit de productieomgeving zonder dat dit van invloed is op de productieomgeving. Het is ideaal voor het uitvoeren van trainingssessies, het testen van nieuwe functies en het bepalen van de installatiefunctionaliteit.

Nieuwe productfuncties worden ook geüpload naar de voorvertoningssandbox-omgeving voordat ze worden geleverd aan de productieomgeving. Uw gebruikers kunnen daar nieuwe functionaliteit uitproberen zonder hun normale werkschema in het milieu van de Productie te beïnvloeden.

De voorvertoningssandbox bevat uw feitelijke productiegegevens. De gegevensstromen van Productie aan Voorproef, en niet in omgekeerde. Het verfrist zich elk weekend, zodat kunnen de gegevens tot één week achter de milieu van de Productie zijn. De punten die sinds laatste worden gecreeerd verfrissen tijd zijn in het milieu van de Sandbox van de Voorproef tot het volgende verfrist zich.

## De voorvertoningssandbox openen

Als systeembeheerder hebt u standaard toegang tot de omgeving van de voorvertoning van de sandbox. Als u geen toegang hebt tot de omgeving van de voorvertoningssandbox zoals beschreven in deze sectie, neemt u contact op met uw [!DNL Workfront] -beheerder of ons ondersteuningsteam.

* [Toegang tot de zandbak van de Voorproef als Stand-Onafhankelijke  [!DNL Workfront Proof]  Klant](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [Toegang tot de zandbak van de Voorproef als a [!DNL Workfront]+[!DNL Workfront Proof]  Klant](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### Toegang tot de voorvertoningssandbox als zelfstandige [!DNL Workfront Proof] klant

1. Navigeer naar deze URL: `https://preview.proofhq.com` .
1. Meld u aan met uw voorvertoningsreferenties.\
   De voorvertoningsgegevens moeten dezelfde zijn als de gegevens voor de productie, tenzij u deze hebt gewijzigd in Productie nadat de voorvertoning is vernieuwd. Logins worden gesynchroniseerd slechts wanneer verfrist voorkomt, die elk weekend plaatsvindt. Ze worden niet automatisch gesynchroniseerd.

### De voorbeeldsandbox openen als een [!DNL Workfront+Workfront] Proefklant

Als systeembeheerder hebt u via de interface van [!DNL Workfront] toegang tot de voorvertoningssandbox van [!DNL Workfront Proof] .

De voorvertoningssandbox van [!DNL Workfront Proof] openen:

1. Meld u aan bij de [!DNL Workfront] -omgeving.
1. Klik op **[!UICONTROL Setup]** in de algemene navigatiebalk.
1. Klik **[!UICONTROL System]** > **[!UICONTROL Preferences]**.

1. Klik in de sectie **[!UICONTROL Test Environments]** op **[!UICONTROL Sandbox Preview]** .

1. Meld u aan met uw voorvertoningsreferenties.\
   Uw voorvertoningsgegevens moeten dezelfde zijn als uw productiegegevens, tenzij u deze in Productie hebt gewijzigd nadat de voorvertoning is vernieuwd. De logins worden alleen gesynchroniseerd wanneer het vernieuwen plaatsvindt. Ze worden niet automatisch gesynchroniseerd.
1. Klik op het pictogram [!DNL Workfront Proof] op de algemene navigatiebalk.\
   ![ proof_access_proofhq.png ](assets/proof-access-proofhq-350x39.png)\
   De voorvertoningsomgeving van [!DNL Workfront Proof] wordt weergegeven.

## E-mails ontvangen vanuit de voorvertoningssandbox

E-mailmeldingen worden nooit geactiveerd vanuit de voorvertoningsomgeving van [!DNL Workfront Proof] .
