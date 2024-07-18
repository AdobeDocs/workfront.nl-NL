---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft Office 365-kalender
description: In een  [!DNL Adobe Workfront Fusion]  scenario, kunt u werkschema's automatiseren die Microsoft Office 365 Kalender gebruiken, evenals het met veelvoudige derstoepassingen en de diensten verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Calendar]

In een [!DNL Adobe Workfront Fusion] -scenario kunt u workflows automatiseren die [!DNL Microsoft Office 365 Calendar] gebruiken en deze koppelen aan meerdere toepassingen en services van derden.

Als u [!DNL Office 365 Calendar] met [!DNL Adobe Workfront Fusion] wilt gebruiken, hebt u een [!DNL Office 365 Excel] -account nodig. U kunt één in [ www.office.com ](https://www.office.com/) tot stand brengen.

Voor instructies over het verbinden van uw Bureau 365 rekening met [!DNL Workfront Fusion], zie [ een verbinding aan Adobe  [!DNL Workfront Fusion]  - Basisinstructies ](../../workfront-fusion/connections/connect-to-fusion-general.md) creëren

Nadat u toestemming hebt verleend, wordt u teruggeleid naar de [!UICONTROL Workfront Fusion] beheerpagina waar u kunt doorgaan met het maken van uw scenario.

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
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het [!UICONTROL Select] - of [!UICONTROL Prime] [!DNL Adobe Workfront] -abonnement hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Als u [!DNL Microsoft Office 365 Calendar] -modules wilt gebruiken, moet u een [!DNL Microsoft Office 365 Calendar] -account hebben.

## De service [!DNL Office 365 Calendar] verbinden met [!DNL Workfront Fusion]

Voor instructies over het aansluiten van uw [!DNL Office 365 Calendar] rekening aan [!UICONTROL Workfront Fusion], zie [ een verbinding tot stand brengen [!UICONTROL Adobe Workfront Fusion] - Basisinstructies ](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Sommige Microsoft-toepassingen gebruiken dezelfde verbinding, die is gekoppeld aan individuele gebruikersmachtigingen. Daarom bij het creëren van een verbinding, toont het scherm van de toestemmingstoestemming om het even welke toestemmingen die eerder aan de verbinding van deze gebruiker werden verleend, naast om het even welke nieuwe toestemmingen nodig voor de huidige toepassing.
>
>Bijvoorbeeld, als een gebruiker &quot;Gelezen lijst&quot;toestemmingen heeft die via de schakelaar van Excel worden verleend en dan een verbinding in de schakelaar van Vooruitzichten creeert om e-mails te lezen, zal het scherm van de toestemmingstoestemming zowel de reeds verleende &quot;Gelezen lijst&quot;toestemming en de onlangs vereiste &quot;Schrijf e-mail&quot;toestemming tonen.

## [!DNL Microsoft Office 365 Calendar] modules en hun velden

Wanneer u [!DNL Microsoft Office 365 Calendar] modules configureert, geeft [!DNL Workfront Fusion] de onderstaande velden weer. Daarnaast kunnen aanvullende [!DNL Microsoft Office 365 Calendar] -velden worden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Voor meer informatie, zie [ informatie van de Kaart van één module aan een andere in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Gebeurtenis](#event)
* [Kalender](#calendar)
* [Overige](#other)

### Gebeurtenis

* [[!UICONTROL Watch Events]](#watch-events)
* [[!UICONTROL Search Events]](#search-events)
* [[!UICONTROL Get an Event]](#get-an-event)
* [[!UICONTROL Create an Event]](#create-an-event)
* [[!UICONTROL Update an Event]](#update-an-event)
* [[!UICONTROL Delete an Event]](#delete-an-event)

#### [!UICONTROL Watch Events]

Deze triggermodule haalt de details van een gebeurtenis op wanneer de gebeurtenis in de geselecteerde kalender wordt gemaakt, bijgewerkt, verwijderd, gestart of beëindigd.

>[!NOTE]
>
>Selecteer [!UICONTROL By Updated Time] in het veld [!UICONTROL Watch events] om te controleren op verwijderde exemplaren van een gebeurtenisreeks. Deze module controleert niet op verwijderde, enkele gebeurtenissen of verwijderde gebeurtenisreeksen.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] rekening aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch events]</td> 
   <td> <p>Selecteer hoe u gebeurtenissen wilt bekijken.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL By Created Time]</strong> </p> <p>Kijk naar nieuwe gebeurtenissen.</p> </li> 
     <li> <p><strong>[!UICONTROL By Updated Time]</strong> </p> <p>Kijk naar bijgewerkte gebeurtenissen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar Group ID]</td> 
   <td>Selecteer de [!UICONTROL calendar group] die de kalender bevat waarin u gebeurtenissen wilt bekijken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar]</td> 
   <td> <p>Selecteer de specifieke kalender die u wilt bekijken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Stel de filtervoorwaarden in op filterresultaten op onderwerp, gebeurtenis-id of hoofdtekst.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Voer het maximale aantal berichten in dat [!DNL Workfront Fusion] tijdens één cyclus van de uitvoering van het scenario moet retourneren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search Events]

In deze zoekmodule worden de details van een gebeurtenis opgehaald wanneer de gebeurtenis in de geselecteerde kalender wordt gemaakt, bijgewerkt, verwijderd, gestart of beëindigd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] rekening aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar Group ID]</td> 
   <td>Selecteer de [!UICONTROL calendar group] die de kalender bevat waarin u gebeurtenissen wilt bekijken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar]</td> 
   <td> <p>Selecteer de specifieke kalender die u wilt bekijken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Stel de filtervoorwaarden in op filterresultaten. U kunt filteren op de volgende eigenschappen:</p> 
    <ul> 
     <li>[!UICONTROL Subject]</li> 
     <li>[!UICONTROL Event ID]</li> 
     <li>[!UICONTROL Created Date Time]</li> 
     <li>[!UICONTROL Last Modified Date Time]</li> 
     <li>[!UICONTROL Body Preview]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td> <p>Selecteer hoe u de resultaten wilt bestellen.</p> 
    <ul> 
     <li><strong>[!UICONTROL Subject]</strong>, oplopend of aflopend</li> 
     <li><strong>[!UICONTROL Created Date Time]</strong>, oplopend of aflopend</li> 
     <li><strong>[!UICONTROL Last Modified Date Time]</strong>, oplopend of aflopend</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Voer het maximale aantal gebeurtenissen in dat [!DNL Workfront Fusion] tijdens één cyclus van uitvoering van het scenario moet retourneren.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get an Event]

Deze actiemodule wint details van de gespecificeerde gebeurtenis terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] rekening aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Voer de id in van de gebeurtenis waarover u details wilt ophalen of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create an Event]

