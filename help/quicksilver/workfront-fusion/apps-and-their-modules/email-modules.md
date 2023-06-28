---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: E-mailmodules
description: In een [!DNL Adobe Workfront Fusion] U kunt uw e-mailaccount koppelen aan meerdere toepassingen en services van derden. Hierdoor kunt u e-mails downloaden via IMAP, e-mails verzenden via SMTP, nieuwe concepten maken, e-mails verplaatsen en kopiëren naar een andere map, markeren als gelezen of ongelezen en e-mails verwijderen.
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '2104'
ht-degree: 0%

---

# E-mailmodules

In een [!DNL Adobe Workfront Fusion] U kunt uw e-mailaccount koppelen aan meerdere toepassingen en services van derden. Hierdoor kunt u e-mails downloaden via IMAP, e-mails verzenden via SMTP, nieuwe concepten maken, e-mails verplaatsen en kopiëren naar een andere map, markeren als gelezen of ongelezen en e-mails verwijderen.

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] of hoger</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereisten: Als u de [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Oudere productvereisten: Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Sluit uw e-mail aan op Workfront Fusion {#connect-your-email-to-workfront-fusion}

* [Verbinding maken met Google](#connect-to-google)
* [Verbinding maken met andere e-mailservices (SMAP)](#connect-to-other-email-services-smap)

### Verbinden met [!DNL Google]

Gebruik deze optie om scenario&#39;s met e-mailmodules tot stand te brengen die een verbinding aan uw vereisen [!DNL Google] account. Dit is een account met beperkt bereik.

U kunt een verbinding maken met uw [!DNL Google] rechtstreeks vanuit een e-mailmodule.

1. Klik in een willekeurige e-mailmodule op **[!UICONTROL Add]** naast de [!UICONTROL Connection] veld.
1. Selecteren **[!DNL Google]** als verbindingstype.
1. Voer een naam in voor de verbinding.
1. (Optioneel) Voer uw [!UICONTROL [!DNL Google] Client ID] en [!UICONTROL Client Secret].
1. Klikken **[!UICONTROL Continue]** om de verbinding tot stand te brengen en terug naar de module te gaan.

### Verbinding maken met andere e-mailservices (SMAP)

De verbinding van SMAP staat u toe om tot uw brievenbus ver toegang te hebben en berichten in uw brievenbus te lezen of te manipuleren. De SMAP-verbinding wordt door de meeste e-mailmodules gebruikt.

1. Klik in een willekeurige e-mailmodule op **[!UICONTROL Add]** naast de [!UICONTROL Connection] veld.
1. Selecteren **[!UICONTROL Others (SMTP)]** als verbindingstype.
1. Voer een **[!UICONTROL Name]** voor de verbinding.
1. Selecteer uw **[!UICONTROL Email provider]** in de lijst. Selecteer Overige als uw e-mailprovider niet in de lijst voorkomt.
1. Voer uw **[!UICONTROL Email address]**, **[!UICONTROL Your full name]**, uw **[!UICONTROL User name]** en uw **[!UICONTROL Password]**.
1. (Voorwaardelijk) Als uw provider zich niet in de lijst bevindt, voert u uw **[!UICONTROL SMTP server]** en **[!UICONTROL Port]** en geeft u op of u **[!UICONTROL Use a secure connection (TLS)]**. Om deze informatie te vinden, controleer [!UICONTROL Help] sectie voor uw brievenbus. Neem contact op met uw e-mailprovider als deze gegevens niet beschikbaar zijn.
1. Klikken **[!UICONTROL Continue]** om de verbinding tot stand te brengen en terug naar de module te gaan.

## [!UICONTROL Email] modules en hun velden

Wanneer u [!UICONTROL Email] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Afhankelijk van factoren zoals uw toegangsniveau in de app of service, kunnen er naast deze velden mogelijk extra velden worden weergegeven. Een bolde titel in een module wijst op een vereist gebied.

Sommige e-mailvelden bevatten mogelijk al gegevens omdat u deze in een andere module hebt gebruikt in het scenario. Raadpleeg de documentatie bij de e-mail Help als u hierover informatie nodig hebt.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>De unieke e-mailid wordt &#39;[!UICONTROL Email ID (UID)]&#39; is de id van de e-mail. De e-mailid is specifiek voor elke map van de e-mail.

* [Triggers](#triggers)
* [Handelingen](#actions)
* [Iteratoren](#iterators)

### Triggers

#### [!UICONTROL Watch Emails]

Triggers wanneer een nieuw e-mailbericht wordt ontvangen voor verwerking volgens opgegeven criteria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het verbinden van uw e-mailaccount met [!UICONTROL Workfront Fusion], zie <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Uw e-mail verbinden met [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] </td> 
   <td> <p>Selecteer de map met de e-mails die u wilt controleren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criteria]</p> </td> 
   <td> <p>Selecteer de criteria aan de hand waarvan je e-mailberichten wilt bekijken:</p> 
    <ul> 
     <li>[!UICONTROL All Emails]</li> 
     <li>[!UICONTROL Only Read Emails]</li> 
     <li>[!UICONTROL Only Unread Emails]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sender Email Address] </td> 
   <td> <p>Voer het e-mailadres in van de afzender wiens e-mails u wilt volgen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Recipient Email Address]</td> 
   <td> <p> Voer het e-mailadres in van de ontvanger van wie u de e-mails wilt bekijken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Voer het onderwerp in van het e-mailbericht dat u wilt bekijken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Phrase] </td> 
   <td> <p>Voer trefwoorden in om alleen die e-mailberichten met specifieke zinsdelen te bekijken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mark message(s) as read when fetched]</td> 
   <td> <p>Schakel deze optie in om de ongelezen e-mail te markeren zoals deze wordt gelezen nadat de details zijn opgehaald.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of results]</td> 
   <td> <p> Het maximum aantal e-mailberichten [!DNL Workfront Fusion] moet tijdens één cyclus van de scenariouitvoering worden geretourneerd.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Handelingen

* [[!UICONTROL Send an Email]](#send-an-email)
* [[!UICONTROL Create a Draft]](#create-a-draft)
* [[!UICONTROL Mark an Email as Read]](#mark-an-email-as-read)
* [[!UICONTROL Mark an Email as Unread]](#mark-an-email-as-unread)
* [[!UICONTROL Move an Email]](#move-an-email)
* [[!UICONTROL Copy an Email]](#copy-an-email)
* [[!UICONTROL Delete an Email]](#delete-an-email)
* [[!UICONTROL Get Emails]](#get-emails)

#### [!UICONTROL Send an Email]

Hiermee verzendt u een nieuwe e-mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het verbinden van uw e-mailaccount met [!DNL Workfront Fusion], zie <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Uw e-mail verbinden met [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Save Message after Sending]</td> 
   <td>Nadat het e-mailbericht is verzonden, wordt het opgeslagen in uw postvak. Schakel deze optie in als u de e-mails die u hebt verzonden wilt opslaan met [!DNL Workfront Fusion] aan de <i>[!UICONTROL Sent mail]</i> of een andere map in uw postvak. Sommige e-mailservices, zoals [!DNL Gmail], sla verzonden berichten automatisch op.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL To] </td> 
   <td> <p>Voeg de e-mailadressen toe waarnaar u de e-mail wilt verzenden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Voer de onderwerpregel van de e-mail in of wijs deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
   <td> <p>Selecteer [!UICONTROL content] type voor de e-mail:</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Plaintext]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content] </td> 
   <td> <p>Voer de e-mailinhoud in of wijs deze toe in de indeling HTML met behulp van HTML-tags of in de normale tekst, afhankelijk van wat u hebt gekozen in het dialoogvenster [!UICONTROL Content Type] veld.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Een bijlage toevoegen:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Voer de bestandsnaam in. Bijvoorbeeld voorbeeld voorbeeld voorbeeld.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Voer het pad naar de map in waar u de bijlage wilt uploaden.</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>Voer de [!UICONTROL content ID] om de bijlage (afbeelding) in te voegen in de inhoud.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy Recipient] </td> 
   <td> <p>Voer een of meer e-mailadressen in of wijs deze toe waarnaar u een kopie van deze e-mail wilt verzenden. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Blind Copy Recipient]</td> 
   <td> <p> Voer een of meer e-mailadressen in of wijs deze toe waarnaar u een kopie van deze e-mail wilt verzenden zonder dat het e-mailadres in de e-mail wordt weergegeven.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL From] </td> 
   <td> <p>Voer het e-mailadres (en de naam, indien nodig) in of wijs dit toe in het dialoogvenster [!UICONTROL From] in de e-mail. </p> <p>Belangrijk: Gebruik de juiste syntaxis: <code>name@email.com</code> of <code>"Name" name@email.com</code>.</p> <p>Opmerking: Normaal gesproken [!DNL Workfront Fusion] gebruikt het e-mailadres dat u hebt ingevoerd bij het maken van de verbinding als het verzendadres. Als u een ander e-mailadres opgeeft, kan er een fout optreden bij het verzenden van een bericht omdat uw account geen toestemming heeft om e-mails van een ander adres te verzenden dan uw eigen adres. Bijv. <code>test@mail.com</code> of "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>Voer het e-mailadres in dat in het dialoogvenster verschijnt of wijs het e-mailadres toe [!UICONTROL Sender] in de e-mail.</p> <p>Tip: Als u niet zeker weet of u dit veld of het veld Van wilt gebruiken, raden wij u aan het veld Van te kiezen.</p> <p>Belangrijk: Gebruik de juiste syntaxis: <code>name@email.com</code> of <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reply-To]</td> 
   <td> <p> Als u op deze e-mail antwoorden wilt verzenden naar een ander adres dan het adres 'van', voer dan het e-mailadres in waarnaar u op deze e-mail wilt antwoorden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL In-Reply-To]</td> 
   <td> <p> Als u een specifieke e-mail beantwoordt, voert u de id in van het e-mailbericht waarop u reageert of wijst u deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL References] </td> 
   <td> <p>Voer de bericht-id's in van alle reacties in de thread.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Priority]</p> </td> 
   <td> <p>Selecteer de prioriteit van de e-mail:</p> 
    <ul> 
     <li>[!UICONTROL High]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Low]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
   <td> <p>Voeg de kopteksten toe:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>Voeg de toets toe. Bijvoorbeeld: [!UICONTROL Sender], [!UICONTROL Date], [!UICONTROL To], enzovoort.</p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Voer de waarde voor de toets in.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a Draft]

