---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Een proefdruk delen vanuit de proefdrukviewer
description: U kunt een proefdruk delen vanuit de proefdrukviewer als delen is ingeschakeld door de eigenaar of maker van de proefdruk.
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1512'
ht-degree: 0%

---

# Een proefdruk delen vanuit de proefdrukviewer

U kunt een proefdruk delen vanuit de proefdrukviewer als delen is ingeschakeld door de eigenaar of maker van de proefdruk.

>[!IMPORTANT]
>
>De instelling Delen van proefdrukken via een openbare URL of code insluiten moet zijn ingeschakeld.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Huidig plan: Pro of hoger</p> <p>of</p> <p>Ouder plan: Selecteren of Premium</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Toegang tot proefdrukfunctionaliteit in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Huidig plan: Werken of plannen</p> <p>Ouder plan: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>Manager of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de beheerder van de Workfront of Workfront-proefdrukken als u wilt weten welk plan, welke rol of welk proefdrukprofiel u hebt.

## De URL delen

U kunt een proef via een URL delen als de eigenaar de proef voor het delen heeft gevormd. Eigenaars van proefdrukken kunnen instellingen voor delen op elk gewenst moment bijwerken. Zie voor meer informatie [Proefdrukinstellingen bewerken](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

1. Als het linkerpictogrammenu niet wordt weergegeven, klikt u op de knop **Menu** in de linkerbovenhoek van de proefdrukviewer.

   ![](assets/menu-icon-in-proofing-viewer-350x188.png)

1. Klik in het linkerpictogrammenu van de proefdrukviewer op de knop **Delen** pictogram.

   ![Share_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. In de **Proef delen** opties die worden weergegeven, controleert u of **Share-able-koppeling ophalen** is geselecteerd.

1.  Voer een van de volgende handelingen uit:

   * Als u de koppeling naar het klembord wilt kopiëren, klikt u op **Koppeling kopiëren**.

      U kunt de koppeling nu distribueren via een hulpprogramma van derden, zoals een chat of een e-mailtoepassing.

   * Ga als volgt te werk om de koppeling rechtstreeks vanuit Adobe Workfront te e-mailen:

      1. In de **Of e-mailkoppeling naar** -veld, begint u te typen en selecteert u de naam van de ontvanger. Of geef het e-mailadres op van een externe gebruiker met wie u wilt delen.

         >[!NOTE]
         >
         >Als u een alias-e-mail ziet tijdens het delen van een proefdruk, maak dan geen nieuwe gastgebruiker door de originele e-mail in te voeren als een overeenkomstige alias-e-mail bestaat.

      1. Selecteer een van de volgende opties:

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">Openbare koppeling verzenden</td>
            <td><p>Bevat een knop in het e-mailbericht waarmee gebruikers naar de proefdruk worden geleid in de kijker die ze controleren en waarmee ze toegang krijgen tot de weergave.</p><p>Indien <strong>Abonneren op bewijs via openbare URL of insluitcode</strong> is uitgeschakeld voor de proefdruk, kunnen gebruikers zich aanmelden met hun aanmeldingsgegevens voor Workfront om opmerkingen toe te voegen aan de proefdruk. Als deze optie is ingeschakeld, kan iedereen die zijn e-mailadres en naam (geen wachtwoord vereist) opgeeft, ondertekenen en opmerkingen toevoegen aan de proefdruk.</p></td>
           </tr>
           <tr>
            <td role="rowheader">Download-koppeling verzenden</td>
            <td>Bevat een knop in het e-mailbericht waarmee gebruikers naar een downloadpagina worden geleid. Deze knop bevat de bestandsgegevens, de bestandsnaam en de bestandsgrootte, waarbij het bestand inline wordt weergegeven. Gebruikers kunnen vanaf de downloadpagina op de koppeling Downloaden klikken om het bestand te downloaden.</td>
           </tr>
           <tr>
            <td role="rowheader">Aangepast bericht toevoegen</td>
            <td>Hiermee kunt u een aangepast onderwerp en een aangepaste tekst voor de e-mailmelding opgeven.</td>
           </tr>
          </tbody>
         </table>

      1. Klikken **Verzenden**.

         De ontvangers ontvangen een e-mailbericht met informatie over de proefdruk en de knoppen die u wilt opnemen.

         ![](assets/proof-share-email-350x87.png)

## De insluitcode delen

U kunt een proef via insluitcode delen als de proefbesteller het voor dit heeft gevormd.

Een proefdruk delen via de insluitcode:

1. Klik op de werkbalk links van de proefdrukviewer op de knop **Delen** pictogram.

   ![Share_btn_in_viewer__1_.png](assets/share-btn-in-viewer--1-.png)

1. In de **Proef delen** opties die worden weergegeven, klikt u op **Insluitcode ophalen** en klik vervolgens op **Kopiëren**.

## Een proefdruk delen door er gebruikers aan toe te voegen

U kunt gebruikers aan een proef toevoegen terwijl het herzien van een proef als u om het even welke volgende toestemmingen hebt:

* Supervisor- of beheerdersmachtigingen
* Beheerdersmachtigingen en u bent de maker of eigenaar van de proefdrukken
* De toestemmingen van de manager met de de proefdrukrol van de Auteur of van de Moderator

Als de proefdruk een Geautomatiseerde Werkstroom heeft, kunt u de gebruiker aan een individueel stadium toevoegen. Zie voor meer informatie [Geautomatiseerd workflowoverzicht](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Standaard voegen gebruikers die u toevoegt aan de proefdruk:

* U ontvangt een e-mailbericht met een koppeling naar de proefdruk.
* Kan goedkeuringsbesluiten nemen op het bewijs van het Huis of Mijn Gebied van het Werk, zoals beschreven in [Goedkeuring van de werkzaamheden](../../../../review-and-approve-work/manage-approvals/approving-work.md).
* U hoeft geen proefdrukken in te schakelen om de proefdruk te kunnen controleren.

Als Geautomatiseerde workflow is ingeschakeld en u een gebruiker toevoegt aan de proefdruk die geen proefdrukken heeft in Workfront, wordt een nieuw werkgebied gemaakt in de Geautomatiseerde workflow. De gebruiker die u toevoegt, wordt automatisch toegevoegd aan dit nieuwe werkgebied wanneer deze de proefdruk voor het eerst weergeeft. Zie voor meer informatie [Geautomatiseerd workflowoverzicht](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

Een proefdruk delen met individuele gebruikers:

1. Klik op de werkbalk links van de proefdrukviewer op de knop **Delen** pictogram.

   ![Share_btn_in_viewer__2_.png](assets/share-btn-in-viewer--2-.png)

1. Klikken **Ontvangers toevoegen** in de lijst links.
1. Onder **Nieuwe ontvangers voor bewijs** typt u eerst de naam van de gebruiker met wie u de proefdruk wilt delen. Klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.
1. (Optioneel) Wijzig de revisieopties rechts van de naam van de persoon:

   * **Proefdrukrol**: Zie voor meer informatie [Proefdrukrollen beheren in Workfront-proefdrukken](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

   * **Werkgebied**: (Alleen beschikbaar als de proefdruk een geautomatiseerde workflow heeft). Zie voor meer informatie  [Overzicht van geautomatiseerde werkstroomfasen](../../../../review-and-approve-work/proofing/proofing-overview/stages.md).

   * **E-mailwaarschuwingen**: Selecteer een van de volgende opties om op te geven hoe de persoon op de hoogte wordt gesteld van activiteiten op de proefdruk.

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
        <td>Een e-mail wordt alleen naar de controleur verzonden als iemand uitdrukkelijk op zijn opmerking reageert (dit sluit zijn eigen reacties op zijn eigen opmerkingen uit). Dit betekent dat als iemand op het bewijs een nieuwe opmerking maakt, de controleur niet op de hoogte wordt gesteld.<p>Deze instelling wordt aanbevolen voor uw klanten op de proefdruk, zodat zij geen andere opmerkingen over de proefdruk ontvangen en alleen op de hoogte worden gesteld van antwoorden op hun eigen opmerkingen.</p><p>Hoewel revisoren met deze instelling voor e-mailwaarschuwingen geen melding krijgen van andere nieuwe opmerkingen, kunnen ze alle opmerkingen over de proefdrukken wel bekijken in de proefdrukviewer.</p><p>Zie voor meer informatie over opmerkingen <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Opmerkingen over proefdrukken weergeven en beantwoorden</a>.</p></td> 
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
        <td>Workfront verzendt één e-mail met alle commentaren, antwoorden, en besluiten die slechts op dagen worden vermeld wanneer er naast uw activiteiten is.<p>Deze waarschuwing is een goede manier om een samenvatting van het project te zien zonder overweldigd met veelvoudige updates door de dag te worden.</p><p>Een voorbeeld gebruikt geval voor deze samenvatting is een afdelingsleider die de algemene vooruitgang van het project wil controleren.</p><p>Zie voor meer informatie <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Meldingen beheren voor proefopmerkingen en -beslissingen</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Geen e-mail</td> 
        <td>Workfront verzendt geen e-mailberichten.<br>Dit is nuttig voor een persoon die alleen ter referentie aan een bewijs wordt toegevoegd en niet van wijzigingen in kennis hoeft te worden gesteld.<p>Het systeemgebrek is Dagelijkse samenvatting (ook gezien als niet Geplaatst). Als u of uw controleurs geen andere wijzigingen aanbrengen, hebben al uw proefdrukken deze instelling.</p></td> 
       </tr> 
      </tbody> 
     </table>

1. (Optioneel) Herhaal de twee vorige stappen om meerdere gebruikers aan de proefdruk toe te voegen. 
1. (Optioneel) Stel een **Deadline** voor de controleurs (alleen beschikbaar als de proefdruk geen geautomatiseerde workflow heeft).
1. (Optioneel) Selecteer **E-mailbericht verzenden naar nieuwe ontvangers** om hen te laten weten dat u ze aan het bewijs hebt toegevoegd.
1. Als u klaar bent met het toevoegen van gebruikers aan de proefdruk, klikt u op **Gereed.**
