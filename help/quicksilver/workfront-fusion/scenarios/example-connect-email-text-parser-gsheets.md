---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 'Voorbeeld van Adobe Workfront Fusion-scenario: Connect-e-mail, Text Parser en Google Sheets'
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen.
author: Becky
feature: Workfront Fusion
exl-id: ebcfa3b9-3207-441c-9ce5-9af696c0119d
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1099'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] scenario-voorbeeld: Connect email, [!UICONTROL Text Parser] en [!DNL Google Sheets]

>[!IMPORTANT]
>
>Dit artikel wordt in de nabije toekomst verwijderd.

Dit scenario helpt u een logboek van alle e-mailberichten tot stand brengen en hen etiketteren voor verdere actie in een spreadsheet. Hierbij wordt een e-mailhoofdtekst in twee afzonderlijke tabellen in een spreadsheet vastgelegd met Regular Expressions (Regex) als zoekpatronen. Het eerste patroon zoekt naar een uitdrukking en het tweede zoekt naar dezelfde uitdrukking en een e-mailadres.

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] of hoger</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licentie**</td> 
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

Deze zelfstudie vereist basiskennis van reguliere expressies. Om over Regex te leren, bezoek [ https://regexone.com ](https://regexone.com/).

Voeg de eerste module toe en vorm het

1. Zoek naar E-mail en kies **[!UICONTROL Watch emails]** als Trekker.

   >[!NOTE]
   >
   >Terwijl u een [!DNL Google] rekening kunt verbinden gebruikend de E  e-mailmodule, kunt u een [!DNL Gmail] module ook gebruiken.

1. Sluit een [!DNL Google] -account of een andere op IMAP gebaseerde e-mailclient (zoals [!DNL Outlook] ) aan.
1. Selecteer een map waarvan u de inkomende e-mailberichten wilt controleren die u vervolgens hebt verbonden, zoals [!UICONTROL Inbox] .
1. Kies onder [!UICONTROL Criteria] de optie **[!UICONTROL All email]** (of verklein deze naar beneden om e-mails te lezen of te lezen).

   U kunt opgehaalde e-mails ook markeren als gelezen of ongelezen.

1. Stel de [!UICONTROL Maximum number of results] in op 1.

   ![](assets/save-max-as-1-350x304.png)

   U kunt dit veranderen gebaseerd op het volume van berichten u ontvangt. Nochtans, wordt het geadviseerd om een lage waarde te plaatsen en het scenario vaker in werking te stellen.

1. Klik op **[!UICONTROL Show advanced settings]** onderaan.

   ![](assets/show-adv-settings-350x332.png)

1. E-mailberichten filteren op [!UICONTROL Sender address] , [!UICONTROL Subject] en [!UICONTROL Phrase] .

   Zo kunt u alleen relevante e-mails bekijken. In dit voorbeeld hebben we alleen een filter Onderwerp toegevoegd en de andere twee blanco gelaten.

   >[!NOTE]
   >
   >Wij zullen een router toevoegen om naar uitdrukkingen in een e-mail te zoeken gebruikend [!UICONTROL Match Pattern] iterator en een Regular Uitdrukking (Regex) als onderzoekspatroon. Dit stelt ons ook in staat om een scenario van meerdere nutsbedrijven op te bouwen.

1. Wanneer de configuratie is voltooid en u wordt gevraagd op te geven waar u moet beginnen met het bekijken van uw e-mails, klikt u op **[!DNL From now on]** .

   ![](assets/from-now-on-350x236.png)

1. Ga door met [ Zoeken naar [!UICONTROL Flow Control] en voeg een [!UICONTROL Router]](#search-for-flow-control-and-add-a-router) toe

## Zoeken naar [!UICONTROL Flow Control] en een [!UICONTROL Router] toevoegen

1. Voeg een router na om het even welke module toe om de gegevens te verdelen of te dupliceren alvorens het naar de volgende module te verzenden.

   Hier hebben we een [!UICONTROL Router] gebruikt om de hoofdtekst van de e-mail te verzenden naar twee aparte tabellen in een [!DNL Google Sheet] .

   ![](assets/search-for-flow-control-350x220.png)

## De module [!UICONTROL Text Parser] gebruiken

1. Voeg een transformator [!UICONTROL Match Pattern] toe om naar een uitdrukking in een e-mail te zoeken.

   Wij zullen naar de uitdrukking &quot;[!UICONTROL text parser module]&quot;in alle inkomende e-mails zoeken om de lichaamstekst en de naam van de afzender van degenen te vangen die die uitdrukking aanpassen.

   1. Schrijf het patroon als een reguliere expressie:

      tekst\sparser\module

   1. (Optioneel) Gebruik een van de andere patroonopties.

      ![](assets/pattern-350x318.png)

      Meerdere regels is handig als de tekst meerdere regels bevat en u op elke regel naar het patroon moet zoeken. Voor deze zelfstudie moeten we naar het patroon in de hele tekst van de e-mailtekst zoeken. Daarom laten we deze ongecontroleerd.

   1. Op het [!UICONTROL Text] gebied, klik de inhoud van de attributen **Tekst** in de lijst.

      ![](assets/text-content-350x264.png)

      Dit is het attribuut dat de tekst van het e-maillichaam opslaat waarin wij naar het patroon zullen zoeken.

1. Voeg nog een [!UICONTROL Match Pattern] toe die naar dezelfde uitdrukking en een e-mailadres zoekt.

   Dit is met name handig als u klantenaccounts hebt met meerdere gebruikers. Om tijd te besparen, kunt u de [!UICONTROL Text Parser] module klonen u enkel creeerde en het verbinden met de Router.

   ![](assets/clone.png)

1. Bewerk het patroon als volgt:

   text\sparser\smodule.+ \ s ([ \ w.- ] +@ [ \ w.- ]+)

   ![](assets/text-parser-350x202.png)

   Dit patroon zoekt naar de uitdrukking &quot;[!UICONTROL text parser module]&quot;en een e-mailadres zoals john.doe@gmail.com en keert slechts het e-mailadres terug.

   >[!NOTE]
   >
   >Het is belangrijk om uw regex in overeenstemming met de specificatie van de e-mailadressen te schrijven u goedkeurt, maar hierboven behandelt het meeste standaard e-mailadressen.

   * Als u alleen naar het e-mailadres wilt zoeken, kunt u de onderstaande tabel gebruiken:

     ([ \ w.-] +@ [ \ w.- ]+)

   * U kunt ook alleen naar telefoonnummers zoeken met onderstaande regex:

     ^[+]?\ (? (\ d{1, 3}) \)?[\s-]?\(?(\d{3})\?[ \ s-]? \ d \ {3 \} [ \ s- ]? \ d , 4}
Het bovenstaande patroon heeft betrekking op de meest gebruikte indelingen waarin een telefoonnummer is geschreven.

   Als u uw patronen wilt testen, raden we u aan [[!DNL https://regex101.com] ](https://regex101.com/) with [!DNL javascript] als de smaak te gebruiken.

   De rest van de configuratie blijft hetzelfde als de vorige configuratie.

## Voeg de modules [!DNL Google Sheets] toe

Voor [!DNL Sheets], moeten wij eerst een spreadsheet met de vereiste kopballen tot stand brengen.

1. Maak een spreadsheet met de kolommen waaronder u de gebruikersgegevens wilt vastleggen. (U kunt ook een bestaand bestand gebruiken.)

   Maak bijvoorbeeld een bestand met de naam &quot;E-mailgegevens: ondersteuningsticket&quot; met de kolommen Naam afzender, E-mail afzender en E-mailinhoud als kolommen. Geef het werkblad de naam &quot;contains: text parser module&quot;.

1. Voeg de module [!UICONTROL Google Sheets] toe met **[!UICONTROL Add a row]** als de handeling.

   ![](assets/add-a-row-350x174.png)

1. Sluit uw [!DNL Google] -account aan (als u dat nog niet hebt gedaan). Kies het bestand dat u eerder hebt gemaakt, gevolgd door het werkblad te kiezen waarin u de gegevens vastlegt.

   Uw opstelling zou als dit moeten kijken:

   ![](assets/connect-google-acct-350x279.png)

1. Wijs de attributen in de relevante gebieden (kolommen) toe om de moduleopstelling te beëindigen.

   ![](assets/map-attributes-350x282.png)

1. Kloont de module u enkel creeerde en koppel het aan de tweede [!UICONTROL Text Parser] module.

   1. Ga naar uw werkblad, dupliceer het werkblad dat u eerder hebt gemaakt en geef het een naam.

      Geef het bestand bijvoorbeeld de naam &quot;contains: text parser module and email&quot;.

   1. Voeg nog een kolom toe om het e-mailadres op te slaan dat de e-mailhoofdtekst bevat.

      Geef het bijvoorbeeld de naam &quot;E-mailadres gedeeld&quot;.

   1. Klik op de gekloonde module [!DNL Google Sheets] om de installatie te configureren.
   1. Wijzig het werkblad in het nieuwe werkblad dat u zojuist hebt gemaakt.
   1. Wijs de uitvoer van de module [!UICONTROL Match Pattern] ($1) toe aan de kolom waar u het e-mailadres (Gedeeld E-mailadres) wilt opslaan.

      ![](assets/map-the-output.png)

      ![](assets/sender-name-350x411.png)

   1. Klik op **[!UICONTROL OK]**, sla het scenario op en neem het voor een testrun.

      U moet twee aparte e-mails naar het verbonden e-mailadres verzenden:

      * Bevat de uitdrukking &quot;[!UICONTROL text parser module]&quot; (en geen e-mailadres)

        ![](assets/text-parser-module-350x103.png)

      * Bevat bovenstaande zin en een e-mailadres

        ![](assets/above-phrase-and-email-350x106.png)

        Als er geen fouten in uw opstelling zijn, zult u zien dat het eerste aantekenvel alle e-mail vangt die de uitdrukking &quot; [!UICONTROL text parser module]&quot;bevatten terwijl het tweede aantekenvel slechts die vangt die de uitdrukking &quot; [!UICONTROL text parser module]&quot;en een e-mailadres bevatten. U kunt de onderstaande schermafbeeldingen raadplegen.

        Werkblad 1:

        ![](assets/worksheet-1-350x57.png)

        Werkblad 2:

        ![](assets/worksheet-2-350x41.png)

## Bronnen

* [ Vrije oefeningen ](https://regexone.com/) om over Reguliere Uitdrukkingen te leren
* [ leer over Aantal dat van de Telefoon ](https://regexone.com/problem/matching_phone_numbers) het Aanpassen gebruikt Regex
* [ Leer over E-mail het Verstemmen ](https://regexone.com/problem/matching_emails) gebruikend Regex
* [ Test uw Reguliere Uitdrukkingen ](https://regex101.com/)
