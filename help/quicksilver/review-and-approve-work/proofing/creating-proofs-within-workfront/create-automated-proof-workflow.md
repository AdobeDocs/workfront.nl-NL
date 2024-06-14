---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Een geavanceerde proefdruk maken met een geautomatiseerde workflow
description: Met een geautomatiseerde workflow kunt u het controleproces eenvoudiger beheren als uw proces complex is of als u inhoud ter controle regelmatig naar dezelfde personen verzendt. De proefdruk gaat van stadium aan stadium en Adobe Workfront brengt elke gebruiker op de hoogte wanneer het hun beurt is om het te herzien. Zie Geautomatiseerd workflowoverzicht voor meer informatie over geautomatiseerde workflows.
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 0%

---

# Een geavanceerde proefdruk maken met een geautomatiseerde workflow

<!-- Audited: 2/2024 -->

Met een geautomatiseerde workflow kunt u het controleproces eenvoudiger beheren als uw proces complex is of als u inhoud ter controle regelmatig naar dezelfde personen verzendt. De proefdruk gaat van stadium aan stadium en Adobe Workfront brengt elke gebruiker op de hoogte wanneer het hun beurt is om het te herzien. Zie voor meer informatie over geautomatiseerde workflows [Geautomatiseerd workflowoverzicht](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Nieuw: alle</p><p>Huidig abonnement: Pro of hoger</p><p>Verouderd abonnement: Selecteren of hoger</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Toegang tot proefdrukfunctionaliteit in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Nieuw: Standaard</p><p>Huidig plan: Werk of Plan</p> <p>Ouder plan: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>Manager of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot documenten bewerken</p></td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een geavanceerde proefdruk maken met een geautomatiseerde workflow

1. Ga naar het project, de taak, of de kwestie waar u het proef wilt, dan klik **Documenten** tab.
1. Klikken **Nieuw toevoegen** > Proef, upload de inhoud en doorloop de onderstaande secties.

   of

   Houd de cursor boven een bestaand document en klik vervolgens op de knop **Proef maken** > **Geavanceerd proefdrukken** en doorwerkt u de onderstaande secties.

## De proefdrukfasen configureren

1. Kies in de sectie Type workflow de optie **Automatisch**.
1. (Optioneel) Als u een automatische workflowsjabloon wilt gebruiken die uw Workfront-beheerder heeft gemaakt en met u heeft gedeeld, klikt u op **Sjabloon toevoegen** selecteert u de sjabloon in het vak dat wordt weergegeven en klikt u vervolgens op **Sjabloon toevoegen**.

   >[!NOTE]
   >
   >Overweeg het volgende wanneer u een Geautomatiseerde malplaatje van het Werkschema gebruikt:
   >   
   >* De instellingen van een automatische werkstroomsjabloon bepalen wat u kunt doen met de geautomatiseerde workflow voor een proefdruk. Als de knop Een werkgebied toevoegen bijvoorbeeld is uitgeschakeld in de sjabloon, is deze niet zichtbaar wanneer u werkt met de instellingen voor Geautomatiseerde workflow voor de proefdruk.
   >* Wanneer een persoon wordt toegevoegd aan een werkgebied in een Geautomatiseerde malplaatje van het Werkschema, maar ook reeds als recensent op het bewijs aanwezig is, verwijdert het toepassen van het malplaatje de recensent uit het stadium. Als u geen andere revisor aan het werkgebied toevoegt, wordt u in een bericht gevraagd er een toe te voegen.
   >* Uw vermogen om een Geautomatiseerde malplaatje van het Werkschema te wijzigen hangt van de malplaatjemontages af die door de beheerder van Workfront worden gevormd, zoals die in wordt beschreven. Als de mogelijkheid om de sjabloon te wijzigen is uitgeschakeld, kan alleen de eigenaar van de sjabloon deze wijzigen.

1. Configureer de eerste fase van de geautomatiseerde workflow:

   1. (Optioneel) Als u een naam wilt maken voor het eerste werkgebied, klikt u op **Fase 1** Typ vervolgens de naam.
   1. In de **Ontvangers** voegt u revisoren toe aan het werkgebied.

      >[!NOTE]
      >
      >Houd rekening met het volgende wanneer u revisoren aan een werkgebied toevoegt:
      >   
      >* U kunt externe gebruikers met een e-mailadres aan een werkgebied toevoegen.
      >* Nadat u een gebruiker aan een stadium toevoegt, kunt u montages voor die gebruiker op de proef vormen.
      >* U kunt gebruikers rechtstreeks naar een ander werkgebied slepen of u kunt gebruikers naar een werkgebied in het **Staven** diagram. Druk op Shift+Ctrl (Windows) of Shift+Command (Mac) om meerdere gebruikers te selecteren.
      >* U kunt een controleur slechts eenmaal aan een proefdruk toevoegen, wat betekent dat u dezelfde persoon niet aan meer dan één werkgebied kunt toevoegen op de proefdruk.
      >* Revisoren die niet aan een privéfase zijn toegevoegd, kunnen dat stadium niet zien op de proefdruk of de opmerkingen die in dat stadium zijn gemaakt.
      >* Door gebrek, verleent het toevoegen van een gebruiker aan een stadium die gebruiker toegang om de proef van het ogenblik te bekijken de proef wordt gecreeerd. Uw Workfront-beheerder kan gebruikers de toegang tot de proefdruk beperken tot de werkstroom het werkgebied ingaat waar de gebruiker is toegevoegd.

   1. Klikken **Werkgebiedinstellingen**.
   1. Klik op een **Werkgebied activeren** geeft aan hoe het werkgebied moet worden geactiveerd.

      Voor de eerste fase kunt u alleen **Bij proefmaken**, **Op een specifieke datum en tijd**, of **Handmatig**.

   1. (Voorwaardelijk) Als u **Op een specifieke datum en tijd** in de vorige stap selecteert u de datum en het tijdstip waarop u het werkgebied in de **Activeren op** die wordt weergegeven.

   1. Gebruik een van de onderstaande opties om het werkgebied verder te configureren.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Tijdslimiet voor werkgebied instellen</td>
         <td><p>Als u een deadline voor het werkgebied wilt instellen, klikt u op een optie in het dialoogvenster <strong>Deadline-opties</strong> vervolgkeuzelijst. Vervolgens, onder <strong>Deadline</strong>Voer een van de volgende handelingen uit:</p>
          <ul>
           <li>Als u <strong>Specifieke datum instellen</strong>: Selecteer de gewenste datum en tijd voor de deadline.</li>
           <li>Als u <strong>Berekenen vanaf activeringsdatum van werkgebied</strong>: Selecteer het aantal werkdagen dat u aan de activeringsdatum van het werkgebied wilt toevoegen om de deadline te bepalen.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Werkgebied vergrendelen</td>
         <td>Geef op wanneer het werkgebied kan worden vergrendeld. </td>
        </tr>
        <tr>
         <td role="rowheader">Rechten van primaire beslissingen overdragen aan</td>
         <td><p>Selecteer de primaire beslisser in het werkgebied (alleen beschikbaar nadat u ten minste één persoon aan het werkgebied hebt toegevoegd die de rol van fiatteur of hoger heeft). Als u een primaire beslisser selecteert, wordt de <strong>Slechts één besluit vereist</strong> is uitgeschakeld in dit werkgebied.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Voor deze fase slechts één besluit vereisen</td>
         <td>Beëindigt het hele herzieningsproces wanneer een van de besluitvormers een besluit neemt.<p>Deze optie is niet beschikbaar als u een gebruiker hebt aangewezen in het dialoogvenster <strong>Primaire beslisser</strong>vervolgkeuzelijst.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Dit stadium privé maken</td>
         <td>Hiermee kunnen alleen de volgende personen opmerkingen en beslissingen weergeven die tijdens dit werkgebied zijn gemaakt: toezichthouders, Workfront-beheerders en Workfront Proof-beheerders</td>
        </tr>
       </tbody>
      </table>

1. Een ander werkgebied toevoegen en configureren:

   1. Klikken **Nieuwe fase**.
   1. (Optioneel) Als u een naam wilt maken voor het eerste werkgebied, klikt u op **Fase 2** (of **Fase 3**, **Fase 4**, enzovoort) typt u de naam.

   1. Klik op de knop **Werkgebied activeren** selecteert u vervolgens een optie om op te geven of het werkgebied automatisch of handmatig wordt geactiveerd.

      Naast de opties **Bij proefmaken**, **Op een specifieke datum en tijd**, of **Handmatig** kunt u een optie selecteren die afhankelijk is van wat er in de vorige stap is gebeurd:

      ![](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. Als u een werkgebiedoptie activeren hebt geselecteerd die afhankelijk is van wat er in de vorige stap is gebeurd, gebruikt u de opties die de activeringsinstelling lijken te configureren.

      Als u bijvoorbeeld **Als de status van het vorige werkgebied verandert**, selecteert u de **Vorige fase** selecteert u vervolgens de status in het dialoogvenster **Status gewijzigd in** doos.

1. Herhaal desgewenst de vorige stap om meer stappen toe te voegen.

   Aangezien u stadia aan de Geautomatiseerde Werkschema toevoegt, vormt een diagram op het scherm om hen te vertegenwoordigen:

   ![](assets/stages-diagram-350x213.png)

1. Doorgaan met [E-mailinstellingen configureren voor de proefdruk](#configure-email-settings-for-the-proof) hieronder.

## E-mailinstellingen configureren voor de proefdruk {#configure-email-settings-for-the-proof}

1. In de **E-mailmelding** selecteert u of u e-mailmeldingen en een aangepast bericht wilt verzenden aan de gebruikers in [Een geavanceerde proefdruk maken met een geautomatiseerde workflow](#workflow) eerder in dit artikel :

   <table>
      <tbody>
      <tr>
      <td>Ontvangers op de hoogte stellen van dit bewijs</td>
      <td>Selecteer deze optie om een e-mailbericht naar gebruikers te verzenden. Wanneer <strong>Basis delen</strong> is geselecteerd in het dialoogvenster <strong>Workflow</strong> wordt een e-mailmelding verzonden wanneer de proefdruk wordt gemaakt. Wanneer <strong>Geautomatiseerde workflow</strong> is geselecteerd in het dialoogvenster <strong>Workflow</strong> wordt een e-mailmelding verzonden wanneer de proefdruk het werkgebied van de geautomatiseerde workflow ingaat waaraan de gebruiker is gekoppeld.</td>
      </tr>
      <tr>
      <td>Aangepast bericht toevoegen</td>
      <td>Selecteer deze optie om een aangepast bericht op te nemen in het bericht. U kunt een onderwerp en berichttekst opgeven. De berichttekst kan tekstopmaak bevatten, zoals vet, opsommingstekens en hyperlinks.</td>
      </tr>
      </tbody>
      </table>


1. Doorgaan met [Proofinginstellingen configureren](#configure-proof-settings) hieronder.

## Proofinginstellingen configureren {#configure-proof-settings}

1. In de **Proefinstellingen** selecteert u een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aanmelding vereisen - proefdruk kan alleen worden gedeeld met andere gebruikers</td> 
      <td>Als deze optie is uitgeschakeld (standaard), kan iedereen met de URL de proefdruk bekijken. <br>Wanneer deze optie is geselecteerd:
       <ul>
        <li>Alleen Workfront Proof-gebruikers kunnen de proefdruk bekijken.</li>
        <li>Gebruikers kunnen zich alleen aanmelden bij de proefdruk als ze aan de proefdruk zijn toegevoegd.</li>
        <li>Abonnementen kunnen niet worden ingeschakeld.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Slechts één besluit vereist voor dit bewijs</td> 
      <td>Wanneer deze optie is geselecteerd, wordt de evaluatie voltooid nadat een van de besluitvormers zijn besluit heeft genomen.<br>Deze optie is standaard uitgeschakeld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vereisen dat besluiten elektronisch worden ondertekend</td> 
      <td>Gebruikers moeten hun gebruikersnaam en wachtwoord opgeven op het moment dat zij een beslissing nemen over een bewijs.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bewijs vergrendelen wanneer alle vereiste beslissingen zijn genomen</td> 
      <td>Als deze instelling is ingeschakeld, wordt de proefdrukstatus vergrendeld nadat alle beslissingen zijn genomen. De status wordt automatisch gewijzigd van ontgrendeld in vergrendeld wanneer de laatste fiatteur zijn beslissing neemt.<br>Deze optie is standaard uitgeschakeld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Origineel bestand downloaden</td> 
      <td>Als deze optie is geselecteerd, kunnen revisoren het originele bestand downloaden van waaruit de proefdruk is gemaakt.<br>Wanneer deze optie is uitgeschakeld, is het pictogram Downloaden niet meer zichtbaar.<br>Deze optie is standaard ingeschakeld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proef delen via openbare URL of insluitcode</td> 
      <td>Als deze optie is geselecteerd, kan de proefdruk worden gedeeld via een openbare URL of insluitcode.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abonneren op bewijs via openbare URL of insluitcode</td> 
      <td>Als deze optie is geselecteerd, kunnen personen die niet expliciet aan de proefdruk zijn toegevoegd, zich op de proefdruk abonneren. De persoon die zich op de proef abonneert, krijgt de rol en e-mail die u in de volgende montages bepaalt:
       <ul>
        <li><strong>Abonnementenrol:</strong> De standaardproefdrukrol die wordt toegewezen aan alle revisoren die zich op de proefdruk abonneren.</li>
        <li><strong>Instellingen voor e-mailwaarschuwingen voor abonnees:</strong> De standaard e-mailwaarschuwing die wordt toegewezen aan alle revisoren die zich op de proefdruk abonneren.</li>
       </ul><p>
        <ul>
         <li><strong>Bewijs van toegang via e-mailkoppeling vereist voor:</strong> Configureer of de abonnee een e-mail ontvangt met een koppeling naar de proefdruk. U kunt <strong>Geen e-mail</strong> (E-mailkoppeling is niet vereist voor toegang tot de proefdruk), <strong>Alleen e-mail met verificatie</strong> (de abonnee ontvangt een koppeling naar de proefdruk via e-mail zonder verificatie), of <strong>E-mails over validatie en proefdrukken</strong> (de abonnee ontvangt een koppeling naar de proefdruk via e-mail en moet op de koppeling klikken om toegang te krijgen tot een proefdruk. Deze optie heeft tot doel ervoor te zorgen dat de persoon een correct e-mailadres heeft ingevoerd waartoe hij toegang heeft).</li>
        </ul><p><strong>Opmerking:</strong> Als de proefdrukken de Geautomatiseerde Werkstroom in bijlage hebben alle abonnementen zullen bevestigingse-mail aan de bewijseigenaars produceren, zodat kunnen zij beslissen welk stadium de persoon aan zou moeten worden toegevoegd.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Proef maken**.

   Workfront begint met het genereren van een proefdruk van de geselecteerde documenten of websites. Afhankelijk van de bestandsgrootte en het type kan de vertraging bij het uploaden van een document variëren. Wees geduld, want het duurt langer om grotere bestanden te genereren. U kunt van de pagina weg navigeren en Workfront blijft uw bestand genereren. De maximale grootte voor het uploaden van bestanden is 4 GB.

1. Klik op **Proef openen** om de proefdrukviewer te starten.

   ![](assets/open-proof-350x132.png)

   Gebruikers die geen proefdrukken op hun account hebben ingeschakeld, kunnen het document nog steeds bekijken en opmerkingen naar de proefdruk maken [.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)
