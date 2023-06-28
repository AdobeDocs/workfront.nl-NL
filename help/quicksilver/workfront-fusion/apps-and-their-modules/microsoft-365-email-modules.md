---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft Office 365-e-mail
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die Microsoft Office 365 E-mail gebruiken, evenals het verbinden met veelvoudige derdetoepassingen en de diensten.
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1502'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Email]

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!UICONTROL Microsoft Office 365 Email]en deze verbinding maken met meerdere toepassingen en services van derden.

Voor gebruik [!UICONTROL Office 365 Email] with [!DNL Adobe Workfront Fusion]is het noodzakelijk [!UICONTROL Office 365 account]. U kunt er een maken op www.office.com.

Voor instructies over het aansluiten van uw [!UICONTROL Office 365] account aan [!DNL Workfront Fusion], zie [Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies](../../workfront-fusion/connections/connect-to-fusion-general.md)

Nadat u toestemming hebt verleend, wordt u teruggeleid naar [!UICONTROL Workfront Fusion] beleidspagina waar u kunt blijven creërend uw scenario.

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

Te gebruiken [!DNL Microsoft Office 365 Email] modules, moet u een [!DNL Microsoft Office 365 Email] account.

## [!DNL Microsoft Office 365 Email] modules en hun velden

Wanneer u [!DNL Microsoft Office 365 Email] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Microsoft Office 365 Email] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Bericht](#message)
* [Conceptbericht](#draft-message)
* [Bijlage](#attachment)
* [Overige](#other)

### Bericht

* [[!UICONTROL Watch Messages]](#watch-messages)
* [[!UICONTROL Search messages]](#search-messages)
* [[!UICONTROL Get a message]](#get-a-message)
* [[!UICONTROL Create and Send a Message]](#create-and-send-a-message)
* [[!UICONTROL Move a Message]](#move-a-message)
* [[!UICONTROL Delete a Message]](#delete-a-message)

#### [!UICONTROL Watch Messages]

Triggers wanneer een nieuw e-mailbericht wordt verzonden of ontvangen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Watch Messages]</p> </td> 
   <td> <p>Selecteer de berichten die u wilt bekijken:</p> 
    <ul> 
     <li>[!UICONTROL Only Unread]</li> 
     <li>[!UICONTROL Only read]</li> 
     <li>[!UICONTROL All]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder]</td> 
   <td> <p>Selecteer de map met de berichten die u wilt bekijken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Voer uw zoekopdracht in. Voor informatie over hoe te om een onderzoeksvraag te schrijven, zie [!DNL Microsoft] ondersteuningsartikel <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">E-mail en personen zoeken in [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Voer het maximum aantal berichten in [!DNL Workfront Fusion] moet tijdens één cyclus van de scenariouitvoering worden geretourneerd.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search messages]

Hiermee zoekt u berichten op basis van specifieke criteria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder]</td> 
   <td> <p>Selecteer de map met de berichten die u wilt doorzoeken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>Voer uw zoekopdracht in. Voor informatie over hoe te om een onderzoeksvraag te schrijven, zie [!DNL Microsoft] ondersteuningsartikel <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">E-mail en personen zoeken in [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td> <p>Selecteer hoe u de resultaten wilt bestellen:</p> 
    <ul> 
     <li>[!UICONTROL Subject (Ascending or descending)]</li> 
     <li>[!UICONTROL Created Date Time (Ascending or descending)]</li> 
     <li>[!UICONTROL Last Modified Date Time (Ascending or descending)]</li> 
     <li>[!UICONTROL Received Date Time (Ascending or descending)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Voer het maximum aantal berichten in [!DNL Workfront Fusion] moet tijdens één cyclus van de scenariouitvoering worden geretourneerd.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a message]

Hiermee worden de metagegevens van een bepaald bericht opgehaald

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Selecteer of wijs identiteitskaart van het bericht toe u meta-gegevens voor wilt terugwinnen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get MIME contents]</td> 
   <td>Schakel deze optie in om gegevens over de MIME-inhoud van het bericht op te halen. [!UICONTROL MIME] inhoud kan afbeeldingen, audio, video of andere bestandstypen bevatten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create and Send a Message]

Hiermee maakt en verstuurt u een e-mailbericht.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Voer de onderwerpregel van het bericht in of wijs deze toe.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>Selecteer of de hoofdinhoud van het bericht HTML of Tekst is.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td> <p>Voer de tekst van de berichttekst van de e-mail in of wijs deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Selecteer het belang van de e-mail</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>Voeg het e-mailadres toe waarnaar u de berichten wilt verzenden:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Voer de naam van de contactpersoon in</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Voer het e-mailadres van de contactpersoon in.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Voeg de ontvangers toe die u een exemplaar van het bericht wilt ontvangen:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Voer de naam van de contactpersoon in</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Voer het e-mailadres van de contactpersoon in.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bcc Recipients]</p> </td> 
   <td> <p>Voeg de ontvangers toe die u in het bericht wilt kopiëren, zonder dat andere ontvangers hun namen of e-mailadressen kunnen zien:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Voer de naam van de contactpersoon in</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Voer het e-mailadres van de contactpersoon in.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Voeg de bijlagen toe aan de e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Voer de bestandsnaam in. Voorbeeld: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Voer de bestandsgegevens in op het veld of wijs de bron van het bestand toe.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Internet Message Headers]</td> 
   <td> <p>Voeg de berichtkopteksten voor e-mail toe.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Voer de naam van de koptekst in</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Voer een waarde in voor de koptekst.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Move a Message]

Verplaatst een e-mailbericht naar een geselecteerde map in de postbus.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Selecteer of wijs identiteitskaart van het bericht toe u naar een verschillende omslag wilt bewegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder] </td> 
   <td> <p>Selecteer of wijs identiteitskaart van de omslag toe waar u het bericht wilt bewegen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Message]

