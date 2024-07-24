---
product-area: documents;setup
navigation-topic: review-a-proof
title: De instellingen voor de proefdrukviewer configureren
description: U kunt instellingen configureren voor zowel de webtestviewer als de Desktop Proofing Viewer.
author: Courtney
feature: Digital Content and Documents
exl-id: 3993cd67-90a9-4d7e-bbc0-7b9bd1057f54
source-git-commit: 8af531868249f609113af6d2a8465af01edcbc3f
workflow-type: tm+mt
source-wordcount: '1417'
ht-degree: 0%

---

# De instellingen voor de proefdrukviewer configureren

U kunt de volgende instellingen configureren voor zowel de webtestviewer als de Desktop Proofing Viewer:

* Of opmerkingsmarkeringen en punten worden weergegeven op proefdrukken.
* Geeft aan of de markeringsgereedschappen boven in de proefdrukviewer worden weergegeven of in een vervolgkeuzemenu.
* Welke e-mailberichten u als recensent op de proef ontvangt u open hebt.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the Desktop Proofing Viewer is the default viewer for all types of proofs (static and video, as well as interactive).</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For comparative information about the Web Proofing Viewer and the Desktop Proofing Viewer, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p>
-->

U kunt de volgende instellingen configureren voor de Desktop Proofing Viewer:

* Hoe wilt u dat koppelingen binnen website-inhoud worden geopend in de viewer.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the background color of the Desktop Proofing Viewer is the default near-black color or white.</li>
  -->

* Wat gebeurt er als u op een koppeling klikt die is ingesteld op openen in een nieuw browsertabblad of venster.
* Wis de cachegegevens die met de proefdruk die u bekijkt kunnen worden opgeslagen, zodat inhoud zoals pop-ups (die door cachegegevens van de browser kunnen worden geblokkeerd) in de viewer kan worden weergegeven.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Huidig abonnement: Pro of hoger</p> <p>of</p> <p>Verouderd abonnement: Selecteren of Premium</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref"> Toegang tot het proefdrukken van functionaliteit in Workfront </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Huidig plan: Werk of Plan</p> <p>Ouder plan: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>Manager of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, rol, of Profiel van de Toestemming van het Bewijs u hebt, contacteer uw beheerder van Workfront of van Workfront Proof.

+++

## De instellingen voor de proefdrukviewer configureren

De instellingen voor de proefdrukviewer configureren:

1. Open de webtestviewer of de Desktop Proofing Viewer op een van de volgende manieren:

   * Als u bewijs binnen Adobe Workfront, naar een documentlijst gaat die een proef bevat u wilt bekijken, over het document beweegt, dan klik **Open proef**.
   * Als u Workfront Proof gebruikt, klik **ga naar het pictogram van het Bewijs** voor de proef in het Dashboard of een lijst van Mening ![](assets/go-to-proof-blue-icon.png).

1. Als de linkertoolbar niet toont, klik het **pictogram van het Menu**, dat in de upper-left hoek van de Kijker van het Bewijs van het Web wordt gevestigd.

   ![](assets/menu-icon-in-proofing-viewer-350x228.png)

1. In de linkertoolbar, klik het **pictogram van Montages** ![](assets/settings-icon-in-pv.png).

