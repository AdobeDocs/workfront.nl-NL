---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Een geautomatiseerde workflow maken of bewerken voor een bestaande proefdruk
description: Met geautomatiseerde workflows kunt u het revisieproces eenvoudiger beheren als uw proces complex is of als u regelmatig inhoud ter controle naar dezelfde groepen personen verzendt. Wanneer u een proef met een Geautomatiseerde Werkstroom creeert, beweegt de proef zich van stadium aan stadium tot definitieve goedkeuring. Deelnemers krijgen een melding wanneer het hun beurt is om het document te reviseren.
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: f252e3562b8ea73486d407138251b3d15d4b9f3a
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 0%

---

# Een geautomatiseerde workflow maken of bewerken voor een bestaande proefdruk

Met geautomatiseerde workflows kunt u het revisieproces eenvoudiger beheren als uw proces complex is of als u regelmatig inhoud ter controle naar dezelfde groepen personen verzendt. Wanneer u een proef met een Geautomatiseerde Werkstroom creeert, beweegt de proef zich van stadium aan stadium tot definitieve goedkeuring. Deelnemers krijgen een melding wanneer het hun beurt is om het document te reviseren.

Voor informatie over het creëren van een Geautomatiseerd Werkschema voor een nieuw bewijs, zie [ een geavanceerd bewijs met een Geautomatiseerd werkschema ](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md) creëren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Huidig abonnement: Pro of hoger</p> <p>of</p> <p>Verouderd plan: Premium</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref"> Toegang tot het proefdrukken van functionaliteit in Workfront </a>.</p> </td> 
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
   <td> <p>Toegang tot documenten bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, rol, of Profiel van de Toestemming van het Bewijs u hebt, contacteer uw beheerder van Workfront of van Workfront Proof.

+++

## Een geautomatiseerde workflow maken of bewerken voor een bestaande proefdruk:

1. Houd de muis boven het document in het gebied Documenten en klik vervolgens op Proofingworkflow.

   of

   Als u de proef in de het proeven kijker bekijkt, klik **Werkschema** ![](assets/workflow-icon-proofing-viewer.png) in het linkerpaneel, dan klik het Edit pictogram ![](assets/edit-icon-proofing-viewer.png) om de Geautomatiseerde montages van het Werkschema voor de proef te openen.

1. (Voorwaardelijk) als de proef momenteel een basiswerkschema (zonder stadia) gebruikt, klik **Bekeerling aan Geautomatiseerde Werkschema** in het scherm dat verschijnt.

   >[!NOTE]
   >
   >U kunt het eerste werkgebied niet bewerken wanneer u een standaardworkflow omzet in een geautomatiseerde workflow, maar u kunt wel nieuwe fasen toevoegen en configureren.