Hiermee verwijdert u een bestaand e-mailbericht.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Selecteer of wijs identiteitskaart van het bericht toe u wilt schrappen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Conceptbericht

* [Conceptbericht maken](#create-a-draft-message)
* [Conceptbericht verzenden](#send-a-draft-message)
* [Een bericht bijwerken](#update-a-message)

#### [!UICONTROL Create a Draft Message]

Hiermee maakt u een nieuw e-mailbericht.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Voer de onderwerpregel van het bericht in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>Selecteer of de hoofdinhoud van het bericht HTML of Tekst is.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td> <p>Voer de tekst van de berichttekst van de e-mail in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Selecteer het belang van de e-mail</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>Voeg de ontvangers toe waarnaar u de berichten wilt verzenden:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Voer de naam van de contactpersoon in</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Voer het e-mailadres van de contactpersoon in.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Voeg de ontvangers toe u een exemplaar van het bericht wilt ontvangen:</p> 
    <ul> 
     <li> <p><strong>Naam</strong> </p> <p>Voer de naam van de contactpersoon in</p> </li> 
     <li> <p><strong>E-mailadres</strong> </p> <p>Voer het e-mailadres van de contactpersoon in.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>BCC-ontvangers</p> </td> 
   <td> <p>Voeg de ontvangers toe die u in het bericht wilt kopiëren, zonder dat andere ontvangers hun namen of e-mailadressen kunnen zien:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Voer de naam van de contactpersoon in</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Voer het e-mailadres van de contactpersoon in.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Voeg de bijlagen toe aan de e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Voer de bestandsnaam in. Voorbeeld: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Voer de bestandsgegevens in op het veld of wijs de bron van het bestand toe.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Send a Draft Message]

Hiermee verzendt u een e-mailbericht dat momenteel in concept is.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Draft Message ID]</td> 
   <td> <p> Selecteer of wijs identiteitskaart van het Bericht van het ontwerp toe u wilt verzenden.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a Message]

Werkt een bestaand bericht bij.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a message ID]</td> 
   <td> <p>Selecteer hoe u het bericht wilt identificeren dat u wilt bijwerken:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter Manually]</strong> </p> <p>Voer de bericht-id in of wijs deze toe.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Selecteer de map met het bericht dat u wilt bijwerken en selecteer vervolgens het bericht</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Voer de onderwerpregel van het bericht in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td> <p>Voer de tekst van de berichttekst van de e-mail in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Selecteer het belang van de e-mail</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>Voeg het e-mailadres toe waarnaar u de berichten wilt verzenden:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Voer de naam van de contactpersoon in</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Voer het e-mailadres van de contactpersoon in.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>Voeg de ontvangers toe u een exemplaar van het bericht wilt ontvangen:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Voer de naam van de contactpersoon in</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Voer het e-mailadres van de contactpersoon in.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bcc Recipients]</p> </td> 
   <td> <p>Voeg de ontvangers toe die u in het bericht wilt kopiëren, zonder dat andere ontvangers hun namen of e-mailadressen kunnen zien:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Voer de naam van de contactpersoon in</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>Voer het e-mailadres van de contactpersoon in.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Voeg de bijlagen toe aan de e-mail:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>Voer de bestandsnaam in. Voorbeeld: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Voer de bestandsgegevens in op het veld of wijs de bron van het bestand toe.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mark it as Read]</td> 
   <td>Schakel deze optie in om het bijgewerkte bericht als gelezen te markeren.</td> 
  </tr> 
 </tbody> 
</table>

### Bijlage

* [[!UICONTROL List Attachments]](#list-attachments)
* [[!UICONTROL Download an Attachment]](#download-an-attachment)

#### [!UICONTROL List Attachments]

Deze module wint een lijst van gehechtheid terug die tot het gespecificeerde bericht behoort.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Selecteer of wijs identiteitskaart van het bericht toe u gehechtheid van wilt terugwinnen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal gehechtheid in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download an Attachment]

Deze module downloadt de opgegeven bijlage.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Selecteer of wijs identiteitskaart van het bericht toe dat de gehechtheid bevat u wilt downloaden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment ID]</td> 
   <td> <p>Voer de id in van de bijlage die u wilt downloaden of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Overige

* [[!UICONTROL Make an API Call]](#make-an-api-call)
* [[!UICONTROL Add an Attachment]](#add-an-attachment)

#### [!UICONTROL Make an API Call]

In deze module kunt u een aangepaste API-aanroep uitvoeren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Een pad invoeren ten opzichte van <code>https://graph.microsoft.com</code>. Voorbeeld:<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van de aanvraag toe in de vorm van een standaard JSON-object. Bijvoorbeeld: <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] Hiermee voegt u de machtigingsheaders voor u toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Voeg de query voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:  <p>Bij het gebruik van voorwaardelijke instructies zoals <code>if</code> in uw JSON, plaats de aanhalingstekens buiten de voorwaardelijke verklaring.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add an Attachment]

Deze module voegt een grote gehechtheid aan een bericht toe.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Selecteer of wijs identiteitskaart van het bericht toe u een gehechtheid aan wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Selecteer een bestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> </td> 
  </tr> 
 </tbody> 
</table>