1. Vorm om het even welke volgende **Montages** die vertoning.

   Welke instellingen beschikbaar zijn, is afhankelijk van het type proefdruk dat u hebt geopend.

   * **toon markeringen** (altijd beschikbaar in de Kijker van het Keuren van het Web en de Kijker van het Bewijs van de Desktop): Dit zijn de commentaarmarkeringen die de recensenten aan proeven toevoegen wanneer zij de prijsverhogingshulpmiddelen gebruiken. Als u deze uitschakelt, kunt u ze nog steeds zien wanneer u op een opmerking in de lijst met opmerkingen klikt.

     Deze instelling is van invloed op alle proefdrukken die u opent.

   * **toon spelden** (altijd beschikbaar in de Kijker van het Keuren van het Web en de Kijker van het Bewijs van de Desktop): Dit zijn de genummerde spelden die de recensenten aan proeven toevoegen wanneer zij de prijsverhogingshulpmiddelen gebruiken. Ze geven aan waar en in welke volgorde de revisor opmerkingen heeft toegevoegd. Als u deze uitschakelt, kunt u ze nog steeds zien wanneer u op een opmerking in de lijst met opmerkingen klikt.

     Deze instelling is van invloed op alle proefdrukken die u opent.

   * **gebruik uitgebreide prijsverhogingshulpmiddelen** (altijd beschikbaar in de Kijker van het Keuren van het Web en de Kijker van het Proofing van de Desktop): Door gebrek, tonen de de optiesvertoning van het prijsverhogingshulpmiddel over de bovenkant van de het proef kijker. U kunt deze configureren voor weergave in een verticaal menu dat alleen wordt geopend wanneer u erop klikt.

     Deze instelling geldt voor alle proefdrukken die u opent.

   * **verzend me e-mailberichten over** (altijd beschikbaar in de Kijker van het Proofing van het Web en de Kijker van het Proofing van de Desktop): Klik één van de hieronder opties. Deze instelling is alleen van invloed op de proefdruk die u hebt geopend. Voor meer informatie, zie [ Meldingen voor de proefdrukcommentaren en besluiten overzicht ](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Alle activiteiten</td> 
        <td>Workfront stuurt een e-mail naar de controleur telkens wanneer er activiteiten op het bewijs zijn, zoals een nieuwe opmerking, een nieuw antwoord of een nieuw besluit. <p>Dit is een goede optie voor de persoon die het proefdrukproces beheert omdat het hen toestaat om de activiteit te zien aangezien het gebeurt. </p><p>Gebruikers ontvangen geen e-mailbericht over hun eigen activiteiten.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Reacties op mijn opmerkingen</td> 
        <td>Een e-mail wordt alleen naar de controleur verzonden als iemand uitdrukkelijk op zijn opmerking reageert (dit sluit zijn eigen reacties op zijn eigen opmerkingen uit). Dit betekent dat als iemand op het bewijs een nieuwe opmerking maakt, de controleur niet op de hoogte wordt gesteld.<p>Deze instelling wordt aanbevolen voor uw klanten op de proefdruk, zodat zij geen andere opmerkingen over de proefdruk ontvangen en alleen op de hoogte worden gesteld van antwoorden op hun eigen opmerkingen.</p><p>Hoewel revisoren met deze instelling voor e-mailwaarschuwingen geen melding krijgen van andere nieuwe opmerkingen, kunnen ze alle opmerkingen over de proefdrukken wel bekijken in de proefdrukviewer.</p><p>Voor informatie over commentaren, zie <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref"> Mening en antwoord aan proefdrukcommentaren </a>.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Besluiten</td> 
        <td>Workfront stuurt een e-mailbericht alleen naar de controleur wanneer iemand een beslissing neemt.<p>Dit kan nuttig zijn voor de persoon die het goedkeuringsproces beheert (zoals een projectmanager) en moet de vooruitgang op het bewijs controleren en zien welke gebruikers hun besluit hebben genomen.</p><p>Je wordt pas op de hoogte gesteld van je eigen beslissing als je een bevestigingsoptie voor e-mail selecteert wanneer je je beslissing verzendt.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Definitief besluit</td> 
        <td>Workfront stuurt een e-mail wanneer de laatste fiatteur van het bewijs zijn beslissing heeft genomen.<p>Deze waarschuwing wordt vaak gebruikt door de ontwerper, die gewoonlijk niet aan de daadwerkelijke overzichtsbespreking hoeft deel te nemen. Wanneer het definitieve besluit wordt genomen, wordt de ontwerper op de hoogte gebracht en kan dan actie ondernemen op om het even welke noodzakelijke veranderingen.</p><p>Deze waarschuwing kan ook nuttig zijn voor een afdelingsleider die slechts op de hoogte moet worden gebracht wanneer het overzichtsproces wordt gebeëindigd.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Uuroverzicht</td> 
        <td>Workfront stuurt elk uur een e-mail naar de controleur met een overzicht van alle opmerkingen, antwoorden en beslissingen die in het uur zijn genomen.<p>Het e-mailbericht wordt alleen verzonden wanneer er in het afgelopen uur andere activiteiten plaatsvinden dan die van uzelf. </p><p>Deze waarschuwing is een goede manier om een overzicht van het project te zien.</p><p>Een voorbeeld van een gebruiksgeval voor deze samenvatting is een senior controleur die een overzicht van het project nodig heeft, maar niet onmiddellijk op de hoogte hoeft te worden gesteld van alle activiteiten op de proefdruk.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Dagelijkse samenvatting</td> 
        <td>Workfront verzendt één e-mail met alle commentaren, antwoorden, en besluiten die slechts op dagen worden vermeld wanneer er naast uw activiteiten is.<p>Deze waarschuwing is een goede manier om een samenvatting van het project te zien zonder overweldigd met veelvoudige updates door de dag te worden.</p><p>Een voorbeeld gebruikt geval voor deze samenvatting is een afdelingsleider die de algemene vooruitgang van het project wil controleren.</p><p>Voor meer informatie, zie <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref"> berichten voor proefdrukcommentaren en besluiten </a> leiden.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Geen e-mail</td> 
        <td>Workfront verzendt geen e-mailberichten.<br> dit is nuttig voor een persoon die aan een proef slechts voor verwijzingsdoeleinden wordt toegevoegd en te hoeven niet van om het even welke veranderingen worden op de hoogte gebracht.<p>Het systeemgebrek is Dagelijkse samenvatting (ook gezien als niet Geplaatst). Als u of uw controleurs geen andere wijzigingen aanbrengen, hebben al uw proefdrukken deze instelling.</p></td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p><strong>Use desktop app as default</strong>: By default, static and video proofs open in the Web Proofing Viewer in your web browser, and interactive proofs open in the Desktop Proofing Viewer app. This setting lets you configure the Desktop Proofing Viewer as the default viewer for all types of proofs (static and video, as well as interactive). For more information about this setting, see in the article . For comparative information about the two viewers, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p> </li>   
     -->

   * **wanneer het klikken van hyperlinks in een proef** (beschikbaar slechts in de Kijker van het Bewijs van de Desktop): Selecteer een optie om te specificeren wat in de Kijker van het Bewijzen van de Desktop gebeurt wanneer u een verbinding klikt die in een nieuw browser lusje of een venster wordt geplaatst te openen.

     Deze instelling geldt voor alle interactieve proefdrukken die u opent.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Openen in de proefdrukviewer</td> 
        <td>De koppelingen worden altijd geopend in de Desktop Proofing Viewer en u kunt de gekoppelde inhoud controleren. </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Openen in de browser</td> 
        <td>Koppelingen worden altijd geopend in de browser, niet in een proefdrukviewer. U kunt de gekoppelde inhoud niet controleren.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Mij telkens vragen</td> 
        <td> <p>Telkens wanneer u de koppeling wilt openen in de Desktop Proofing Viewer of in de browser, wordt u hierom gevraagd. Als u de koppeling opent in de Desktop Proofing Viewer, kunt u de gekoppelde inhoud controleren. Als u de koppeling opent in de browser, kunt u de gekoppelde inhoud niet controleren.</p> <p> <img src="assets/proof-desktop-alwaysask-350x243.png" alt="proof_desktop_alwaysask.png" style="width: 350;height: 243;"> </p> <p>Deze instelling is alleen van invloed op de proefdruk die u hebt geopend.</p> </td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Background color</strong> (available when you open interactive content in the Desktop Proofing Viewer or Web Proofing Viewer): Change the background color of the Desktop Proofing Viewer from the default near-black color to white. This can make it easier to see interactive content that has a transparent background instead of a white background.</li>   
     -->

   * **Duidelijk geheime voorgeheugen**: ontruimt de browser geheim voorgeheugengegevens die met een interactieve proef zouden kunnen worden bewaard u bekijkt. Hierdoor kan inhoud zoals pop-ups (die door cachegegevens van de browser kunnen worden geblokkeerd) worden weergegeven in de Desktop Proofing Viewer.

     De gegevens die gewist worden, zijn onder andere de HTTP-cache (zoals afbeeldingen die opnieuw worden gebruikt nadat de volgende pagina is vernieuwd) en de cache met gegevens over de webopslag (zoals cookies en gegevens die gebruikers identificeren).

     Deze instelling is alleen van invloed op de proefdruk die u hebt geopend.
