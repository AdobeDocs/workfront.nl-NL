---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 'Voorbeeld van Adobe Workfront Fusion-scenario: E-mail, de Parser van de Tekst van Connect, en Google Bladen "'
description: Dit scenario helpt u een logboek van alle e-mailberichten tot stand brengen en hen etiketteren voor verdere actie in een spreadsheet. Hierbij wordt een e-mailhoofdtekst in twee afzonderlijke tabellen in een spreadsheet vastgelegd met Regular Expressions (Regex) als zoekpatronen. Het eerste patroon zoekt naar een uitdrukking en het tweede zoekt naar dezelfde uitdrukking en een e-mailadres.
author: Becky
feature: Workfront Fusion
exl-id: ebcfa3b9-3207-441c-9ce5-9af696c0119d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1095'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] voorbeeld scenario: E-mailadres verbinden [!UICONTROL Text Parser], en [!DNL Google Sheets]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Deze zelfstudie vereist basiskennis van reguliere expressies. Ga voor meer informatie over Regex naar [https://regexone.com](https://regexone.com/).

Voeg de eerste module toe en vorm het

1. Zoeken naar e-mail en kies **[!UICONTROL Watch emails]** als de trigger.

   >[!NOTE]
   >
   >Terwijl u verbinding kunt maken met een [!DNL Google] account met Ee-mailmodule kunt u ook een [!DNL Gmail] module.

1. Verbind één van beide [!DNL Google] account of een andere e-mailclient op basis van IMAP (zoals [!DNL Outlook]).
1. Selecteer een map waarvan u de inkomende e-mails wilt controleren, bijvoorbeeld [!UICONTROL Inbox].
1. Onder [!UICONTROL Criteria]kiest u **[!UICONTROL All email]** (of verklein het naar beneden om e-mails te lezen of ongelezen).

   U kunt opgehaalde e-mails ook markeren als gelezen of ongelezen.

1. Stel de [!UICONTROL Maximum number of results] tot en met 1.

   ![](assets/save-max-as-1-350x304.png)

   U kunt dit veranderen gebaseerd op het volume van berichten u ontvangt. Nochtans, wordt het geadviseerd om een lage waarde te plaatsen en het scenario vaker in werking te stellen.

1. Klikken **[!UICONTROL Show advanced settings]** onderaan.

   ![](assets/show-adv-settings-350x332.png)

1. E-mailberichten filteren op [!UICONTROL Sender address], [!UICONTROL Subject] en [!UICONTROL Phrase].

   Zo kunt u alleen relevante e-mails bekijken. In dit voorbeeld hebben we alleen een filter Onderwerp toegevoegd en de andere twee blanco gelaten.

   >[!NOTE]
   >
   >Wij zullen een router toevoegen om naar uitdrukkingen in e-mail te zoeken gebruikend [!UICONTROL Match Pattern] iterator en een reguliere expressie (Regex) als een zoekpatroon. Dit stelt ons ook in staat om een scenario van meerdere nutsbedrijven op te bouwen.

1. Als de configuratie is voltooid en u wordt gevraagd op te geven waar u moet beginnen met het bekijken van uw e-mails, klikt u op **[!DNL From now on]**.

   ![](assets/from-now-on-350x236.png)

