---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: create-proofs-and-files
title: Dropzone
description: Als u het ondernemingsplan hebt, kunt u Dropzone gebruiken om nieuwe proefdrukken en nieuwe versies van proefdrukken naar uw account te verzenden zonder u aan te hoeven melden bij uw account.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e66142fa-3b0d-4821-9aa5-040c62f00d62
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 0%

---

# Dropzone

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [ het Bewijzen ](../../../review-and-approve-work/proofing/proofing.md).

Als u het ondernemingsplan hebt, kunt u Dropzone gebruiken om nieuwe proefdrukken en nieuwe versies van proefdrukken naar uw account te verzenden zonder u aan te hoeven melden bij uw account.

Wanneer u een proef via Dropzone voorlegt, verschijnt het in de pagina Dropzone in uw [!DNL Workfront Proof] rekening. Vanaf dat punt kunt u het in uw werkschema leiden.

## Een nieuwe proef indienen via de Dropzone-URL

1. In uw browser, ga naar unieke Dropzone URL, zoals die in [ wordt beschreven vormt dropzone in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. Voer uw e-mailadres in.
1. Klik op **[!UICONTROL Select a file]** of **[!UICONTROL Capture a web page]** en kies het bestand of de webpagina die u wilt uploaden.

1. Voer de beveiligingscode in en klik op **[!UICONTROL Next]** .\
   In een voortgangsbalk ziet u de voortgang van het uploaden.\
   In het volgende scherm kunt u Proefgegevens toevoegen.\
   Deze sectie wordt alleen weergegeven als deze is ingeschakeld in de Dropzone-instellingen.

1. Klik op **[!UICONTROL Next]** als u de details hebt ingevuld.
1. Alle revisoren die aan de proefdruk zijn toegevoegd, ontvangen hun e-mailbericht pas nadat de proefdruk is geactiveerd (zie hieronder).
1. Uw proefdruk wordt door de volgende staten geleid nadat u het aan Dropzone voorlegt:

   * Wanneer u een bestand voor het eerst uploadt naar de Dropzone, wordt de proefdruk weergegeven als Concept.
   * Zodra u de verzending hebt voltooid, wordt de proefdruk weergegeven in uw Dropzone als Verzonden.
   * Nadat de proefdruk is geactiveerd en ontgrendeld, wordt deze in uw Dropzone weergegeven als Actief.
   * Als de proefdruk vergrendeld is, wordt deze in de dropzone weergegeven als Vergrendeld.

## Een nieuwe versie van een bestaand bewijs verzenden via de Dropzone-URL

1. In uw browser, ga naar unieke Dropzone URL, zoals die in [ wordt beschreven vormt dropzone in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)
1. Voer uw e-mailadres in.
1. Schakel het selectievakje in om aan te geven dat u een nieuwe versie van een bestaande proefdruk uploadt.\
   Zie voor meer informatie over het maken van een nieuwe versie van een proefdruk.
1. Klik op **[!UICONTROL Select a file]** of **[!UICONTROL Capture a web page]** en kies het bestand of de webpagina die u wilt uploaden.

1. Voer de beveiligingscode in en klik op **[!UICONTROL Next]** .\
   In een voortgangsbalk ziet u de voortgang van het uploaden.\
   Workfront Proof stuurt u een validatie-e-mail.

1. Klik op de koppeling in de e-mail.\
   Het venster Dropzone wordt in uw browser geopend via e-mail. De koppeling in het e-mailbericht is 24 uur geldig.
1. Selecteer de vorige versie van de proefdruk (alleen de proefdrukken die u hebt gemaakt/verzonden, worden weergegeven).\
   In het volgende scherm kunt u proefdrukdetails toevoegen.\
   Deze sectie wordt alleen weergegeven als deze is ingeschakeld in Dropzone-instellingen.

1. Typ de details en klik op **[!UICONTROL Next]** .

   >[!NOTE]
   >
   >Alle revisoren die aan de proefdruk zijn toegevoegd, ontvangen hun e-mailbericht pas nadat de proefdruk is geactiveerd (zie hieronder).

   Uw proefdruk wordt door de volgende staten geleid nadat u het aan Dropzone voorlegt:

   * Wanneer u een bestand voor het eerst uploadt naar de Dropzone, wordt de proefdruk weergegeven als Concept.
   * Zodra u de verzending hebt voltooid, wordt de proefdruk weergegeven in uw Dropzone als Verzonden.
   * Nadat de proefdruk is geactiveerd en ontgrendeld, wordt deze in uw Dropzone weergegeven als Actief.
   * Als de proefdruk vergrendeld is, wordt deze in de dropzone weergegeven als Vergrendeld.

## Een proefexemplaar per e-mail verzenden naar de dropzone

>[!NOTE]
>
>Het verzenden van een proefdruk naar de dropzone wordt niet meer ondersteund.


## Uw verzending voltooien

Workfront stuurt u (de verzender) een e-mail met het verzoek om uw verzending te voltooien, waarin u wordt gevraagd te bevestigen of het bestand een nieuwe proefversie of een nieuwe versie was. De koppeling in het e-mailbericht is 24 uur geldig.

1. Klik op de koppeling en volg de bovenstaande stappen, afhankelijk van het feit of het een nieuwe proefdruk of een nieuwe versie van een bestaande proefdruk betreft.

## Het proefexemplaar activeren

De eigenaar van de Dropzone ontvangt een e-mail met kennisgeving waarin wordt meegedeeld dat een nieuw bewijs is ingediend bij de Dropzone:

* De proefdruk wordt weergegeven op de pagina Dropzone in uw account (klik op de koppeling in het linkernavigatiezijpaneel om de pagina Dropzone te openen).
* De proef is toegankelijk door de eigenaar Dropzone (of een gebruiker die minstens een profiel van de Supervisor heeft). De eigenaar kan worden gewijzigd binnen de Dropzone-instellingen (alleen een Factuurbeheerder of een beheerder kan dit doen).
* Voordat de proefdruk kan worden bewerkt, moet deze worden geactiveerd/ontgrendeld door de eigenaar van de dropzone (een gebruiker met ten minste een Supervisor-profiel kan dit ook doen). De status van de proefdruk wordt weergegeven als Verzonden totdat deze is geactiveerd/ontgrendeld.

De proefdruk activeren:

1. Ga naar het vervolgkeuzemenu rechts van de proefdruk en klik op **[!UICONTROL Activate]** .
1. Nadat de proefdruk is geactiveerd/ontgrendeld:

   * De proefdrukstatus verandert in Actief.
   * Personen die aan de proefdruk zijn toegevoegd, ontvangen een e-mail met de kennisgeving dat ze over een nieuw bewijs beschikken om dit te controleren. (Er wordt geen e-mail verzonden totdat de proefdruk is geactiveerd/ontgrendeld.)
   * Aan de proefdruk kan normaal worden gewerkt
   * Indien de verzender zich ook expliciet aan de bewijsvoering toevoegt, ontvangt hij geen e-mail met een nieuw bewijsmiddel. Voor meer informatie, zie [ Nieuwe proef e-mail ](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

## Uw dropzone beheren

Met de pagina Dropzone kunt u de verzendingen naar uw Dropzone eenvoudig beheren. De Dropzone-pagina bevat de volgende opties en functionaliteit:

* Pagina-indeling (1)
* Kies of u gearchiveerde proefdrukken wilt opnemen in de weergave (2)
* Knoppen voor handelingen (3)
* Sorteren (4)
* Filter (5)
* Menu Proefacties (6)
* De proefdruk verwijderen (7)
* Proofingoverzicht uitvouwen/samenvouwen (8)
* Een proefdruk selecteren (9)

De opties voor paginalay-out en sorteren en filteren zijn gelijk aan die in de lijsten van [!DNL Views] . Zie [ Punten op de Pagina van Weergaven binnen  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) voor meer informatie beheren.

![ New_Dropzone_design__Feb_2013_.jpg ](assets/new-dropzone-design--feb-2013--350x224.jpg)
