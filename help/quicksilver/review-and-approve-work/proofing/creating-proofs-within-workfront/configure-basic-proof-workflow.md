---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Een geavanceerde proefdruk maken met een standaardworkflow
description: Met een basisworkflow kunt u meerdere revisoren een proefdruk laten maken, maar deze zijn niet in fasen geordend. Alle revisoren die u toevoegt, hebben direct toegang tot de proefdruk nadat u deze hebt gemaakt.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1858'
ht-degree: 0%

---

# Een geavanceerde proefdruk maken met een standaardworkflow

<!-- Audited: 1/2024 -->

Met een basisworkflow kunt u meerdere revisoren een proefdruk laten maken, maar deze zijn niet in fasen geordend. Alle revisoren die u toevoegt, hebben direct toegang tot de proefdruk nadat u deze hebt gemaakt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td>
   <p>Nieuw: alle</p>
    <p>Huidig abonnement: Pro of hoger</p>
   <p>Verouderd abonnement: Selecteren of hoger</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref"> Toegang tot het proefdrukken van functionaliteit in Workfront </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
   <p>Nieuw: Standaard</p>
    <p>Huidig: Werk of Plan</p> <p>Ouder plan: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>Manager of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot documenten bewerken</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, rol, of Profiel van de Toestemming van het Bewijs u hebt, contacteer uw beheerder van Workfront of van Workfront Proof.

+++

## Een geavanceerde proefdruk maken met een standaardworkflow

1. Ga naar het project, de taak, of de kwestie waar u de proef wilt, dan klik de **Documenten** tabel.
1. Klik **toevoegen nieuw** > Bewijs, upload de inhoud, dan werk door de hieronder vermelde secties.

   of

   Beweeg over een bestaand document, dan klik **creëren Bewijs** > **Geavanceerde Bewijs** en het werk door de hieronder vermelde secties.

## De workflow configureren en revisoren toevoegen

1. In de het type van Werkschema sectie, kies **Basis**.
1. Geef de gebruikers op die u wilt toevoegen en kies een proefdrukrol.

   ![ Nieuwe proefdrukrollen ](assets/new-proof---roles-350x213.png)

1. In de volgende tabel worden elke rol en de bijbehorende rechten weergegeven.

   <table border="1" cellspacing="15" cellpadding="1"> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p> </p> </th> 
      <th> <p><strong> Mening een proef </strong> </p> </th> 
      <th> <p><strong> voeg markeringen </strong> toe </p> </th> 
      <th> <p><strong> voeg commentaren </strong> toe </p> </th> 
      <th> <p><strong> geeft eigen commentaren uit als er geen antwoorden zijn </strong> </p> </th> 
      <th> <p><strong> maak een besluit </strong> </p> </th> 
      <th> <p><strong> Schrap commentaren die door anderen worden gemaakt </strong> </p> </th> 
      <th>Opmerkingen oplossen</th> 
      <th>Handelingen toepassen op opmerkingen</th> 
      <th> <p><strong> geef de proef </strong> uit </p> </th> 
      <th>De proefdruk delen met anderen</th> 
      <th>Nieuwe versie maken</th> 
      <th> <p><strong> de goedkeuringsverzoeken van de Mening op het gebied van het Huis </strong> </p> </th> 
      <th>Nieuwe revisoren toevoegen</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong> las slechts </strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong> Recensent </strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong> Fiatteur </strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong> Recensent &amp; Fiatteur </strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong> Auteur </strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> </td> 
      <td>✓</td> 
     </tr> 
     <tr> 
      <td> <p><strong> Moderator </strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p><strong> ✓ </strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
     </tr> 
    </tbody> 
   </table>