Deze actiemodule maakt een nieuwe gebeurtenis.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] rekening aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Voer een titel voor de gemaakte gebeurtenis in of wijs deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start date]</td> 
   <td> Voer één tijdstip in waarop de gebeurtenis begint in een gecombineerde datum- en tijdrepresentatie. Gebruik de notatie <code>({date}T{time}</code>, bijvoorbeeld <code>2017-08-29T04:00:00.0000000</code> . Voor een lijst van gesteunde datum en tijdformaten, zie <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref"> Druk van het Type in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL End date]</td> 
   <td> Voer één tijdstip in waarop de gebeurtenis eindigt op een gecombineerde datum- en tijdrepresentatie. Gebruik de notatie <code>{date}T{time}</code>, bijvoorbeeld <code>2017-08-29T04:00:00.0000000</code> . Voor een lijst van gesteunde datum en tijdformaten, zie <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref"> Druk van het Type in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder on]</td> 
   <td>Selecteer of u een herinnering voor deze gebeurtenis wilt activeren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder]</td> 
   <td>Voer het aantal minuten voor het begin van de gebeurtenis in of wijs het aantal minuten toe wanneer de herinnering moet worden geactiveerd.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Selecteer het belang van deze gebeurtenis.</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensitivity] </td> 
   <td> <p>Selecteer de gevoeligheid van deze gebeurtenis.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>De ontvanger ziet een "[!UICONTROL Please treat this as Personal]"bericht.</p> </li> 
     <li> <p><strong>[!UICONTROL Private]</strong> </p> <p>De ontvanger ziet een "[!UICONTROL Please treat this as Private]"bericht. Deze gebeurtenis wordt niet doorgestuurd of door de inbox-regels van de ontvanger omgeleid.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidential]</strong> </p> <p>De ontvanger ziet een "[!UICONTROL Please treat this as Confidential]"bericht. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content type]</td> 
   <td>Selecteer of de inhoud van de hoofdtekst onbewerkte tekst of HTML is.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td>Typ of wijs de hoofdtekst van het bericht toe dat aan de gebeurtenis is gekoppeld. De notatie kan HTML of tekst zijn (zoals opgegeven in het veld [!UICONTROL Body Content Type] hierboven).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Location]</td> 
   <td> <p>Voer de locatie-informatie voor de gebeurtenis in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Response requested]</td> 
   <td>Selecteer <strong>[!UICONTROL Yes]</strong> om de genodigde te vragen een antwoord op de uitnodiging voor de gebeurtenis te verzenden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show as]</td> 
   <td> <p>Selecteer hoe u de gebeurtenis wilt weergeven aan de personen die uw kalender weergeven.</p> 
    <ul> 
     <li>[!UICONTROL Free]</li> 
     <li>[!UICONTROL Tentative]</li> 
     <li>[!UICONTROL Busy]</li> 
     <li>[!UICONTROL Out of office]</li> 
     <li>[!UICONTROL Working elsewhere]</li> 
     <li>[!UICONTROL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attendees]</p> </td> 
   <td> <p>Voeg deelnemers aan de gebeurtenis toe.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Voer de naam van de deelnemer in.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>Voer het e-mailadres van de deelnemer in.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Category]</td> 
   <td>Typ of wijs de categorieën toe die u wilt dat de gebeurtenis op de kalender wordt weergegeven.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update an Event]

