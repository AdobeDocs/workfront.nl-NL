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

Met een geautomatiseerde workflow kunt u het controleproces eenvoudiger beheren als uw proces complex is of als u inhoud ter controle regelmatig naar dezelfde personen verzendt. De proefdruk gaat van stadium aan stadium en Adobe Workfront brengt elke gebruiker op de hoogte wanneer het hun beurt is om het te herzien. Voor meer informatie over Geautomatiseerde werkschema&#39;s, zie [ Geautomatiseerd overzicht van het Werkschema ](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Nieuw: alle</p><p>Huidig abonnement: Pro of hoger</p><p>Verouderd abonnement: Selecteren of hoger</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref"> Toegang tot het proefdrukken van functionaliteit in Workfront </a>.</p> </td> 
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

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een geavanceerde proefdruk maken met een geautomatiseerde workflow

1. Ga naar het project, de taak, of de kwestie waar u de proef wilt, dan klik de **Documenten** tabel.
1. Klik **toevoegen nieuw** > Bewijs, upload de inhoud, dan werk door de hieronder vermelde secties.

   of

   Beweeg over een bestaand document, dan klik **creëren Bewijs** > **Geavanceerde Bewijs** en het werk door de hieronder vermelde secties.

## De proefdrukfasen configureren

1. In de het type van Werkschema sectie, kies **Geautomatiseerd**.
1. (Facultatief) als u een Geautomatiseerd malplaatje van het Werkschema wilt gebruiken dat uw beheerder van Workfront creeerde en met u deelde, **voegt malplaatje** toe, selecteert het malplaatje in de doos die verschijnt, dan klik **malplaatje** toevoegen.

   >[!NOTE]
   >
   >Overweeg het volgende wanneer u een Geautomatiseerde malplaatje van het Werkschema gebruikt:
   >   
   >* De instellingen van een automatische werkstroomsjabloon bepalen wat u kunt doen met de geautomatiseerde workflow voor een proefdruk. Als de knop Een werkgebied toevoegen bijvoorbeeld is uitgeschakeld in de sjabloon, is deze niet zichtbaar wanneer u werkt met de instellingen voor Geautomatiseerde workflow voor de proefdruk.
   >* Wanneer een persoon wordt toegevoegd aan een werkgebied in een Geautomatiseerde malplaatje van het Werkschema, maar ook reeds als recensent op het bewijs aanwezig is, verwijdert het toepassen van het malplaatje de recensent uit het stadium. Als u geen andere revisor aan het werkgebied toevoegt, wordt u in een bericht gevraagd er een toe te voegen.
   >* Uw vermogen om een Geautomatiseerde malplaatje van het Werkschema te wijzigen hangt van de malplaatjemontages af die door de beheerder van Workfront worden gevormd, zoals die in wordt beschreven. Als de mogelijkheid om de sjabloon te wijzigen is uitgeschakeld, kan alleen de eigenaar van de sjabloon deze wijzigen.

1. Configureer de eerste fase van de geautomatiseerde workflow:

   1. (Facultatief) als u een naam voor het eerste stadium wilt tot stand brengen, klik **Stadium 1**, dan typ de naam.
   1. In de **Ontvangers** sectie voor het stadium, voeg recensenten aan het stadium toe.

      >[!NOTE]
      >
      >Houd rekening met het volgende wanneer u revisoren aan een werkgebied toevoegt:
      >   
      >* U kunt externe gebruikers met een e-mailadres aan een werkgebied toevoegen.
      >* Nadat u een gebruiker aan een stadium toevoegt, kunt u montages voor die gebruiker op de proef vormen.
      >* U kunt gebruikers rechtstreeks aan een ander stadium slepen, of u kunt gebruikers aan een stadium op het **Stadium** diagram slepen. Druk op Shift+Ctrl (Windows) of Shift+Command (Mac) om meerdere gebruikers te selecteren.
      >* U kunt een controleur slechts eenmaal aan een proefdruk toevoegen, wat betekent dat u dezelfde persoon niet aan meer dan één werkgebied kunt toevoegen op de proefdruk.
      >* Revisoren die niet aan een privéfase zijn toegevoegd, kunnen dat stadium niet zien op de proefdruk of de opmerkingen die in dat stadium zijn gemaakt.
      >* Door gebrek, verleent het toevoegen van een gebruiker aan een stadium die gebruiker toegang om de proef van het ogenblik te bekijken de proef wordt gecreeerd. Uw Workfront-beheerder kan gebruikers de toegang tot de proefdruk beperken tot de werkstroom het werkgebied ingaat waar de gebruiker is toegevoegd.

   1. Klik **montages van het Stadium**.
   1. Klik **activeer stadium** optie om erop te wijzen hoe u het stadium wilt activeren.

      Voor het eerste stadium, kunt u slechts **op proefverwezenlijking** selecteren, **op een specifieke datum en een tijd**, of **manueel**.

   1. (Voorwaardelijk) als u **op een specifieke datum en een tijd** in de vorige stap selecteerde, selecteer de datum en de tijd wanneer u het stadium in **wilt activeren op** doos die verschijnt.

   1. Gebruik een van de onderstaande opties om het werkgebied verder te configureren.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Tijdslimiet voor werkgebied instellen</td>
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
         <td role="rowheader">Rechten van primaire beslissingen overdragen aan</td>
         <td><p>Selecteer de primaire beslisser in het werkgebied (alleen beschikbaar nadat u ten minste één persoon aan het werkgebied hebt toegevoegd die de rol van fiatteur of hoger heeft). Als u een Primaire besluitvormer selecteert, wordt <strong> slechts één vereiste besluit </strong> optie onbruikbaar gemaakt op dit stadium.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Voor deze fase slechts één besluit vereisen</td>
         <td>Beëindigt het hele herzieningsproces wanneer een van de besluitvormers een besluit neemt.<p>Deze optie is niet beschikbaar als u een gebruiker in het <strong> Primaire drop-down menu van de besluitvormer </strong> wees.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Dit stadium privé maken</td>
         <td>Hiermee kunnen alleen de volgende personen opmerkingen en beslissingen weergeven die tijdens dit werkgebied zijn gemaakt: toezichthouders, Workfront-beheerders en Workfront Proof-beheerders</td>
        </tr>
       </tbody>
      </table>

