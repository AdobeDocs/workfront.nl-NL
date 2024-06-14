---
product-area: requests
navigation-topic: create-requests
title: Adobe Workfront-aanvragen maken en verzenden
description: Geplande werkzaamheden worden in Adobe Workfront vertegenwoordigd door projecten en taken. Nochtans, zou u in een milieu kunnen werken waar ongeplande werk-in de vorm van willekeurig verzoek-binnen op elk ogenblik kan komen. Workfront biedt een workflow voor het aanpassen van dit type omgeving via het gebruik van Request Queues.
author: Alina
feature: Work Management
exl-id: 8b023a3d-326d-4d63-9e1e-8171553a9e23
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '2334'
ht-degree: 0%

---

# Adobe Workfront-aanvragen maken en verzenden

<!--Audited: 12/2023-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Linked to the UI - do not change/ remove; THIS IS NOW SPLIT IN THREE ARTICLES>> MAKE SURE THE TRANSITION TO THE OTHER TWO IS CLEAR SINCE THIS IS LINKED TO UI)</p>
<p>(NOTE: If they come out with templates AND drafts, consider splitting this article to keep Create in one and Working with Drafts and Requests in another??)</p>
<p>(NOTE: this article is linked from Submitting Workfront Requests from Salesforce) </p>
</div>
-->

Geplande werkzaamheden worden in Adobe Workfront vertegenwoordigd door projecten en taken. U kunt echter werken in een omgeving waar ongeplande werkzaamheden, in de vorm van verzoeken, op elk moment kunnen worden uitgevoerd. Workfront biedt een workflow voor het aanpassen van dit type omgeving via het gebruik van Request Queues.

