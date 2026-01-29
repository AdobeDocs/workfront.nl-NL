---
title: Aanvragen voor Adobe Workfront-planning verzenden
description: Nadat iemand een verbinding met een verzoekformulier met u van een verslagtype pagina in de Planning van Adobe Workfront deelt, kunt u een verzoek toevoegen om verslagen voor het verslagtype tot stand te brengen verbonden aan het verzoekformulier.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: f5d6918889b7fed1159274105ee706a027f621bf
workflow-type: tm+mt
source-wordcount: '2176'
ht-degree: 0%

---

# Adobe Workfront-planningsverzoeken verzenden om records te maken

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

Nadat een werkruimtebeheerder een aanvraagformulier voor een recordtype heeft gemaakt in Adobe Workfront Planning, kunt u het formulier gebruiken om aanvragen in te dienen die records maken voor het recordtype dat aan het formulier is gekoppeld.

U kunt een aanvraag voor Workfront-planning vanuit de volgende gebieden indienen:

* Vanuit het gebied Aanvragen van Workfront.
* Vanuit een directe koppeling naar het gedeelde aanvraagformulier.
* Wanneer u een nieuwe record toevoegt of aanvraagt, gaat u vanaf de pagina met recordtypen. Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/create-records.md) creëren.

In dit artikel wordt beschreven hoe u een verzoek kunt indienen om nieuwe records toe te voegen aan een recordtype vanuit het gebied Verzoeken van Workfront of via een gedeelde koppeling.

Workfront-gebruikers en externe gebruikers kunnen aanvragen indienen voor planningsrecordtypen. Met de aanvragen worden records gemaakt voor het recordtype dat aan het aanvraagformulier is gekoppeld. <!--double check on the external users-->

Voor informatie over hoe een werkruimtemanager een verzoekvorm kan tot stand brengen en het met een verslagtype associeert, zie [ een verzoekvorm in de Planning van Adobe Workfront ](/help/quicksilver/planning/requests/create-request-form.md) creëren en beheren.

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

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

U moet het volgende opgeven voordat u een aanvraag kunt indienen bij een Workfront-aanvraagformulier voor planning:

* In Workfront Planning moet het volgende bestaan:

   * Een werkruimte
   * Een recordtype
   * Een aanvraagformulier dat is gekoppeld aan een recordtype.

     Voor informatie, zie [ een verzoekvorm in de Planning van Adobe Workfront ](/help/quicksilver/planning/requests/create-request-form.md) creëren.

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

  Voor informatie, zie [ verslagen ](/help/quicksilver/planning/records/create-records.md) creëren.
* Records die zijn gemaakt door het verzenden van aanvraagformulieren, worden verbonden met de oorspronkelijke aanvraag. Deze verbinding kan niet worden verwijderd.
* U kunt zowel de gemaakte records als het verzoek op de volgende gebieden weergeven:
   * Verzoeken in Workfront

  <div class="preview">

   * Records in een recordtypepagina in het veld Oorspronkelijke aanvraagverbinding
   * De de voorproefdoos van Details van het verslag in het Originele gebied van de verzoekverbinding

  </div>
* Verzonden verzoeken worden weergegeven in het gebied Verzoeken van Workfront.
* De ingediende planningsverzoeken zijn zichtbaar slechts in de nieuwe het vragen ervaring. U kunt de verzoeken van de Planning niet in de ervaring van het erfenisverzoek zien.
Voor informatie, zie [ verzoeken ](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md) creëren en voorleggen.
* Er zijn beperkingen in de manier waarop bepaalde veldtypen worden weergegeven in een aanvraagformulier, of de pagina met aanvraagdetails nadat een formulier is verzonden.

  Voor informatie, zie [ creeer en beheer een verzoekvorm in de Planning van Adobe Workfront ](/help/quicksilver/planning/requests/create-request-form.md).

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Een verzoek indienen bij Workfront Planning in het gedeelte Aanvragen van Workfront

{{step1-to-requests}}

1. Laat de **Schakelaar aan een nieuwe ervaring** toe plaatsend, in de hoger-juiste hoek van het scherm.
Het toelaten van dit plaatsen maakt de het verzoekvormen van de Planning van Workfront beschikbaar in het **gebied van Verzoeken** van Workfront.

   >[!TIP]
   >
   >Deze instelling is alleen beschikbaar wanneer uw Workfront-instantie is aangemeld bij de Adobe Unified Experience.
   >
   >Als u Workfront-planningsaanvragen op dit gebied wilt indienen, moet u aan de volgende voorwaarden voldoen:
   >
   >* Uw bedrijf heeft een Workfront Planning-licentie aangeschaft.
   >
   >* U hebt toegang tot minstens één werkruimte.

1. Klik in **wat verzoek u** bar wilt voorleggen om een lijst van verzoekvormen te openen.
1. Selecteer een aanvraagformulier in de lijst of typ de naam van het aanvraagformulier en selecteer het vervolgens in de lijst.

   Bovenaan wordt een venster geopend met bovenaan de naam van het aanvraagformulier.