1. Een ander werkgebied toevoegen en configureren:

   1. Klik **Nieuw stadium**.
   1. (Facultatief) als u een naam voor het eerste stadium wilt tot stand brengen, **Stadium 2** (of **Stadium 3**, **Stadium 4**, etc.) klikken, dan typ de naam.

   1. Klik **activeer stadium**, dan selecteer een optie om te specificeren of het stadium automatisch of manueel wordt geactiveerd.

      Naast de opties **op proefverwezenlijking**, **op een specifieke datum en een tijd**, of **manueel**, kunt u een optie selecteren die van wat in de vorige stap afhankelijk is voorgekomen:

      ![](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. Als u een werkgebiedoptie activeren hebt geselecteerd die afhankelijk is van wat er in de vorige stap is gebeurd, gebruikt u de opties die de activeringsinstelling lijken te configureren.

      Bijvoorbeeld, als u **selecteerde toen de vorige veranderingen van het stadium**, het **Vorige stadium** selecteren, dan de status in de **Status veranderde in** doos.

1. Herhaal desgewenst de vorige stap om meer stappen toe te voegen.

   Aangezien u stadia aan de Geautomatiseerde Werkschema toevoegt, vormt een diagram op het scherm om hen te vertegenwoordigen:

   ![](assets/stages-diagram-350x213.png)

1. Ga met [ verder vormen e-mailmontages voor de proef ](#configure-email-settings-for-the-proof) hieronder.

## E-mailinstellingen configureren voor de proefdruk {#configure-email-settings-for-the-proof}

1. In de **E-mail- bericht** sectie, selecteer of om e-mailberichten en een douanebericht naar de gebruikers te verzenden u in [ selecteerde creeer een geavanceerde proef met een Geautomatiseerd werkschema ](#workflow) vroeger in dit artikel:

   <table>
      <tbody>
      <tr>
      <td>Ontvangers op de hoogte stellen van dit bewijs</td>
      <td>Selecteer deze optie om een e-mailbericht naar gebruikers te verzenden. Wanneer <strong> Basis het delen </strong> in de <strong> 3} sectie van het Werkschema {wordt geselecteerd, wordt een e-mailbericht verzonden wanneer de proef wordt gecreeerd. </strong> Wanneer <strong> Geautomatiseerde werkschema </strong> in de <strong> 3} sectie van het Werkschema {wordt geselecteerd, wordt een e-mailbericht verzonden wanneer het bewijs het stadium van het Geautomatiseerde Werkschema ingaat dat de gebruiker met wordt geassocieerd.</strong></td>
      </tr>
      <tr>
      <td>Aangepast bericht toevoegen</td>
      <td>Selecteer deze optie om een aangepast bericht op te nemen in het bericht. U kunt een onderwerp en berichttekst opgeven. De berichttekst kan tekstopmaak bevatten, zoals vet, opsommingstekens en hyperlinks.</td>
      </tr>
      </tbody>
      </table>


1. Ga met [ verder vormen proefmontages ](#configure-proof-settings) hieronder.

## Proofinginstellingen configureren {#configure-proof-settings}

1. In de **sectie van de Montages van het Bewijs**, selecteer om het even welke volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aanmelding vereisen - proefdruk kan alleen worden gedeeld met andere gebruikers</td> 
      <td>Als deze optie is uitgeschakeld (standaard), kan iedereen met de URL de proefdruk bekijken. <br> wanneer deze optie wordt geselecteerd:
       <ul>
        <li>Alleen Workfront Proof-gebruikers kunnen de proefdruk bekijken.</li>
        <li>Gebruikers kunnen zich alleen aanmelden bij de proefdruk als ze aan de proefdruk zijn toegevoegd.</li>
        <li>Abonnementen kunnen niet worden ingeschakeld.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Slechts één besluit vereist voor dit bewijs</td> 
      <td>Wanneer deze optie is geselecteerd, wordt de evaluatie voltooid nadat een van de besluitvormers zijn besluit heeft genomen.<br> deze optie wordt onbruikbaar gemaakt door gebrek.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vereisen dat besluiten elektronisch worden ondertekend</td> 
      <td>Gebruikers moeten hun gebruikersnaam en wachtwoord opgeven op het moment dat zij een beslissing nemen over een bewijs.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bewijs vergrendelen wanneer alle vereiste beslissingen zijn genomen</td> 
      <td>Als deze instelling is ingeschakeld, wordt de proefdrukstatus vergrendeld nadat alle beslissingen zijn genomen. De status wordt automatisch gewijzigd van ontgrendeld in vergrendeld wanneer de laatste fiatteur zijn beslissing neemt.<br> deze optie wordt onbruikbaar gemaakt door gebrek.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Origineel bestand downloaden</td> 
      <td>Als deze optie is geselecteerd, kunnen revisoren het originele bestand downloaden van waaruit de proefdruk is gemaakt.<br> wanneer deze optie wordt geschrapt, is het pictogram van de Download niet meer zichtbaar.<br> Deze optie wordt toegelaten door gebrek.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proef delen via openbare URL of insluitcode</td> 
      <td>Als deze optie is geselecteerd, kan de proefdruk worden gedeeld via een openbare URL of insluitcode.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abonneren op bewijs via openbare URL of insluitcode</td> 
      <td>Als deze optie is geselecteerd, kunnen personen die niet expliciet aan de proefdruk zijn toegevoegd, zich op de proefdruk abonneren. De persoon die zich op de proef abonneert, krijgt de rol en e-mail die u in de volgende montages bepaalt:
       <ul>
        <li><strong> de rol van de Abonnee:</strong> de standaardproefdrukrol die aan alle recensenten wordt toegewezen die aan de proef intekenen.</li>
        <li><strong> e-mail waakzame montages voor abonnees:</strong> het standaard e-mailalarm dat aan alle recensenten wordt toegewezen die aan de proef intekenen.</li>
       </ul><p>
        <ul>
         <li><strong> vereiste toegang van het Bewijs via e-mailverbinding voor:</strong> Vorm of de abonnee een e-mail met een verbinding aan de proef ontvangt. U kunt <strong> Geen e-mail </strong> selecteren (de e-mailverbinding wordt niet vereist om tot de proef toegang te hebben), <strong> het bericht van het Bewijs slechts </strong> (de abonnee ontvangt een verbinding aan de proef via e-mail zonder enige controle), of <strong> Bevestiging en proef bericht e-mails </strong> (de abonnee ontvangt een verbinding aan de proef via e-mail en moet de verbinding klikken om tot een proef toegang te hebben, is het doel van deze optie ervoor te zorgen dat de persoon een correct is ingegaan e-mailadres waartoe zij toegang hebben).</li>
        </ul><p><strong> Nota:</strong> als de proeven het Werkschema hebben geautomatiseerd alle abonnementen zullen bevestigingse-mail aan de bewijseigenaars produceren, zodat konden zij beslissen welk stadium de persoon aan zou moeten worden toegevoegd.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **creëren Bewijs**.

   Workfront begint met het genereren van een proefdruk van de geselecteerde documenten of websites. Afhankelijk van de bestandsgrootte en het type kan de vertraging bij het uploaden van een document variëren. Wees geduld, want het duurt langer om grotere bestanden te genereren. U kunt van de pagina weg navigeren en Workfront blijft uw bestand genereren. De maximale grootte voor het uploaden van bestanden is 4 GB.

1. Nadat de proef wordt geproduceerd, klik **Open proef** om de het proef kijker te lanceren.

   ![](assets/open-proof-350x132.png)

   Gebruikers die geen proefdrukken op hun account hebben ingeschakeld, kunnen het document nog steeds bekijken en opmerkingen naar de proefdruk maken [ . ](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)