1. Doorgaan naar [Zoeken naar [!UICONTROL Flow Control] en voeg een [!UICONTROL Router]](#search-for-flow-control-and-add-a-router)

## Zoeken naar [!UICONTROL Flow Control] en voeg een [!UICONTROL Router]

1. Voeg een router na om het even welke module toe om de gegevens te verdelen of te dupliceren alvorens het naar de volgende module te verzenden.

   Hier hebben we een [!UICONTROL Router] de hoofdtekst van de e-mail naar twee aparte tabellen in een [!DNL Google Sheet].

   ![](assets/search-for-flow-control-350x220.png)

## Gebruik de [!UICONTROL Text Parser] Module

1. Voeg een [!UICONTROL Match Pattern] transformator om naar een uitdrukking in een e-mail te zoeken.

   We zullen zoeken naar de uitdrukking &quot;[!UICONTROL text parser module]&quot; in alle inkomende e-mails om de tekst van de hoofdtekst en de naam van de afzender vast te leggen van de tekst die met die uitdrukking overeenkomt.

   1. Schrijf het patroon als een reguliere expressie:

      tekst\sparser\module

   1. (Optioneel) Gebruik een van de andere patroonopties.

      ![](assets/pattern-350x318.png)

      Meerdere regels is handig als de tekst meerdere regels bevat en u op elke regel naar het patroon moet zoeken. Voor deze zelfstudie moeten we naar het patroon in de hele tekst van de e-mailtekst zoeken. Daarom laten we deze ongecontroleerd.

   1. In de [!UICONTROL Text] veld, klik op het kenmerk **Tekstinhoud** in de lijst.

      ![](assets/text-content-350x264.png)

      Dit is het attribuut dat de tekst van het e-maillichaam opslaat waarin wij naar het patroon zullen zoeken.

1. Nog een toevoegen [!UICONTROL Match Pattern] die naar dezelfde uitdrukking en een e-mailadres zoekt.

   Dit is met name handig als u klantenaccounts hebt met meerdere gebruikers. Als u tijd wilt besparen, kunt u de opdracht [!UICONTROL Text Parser] module u enkel creeerde en het verbindt met de Router.

   ![](assets/clone.png)

1. Bewerk het patroon als volgt:

   text\sparser\smodule.+\s([\w.-]+@[\w.-]+)

   ![](assets/text-parser-350x202.png)

   Dit patroon zoekt naar de uitdrukking &quot;[!UICONTROL text parser module]&quot; en een e-mailadres zoals john.doe@gmail.com en retourneert alleen het e-mailadres.

   >[!NOTE]
   >
   >Het is belangrijk om uw regex in overeenstemming met de specificatie van de e-mailadressen te schrijven u goedkeurt, maar hierboven behandelt het meeste standaard e-mailadressen.

   * Als u alleen naar het e-mailadres wilt zoeken, kunt u de onderstaande tabel gebruiken:

      ([\w.-]+@[\w.-]+)

   * U kunt ook alleen naar telefoonnummers zoeken met onderstaande regex:

      ^[+]?\(?(\d{1,3})\)?[\s-]?\(?(\d{3})\?[\s-]?\d{3}[\s-]?\d{3,4} Het bovenstaande patroon behandelt de meeste algemene formaten waarin een telefoonaantal wordt geschreven.
   Om uw patronen te testen, adviseren wij het gebruiken [[!DNL https://regex101.com]](https://regex101.com/) with [!DNL javascript] als de smaak.

   De rest van de configuratie blijft hetzelfde als de vorige configuratie.

## Voeg de [!DNL Google Sheets] modules

Voor [!DNL Sheets]We moeten eerst een spreadsheet maken met de vereiste kopteksten.

1. Maak een spreadsheet met de kolommen waaronder u de gebruikersgegevens wilt vastleggen. (U kunt ook een bestaand bestand gebruiken.)

   Maak bijvoorbeeld een bestand met de naam &#39;E-mailgegevens: Support Ticket&quot; met de naam van de afzender, de e-mail van de afzender en e-mailinhoud als kolommen. Noem het aantekenvel &quot;bevat: text parser module.&quot;

1. Voeg de [!UICONTROL Google Sheets] module met **[!UICONTROL Add a row]** als de handeling.

   ![](assets/add-a-row-350x174.png)

1. Verbind uw [!DNL Google] account (als je dat nog niet hebt gedaan). Kies het bestand dat u eerder hebt gemaakt, gevolgd door het werkblad te kiezen waarin u de gegevens vastlegt.

   Uw opstelling zou als dit moeten kijken:

   ![](assets/connect-google-acct-350x279.png)

1. Wijs de attributen in de relevante gebieden (kolommen) toe om de moduleopstelling te beëindigen.

   ![](assets/map-attributes-350x282.png)

1. Kloont de module u enkel creeerde en koppel het aan de tweede [!UICONTROL Text Parser] module.

   1. Ga naar uw werkblad, dupliceer het werkblad dat u eerder hebt gemaakt en geef het een naam.

      Geef het bestand bijvoorbeeld de naam &quot;contains: text parser module and email.&quot;

   1. Voeg nog een kolom toe om het e-mailadres op te slaan dat de e-mailhoofdtekst bevat.

      Geef het bijvoorbeeld de naam &quot;E-mailadres gedeeld&quot;.

   1. Klik op de gekloonde knop [!DNL Google Sheets] om de opstelling te vormen.
   1. Wijzig het werkblad in het nieuwe werkblad dat u zojuist hebt gemaakt.
   1. De uitvoer toewijzen vanuit de [!UICONTROL Match Pattern] module ($1) aan de kolom waar u het e-mailadres (Gedeeld E-mailadres) wilt opslaan.

      ![](assets/map-the-output.png)

      ![](assets/sender-name-350x411.png)

   1. Klikken **[!UICONTROL OK]**, sparen het scenario, en neem het voor een testlooppas.

      U moet twee aparte e-mails naar het verbonden e-mailadres verzenden:

      * Bevat de zin &quot;[!UICONTROL text parser module]&quot; (en geen e-mailadres)

         ![](assets/text-parser-module-350x103.png)

      * Bevat bovenstaande zin en een e-mailadres

         ![](assets/above-phrase-and-email-350x106.png)

         Als er geen fouten in de installatie voorkomen, worden in het eerste werkblad alle e-mails met de uitdrukking &quot;[!UICONTROL text parser module]&quot; terwijl in het tweede werkblad alleen die worden vastgelegd die de uitdrukking &quot;[!UICONTROL text parser module]&quot; en een e-mailadres. U kunt de onderstaande schermafbeeldingen raadplegen.

         Werkblad 1:

         ![](assets/worksheet-1-350x57.png)

         Werkblad 2:

         ![](assets/worksheet-2-350x41.png)

## Bronnen

* [Vrije oefeningen](https://regexone.com/) voor meer informatie over reguliere expressies
* [Meer informatie over overeenkomsten met telefoonnummers](https://regexone.com/problem/matching_phone_numbers) Regex gebruiken
* [Meer informatie over e-mailovereenkomsten](https://regexone.com/problem/matching_emails) Regex gebruiken
* [Reguliere expressies testen](https://regex101.com/)