Hiermee maakt u een nieuw concept en voegt u dit toe aan een geselecteerde map.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het verbinden van uw e-mailaccount met [!UICONTROL Workfront Fusion], zie <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Uw e-mail verbinden met [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Selecteer de map waarin u het concept-e-mailbericht wilt maken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL To] </td> 
   <td> <p>Voer het e-mailadres in of wijs het toe waarnaar u de e-mail wilt verzenden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Voer de onderwerpregel van de e-mail in of wijs deze toe.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
   <td> <p>Selecteer het inhoudstype voor de e-mail:</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Plain Text]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content] </td> 
   <td> <p>Voer de e-mailinhoud in of wijs deze toe in de indeling HTML met behulp van HTML-tags of in de normale tekst, afhankelijk van wat u hebt gekozen in het dialoogvenster [!UICONTROL Content Type] veld.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Een bijlage toevoegen:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Voer de bestandsnaam in. Bijvoorbeeld voorbeeld voorbeeld voorbeeld.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Voer het pad naar de map in waar u de bijlage wilt uploaden.</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>Voer de inhoud-id in om de bijlage (afbeelding) in de inhoud in te voegen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy Recipient] </td> 
   <td> <p>Voer een of meer e-mailadressen in of wijs deze toe waarnaar u een kopie van deze e-mail wilt verzenden. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Blind Copy Recipient]</td> 
   <td> <p> Voer een of meer e-mailadressen in of wijs deze toe waarnaar u een kopie van deze e-mail wilt verzenden zonder dat het e-mailadres in de e-mail wordt weergegeven.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL From] </td> 
   <td> <p>Voer het e-mailadres (en de naam, indien nodig) in of wijs dit toe in het dialoogvenster [!UICONTROL From] in de e-mail. </p> <p>Belangrijk: Gebruik de juiste syntaxis: <code>name@email.com</code> of <code>"Name" name@email.com</code>.</p> <p>Opmerking: Normaal gesproken [!DNL Workfront Fusion] gebruikt het e-mailadres dat u hebt ingevoerd bij het maken van de verbinding als het verzendadres. Als u een ander e-mailadres opgeeft, kan er een fout optreden bij het verzenden van een bericht omdat uw account geen toestemming heeft om e-mails van een ander adres te verzenden dan uw eigen adres. Bijv. <code>test@mail.com</code> of "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>Voer het e-mailadres in dat in het dialoogvenster verschijnt of wijs het e-mailadres toe [!UICONTROL Sender] in de e-mail.</p> <p>Tip: Als u niet zeker weet of u dit veld of het veld Van wilt gebruiken, raden wij u aan het veld Van te kiezen.</p> <p>Belangrijk: Gebruik de juiste syntaxis: <code>name@email.com</code> of <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Reply-To]</td> 
   <td> <p> Als u wilt dat antwoorden op deze e-mail naar een ander adres worden verzonden dan "[!UICONTROL from]", voer het e-mailadres in waarnaar je op deze e-mail wilt reageren.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL In-Reply-To]</td> 
   <td> <p> Als u een specifieke e-mail beantwoordt, voert u de id in van het e-mailbericht waarop u reageert of wijst u deze toe.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL References] </td> 
   <td> <p>Voer de bericht-id's in van alle reacties in de thread.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Priority]</p> </td> 
   <td> <p>Selecteer de prioriteit van de e-mail:</p> 
    <ul> 
     <li>[!UICONTROL High]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Low]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
   <td> <p>Voeg de kopteksten toe:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>Voeg de toets toe. Bijvoorbeeld Afzender, Datum, Aan, enzovoort.</p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Voer de waarde voor de toets in.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mark an Email as Read]