1. De gebruikers op nieuwe plannen van Workfront kunnen auteur of moderatorrollen aan om het even welke gebruikers in het systeem verlenen. De gebruikers op erfenisplannen kunnen auteur of moderatorrollen aan om het even welke gebruiker met een proefvergunning in het systeem verlenen.
1. (Optioneel) Selecteer, terwijl de vervolgkeuzelijst nog steeds is geopend, aanvullende machtigingen die onder aan het menu beschikbaar zijn:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Opmerkingen oplossen en handelingen toepassen </td> 
      <td> <p>Hiermee kan de Workfront-gebruiker het volgende doen:</p> 
       <ul> 
        <li>Los een commentaar op nadat het is gericht, zoals die in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref"> wordt verklaard de bewijsdrukcommentaren van de Los </a>.</li> 
        <li>Pas acties op commentaren toe, zoals die in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref"> acties van het Gebruik op proefdrukcommentaren </a> worden verklaard. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proef delen door labels toe te wijzen</td> 
      <td> <p>Staat de recensent toe om het even welke gebruiker van Workfront aan de proef toe te voegen zoals die in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref"> wordt verklaard de gebruikers van de Markering om een proef </a> te delen.</p> <p>Opmerking:  <p>Als deze twee opties niet beschikbaar (grijs weergegeven) zijn, beschikt de gebruiker al over een machtigingsprofiel waarmee opmerkingen kunnen worden opgelost, handelingen kunnen worden toegepast op opmerkingen en een gebruiker kan worden gelabeld. </p> <p>Als de opties niet worden weergegeven, is de persoon die u hebt toegevoegd geen houder van een Workfront-licentie.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Herhaal stap 1-3 voor alle andere gebruikers die u aan de proefdruk hebt toegevoegd.
1. Voor elke gebruiker u deelt met, in de **E-mail alarm** drop-down lijst, selecteer het type e-mailalarm deze gebruiker ontvangt wanneer de mensen commentaren en besluiten over het bewijs maken:

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

1. Ga met [ verder vormen e-mailmontages voor de proef ](#configure-email-settings-for-the-proof) hieronder.

## E-mailinstellingen configureren voor de proefdruk {#configure-email-settings-for-the-proof}

1. In de **E-mail- bericht** sectie, selecteer of om e-mailberichten en een douanebericht naar de gebruikers te verzenden u in [ selecteerde creeer een geavanceerde proef met een Basiswerkschema ](#workflow) vroeger in dit artikel:

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
        <li><strong> de rol van de Abonnee:</strong> de standaardproefdrukrol die aan alle recensenten wordt toegewezen die aan de proef intekenen. </li>
        <li><strong> e-mail waakzame montages voor abonnees:</strong> het standaard e-mailalarm dat aan alle recensenten wordt toegewezen die aan de proef intekenen.</li>
       </ul><p>
        <ul>
         <li><strong> vereiste toegang van het Bewijs via e-mailverbinding voor:</strong> Vorm of de abonnee een e-mail met een verbinding aan de proef ontvangt. U kunt <strong> Geen e-mail </strong> selecteren (de e-mailverbinding wordt niet vereist om tot de proef toegang te hebben), <strong> het bericht van het Bewijs slechts </strong> (de abonnee ontvangt een verbinding aan de proef via e-mail zonder enige controle), of <strong> Bevestiging en proef bericht e-mails </strong> (de abonnee ontvangt een verbinding aan de proef via e-mail en moet de verbinding klikken om tot een proef toegang te hebben, is het doel van deze optie ervoor te zorgen dat de persoon een correct is ingegaan e-mailadres waartoe zij toegang hebben).</li>
        </ul><p>Opmerking:  Als de proefdrukken de Geautomatiseerde Werkstroom in bijlage hebben alle abonnementen zullen bevestigingse-mail aan de bewijseigenaars produceren, zodat kunnen zij beslissen welk stadium de persoon aan zou moeten worden toegevoegd.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **creëren Bewijs**.

   Workfront begint met het genereren van een proefdruk van de geselecteerde documenten of websites. Afhankelijk van de bestandsgrootte en het type kan de vertraging bij het uploaden van een document variëren. Wees geduld, want het duurt langer om grotere bestanden te genereren. U kunt van de pagina weg navigeren en Workfront blijft uw bestand genereren. De maximale grootte voor het uploaden van bestanden is 4 GB.

1. Nadat de proef wordt geproduceerd, klik **Open proef** om de het proef kijker te lanceren.

   ![ Open proef ](assets/open-proof-350x132.png)

   Gebruikers die geen proefdrukken op hun account hebben ingeschakeld, kunnen het document nog steeds bekijken en opmerkingen naar de proefdruk maken.