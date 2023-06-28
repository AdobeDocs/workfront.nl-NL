---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Gmail-modules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die Gmail gebruiken, evenals het verbinden met veelvoudige derdetoepassingen en de diensten.
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1548'
ht-degree: 0%

---

# [!DNL Gmail] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Gmail]en deze verbinding maken met meerdere toepassingen en services van derden.

Als u instructies bij het creëren van een scenario nodig hebt, zie [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Voor informatie over modules, zie [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Vereisten

Te gebruiken [!DNL Gmail] modules, moet u een [!DNL Gmail] account.

## Verbinden [!DNL Gmail] tot [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [Verbinden [!DNL Gmail] tot [!DNL Workfront Fusion] gebruiken van [!DNL G Suite]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [Verbinden [!DNL Gmail] tot [!DNL Workfront Fusion] gebruiken [!DNL gmail.com] of [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### Verbinden [!DNL Gmail] tot [!DNL Workfront Fusion] gebruiken[!DNL  G Suite] {#connect-gmail-to-workfront-fusion-using-g-suite}

Voor instructies over het aansluiten van uw [!DNL G Suite] account aan [!UICONTROL Workfront Fusion], zie [Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) in het artikel [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Verbinden [!DNL Gmail] tot [!DNL Workfront Fusion] gebruiken [!DNL gmail.com] of [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

Als u [!DNL @gmail.com] of [!DNL @googlemail.com] gebruiker u moet een cliënt OAuth op creëren [de [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) om een [!UICONTROL Client ID] en [!UICONTROL Client Secret].

Voor geleidelijke instructies op hoe te om de cliënt OAuth tot stand te brengen en te verkrijgen [!UICONTROL Client ID] en [!UICONTROL Client Secret], zie [Adobe Workfront Fusion met Google Services verbinden met behulp van een aangepaste OAuth-client](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] modules en hun velden

Wanneer u [!DNL Gmail] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Gmail] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Handelingen](#actions)
* [Iteratoren](#iterators)

### Triggers

#### [!UICONTROL Watch emails]

Deze triggermodule voert een scenario uit wanneer een nieuwe e-mail wordt ontvangen om te worden verwerkt.

De module retourneert alle standaardvelden die zijn gekoppeld aan de record of records, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies voor het aansluiten van uw [!DNL Gmail] account aan [!DNL Workfront Fusion], zie <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer de e-mailmap die u wilt controleren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Filter type] </td> 
   <td> <p>Selecteer het filtertype dat u wilt gebruiken om e-mailberichten te bekijken</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Simple filter]</strong> </p> <p>Vul de [!UICONTROL Criteria], [!UICONTROL Sender Email Address], [!UICONTROL Subject], en [!UICONTROL Search Phrase] velden</p> </li> 
     <li> <p> <strong>[!UICONTROL Gmail filter]</strong> </p> <p>In de [!UICONTROL Query] Voer de query in die u wilt gebruiken om e-mailberichten te filteren.</p> <p>Voor meer informatie over [!DNL Gmail] filters, zie <a href="https://support.google.com/mail/answer/7190">Zoekoperatoren</a> in de [!DNL Gmail] documentatie.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Criteria]</td> 
   <td>Selecteer of u wilt controleren [!UICONTROL all email], [!UICONTROL only read emails], of [!UICONTROL only unread] e-mails.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sender email address]</td> 
   <td> <p> Voer een e-mailadres in om alleen e-mails te volgen die van dat adres zijn verzonden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject]</td> 
   <td>Voer een tekstreeks in om alleen e-mails te bekijken waarin die tekstreeks in het onderwerp voorkomt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search phrase]</td> 
   <td>Voer een tekstreeks in om alleen e-mailberichten te bekijken die die tekstreeks ergens in de e-mail hebben.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mark email message(s) as read when fetched]</td> 
   <td> <p> Schakel deze optie in om opgehaalde e-mails te markeren als gelezen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of results]</td> 
   <td> <p> Stel het maximale aantal resultaten in dat [!DNL Workfront Fusion] werkt met één cyclus.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Handelingen