Deze actiemodule werkt een bestaande gebeurtenis bij.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] rekening aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td>Voer de id in van de gebeurtenis die u wilt bijwerken, of selecteer de id van de gebeurtenis.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>Voer een titel voor de gemaakte gebeurtenis in of wijs deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start date]</td> 
   <td> Voer één tijdstip in waarop de gebeurtenis begint in een gecombineerde datum- en tijdrepresentatie. Gebruik de notatie <code>{date}T{time}</code>, bijvoorbeeld <code>2017-08-29T04:00:00.0000000</code> . Voor een lijst van gesteunde datum en tijdformaten, zie <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref"> Druk van het Type in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL End date]</td> 
   <td> Voer één tijdstip in waarop de gebeurtenis eindigt op een gecombineerde datum- en tijdrepresentatie. Gebruik de notatie <code>({date}T{time}</code>, bijvoorbeeld <code>2017-08-29T04:00:00.0000000</code> . Voor een lijst van gesteunde datum en tijdformaten, zie <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref"> Druk van het Type in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder on]</td> 
   <td>Selecteer of u een herinnering voor deze gebeurtenis wilt activeren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder]</td> 
   <td>Voer het aantal minuten voor het begin van de gebeurtenis in of wijs het aantal minuten toe wanneer de herinnering moet worden geactiveerd.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>Selecteer het belang van deze gebeurtenis.</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensitivity] </td> 
   <td> <p>Selecteer de gevoeligheid van deze gebeurtenis.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>De ontvanger ziet een "[!UICONTROL Please treat this as Personal]"bericht.</p> </li> 
     <li> <p><strong>[!UICONTROL Private]</strong> </p> <p>De ontvanger ziet een "[!UICONTROL Please treat this as Private]"bericht. Deze gebeurtenis wordt niet doorgestuurd of door de inbox-regels van de ontvanger omgeleid.</p> </li> 
     <li> <p><strong>[!UICONTROL Confidential]</strong> </p> <p>De ontvanger ziet een "[!UICONTROL Please treat this as Confidential]"bericht. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content type]</td> 
   <td>Selecteer of de hoofdinhoud van het bericht dat aan de gebeurtenis is gekoppeld, onbewerkte tekst of HTML is.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td>Typ of wijs de hoofdtekst van het bericht toe dat aan de gebeurtenis is gekoppeld. De notatie kan HTML of tekst zijn (zoals opgegeven in het veld [!UICONTROL Body Content Type] hierboven).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Location]</td> 
   <td> <p>Voer de locatie-informatie voor de gebeurtenis in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Response requested]</td> 
   <td>Selecteer <strong>[!UICONTROL Yes]</strong> om de genodigde te vragen een antwoord op de uitnodiging voor de gebeurtenis te verzenden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show as]</td> 
   <td> <p>Selecteer hoe u de gebeurtenis wilt weergeven aan de personen die uw kalender weergeven.</p> 
    <ul> 
     <li>[!UICONTROL Free]</li> 
     <li>[!UICONTROL Tentative]</li> 
     <li>[!UICONTROL Busy]</li> 
     <li>[!UICONTROL Out of office]</li> 
     <li>[!UICONTROL Working elsewhere]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attendees]</p> </td> 
   <td> <p>Voeg deelnemers aan de gebeurtenis toe.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Voer de naam van de deelnemer in.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>Voer het e-mailadres van de deelnemer in.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Category]</td> 
   <td>Typ of wijs de categorieën toe die u wilt dat de gebeurtenis op de kalender wordt weergegeven.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete an Event]