Hiermee markeert u een e-mail of concept in een geselecteerde map als gelezen door het instellen van de optie [!UICONTROL Read] markering.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het verbinden van uw e-mailaccount met [!UICONTROL Workfront Fusion], zie <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Uw e-mail verbinden met [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Selecteer de map van het e-mailbericht dat u als gelezen wilt markeren. Voorbeeld: Primair.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Email ID (UID)]</p> </td> 
   <td> <p>Voer de e-mailid in van het e-mailbericht dat u als gelezen wilt markeren.</p> <p>U kunt de id van het e-mailbericht ophalen met de [!UICONTROL Email] &gt;[!UICONTROL Watch Email] of [!UICONTROL Search Email] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mark an Email as Unread]

Hiermee markeert u een e-mail of concept in een geselecteerde map als ongelezen door de markering Ongelezen in te stellen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het verbinden van uw e-mailaccount met [!UICONTROL Workfront Fusion], zie <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Uw e-mail verbinden met [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Selecteer de map van het e-mailbericht dat u als ongelezen wilt markeren. Voorbeeld: Primair.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Email ID (UID)]</p> </td> 
   <td> <p>Voer de e-mailid in van het e-mailbericht dat u als ongelezen wilt markeren.</p> <p>U kunt de id van het e-mailbericht ophalen met de [!UICONTROL Email] &gt;[!UICONTROL Watch Email] of [!UICONTROL Search Email] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Move an Email]