1. Voorwaardelijk) om een Geautomatiseerd malplaatje van het Werkschema te gebruiken dat uw beheerder van Adobe Workfront creeerde en met u deelde, **toevoegt malplaatje**, selecteert het malplaatje in de doos die verschijnt, dan klik **voegt malplaatje** toe.

   Voor meer informatie, zie [ Ongeveer gebruikend de Geautomatiseerde malplaatjes van het Werkschema ](#about-using-automated-workflow-templates) in dit artikel.

1. Een werkgebied toevoegen aan de automatische workflow:

   1. Klik **Nieuw stadium** dichtbij de hoger-juiste hoek.
   1. In de doos die verschijnt, typ a **Naam** voor het stadium.
   1. (Optioneel) Stel een deadline in voor het werkgebied.
   1. In **activeer stadium** sectie, kies hoe u het stadium wilt activeren:


      <table>
      <tbody>
      <tr>
      <td><strong>Bij proefmaken</strong></td>
      <td>Het werkgebied wordt automatisch geactiveerd omdat de proefdruk al is gemaakt.</td>
      </tr>
      <tr>
      <td><strong>Wanneer de deadline van de vorige fase verstrijkt</strong></td>
      <td>Klik het vorige stadium in de <strong> drop-down lijst van het stadium van de Ouder </strong>.</td>
      </tr>
      <tr>
      <td><strong>Op een specifieke datum en tijd</strong></td>
      <td>Klik <strong> op </strong> doos om de datum te selecteren, dan klik de doos aan het recht om de tijd te selecteren.</td>
      </tr>
      <tr>
      <td><strong>Alle beslissingen worden goedgekeurd of goedgekeurd met wijzigingen in het bovenliggende werkgebied</strong></td>
      <td>Klik het ouderstadium in de <strong> drop-down lijst van het stadium van de Ouder </strong>.</td>
      </tr>
      <tr>
      <td><strong>Alle besluiten worden goedgekeurd op ouderstadium</strong></td>
      <td>Klik het ouderstadium in de <strong> drop-down lijst van het stadium van de Ouder </strong>.</td>
      </tr>
      <tr>
      <td><strong>Alle besluiten worden genomen</strong></td>
      <td>Klik het ouderstadium in de <strong> drop-down lijst van het stadium van de Ouder </strong>.</td>
      </tr>
      </tbody>
      </table>


   1. Voer een naam of e-mailadres in en configureer instellingen voor controleurs voor het werkgebied.

      Voor informatie over het toevoegen van recensenten, zie [ Ongeveer toevoegend recensenten aan een stadium ](#about-adding-reviewers-to-a-stage) in dit artikel.

   1. Gebruik een van de volgende opties om het werkgebied verder te configureren:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong> Deadline opties </strong> </td>
         <td><p>Om een deadline voor het stadium te plaatsen, klik een optie in de <strong> drop-down lijst van de Opties van de Deadline </strong>. Dan, onder <strong> Deadline </strong>, doe één van het volgende:</p>
          <ul>
           <li>Als u <strong> verkoos Vastgestelde specifieke datum </strong>: Selecteer de deadline datum en de tijd u wilt.</li>
           <li>Als u <strong> kiest berekent van de datum van de werkgebiedactivering </strong>: Selecteer het aantal bedrijfsdagen u aan de datum van de werkgebiedactivering wilt toevoegen om de deadline te bepalen.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Werkgebied vergrendelen</td>
         <td>Geef op wanneer het werkgebied kan worden vergrendeld. </td>
        </tr>
        <tr>
         <td role="rowheader">Primaire beslisser</td>
         <td><p>Selecteer de primaire beslisser in het werkgebied (alleen beschikbaar nadat u ten minste één persoon aan het werkgebied hebt toegevoegd die de rol van fiatteur of hoger heeft). Als u een Primaire besluitvormer selecteert, wordt <strong> slechts één vereiste besluit </strong> optie onbruikbaar gemaakt op dit stadium.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Slechts één besluit vereist</td>
         <td>Beëindigt het hele herzieningsproces wanneer een van de besluitvormers een besluit neemt.<p>Deze optie is niet beschikbaar als u een gebruiker in het <strong> Primaire drop-down menu van de besluitvormer </strong> wees.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Privéstadium</td>
         <td>Hiermee kunnen alleen de volgende personen opmerkingen en beslissingen weergeven die tijdens dit werkgebied zijn gemaakt: toezichthouders, Adobe Workfront-beheerders en Workfront Proof-beheerders</td>
        </tr>
        <tr>
         <td role="rowheader">Personen per e-mail op de hoogte stellen</td>
         <td>Hiermee waarschuwt u revisoren met een e-mailmelding wanneer het hun beurt is om aan de proefdruk te werken.</td>
        </tr>
       </tbody>
      </table>

   1. Klik **voeg stadium** toe.

1. Herhaal desgewenst de vorige stap om meer stappen toe te voegen.

   Aangezien u stadia aan de Geautomatiseerde Werkschema toevoegt, vormt een diagram op het scherm om hen te vertegenwoordigen:

   ![](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. Wanneer u klaar bent toevoegend stadia, klik **Gedaan**.

## Informatie over het gebruik van automatische workflowsjablonen {#about-using-automated-workflow-templates}

Overweeg het volgende wanneer u een Geautomatiseerde malplaatje van het Werkschema gebruikt:

1. De instellingen van een automatische werkstroomsjabloon bepalen wat u kunt doen met de geautomatiseerde workflow voor een proefdruk. Als de knop Een werkgebied toevoegen bijvoorbeeld is uitgeschakeld in de sjabloon, is deze niet zichtbaar wanneer u werkt met de instellingen voor Geautomatiseerde workflow voor de proefdruk.
1. Wanneer een persoon wordt toegevoegd aan een werkgebied in een Geautomatiseerde malplaatje van het Werkschema, maar ook reeds als recensent op het bewijs aanwezig is, verwijdert het toepassen van het malplaatje de recensent uit het stadium. Als u geen andere revisor aan het werkgebied toevoegt, wordt u in een bericht gevraagd er een toe te voegen.
1. Uw vermogen om een Geautomatiseerde malplaatje van het Werkschema te wijzigen hangt van de malplaatjemontages af die door de beheerder van Workfront worden gevormd, zoals die in wordt beschreven. Als de mogelijkheid om de sjabloon te wijzigen is uitgeschakeld, kan alleen de eigenaar van de sjabloon deze wijzigen.

## Revisoren toevoegen aan een werkgebied {#about-adding-reviewers-to-a-stage}

Houd rekening met het volgende wanneer u revisoren aan een werkgebied toevoegt:

* Nadat u een gebruiker aan een stadium toevoegt, kunt u montages voor die gebruiker op de proef vormen, zoals de proefdrukrol en om het even welke extra toestemmingen zij zouden moeten hebben en het type e-mailalarm zij zullen ontvangen wanneer de mensen commentaren en besluiten over de proef maken.
* U kunt een of meer gebruikers van het ene werkgebied naar het andere slepen. U kunt gebruikers rechtstreeks aan een ander stadium slepen, of u kunt gebruikers aan een stadium op het **Stadium** diagram slepen. Druk op Shift+Ctrl (Windows) of Shift+Command (Mac) om meerdere gebruikers te selecteren.
* U kunt een controleur slechts eenmaal aan een proefdruk toevoegen, wat betekent dat u dezelfde persoon niet aan meer dan één werkgebied kunt toevoegen op de proefdruk.
* Revisoren die niet aan een privéfase zijn toegevoegd, kunnen dat stadium niet zien op de proefdruk of de opmerkingen die in dat stadium zijn gemaakt.
* Door gebrek, verleent het toevoegen van een gebruiker aan een stadium die gebruiker toegang om de proef van het ogenblik te bekijken de proef wordt gecreeerd.

  Uw Workfront-beheerder kan gebruikers de toegang tot de proefdruk beperken tot de werkstroom het werkgebied ingaat waar de gebruiker is toegevoegd. Zie voor meer informatie  in .