Deze actiemodule verwijdert een bestaande gebeurtenis.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] rekening aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event ID]</td> 
   <td> <p>Voer de id in van de gebeurtenis die u wilt verwijderen of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Kalender

* [[!UICONTROL List Calendars]](#list-calendars)
* [[!UICONTROL Get a Calendar]](#get-a-calendar)
* [[!UICONTROL Create a Calendar]](#create-a-calendar)
* [[!UICONTROL Update a Calendar]](#update-a-calendar)
* [[!UICONTROL Delete a Calendar]](#delete-a-calendar)

#### [!UICONTROL List Calendars]

Deze zoekmodule haalt een lijst op met alle kalenders van de geverifieerde gebruiker.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] rekening aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar Group ID]</td> 
   <td>Selecteer de [!UICONTROL calendar group] die de kalenders bevat die u wilt weergeven.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Voer het maximale aantal kalenders in dat [!DNL Workfront Fusion] tijdens één cyclus van uitvoering van het scenario moet retourneren.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Calendar]

Deze actiemodule wint details over één enkele kalender terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] rekening aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td> <p>Voer de id in van de kalender waarover u details wilt ophalen of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a Calendar]

Met deze actiemodule maakt u een nieuwe kalender in uw Google-account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] rekening aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar name]</td> 
   <td> <p>Voer een naam in voor de nieuwe kalender.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a Calendar]

Deze actiemodule bewerkt een bestaande kalender.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] rekening aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td>Voer de [!UICONTROL Calendar ID] in voor de kalender die u wilt bijwerken. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New Calendar name]</td> 
   <td> <p>Voer een naam in voor de nieuwe kalender.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Calendar]

Met deze actiemodule verwijdert u een bestaande kalender.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] rekening aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar ID]</td> 
   <td>Voer de [!UICONTROL Calendar] -id in voor de kalender die u wilt verwijderen.</td> 
  </tr> 
 </tbody> 
</table>

### Overige

#### [!UICONTROL Make an API Call]

In deze module kunt u een aangepaste API-aanroep uitvoeren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] rekening aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override=""> een verbinding tot stand brengen [!DNL Adobe Workfront Fusion] - Basisinstructies </a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Voer een pad in dat relatief is ten opzichte van <code>https://graph.microsoft.com</code> . Voorbeeld:<code> /v1.0/me/events</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override=""> HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a> voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van de aanvraag toe in de vorm van een standaard JSON-object. Bijvoorbeeld <code>{"Content-type":"application/json"}</code> . [!DNL Workfront Fusion] voegt de machtigingsheaders voor u toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Voeg de query voor de API-aanroep toe als een standaard JSON-object.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:   <p>Wanneer u voorwaardelijke instructies gebruikt, zoals <code>if</code> in uw JSON, plaatst u de aanhalingstekens buiten de voorwaardelijke instructie.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