1. Werk de velden bij die beschikbaar zijn in het aanvraagformulier. Velden met een rood sterretje zijn vereist.
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

   * Als het aanvraagformulier aan een goedkeuring is gekoppeld, wordt het verzoek toegevoegd aan de lijst Verzoeken in het gebied Workfront Requests en de widget Mijn verzoeken met de status In behandeling. Een nieuwe record wordt pas aan de recordtypepagina toegevoegd nadat de fiatteurs de record hebben goedgekeurd.

     Voor informatie, zie [ een goedkeuring aan een verzoekvorm ](/help/quicksilver/planning/requests/add-approval-to-request-form.md) toevoegen.

   * <span class="preview"> u kunt het Originele gebied van de verzoekverbinding aan een verslagtype in Planning toevoegen die de naam van het originele verzoek toont. Voor informatie, zie [ Connect verslagtypes ](/help/quicksilver/planning/architecture/connect-record-types.md). </span>
   * Het verzoek is alleen zichtbaar voor de eigenaar, fiatteur en de personen die minstens weergavemachtigingen hebben voor de werkruimte. Workfront-beheerders kunnen alle aanvragen weergeven die naar elke werkruimte in het systeem worden verzonden.

   * U ontvangt een melding in de app en een e-mail dat de aanvraag met succes is verzonden of ter controle is verzonden.
   * Als het aanvraagformulier aan een goedkeuring is gekoppeld, ontvangen de fiatteurs een in-app en een e-mailmelding om de aanvraag te beoordelen en goed te keuren.

     >[!NOTE]
     >
     >De e-mail en in-app meldingen zijn alleen zichtbaar wanneer het exemplaar van Workfront van uw organisatie is aangemeld bij de Adobe Unified Experience.
     >
     >Er is een koppeling naar het verzoek in het bevestigingsbericht of goedkeuringsbericht van de e-mail.

1. (Facultatief) klik **Mening uw verzoek** in het bevestigingsbericht, om het verzoek te openen, of het **X** pictogram te klikken om de bevestiging te sluiten.
1. (Optioneel) Voer in de lijst met verzoeken een van de volgende handelingen uit:

   * Klik **Filters** en begin toevoegend voorwaarden voor welke verzoeken u in de lijst van Verzoeken wilt bekijken.

     ![ het Uitgeven filters op het gebied van Verzoeken ](assets/filters-editing-box-in-requests-planning-tab.png)

     U kunt filteren op de volgende velden:

      * **Workspace**: De werkruimte de verzoekvorm wordt geassocieerd met.
      * **Type van Verslag**: Het verslagtype het verzoekvorm wordt geassocieerd met.
      * **Datum van de Ingang**: De datum toen het verzoek werd voorgelegd.
      * **vorm van het Verzoek**: De naam van de verzoekvorm die wordt gebruikt om het verzoek voor te leggen.
      * **Status**: De status van het verzoek.
      * **ingegaan door**: De naam van de gebruiker die het verzoek toevoegde. Als het verzoek door iemand buiten Workfront werd toegevoegd, **ingegaan door** gebied toont `N/A`.
      * **Gecreeerde objecten status**: De status van het gecreeerde verslag.

     U kunt veelvoudige filters hebben die door of **worden aangesloten en** of **of**.
De aanvraaglijst wordt automatisch gefilterd, aangezien u de filtervoorwaarden toevoegt.

   * Klik **Kolommen** om het **zicht en de orde van Gebieden** vakje te openen, dan de kolommen in de verzoeklijst te verbergen, te tonen of te herschikken.

     >[!TIP]
     >
     >U kunt geen kolommen meer toevoegen.

     ![ Kolommen die doos op het gebied van Verzoeken uitgeven ](assets/columns-editing-box-in-requests-planning-tab.png)
   * Klik het **+** pictogram in de hoger-juiste hoek van de verzoeklijst om de **manager van de Kolom** te openen en kolommen in de verzoeklijst toe te voegen of te verwijderen.

1. Klik op de naam van een aanvraag in de lijst.

   De pagina met aanvraagdetails wordt geopend.

   ![ pagina van het Verzoek met commentaar ](assets/new-request-page-with-comment.png)

1. (Facultatief) ga een commentaar op het **gebied van Commentaren** in.
1. (Voorwaardelijk) als de verzoekvorm niet met een goedkeuring wordt geassocieerd, of als het verzoek is goedgekeurd, klik de naam van het verzoek, dan klik de naam van het verslag op het **Gemaakt objecten** gebied.

   De pagina van het verslag opent in de Planning van Workfront.

   >[!TIP]
   >
   >* Als het primaire gebied van het verslag niet in de verzoekvorm werd bijgewerkt, de naam van het verslag op het gebied van het Verslag van de verzoekvertoningen als **Naamloos**.
   >
   >* Als het aanvraagformulier is gekoppeld aan een goedkeuring, moet de goedkeuring worden verleend voordat u toegang krijgt tot de record op de aanvraagpagina.

1. (Facultatief) klik de naam van het **type van Verslag**.

   De pagina met recordtypen wordt geopend in Workfront Planning.