* [[!UICONTROL Send an email]](#send-an-email)
* [[!UICONTROL Create a draft]](#create-a-draft)
* [[!UICONTROL Mark an email as read]](#mark-an-email-as-read)
* [[!UICONTROL Mark an email as unread]](#mark-an-email-as-unread)
* [[!UICONTROL Move an email]](#move-an-email)
* [[!UICONTROL Copy an email]](#copy-an-email)
* [[!UICONTROL Delete an email]](#delete-an-email)
* [[!UICONTROL Modify email labels]](#modify-email-labels)

#### [!UICONTROL Send an email]

Deze actiemodule verzendt een nieuwe e-mail.

U geeft de ontvanger van de e-mail op.

De module retourneert de id van de e-mail en alle bijbehorende velden, samen met eventuele aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies voor het aansluiten van uw [!DNL Gmail] account aan [!DNL Workfront Fusion], zie <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] tot [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL From]</td> 
   <td> <p>Voer een e-mailadres van een afzender in of wijs dit toe.</p> <p>Opmerking: Als u een onjuist e-mailadres opgeeft, kan er een fout optreden bij het verzenden van een bericht omdat uw account geen toestemming heeft om e-mails te verzenden van een ander adres dan uw eigen adres.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>Klikken <strong>[!UICONTROL Add]</strong>Voer vervolgens het e-mailadres voor elke ontvanger in of wijs dit toe.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>Voer het onderwerp van de e-mail in of wijs deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Voer de e-mailinhoud (hoofdtekst van bericht) in of wijs deze toe. HTML-tags zijn toegestaan.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attachments] </td> 
   <td> <p>Klikken <strong>[!UICONTROL Add]</strong> om een bijlage toe te voegen. U kunt een bestand uit de vorige modules toewijzen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copy recipients]</td> 
   <td> <p> Klikken <strong>[!UICONTROL Add]</strong>Voer vervolgens het e-mailadres voor elke ontvanger van de kopie in of wijs dit toe.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Blind copy recipients]</td> 
   <td> <p> Klikken <strong>[!UICONTROL Add]</strong>Voer vervolgens het e-mailadres in of wijs het toe aan elke ontvanger van de blinde kopie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a draft]

In deze actiemodule wordt een nieuw e-mailconcept gemaakt en toegevoegd aan een map die u opgeeft.

U geeft de map op waarin u een concept wilt maken.

De module retourneert de id van het e-mailconcept en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies voor het aansluiten van uw [!DNL Gmail] account aan [!DNL Workfront Fusion], zie <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer [!DNL Gmail] map waarin u een concept wilt maken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>Klikken <strong>[!UICONTROL Add]</strong>Voer vervolgens het e-mailadres voor elke ontvanger in of wijs dit toe.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>Voer het onderwerp van de e-mail in of wijs deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Voer de e-mailinhoud (hoofdtekst van bericht) in of wijs deze toe. HTML-tags zijn toegestaan.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attachments] </td> 
   <td> <p>Klikken <strong>[!UICONTROL Add]</strong> om een bijlage toe te voegen. U kunt een bestand uit de vorige modules toewijzen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copy recipients]</td> 
   <td> <p> Klikken <strong>[!UICONTROL Add]</strong>Voer vervolgens het e-mailadres voor elke ontvanger van de kopie in of wijs dit toe.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Blind copy recipients]</td> 
   <td> <p> Klikken <strong>[!UICONTROL Add]</strong>Voer vervolgens het e-mailadres in of wijs het toe aan elke ontvanger van de blinde kopie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mark an email as read]

Deze actiemodule markeert een e-mail als gelezen.

U geeft de id van het e-mailbericht en de bijbehorende map op.

De module retourneert de id van de e-mail en alle bijbehorende velden, samen met eventuele aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies voor het aansluiten van uw [!DNL Gmail] account aan [!DNL Workfront Fusion], zie <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer [!DNL Gmail] map die de e-mail bevat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)]</td> 
   <td> <p> Voer de e-mailid in of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Mark an email as unread]

