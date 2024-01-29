---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Een geavanceerde proefdruk maken met een standaardworkflow
description: Met een basisworkflow kunt u meerdere revisoren een proefdruk laten maken, maar deze zijn niet in fasen geordend. Alle revisoren die u toevoegt, hebben direct toegang tot de proefdruk nadat u deze hebt gemaakt.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
source-git-commit: d71ee30378c39975366f4f257e3f7b17aba0c0ae
workflow-type: tm+mt
source-wordcount: '1842'
ht-degree: 0%

---

# Een geavanceerde proefdruk maken met een standaardworkflow

<!-- Audited: 1/2024 -->

Met een basisworkflow kunt u meerdere revisoren een proefdruk laten maken, maar deze zijn niet in fasen geordend. Alle revisoren die u toevoegt, hebben direct toegang tot de proefdruk nadat u deze hebt gemaakt.

## Toegangsvereisten

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
   <p>Verouderd abonnement: Selecteren of hoger</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Toegang tot proefdrukfunctionaliteit in Workfront</a>.</p> </td> 
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

&#42;Neem contact op met de beheerder van de Workfront of Workfront-proefdrukken als u wilt weten welk plan, welke rol of welk proefdrukprofiel u hebt.

## Een geavanceerde proefdruk maken met een standaardworkflow

1. Ga naar het project, de taak, of de kwestie waar u het proef wilt, dan klik **Documenten** tab.
1. Klikken **Nieuw toevoegen** > Proef, upload de inhoud en doorloop de onderstaande secties.

   of

   Houd de cursor boven een bestaand document en klik vervolgens op de knop **Proef maken** > **Geavanceerd proefdrukken** en doorwerkt u de onderstaande secties.

## De workflow configureren en revisoren toevoegen

1. Kies in de sectie Type workflow de optie **Basis**.
1. Geef de gebruikers op die u wilt toevoegen en kies een proefdrukrol.

   ![](assets/new-proof---roles-350x213.png)

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
      <th> <p><strong>Een proefafdruk weergeven</strong> </p> </th> 
      <th> <p><strong>Markeringen toevoegen</strong> </p> </th> 
      <th> <p><strong>Opmerkingen toevoegen</strong> </p> </th> 
      <th> <p><strong>Eigen opmerkingen bewerken als er geen reacties zijn</strong> </p> </th> 
      <th> <p><strong>Beslissingen nemen</strong> </p> </th> 
      <th> <p><strong>Opmerkingen van anderen verwijderen</strong> </p> </th> 
      <th>Opmerkingen oplossen</th> 
      <th>Handelingen toepassen op opmerkingen</th> 
      <th> <p><strong>De proefdruk bewerken</strong> </p> </th> 
      <th>De proefdruk delen met anderen</th> 
      <th>Nieuwe versie maken</th> 
      <th> <p><strong>Goedkeuringsaanvragen weergeven in het gedeelte Home</strong> </p> </th> 
      <th>Nieuwe revisoren toevoegen</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>Alleen-lezen</strong> </p> </td> 
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
      <td> <p><strong>Revisor</strong> </p> </td> 
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
      <td> <p><strong>Fiatteur</strong> </p> </td> 
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
      <td> <p><strong>Revisor en fiatteur</strong> </p> </td> 
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
      <td> <p><strong>Auteur</strong> </p> </td> 
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
      <td> <p><strong>Moderator</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p><strong>✓</strong> </p> </td> 
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
        <li>Een opmerking oplossen nadat deze is behandeld, zoals wordt uitgelegd in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">Proefdrukopmerkingen oplossen</a>.</li> 
        <li>Handelingen toepassen op opmerkingen, zoals wordt uitgelegd in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">Handelingen gebruiken voor opmerkingen bij proefdrukken</a>. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proef delen door labels toe te wijzen</td> 
      <td> <p>Hiermee kan de controleur een Workfront-gebruiker aan de proefdruk toevoegen, zoals wordt uitgelegd in <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">Gebruikers een proef laten delen</a>.</p> <p>Opmerking:  <p>Als deze twee opties niet beschikbaar (grijs weergegeven) zijn, beschikt de gebruiker al over een machtigingsprofiel waarmee opmerkingen kunnen worden opgelost, handelingen kunnen worden toegepast op opmerkingen en een gebruiker kan worden gelabeld. </p> <p>Als de opties niet worden weergegeven, is de persoon die u hebt toegevoegd geen houder van een Workfront-licentie.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Herhaal stap 1-3 voor alle andere gebruikers die u aan de proefdruk hebt toegevoegd.