Nadat u een verzoek in een Rij van het Verzoek creeert, kunt u of het toewijzen om worden voltooid of u kunt het in een taak of een project omzetten.\
Voor meer informatie over het omzetten van kwesties in een taak of een project, zie het artikel [Overzicht van conversie van problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

U kunt op de volgende manieren een aanvraag maken:

* Geheel opnieuw, zoals beschreven in dit artikel.
* Van concepten. Zie voor meer informatie [Verzoeken maken op basis van concepten](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).
* Van een bestaand verzoek, door een exemplaar te kopiëren en voor te leggen. Zie voor meer informatie [Verzoeken kopiëren en verzenden](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuw: Medewerker of hoger</p>
   of
   <p>Huidig: Verzoek of hoger</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot problemen bewerken</p>  </td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten voor het gebruik van aanvraagwachtrijen

Een Workfront-beheerder moet aanvraagwachtrijen maken en beschikbaar stellen aan gebruikers voordat deze functie kan worden gebruikt. Een gebruiker met een Planner-licentie en met de machtiging Bewerken tot projecten en Beheren voor een specifiek project kan ook aanvraagwachtrijen maken.

Voor informatie over hoe te om de Queuten van Verzoeken te creëren, zie het artikel [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Een Workfront-beheerder moet de volgende componenten van een aanvraagwachtrij maken:

* Een project in Huidige status, die als Rij van het Verzoek van de Hulp wordt gepubliceerd.
* De Onderwerpen van de rij.\
  Zie het artikel voor meer informatie [Werkvoorraadonderwerpen maken](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

* Verpletterend Regels.\
  Zie het artikel voor meer informatie [Verpletterende regels maken](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

* (Optioneel) Onderwerpgroepen.\
  Zie het artikel voor meer informatie [Onderwerpgroepen maken](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

* (Optioneel) Aangepast formulier aanvragen.\
  Zie het artikel voor meer informatie [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* (Optioneel) Verzoek om goedkeuring.\
  Zie het artikel voor meer informatie [Een goedkeuringsproces voor werkitems maken](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Verzoeken maken en concepten genereren in de Workfront-webapp

Wanneer u een verzoek maakt in de Workfront-webapp, slaat Workfront het verzoek op als een concept voordat u het verzendt. Workfront maakt een concept zodra je de wachtrij met aanvragen hebt geselecteerd en gegevens voor de wachtrij hebt ingevoerd.

U kunt doorgaan met het verzenden van de aanvraag, of u kunt alle beschikbare gegevens invullen en er vanaf navigeren om deze later te voltooien. Workfront slaat het geschreven verzoek dat u in de map Concepts hebt gestart op.

>[!IMPORTANT]
>
>Houd rekening met het volgende wanneer u werkt met concepten:
>
>* Workfront maakt geen conceptaanvragen wanneer u deze vanuit een externe toepassing verzendt, zoals ze naar Workfront verzendt of ze met een andere toepassing maakt. Wanneer u een aanvraag indient van buiten de Workfront-webtoepassing, wordt de aanvraag opgeslagen in de sectie Verzenden.
>* Als de structuur van een aanvraagwachtrij verandert, hebt u geen toegang meer tot bestaande concepten. Bijvoorbeeld, als een rijonderwerp wordt verwijderd, of een onderwerpgroep wordt toegevoegd, zijn de bewaarde concepten niet meer toegankelijk.
>

Voor informatie over het creëren van verzoeken van bestaande concepten, zie [Verzoeken maken op basis van concepten](../../../manage-work/requests/create-requests/create-requests-from-drafts.md). Voor informatie over het schrappen van verzoekconcepten, zie ook [Een aanvraagconcept verwijderen](../../../manage-work/requests/create-requests/delete-request-draft.md).

Een aanvraag maken in de Workfront-webapp:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   </MadCap:conditionalText>
   -->

1. Klikken  **Verzoeken** en klik vervolgens op **Nieuwe aanvraag** rechtsboven op de pagina.

   >[!TIP]
   >
   >* U kunt tot de Nieuwe optie van het Verzoek van om het even welke sectie op het gebied van Verzoeken toegang hebben.
   >* De optie Nieuw verzoek is grijs als u geen toegang hebt om problemen te maken.

1. (Voorwaardelijk) Klik binnen **Type aanvraag** en voer een van de volgende handelingen uit:

   * Van de **Recente paden** selecteert u een pad dat u onlangs hebt gebruikt om een aanvraagwachtrij te openen. Een weg omvat de verzoekrij, de onderwerpgroepen, en het rijonderwerp dat u onlangs indiende. De laatste drie paden worden standaard weergegeven.

     >[!NOTE]
     >
     >Workfront slaat alleen een pad op als je er een aanvraag voor hebt ingediend. Er worden geen paden voor opgestelde verzoeken gemaakt.

     ![](assets/list-of-recent-paths-and-request-queues-when-entering-new-request-nwe-350x295.png)

   * Van de **Wachtrijen aanvragen** , selecteert u een aanvraagwachtrij.
   * Voer een trefwoord in dat bij een eerder geopend pad hoort om naar een aanvraagwachtrij te zoeken.

     Bijvoorbeeld, als u een verzoekrij genoemd &quot;Helpdesk&quot;met een Groep van het Onderwerp genoemd &quot;Plaats&quot;en een Onderwerp van de Rij genoemd &quot;Verre&quot;hebt, kunt u &quot;ver&quot;en alle verzoekrijen typen die &quot;ver&quot;in om het even welk element van hun wegvertoning bevatten.

     >[!TIP]
     >
     >Wanneer u een naam typt die een speciaal karakter bevat, de verzoekrij, het rijonderwerp, of de vertoning van de onderwerpgroep zelfs wanneer u het typen van het karakter weglaat.

     ![](assets/request-queue-search-findings-with-highlighted-results-350x210.png)

     De lijst met beschikbare aanvraagrijen en recente paden wordt dynamisch bijgewerkt en bevat alleen paden die het trefwoord bevatten dat in de resultaten is gemarkeerd.

     De resultaten van de zoekopdracht worden weergegeven in de volgende gebieden:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Wachtrijen aanvragen</td> 
        <td>De rijen van het verzoek die het sleutelwoord in hun naam bevatten</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Paden aanvragen</td> 
        <td> <p>Paden (die aanvraagrijen, onderwerpgroepen, rijonderwerpen omvatten) die het sleutelwoord in om het even welke namen van hun elementen bevatten</p> </td> 
       </tr> 
      </tbody> 
     </table>

   >[!TIP]
   >
   >* De eerste 200 verzoekrijen tonen door gebrek, in alfabetische orde.
   >* De naam van de verzoekrij is de naam van het project dat als Rij van het Verzoek van de Hulp is gepubliceerd.
   >* De beschrijving van het project dat als de geselecteerde vertoningen van de verzoekrij aan het recht van de naam van de verzoekrij wordt gevormd.
   >   
   >Voor meer informatie over hoe te om een project als Rij van het Verzoek van de Hulp te publiceren, zie het artikel [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. In de **Nieuwe aanvraag** Voer een van de volgende handelingen uit in de vorm:

   * (Voorwaardelijk) selecteer een beschikbaar ontwerp van het berichtbericht dat onder het gebied van het Type van Verzoek wordt getoond.

     Dit gebied wordt alleen weergegeven als u concepten hebt opgeslagen voordat u ze verzendt.

     De drie meest recente concepten van drie verschillende rijonderwerpen worden standaard weergegeven.

     ![](assets/new-drafts-after-new-request-area-was-removed-350x162.png)

   * Voer een nieuwe aanvraag in de geselecteerde wachtrij in.

     Een nieuw concept wordt automatisch voor u opgeslagen in de sectie Concepten nadat u informatie voor het nieuwe verzoek hebt ingevoerd en u het verzoek een naam geeft in het veld Onderwerp.

1. (Optioneel) Als uw aanvraagwachtrij onderwerpgroepen bevat, selecteert u de naam van de onderwerpgroep in het eerste vervolgkeuzeveld. Anders, selecteer een Onderwerp van de Rij.

   >[!TIP]
   >
   >Wanneer u over een Onderwerpgroep of een Onderwerp van de Rij beweegt, toont het gebied van de Beschrijving aan het recht. Dit bevat extra informatie over de onderwerpgroep of het rijonderwerp.
   >
   >
   >![](assets/show-description-on-queue-topic-when-submitting-request-nwe-350x81.png)   >
   >

   U kunt tot 10 rijen van Onderwerpgroepen hebben die in uw Rij van het Verzoek worden gebouwd.\
   Raadpleeg het artikel voor meer informatie over het maken van onderwerpgroepen [Onderwerpgroepen maken](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Voor meer informatie over het creëren van de Onderwerpen van de Rij, zie het artikel [Werkvoorraadonderwerpen maken](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   >[!TIP]
   >
   >Als u een concept of een vorig pad hebt geselecteerd, zijn de onderwerpgroepen en de rijonderwerpen al geselecteerd. U kunt desgewenst een andere selectie maken.

1. Afhankelijk van welke velden de Workfront-beheerder in het dialoogvenster **Nieuwe probleemvelden** van de **Wachtrij** Subtab op het project, zou u om het even welke volgende gebieden kunnen vinden wanneer u een nieuw verzoek indient:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Onderwerp</strong> </td> 
      <td>Geef een naam op voor uw aanvraag. Dit is een verplicht veld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beschrijving</strong> </td> 
      <td>Geef een beschrijving op voor uw aanvraag.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Geef een URL op die betrekking kan hebben op uw verzoek.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioriteit</strong> </td> 
      <td> <p>Geef een prioriteit voor uw verzoek op. De prioriteit moet bepalen hoe snel u vindt dat dit verzoek moet worden opgelost. De standaardopties zijn: </p> 
       <ul> 
        <li>Geen</li> 
        <li>Laag </li> 
        <li>Normaal</li> 
        <li>Hoog</li> 
        <li>Dringend</li> 
       </ul> <p>Uw systeembeheerder kan de namen van prioriteiten wijzigen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ernst</strong> </td> 
      <td> <p>Geef de ernst van uw verzoek op. De ernst moet bepalen welke invloed dit verzoek op uw werk heeft als het niet op tijd wordt opgelost. De standaardopties zijn:</p> 
       <ul> 
        <li>Cosmetisch</li> 
        <li>Verwardheid</li> 
        <li>Fout met tijdelijke oplossing</li> 
        <li>Fout zonder tijdelijke oplossing</li> 
        <li>Fatale fout</li> 
       </ul> <p>De systeembeheerder kan de namen van de bestandscontroles wijzigen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Primaire contactpersoon</strong> </td> 
      <td>De primaire contactpersoon van een verzoek blijft standaard bij u, aangezien u de puntpersoon bent die vragen met betrekking tot het verzoek behandelt. U kunt dit echter wijzigen in elke andere Workfront-gebruiker.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>Toewijzingen</strong> </td> 
      <td> <p><span>Geef de naam op van een actieve gebruiker, taakrol of team waaraan de aanvraag moet worden toegewezen.</span> </p> <p>U kunt slechts één team opgeven.</p>

   <p> Afhankelijk van hoe de verzoekrij opstelling was, zou u één of twee soorten middel aan het verzoek kunnen slechts toewijzen, in plaats van alle drie (bijvoorbeeld, zou u het verzoek aan gebruikers kunnen slechts kunnen toewijzen).</p>

   <p>Als een verpletterende regel ook aan de verzoekrij wordt geassocieerd en het het verzoek aan een verschillend type van middel (bijvoorbeeld, een team) automatisch leidt, wordt uw verzoek toegewezen aan zowel de entiteit die u manueel wanneer het voorleggen van het verzoek (gebruikers) en het middel specificeert in de verpletterende regel (het team). </p>

   <p> Raadpleeg de volgende artikelen voor meer informatie:</p> 
      <ul> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Een aanvraagwachtrij maken</a> </p> </li> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Verpletterende regels maken</a> <br> </p> </li> 
      </ul> </p>

   <p><span>Wij adviseren gebruikend het Verpletteren van Regels voor uw Opeenvolging van het Verzoek zodat zij automatisch aan de aangewezen middelen kunnen worden verpletterd.</span> </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Geplande uren</strong> </td> 
      <td> <p>Schatting hoeveel uren het voor dit verzoek om voltooien zou vergen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Geplande begindatum</strong> </td> 
      <td> <p>Geef de datum op waarop de werkzaamheden aan dit verzoek moeten beginnen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Geplande afsluitdatum</strong> </td> 
      <td>Geef de datum op waarop u dit verzoek wilt laten oplossen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong> </td> 
      <td>De standaardstatus van een nieuw verzoek is "Nieuw." Mogelijk is de naam van deze status gewijzigd door uw systeembeheerder. U kunt de status ook wijzigen in iets anders vanuit dit keuzemenu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documenten</strong> </td> 
      <td> <p>Voeg documenten toe aan uw verzoek. </p> <p> Afhankelijk van hoe de verzoekrij opstelling was, zou de sectie van Documenten vóór of na de douanevelden kunnen tonen. </p> <p>Documenten die u uploadt naar Workfront worden 24 uur lang opgeslagen in een geschreven aanvraag. Daarna, moet u hen opnieuw aanhalen wanneer u terugkeert om het ontwerp uit te geven en voor te leggen. Documenten die via andere stations zijn gekoppeld, worden permanent in het concept opgeslagen. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Als uw Workfront-beheerder een aangepast formulier heeft gekoppeld aan de aanvraagwachtrij of het onderwerp van de wachtrij, geeft u de velden in het aangepaste formulier op.\
   Aangepaste formulieren verschillen voor elk Workfront-exemplaar.
1. (Optioneel en voorwaardelijk) Klik op een willekeurig punt tijdens het invoeren van de aanvraag op [!UICONTROL **Concept verwijderen**] als u het concept wilt verwijderen dat automatisch wordt gemaakt. Hiermee verwijdert u het concept dat niet kan worden hersteld. Er wordt een bevestigingsbericht weergegeven om te bevestigen dat u het concept verwijdert.

1. (Optioneel) Klik op [!UICONTROL **Ongedaan maken**] in het bevestigingsbericht als u uw actie wilt terugkeren en het concept wilt behouden.

1. Voer een van de volgende handelingen uit:

   * Klikken **Verzenden** als u klaar bent om het verzoek in te dienen. De aanvraag wordt opgeslagen in de sectie Verzenden. Afhankelijk van de Verpletterende Regel van de Rij van het Verzoek, zou dit verzoek aan een verschillend project dan kunnen worden verpletterd die als Rij van het Verzoek wordt aangewezen. Voor informatie over het verpletteren van regels, zie [Verpletterende regels maken](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

     of

     Klikken **Sluiten** als u niet helemaal klaar bent om het in te dienen en u zou kunnen terugkomen en het later beëindigen. Uw verzoek wordt opgeslagen in de sectie Concepten. De volgende keer dat u een aanvraag voor deze aanvraagwachtrij verzendt, is deze beschikbaar.

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

   Wanneer u het verzoek indient, wordt het concept automatisch verwijderd en kan het niet worden hersteld.

   Voor informatie over het richten van inkomende verzoeken, zie het artikel [Werk- en teamverzoeken beheren](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

   Zie voor meer informatie over het zoeken naar ingediende of opgestelde verzoeken ook [Verzonden aanvragen zoeken](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

## Verzoeken maken van buiten Workfront

U kunt een directe koppeling naar een aanvraagwachtrij delen wanneer u een nieuwe aanvraag indient en deze insluiten in andere toepassingen. Gebruikers die via internet of andere toepassingen toegang krijgen tot deze koppeling, moeten zich ook aanmelden met een actieve Workfront-account om toegang te krijgen tot deze wachtrij en aanvragen naar deze wachtrij te kunnen verzenden. Zie voor meer informatie [Een koppeling delen naar een aanvraagwachtrij](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Verzoeken maken via e-mail naar Workfront

Als uw aanvraagwachtrij is ingeschakeld voor het ontvangen van aanvragen via e-mail, kunt u uw aanvragen rechtstreeks verzenden naar het e-mailadres dat is gekoppeld aan de wachtrij met aanvragen.

De hoofdtekst van de e-mail wordt toegevoegd als de aanvraagbeschrijving.

>[!NOTE]
>
>HTML-opmaak wordt verwijderd wanneer de aanvraag Workfront binnengaat, maar handtekeningen en bestaande inhoud van Reply-to-thread worden niet verwijderd en weergegeven in de aanvraagbeschrijving.

Voor informatie over hoe te om een Rij van het Verzoek toe te laten om verzoeken door e-mail te ontvangen, zie [Gebruikers toestaan een uitgave per e-mail te verzenden naar een aanvraagwachtrij-project](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Verzoeken maken met de Outlook-client

U kunt verzoeken indienen gebruikend de cliënt van Vooruitzichten. U kunt een nieuwe aanvraag maken of een e-mailbericht converteren naar een aanvraag.

Voor informatie over het voorleggen van verzoeken gebruikend de cliënt van Vooruitzichten, zie het artikel [Een Adobe Workfront-aanvraag maken vanuit een Outlook-e-mail](../../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).

## Verzoeken maken met de mobiele Workfront-app

U kunt aanvragen verzenden via de mobiele app op uw smartphone. U kunt een nieuwe aanvraag maken en deze verzenden naar de aanvraagwachtrij die u in de webtoepassing kunt bekijken.

Raadpleeg de sectie Verzoeken in de artikelen voor informatie over het verzenden van aanvragen via de mobiele app:

* [Adobe Workfront voor Android](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md#requests)
* [Adobe Workfront voor iOS](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md#requests)

## Verzoeken maken vanuit andere toepassingen

U kunt aanvragen verzenden met alle toepassingen die zijn geïntegreerd met Workfront:

* U kunt een aangepaste integratie maken tussen Workfront en een andere toepassing waarmee u aanvragen naar Workfront kunt verzenden vanuit de andere toepassing.\
  Raadpleeg het artikel voor meer informatie over aangepaste Workfront-integratie [Adobe Workfront-integratie](../../../administration-and-setup/configure-integrations/workfront-integrations-1.md).

* U kunt aanvragen van Salesforce indienen als u de Workfront-app voor Salesforce hebt geïnstalleerd.\
  Raadpleeg het artikel voor informatie over het verzenden van aanvragen van Salesforce met onze Workfront-app voor Salesforce. [Adobe Workfront-aanvragen verzenden vanuit Salesforce-objecten](../../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

## Verzonden aanvragen zoeken

Voor meer informatie over het zoeken naar ingediende of opgestelde verzoeken raadpleegt u [Verzonden aanvragen zoeken](../../../manage-work/requests/create-requests/locate-submitted-requests.md).
