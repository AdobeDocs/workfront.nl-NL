---
title: Aanvragen voor Adobe Workfront-planning verzenden
description: Nadat iemand een verbinding met een verzoekformulier met u van een verslagtype pagina in de Planning van Adobe Workfront deelt, kunt u een verzoek toevoegen om verslagen voor het verslagtype tot stand te brengen verbonden aan het verzoekformulier.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '2026'
ht-degree: 0%

---

# Adobe Workfront-planningsverzoeken verzenden om records te maken

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [&#x200B; snelle versies voor uw organisatie &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

Nadat een werkruimtebeheerder een aanvraagformulier voor een recordtype heeft gemaakt in Adobe Workfront Planning, kunt u het formulier gebruiken om aanvragen in te dienen die records maken voor het recordtype dat aan het formulier is gekoppeld.

U kunt een aanvraag voor Workfront-planning vanuit de volgende gebieden indienen:

* Vanuit het gebied Verzoeken van Workfront of vanuit de widget Mijn verzoeken in Home.
* Vanuit een directe koppeling naar het gedeelde aanvraagformulier.
* Wanneer u een nieuwe record toevoegt door een aanvraag in te dienen, gaat u vanaf de pagina met recordtypen. Voor informatie, zie [&#x200B; verslagen &#x200B;](/help/quicksilver/planning/records/create-records.md) creëren.

In dit artikel wordt beschreven hoe u een verzoek kunt indienen om nieuwe records toe te voegen aan een recordtype vanuit het gebied Verzoeken van Workfront of via een gedeelde koppeling.

Workspace-managers kunnen aanvraagformulieren maken die u als gebruiker of externe persoon kunt gebruiken om aanvragen in te dienen bij de planning van recordtypen. Met de aanvragen worden records gemaakt voor het recordtype dat aan het aanvraagformulier is gekoppeld.

Voor informatie over hoe een werkruimtemanager een verzoekvorm kan tot stand brengen en het met een verslagtype associeert, zie [&#x200B; een verzoekvorm in de Planning van Adobe Workfront &#x200B;](/help/quicksilver/planning/requests/create-request-form.md) creëren en beheren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakketten</p></td> 
   <td> 
<p>Alle Workfront-pakketten en alle planningspakketten</p>
of
<p>Willekeurig workflowpakket en elk planningspakket</p>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Alle</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Machtigingen weergeven of hoger voor een werkruimte en recordtype als u een Workfront-gebruiker bent</p>  </td> 
  </tr>  
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

U moet het volgende opgeven voordat u een aanvraag kunt indienen bij een Workfront-aanvraagformulier voor planning:

* In Workfront Planning moet het volgende bestaan:

   * Een werkruimte
   * Een recordtype
   * Een aanvraagformulier dat is gekoppeld aan een recordtype.

     Voor informatie, zie [&#x200B; een verzoekvorm in de Planning van Adobe Workfront &#x200B;](/help/quicksilver/planning/requests/create-request-form.md) creëren.

* Het aanvraagformulier moet zo worden gedeeld dat u er toegang toe hebt. De volgende scenario&#39;s bestaan:

   * Intern moet het formulier worden gedeeld met gebruikers die beschikken over de machtiging Weergeven of hoger voor de werkruimte.

     Workfront-gebruikers hebben toegang tot het formulier via een koppeling of zoeken het aanvraagformulier in het gedeelte Verzoeken van Workfront.

   * Extern, door een koppeling naar het recordformulier te delen met externe personen die geen Workfront-account hebben.

     Workfront-gebruikers hebben ook toegang tot de koppeling die met externe personen wordt gedeeld.

* Als de koppeling wordt gedeeld met een koppeling, mag de koppeling naar het formulier niet verlopen.

## Overwegingen bij het indienen van aanvragen bij de planning van Workfront

* U kunt een aanvraag niet bewerken in Workfront nadat u deze hebt verzonden.
* Elk ingediend verzoek maakt een record voor het recordtype dat is gekoppeld aan het formulier dat u gebruikt, als het formulier niet aan een goedkeuring is gekoppeld of als de goedkeuring door alle fiatteurs is verleend.
* Records die zijn gemaakt door aanvraagformulieren in te dienen, zijn identiek aan records die via een andere methode in Workfront Planning zijn toegevoegd.

  Voor informatie, zie [&#x200B; verslagen &#x200B;](/help/quicksilver/planning/records/create-records.md) creëren.
* Records die zijn gemaakt door het verzenden van aanvraagformulieren, worden verbonden met de oorspronkelijke aanvraag. Deze verbinding kan niet worden verwijderd.
* U kunt zowel de gemaakte records als de aanvragen die zijn gebruikt om deze te maken, weergeven op de volgende gebieden:
   * Verzoeken in Workfront.

  <div class="preview">

   * In een verbonden gebied van een verslagtype pagina in de Planning van Workfront wanneer u het verzoek als verbonden verslag toevoegt.
   * In een verbonden gebied van de Details van een verslag in de Planning van Workfront wanneer u het verzoek als verbonden verslag toevoegt.

  </div>

  >[!TIP]
  >
  ><span class="preview"> U kunt de naam van het verzoek op het Onderwerp gebied in het gebied van Verzoeken van Workfront of het Originele gebied van de verzoekverbinding in de Planning van Workfront bekijken. </span>

* De ingediende planningsverzoeken zijn zichtbaar slechts in de nieuwe het vragen ervaring. U kunt de verzoeken van de Planning niet in de ervaring van het erfenisverzoek zien.

  Voor informatie, zie [&#x200B; verzoeken &#x200B;](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md) creëren en voorleggen.
* Er zijn beperkingen in de manier waarop bepaalde veldtypen worden weergegeven in een aanvraagformulier, of de pagina met aanvraagdetails nadat een formulier is verzonden.

  Voor informatie, zie [&#x200B; creeer en beheer een verzoekvorm in de Planning van Adobe Workfront &#x200B;](/help/quicksilver/planning/requests/create-request-form.md).

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Een verzoek indienen bij Workfront Planning in het gedeelte Aanvragen van Workfront

{{step1-to-requests}}

1. Zet de **nieuwe ervaring van het Gebruik** het plaatsen, in de hoger-juiste hoek van het scherm aan.
Het aanzetten van dit het plaatsen maakt de het verzoekvormen van de Planning van Workfront beschikbaar in het **gebied van Verzoeken** van Workfront.

   >[!TIP]
   >
   >Deze instelling is alleen beschikbaar wanneer uw Workfront-instantie is aangemeld bij de Adobe Unified Experience.
   >
   >Als u Workfront-planningsaanvragen op dit gebied wilt indienen, moet u aan de volgende voorwaarden voldoen:
   >
   >* Uw bedrijf heeft een Workfront Planning-licentie aangeschaft.
   >
   >* U hebt toegang tot minstens één werkruimte.

1. Klik in **wat verzoek wilt u voorleggen?** om een lijst met aanvraagformulieren te openen.
1. Selecteer een aanvraagformulier in de lijst of typ de naam van het aanvraagformulier en selecteer het vervolgens in de lijst.

   Bovenaan wordt een venster geopend met bovenaan de naam van het aanvraagformulier.

   >[!TIP]
   >
   >Workfront-aanvraagwachtrijen bevatten de naam van de wachtrij en de naam van het formulier in de lijst met aanvragen. Met planningsaanvragen worden alleen de formuliernaam weergegeven in de lijst met aanvragen.

1. Werk het **Onderwerp** gebied bij. Dit is de naam van de aanvraag. Dit is een verplicht veld.
1. Werk het **gebied van de Naam** bij. Dit is de naam van de toekomstige record.

   >[!TIP]
   >
   >Het **gebied van de Naam** is uniek aan uw organisatie en het zou een verschillend etiket in uw instantie van Workfront kunnen tonen. Het veld is het primaire veld van de record.

1. Werk de overige velden in het aanvraagformulier bij. Velden met een rood sterretje zijn vereist.
1. (Voorwaardelijk) als uw organisatie **Vulling van de Vorm** toestaat die door AI wordt aangedreven, kunt u documenten als herinneringen uploaden. AI gebruikt deze documenten om het formulier in te vullen en u kunt de AI-suggesties accepteren of negeren voordat u de aanvraag verzendt.


   Voor instructies, zie [&#x200B; Vulling van de Vorm van het Gebruik aangedreven door AI om een verzoek in te vullen gebruikend herinneringen of documenten &#x200B;](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).
1. Klik **voorleggen**.

   De verzoekvorm sluit en u keert aan het **gebied van Verzoeken** terug.

   Uw formulier wordt verzonden en de volgende dingen gebeuren:

   * Als het aanvraagformulier niet aan een goedkeuring is gekoppeld, wordt het verzoek toegevoegd aan de lijst Verzoeken in het gebied Workfront Requests en de widget Mijn verzoeken in Home, en wordt een nieuwe record toegevoegd aan het recordtype dat aan het formulier is gekoppeld.

     In de volgende velden worden de aanvraag- en recordgegevens weergegeven in het gebied Verzoeken en in de widget Mijn verzoeken in Home:

      * **Onderwerp**: De naam van het originele verzoek zoals toegevoegd in het gebied van Verzoeken. U kunt niet het **Onderwerp** gebied van het Onderwerp van de verzoeklijst verbergen of verwijderen.
      * **Gemaakt voorwerp**: De naam van het verslag dat van het verzoek werd gecreeerd aangezien het in Planning toont.
      * **type van Objecten**: De naam van de werkruimte en verslagtype waar er verslagen van het verzoek in Planning werden gecreeerd.
      * **Status**: De status van het verzoekvoorwerp.
      * **vorm van het Verzoek**: De naam van de verzoekvorm verbonden aan het verslagtype in Planning.
     <!--* <span class="preview"**Created object status**: The status of the created record.</span> -->

   * Als de verzoekvorm met een goedkeuring werd geassocieerd, wordt het verzoek toegevoegd aan de lijst van Verzoeken in het gebied van Verzoeken van Workfront en Mijn widget van Verzoeken met een status van **In afwachting van overzicht**. Een nieuwe record wordt pas aan de recordtypepagina toegevoegd nadat de fiatteurs de record hebben goedgekeurd.

     Voor informatie, zie [&#x200B; een goedkeuring aan een verzoekvorm &#x200B;](/help/quicksilver/planning/requests/add-approval-to-request-form.md) toevoegen.

   * <span class="preview"> u kunt het **Originele verzoek** verbindingsgebied aan een verslagtype in Planning toevoegen om de naam van het originele verzoek te tonen dat tot een verslag leidde. Voor informatie, zie [&#x200B; Connect verslagtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md). </span>
   * Het verzoek is alleen zichtbaar voor de eigenaar, fiatteur en de personen die minstens weergavemachtigingen hebben voor de werkruimte. Workfront-beheerders kunnen alle aanvragen weergeven die naar elke werkruimte in het systeem worden verzonden.
   * U ontvangt een melding in de app en een e-mail dat de aanvraag met succes is verzonden of ter controle is verzonden.
   * Als het aanvraagformulier aan een goedkeuring is gekoppeld, ontvangen de fiatteurs een in-app en een e-mailmelding om de aanvraag te beoordelen en goed te keuren.

     >[!NOTE]
     >
     >Het e-mailbericht en de meldingen in de app zijn alleen zichtbaar wanneer het exemplaar van Workfront van uw organisatie is aangemeld bij de Adobe Unified Experience.
     >
     >Er is een koppeling naar het verzoek in het bevestigingsbericht of goedkeuringsbericht van de e-mail.

1. (Facultatief) klik **Mening uw verzoek** in het bevestigingsbericht, om het verzoek te openen, of het **X** pictogram te klikken om de bevestiging te sluiten.
1. (Optioneel) Als u de manier wilt beheren waarop de informatie in de lijst met aanvragen wordt weergegeven, werkt u de volgende weergaveelementen voor de lijst bij:

   * Weergave
   * Filter
   * Kolommen

   <!--
   <div class="preview">
      * Group
   * Format cells
   * Row height
      </div>
   -->

   Voor informatie, zie [&#x200B; meningen in het gebied van Verzoeken &#x200B;](/help/quicksilver/manage-work/requests/create-requests/create-views-for-requests-list.md) creëren en leiden.

   <!--   
   1. (Optional) From the requests list, do any of the following:
      * Click **Filters** and start adding conditions for what requests you want to view in the Requests list. 
         ![Editing filters in the Requests area](assets/filters-editing-box-in-requests-planning-tab.png)
         You can filter by the following fields:  
         * **Workspace**: The workspace the request form is associated with.
         * **Object type**: The record type the request form is associated with.
         * **Entry date**: The date when the request was submitted.
         * **Request form**: The name of the request form used to submit the request.
         * **Status**: The status of the request.
         * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.
        You can have multiple filters joined by either **And** or **Or**.
         The request list is filtered automatically, as you add the filter conditions. 
      * Click **Columns** to open the **Fields visibility and order** box, then hide, show, or rearrange the columns in the request list. 
         >[!TIP]
         >
         >You cannot add any more columns. 
         ![Columns editing box in Requests area](assets/columns-editing-box-in-requests-planning-tab.png)
      * Click the **+** icon in the upper-right corner of the request list to open the **Column manager** and add or remove columns in the requests list. 
   -->

1. Klik op de naam van een aanvraag in de lijst.

   De pagina met aanvraagdetails wordt geopend.

   ![&#x200B; pagina van het Verzoek met commentaar &#x200B;](assets/new-request-page-with-comment.png)

1. (Facultatief) ga een commentaar op het **gebied van Commentaren** in.
1. (Voorwaardelijk) als de verzoekvorm niet met een goedkeuring wordt geassocieerd, of als het verzoek is goedgekeurd, klik de naam van het verzoek, dan klik de naam van het verslag op het **Gemaakt objecten** gebied.

   De pagina van het verslag opent in de Planning van Workfront.

   >[!TIP]
   >
   >* Als het primaire gebied van het verslag niet in de verzoekvorm werd bijgewerkt, de naam van het verslag op het gebied van het Verslag van de verzoekvertoningen als **Naamloos**.
   >
   >* Als het aanvraagformulier is gekoppeld aan een goedkeuring, moet de goedkeuring worden verleend voordat u toegang krijgt tot de record op de aanvraagpagina. De record wordt pas gemaakt wanneer de goedkeuring is verleend.

1. (Facultatief) klik de naam van het **type van Verslag**.

   De pagina met recordtypen wordt geopend in Workfront Planning.

## Een aanvraag vanuit een gedeelde koppeling naar een aanvraagformulier indienen bij Workfront Planning

De informatie in deze sectie is slechts van toepassing voor mensen die een verzoek van een gedeelde verbinding indienen en die geen rekening van Workfront zouden kunnen hebben.

De externe mensen hebben geen toegang tot interne gebieden van Workfront, zoals **Verzoeken** of **Huis**.

1. Ga naar de verbinding die met u van een het verslagtype van de Planning van Workfront wordt gedeeld.

1. Werk de velden bij die beschikbaar zijn in het formulier. Velden met een sterretje zijn vereist.

   >[!TIP]
   >
   >   Als het **Onderwerp** gebied beschikbaar is, zal het niet in de Planning van Workfront zichtbaar zijn, nadat het verzoek wordt voorgelegd.
   >
   >Wij adviseren dat u zoveel mogelijk gebieden in uw verzoek bijwerkt om het nieuwe verslag identificeerbaar te maken wanneer het aan het verslagtype in de Planning van Workfront wordt toegevoegd.

1. Klik **voorleggen**.

   Uw formulier wordt verzonden en u ontvangt een bevestiging.

   Als het formulier is gekoppeld aan een goedkeuring, moet het worden goedgekeurd voordat een record wordt gemaakt.

1. (Facultatief) klik **voorleggen een ander verzoek** om een ander verzoek aan de zelfde gedeelde verbinding toe te voegen.

<!--
   * If the request form was not associated with an approval, the request is added to the Requests list in the Workfront Requests area and My Requests widget in Home, and a new record is added to the record type associated with the form. This is available only when you log in to Workfront.
   
   * If the request form was associated with an approval, the request is added to the Requests list in the Workfront Requests area and My Requests widget. A new record is added to the record type page only after all the approvers have approved it. This is available only when you log in to Workfront.
   
      For information, see [Add an approval to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

      >[!IMPORTANT]
      >
      >You can view only the requests submitted by you or anyone else to the workspaces that you have at least permissions to View. Workfront administrators can view all requests submitted to any workspace in the system. <!--ensure this is correct; asking team in slack
   
   
   * You receive an in-app and an email notification that the request has either been submitted successfully or has been sent for review.
   * If the request form was associated with an approval, the approvers receive an in-app and an email notification to review and approve the request.
      >[!NOTE]
      >
      >The email and in-app notification are visible only when your organization's instance of Workfront is onboarded to the Adobe Unified Experience.
   
   <span class="preview"> After the request was approved and the record was created, the Approved by and Approved date fields display information about the approval on the record.</span>


1. (Optional) Click **View your request** to open the request in Workfront.


Or

Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.

   The request details page opens. 

   ![Request page with comment](assets/new-request-page-with-comment.png)

1. (Optional) Enter a comment in the **Comments** area.
1. (Conditional) If the request form is not associated with an approval, or if the request has been approved, click the name of the request, then click the name of the record in the **Created object** field. 

   The record's page opens in Workfront Planning. 

   >[!TIP]
   >
   >* If the record name was not added to the request form, the name of the record in the Record field of the request displays as **Untitled**. 
   >
   >* If the request form is associated with an approval, the approval must be granted before you can access the record from the request page. 

1. (Optional) Click the name of the **Object type**. 

   The record type page opens in Workfront Planning. 

-->

## Een verzoek maken door een bestaande aanvraag te kopiëren

U kunt een aanvraag kopiëren in de lijst met aanvragen in Workfront, de gegevens vervolgens bewerken en verzenden als een nieuwe aanvraag.

Dit is alleen beschikbaar in de nieuwe ervaring die u opvraagt.

Het kopiëren van een bestaand planningsverzoek en het indienen ervan als een nieuw verzoek is vergelijkbaar met het kopiëren van een bestaand Workfront-verzoek.

Voor meer informatie, zie [&#x200B; Exemplaar en leg verzoeken &#x200B;](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md) voor.

## Concepten en verzoeken maken op basis van bestaande concepten

U kunt een concept van een verzoek maken, vervolgens terugkeren naar het concept en het later als verzoek verzenden.

Dit is alleen beschikbaar in de nieuwe ervaring die u opvraagt. Concepten en verzoeken maken op basis van bestaande concepten in Workfront Planning is hetzelfde als deze maken op basis van Adobe Workfront.

Voor meer informatie, zie [&#x200B; verzoeken van concepten &#x200B;](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md) creëren.

## Concepten of ingediende verzoeken verwijderen

U kunt ingediende aanvragen of concepten verwijderen wanneer u de nieuwe ervaring met aanvragen gebruikt.

Wanneer u een planningsverzoek schrapt, komen de volgende dingen voor:

* Het verzoek kan niet worden teruggevorderd.
* De record die op basis van de aanvraag is gemaakt, wordt niet verwijderd.
* Verwijderde concepten kunnen niet worden hersteld. Er zijn geen records gekoppeld aan concepten.

Het verwijderen van planningsverzoeken komt overeen met het verwijderen van Workfront-verzoeken.

Voor informatie, zie [&#x200B; een voorgelegd verzoek of verzoekontwerp &#x200B;](/help/quicksilver/manage-work/requests/create-requests/delete-request-draft.md) schrappen.