1. Voor elke gebruiker met wie u deelt, in **E-mailwaarschuwingen** Selecteer in de vervolgkeuzelijst het type e-mailwaarschuwing dat deze gebruiker ontvangt wanneer mensen opmerkingen maken en beslissingen nemen over de proefdruk:

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
      <td>Een e-mail wordt alleen naar de controleur verzonden als iemand uitdrukkelijk op zijn opmerking reageert (dit sluit zijn eigen reacties op zijn eigen opmerkingen uit). Dit betekent dat als iemand op het bewijs een nieuwe opmerking maakt, de controleur niet op de hoogte wordt gesteld.<p>Deze instelling wordt aanbevolen voor uw klanten op de proefdruk, zodat zij geen andere opmerkingen over de proefdruk ontvangen en alleen op de hoogte worden gesteld van antwoorden op hun eigen opmerkingen.</p><p>Hoewel revisoren met deze instelling voor e-mailwaarschuwingen geen melding krijgen van andere nieuwe opmerkingen, kunnen ze alle opmerkingen over de proefdrukken wel bekijken in de proefdrukviewer.</p><p>Zie voor meer informatie over opmerkingen <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Opmerkingen over proefdrukken weergeven en beantwoorden</a>.</p></td> 
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
      <td>Workfront verzendt één e-mail met alle commentaren, antwoorden, en besluiten die slechts op dagen worden vermeld wanneer er naast uw activiteiten is.<p>Deze waarschuwing is een goede manier om een samenvatting van het project te zien zonder overweldigd met veelvoudige updates door de dag te worden.</p><p>Een voorbeeld gebruikt geval voor deze samenvatting is een afdelingsleider die de algemene vooruitgang van het project wil controleren.</p><p>Zie voor meer informatie <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Meldingen beheren voor proefopmerkingen en -beslissingen</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Geen e-mail</td> 
      <td>Workfront verzendt geen e-mailberichten.<br>Dit is nuttig voor een persoon die alleen ter referentie aan een bewijs wordt toegevoegd en niet van wijzigingen in kennis hoeft te worden gesteld.<p>Het systeemgebrek is Dagelijkse samenvatting (ook gezien als niet Geplaatst). Als u of uw controleurs geen andere wijzigingen aanbrengen, hebben al uw proefdrukken deze instelling.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Doorgaan met [E-mailinstellingen configureren voor de proefdruk](#configure-email-settings-for-the-proof) hieronder.

## E-mailinstellingen configureren voor de proefdruk {#configure-email-settings-for-the-proof}

1. In de **E-mailmelding** selecteert u of u e-mailmeldingen en een aangepast bericht wilt verzenden aan de gebruikers in [Een geavanceerde proefdruk maken met een standaardworkflow](#workflow) eerder in dit artikel :

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
        <li>Alleen gebruikers met Workfront-proefdrukken kunnen de proefdruk bekijken.</li>
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
        <li><strong>Abonnementenrol:</strong> De standaardproefdrukrol die wordt toegewezen aan alle revisoren die zich op de proefdruk abonneren. </li>
        <li><strong>Instellingen voor e-mailwaarschuwingen voor abonnees:</strong> De standaard e-mailwaarschuwing die wordt toegewezen aan alle revisoren die zich op de proefdruk abonneren.</li>
       </ul><p>
        <ul>
         <li><strong>Bewijs van toegang via e-mailkoppeling vereist voor:</strong> Configureer of de abonnee een e-mail ontvangt met een koppeling naar de proefdruk. U kunt <strong>Geen e-mail</strong> (E-mailkoppeling is niet vereist voor toegang tot de proefdruk), <strong>Alleen e-mail met verificatie</strong> (de abonnee ontvangt een koppeling naar de proefdruk via e-mail zonder verificatie), of <strong>E-mails over validatie en proefdrukken</strong> (de abonnee ontvangt een koppeling naar de proefdruk via e-mail en moet op de koppeling klikken om toegang te krijgen tot een proefdruk. Deze optie heeft tot doel ervoor te zorgen dat de persoon een correct e-mailadres heeft ingevoerd waartoe hij toegang heeft).</li>
        </ul><p>Opmerking: als de proefdrukken de automatische werkstroom hebben gekoppeld, worden alle abonnementen per e-mail verzonden met een bevestiging aan de eigenaar van de proefdrukken, zodat deze kan beslissen in welk stadium de persoon moet worden toegevoegd.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Proef maken**.

   Workfront begint met het genereren van een proefdruk van de geselecteerde documenten of websites. Afhankelijk van de bestandsgrootte en het type kan de vertraging bij het uploaden van een document variëren. Wees geduld, want het duurt langer om grotere bestanden te genereren. U kunt van de pagina weg navigeren en Workfront blijft uw bestand genereren. De maximale grootte voor het uploaden van bestanden is 4 GB.

1. Klik op **Proef openen** om de proefdrukviewer te starten.

   ![](assets/open-proof-350x132.png)

   Gebruikers die geen proefdrukken op hun account hebben ingeschakeld, kunnen het document nog steeds bekijken en opmerkingen naar de proefdruk maken.