Hiermee verplaatst u een gekozen e-mail of concept naar een geselecteerde map.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het verbinden van uw e-mailaccount met [!UICONTROL Workfront Fusion], zie <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Uw e-mail verbinden met [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Folder]</td> 
   <td>Selecteer de map met het e-mailbericht waaruit u het e-mailbericht wilt verplaatsen. Voorbeeld: Primair.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination Folder]</td> 
   <td> <p> Selecteer de map waaraan u de e-mail wilt toevoegen. Voorbeeld: Werk.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Email ID (UID)]</p> </td> 
   <td> <p>Voer de e-mailid in van het e-mailbericht dat u naar de doelmap wilt verplaatsen.</p> <p>U kunt de id van het e-mailbericht ophalen met de [!UICONTROL Email] &gt;[!UICONTROL Watch Email] of [!UICONTROL Search Email] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copy an Email]

Hiermee kopieert u een e-mail of concept naar een geselecteerde map.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het verbinden van uw e-mailaccount met [!UICONTROL Workfront Fusion], zie <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Uw e-mail verbinden met [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Folder]</td> 
   <td>Selecteer de map waaruit u de e-mail wilt kopiëren. Voorbeeld: Primair.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination Folder]</td> 
   <td> <p> Selecteer de map waarnaar u de e-mail wilt kopiëren. Voorbeeld: Werk.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Email ID (UID)]</p> </td> 
   <td> <p>Voer de e-mailid in van het e-mailbericht dat u naar de doelmap wilt kopiëren.</p> <p>U kunt de id van het e-mailbericht ophalen met de [!UICONTROL Email] &gt;[!UICONTROL Watch Email] of [!UICONTROL Search Email] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete an Email]