## Een aanvraag vanuit een gedeelde koppeling naar een aanvraagformulier indienen bij Workfront Planning

De informatie in deze sectie is alleen van toepassing op Workfront-gebruikers die een aanvraag via een gedeelde koppeling indienen. Externe personen hebben geen toegang tot interne Workfront-gebieden, zoals Verzoeken of Home.

1. Ga naar de verbinding die met u van een het verslagtype van de Planning van Workfront wordt gedeeld.

1. Werk de velden bij die beschikbaar zijn in het formulier. Velden met een sterretje zijn vereist.

   >[!TIP]
   >
   >   Als het **Onderwerp** gebied beschikbaar is, zal het niet in de Planning van Workfront zichtbaar zijn, nadat het verzoek wordt voorgelegd.
   >
   >Wij adviseren dat u zoveel mogelijk gebieden in uw verzoek bijwerkt om het nieuwe verslag identificeerbaar te maken wanneer het aan het verslagtype in de Planning van Workfront wordt toegevoegd.

1. Klik **voorleggen**.

   Uw formulier wordt verzonden en de volgende dingen gebeuren:

   * Als het aanvraagformulier niet aan een goedkeuring is gekoppeld, wordt het verzoek toegevoegd aan de lijst Verzoeken in het gebied Workfront Requests en de widget Mijn verzoeken in Home, en wordt een nieuwe record toegevoegd aan het recordtype dat aan het formulier is gekoppeld.

   * Als het aanvraagformulier aan een goedkeuring is gekoppeld, wordt het verzoek toegevoegd aan de lijst Verzoeken in de widget Workfront-verzoeken en Mijn verzoeken. Een nieuwe record wordt pas aan de recordtypepagina toegevoegd nadat alle fiatteurs de record hebben goedgekeurd.

     Voor informatie, zie [ een goedkeuring aan een verzoekvorm ](/help/quicksilver/planning/requests/add-approval-to-request-form.md) toevoegen.

     >[!IMPORTANT]
     >
     >U kunt alleen de aanvragen weergeven die door u of iemand anders zijn ingediend bij de werkruimten die u minstens gemachtigd zijn weer te geven. Workfront-beheerders kunnen alle aanvragen weergeven die naar elke werkruimte in het systeem worden verzonden. <!--ensure this is correct; asking team in slack-->

   * U ontvangt een melding in de app en een e-mail dat de aanvraag met succes is verzonden of ter controle is verzonden.
   * Als het aanvraagformulier aan een goedkeuring is gekoppeld, ontvangen de fiatteurs een in-app en een e-mailmelding om de aanvraag te beoordelen en goed te keuren.

     >[!NOTE]
     >
     >De e-mail en in-app meldingen zijn alleen zichtbaar wanneer het exemplaar van Workfront van uw organisatie is aangemeld bij de Adobe Unified Experience.

   <!-- <span class="preview"> After the request was approved and the record was created, the Approved by and Approved date fields display information about the approval on the record.</span>-->

1. (Facultatief) klik **Mening uw verzoek** om het verzoek in Workfront te openen.

   <!--Or-->

   <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. (Facultatief) klik **Belangrijkste menu** > **Verzoeken** om uw verzoek te bekijken, dan de naam van het verzoek te klikken.

   De pagina met aanvraagdetails wordt geopend.

   ![ pagina van het Verzoek met commentaar ](assets/new-request-page-with-comment.png)

1. (Optioneel) Voer een opmerking in het gebied Opmerkingen in.
1. (Voorwaardelijk) als de verzoekvorm niet met een goedkeuring wordt geassocieerd, of als het verzoek is goedgekeurd, klik de naam van het verzoek, dan klik de naam van het verslag op het **Gemaakt objecten** gebied.

   De pagina van het verslag opent in de Planning van Workfront.

   >[!TIP]
   >
   >* Als het verslag naam niet aan de verzoekvorm werd toegevoegd, de naam van het verslag op het gebied van het Verslag van de verzoekvertoningen als **Naamloos**.
   >
   >* Als het aanvraagformulier is gekoppeld aan een goedkeuring, moet de goedkeuring worden verleend voordat u toegang krijgt tot de record op de aanvraagpagina.

1. (Facultatief) klik de naam van het **type van Objecten**.

   De pagina met recordtypen wordt geopend in Workfront Planning.

## Een verzoek maken door een bestaande aanvraag te kopiëren

U kunt een aanvraag kopiëren in de lijst met aanvragen in Workfront, de gegevens vervolgens bewerken en verzenden als een nieuwe aanvraag.

Dit is alleen beschikbaar in de nieuwe ervaring die u opvraagt.

Voor instructies, zie [ Exemplaar en verzend verzoeken ](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Concepten en verzoeken maken op basis van bestaande concepten

U kunt een concept van een verzoek maken, vervolgens terugkeren naar het concept en het later als verzoek verzenden.

Dit is alleen beschikbaar in de nieuwe ervaring die u opvraagt.

Voor instructies, zie [ verzoeken van concepten ](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md) creëren.