Deze actiemodule markeert een e-mail- of e-mailconcept als ongelezen.

U geeft de id van het e-mailbericht en de bijbehorende map op.

De module retourneert de id van de e-mail en alle bijbehorende velden, samen met eventuele aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies voor het aansluiten van uw [!DNL Gmail] account aan [!DNL Workfront Fusion], zie <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer [!DNL Gmail] map die de e-mail bevat.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)] </td> 
   <td> <p>Voer de e-mailid in of wijs deze toe aan het e-mailadres dat u als ongelezen wilt markeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Move an email]

Met deze handelingsmodule wordt een e-mail- of e-mailconcept verplaatst naar een map die u opgeeft.

U geeft de map, de doelmap en de id van de e-mail op.

De module retourneert de id van de e-mail en alle bijbehorende velden, samen met eventuele aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies voor het aansluiten van uw [!DNL Gmail] account aan [!DNL Workfront Fusion], zie <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer [!DNL Gmail] bronmap met het e-mailbericht dat u wilt verplaatsen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination folder]</td> 
   <td> <p> Selecteer [!DNL Gmail] Doelmap waarnaar u de e-mail wilt verplaatsen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)]</td> 
   <td> <p> Voer de e-mailid in of wijs deze toe aan het e-mailbericht dat u wilt verplaatsen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copy an email]

Met deze actiemodule kopieert u een e-mail- of e-mailconcept naar een map die u opgeeft.

U geeft de map, de doelmap en de id van de e-mail op.

De module retourneert de id van de e-mail en alle bijbehorende velden, samen met eventuele aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies voor het aansluiten van uw [!DNL Gmail] account aan [!DNL Workfront Fusion], zie <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer [!DNL Gmail] bronmap met het e-mailbericht dat u wilt kopiëren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination folder]</td> 
   <td> <p>Selecteer [!DNL Gmail] Doelmap waarnaar u de e-mail wilt kopiëren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)]</td> 
   <td> <p>Voer de e-mailid in of wijs deze toe van het e-mailbericht dat u wilt kopiëren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete an email]

Met deze actiemodule verwijdert u een e-mail- of e-mailconcept uit een map die u opgeeft.

De module retourneert de id van de e-mail en alle bijbehorende velden, samen met eventuele aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies voor het aansluiten van uw [!DNL Gmail] account aan [!DNL Workfront Fusion], zie <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL [!DNL Gmail] Bericht-ID]</p> </td> 
   <td> <p>Voer de e-mailid in of wijs deze toe van het e-mailbericht dat u wilt verwijderen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permanently] </td> 
   <td> <p>Schakel deze optie in als u wilt dat de module de e-mail permanent kan verwijderen in plaats van deze naar de prullenbak te verplaatsen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Modify email labels]

Deze actiemodule wijzigt het label van een e-mailbericht dat u opgeeft.

De module retourneert de id van de e-mail en alle bijbehorende velden, samen met eventuele aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies voor het aansluiten van uw [!DNL Gmail] account aan [!DNL Workfront Fusion], zie <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] tot [!UICONTROL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Gmail] Bericht-ID]</td> 
   <td> <p> Voer de e-mailid in of wijs deze toe van het e-mailbericht dat u wilt verwijderen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Labels to add]</p> </td> 
   <td> <p>Selecteer of wijs het label toe u aan het geselecteerde e-mailbericht wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Labels to remove]</td> 
   <td> <p> Selecteer of wijs het label toe u uit het geselecteerde e-mailbericht wilt verwijderen.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>[!UICONTROL Label to add] en [!UICONTROL Label to remove] velden worden alleen door de gebruiker gemaakte labels geladen.

### Iteratoren

#### [!UICONTROL Iterate attachments]

U kunt e-mailbijlagen doorlopen. Elke bijlage is een afzonderlijke bundel in de output van de module. Zie voor meer informatie [Iteratormodule in Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source module] </td> 
   <td> <p>Selecteer de module waarvan u bijlagen wilt doorlopen. </p> </td> 
  </tr> 
 </tbody> 
</table>