Hiermee verwijdert u een e-mail of concept uit de geselecteerde map.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het verbinden van uw e-mailaccount met [!UICONTROL Workfront Fusion], zie <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Uw e-mail verbinden met [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Selecteer de map van het e-mailbericht dat u wilt verwijderen. Voorbeeld: Primair.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Email ID (UID)]</p> </td> 
   <td> <p>Voer de e-mailid in van het e-mailbericht dat u wilt verwijderen.</p> <p>U kunt de id van het e-mailbericht ophalen met de [!UICONTROL Email] &gt;[!UICONTROL Watch Email] of [!UICONTROL Search Email] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expunge]</td> 
   <td> <p>Schakel deze optie in als u wilt dat de module alle berichten die zijn gemarkeerd als permanent kan verwijderen [!UICONTROL Deleted] in de momenteel geopende brievenbus.</p> <p>Opmerking: In [!DNL Gmail], wordt dit gedrag bepaald door de instelling in [!UICONTROL Settings] &gt;[!UICONTROL Forwarding POP/IMAP in IMAP access] sectie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Emails]

Retourneert e-mailberichten die voldoen aan de opgegeven criteria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het verbinden van uw e-mailaccount met [!UICONTROL Workfront Fusion], zie <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Uw e-mail verbinden met [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] </td> 
   <td> <p>Selecteer de map met de e-mails die u wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mark message(s) as read when fetched] </td> 
   <td> <p>Schakel deze optie in als u de ongelezen e-mail wilt markeren zoals deze is gelezen nadat u de details hebt opgehaald.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criteria]</p> </td> 
   <td> <p>Selecteer de criteria voor de e-mails die u wilt ophalen:</p> 
    <ul> 
     <li>[!UICONTROL All Emails]</li> 
     <li>[!UICONTROL Only Read Emails]</li> 
     <li>[!UICONTROL Only Unread Emails]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sender Email Address] </td> 
   <td> <p>Voer het e-mailadres in of wijs het e-mailadres toe van de afzender van wie u de e-mails wilt ophalen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Recipient Email Address]</td> 
   <td> <p> Voer het e-mailadres in of wijs het e-mailadres toe van de ontvanger van wie u de e-mails wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL From date] </td> 
   <td> <p>Voer de datum in of wijs de datum toe waarop de e-mails die op of na de opgegeven datum zijn verwerkt, moeten worden opgehaald.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Before date]</td> 
   <td> <p> Voer de datum in of wijs de datum toe waarop de e-mails die op of voor de opgegeven datum zijn verwerkt, moeten worden opgehaald.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>Voer het onderwerp in van de e-mail die u wilt ophalen of wijs het onderwerp ervan toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Phrase] </td> 
   <td> <p>Voer trefwoorden in of wijs deze toe om alleen die e-mails met specifieke woordgroepen op te halen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email ID (UID)]</td> 
   <td> <p> Voer de e-mailid (UID) in van het e-mailbericht waarvan u de gegevens wilt ophalen.</p> <p>U kunt de unieke id van het e-mailbericht ophalen met [!DNL Workfront Fusion]s[!UICONTROL  Watch Email] of [!UICONTROL Search Email] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of results]</td> 
   <td> <p> Het maximum aantal e-mailberichten [!DNL Workfront Fusion] moet tijdens één cyclus van de scenariouitvoering worden geretourneerd.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Continue the execution of the route even if the module returns no results]</td> 
   <td> <p> Selecteer deze optie als u de module wilt blijven uitvoeren, zelfs als er geen resultaten worden geretourneerd.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Iteratoren

#### [!UICONTROL Iterate Attachments]

De rentetarieven ontvingen gehechtheid één voor één.

In de module E-mailiterator kunt u e-mailbijlagen afzonderlijk beheren. U kunt bijvoorbeeld instellen dat u e-mailberichten wilt bekijken om de e-mails met bijlagen te doorlopen en waarschuwingen te ontvangen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source module]</td> 
   <td> <p>Selecteer de module die het e-mailbericht weergeeft met de bijlagen die u wilt doorlopen.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie over iterators, zie [Interventiemodule in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
