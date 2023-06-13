---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Een proefdruk delen in Adobe Workfront
description: U kunt een proefdocument delen in Adobe Workfront door het document te delen of door gebruikers aan de proefdruk toe te voegen.
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: 5c0cd18074cffdf0a4fe15affaf61add7314a83a
workflow-type: tm+mt
source-wordcount: '1221'
ht-degree: 0%

---

# Een proefdruk delen in Adobe Workfront

U kunt een proefdocument delen in Adobe Workfront door het document te delen of door gebruikers aan de proefdruk toe te voegen.

Als u de proefdruk deelt, zoals in dit artikel wordt uitgelegd, heeft de ontvanger dezelfde toegang tot het document en de proefdruk. Bovendien kunt u de ontvanger om goedkeuring vragen voor het bewijs.

>[!TIP]
>
>U kunt ook een proef delen vanuit de testviewer. Zie voor instructies [Een proefdruk delen vanuit de proefdrukviewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

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
   <td role="rowheader">Rol proefdrukken</td> 
   <td>Auteur of moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de beheerder van de Workfront of Workfront-proefdrukken als u wilt weten welk plan, welke rol of welk proefdrukprofiel u hebt.

## Een proefdrukkoppeling delen

Als u een proefdrukkoppeling deelt, kunnen Workfront-gebruikers toegang bekijken. Gebruikers kunnen opmerkingen maken over de proefdruk en zich abonneren op e-mailmeldingen voor de proefdruk met hun aanmeldingsgegevens voor Workfront. Gebruikers die geen proef maken, kunnen opmerkingen maken en zich abonneren met een e-mailadres en weergavenaam.

>[!IMPORTANT]
>
>De instelling Delen van proefdrukken via een openbare URL of code insluiten moet zijn ingeschakeld.

1. Selecteer het document dat de proefdruk bevat die u met gebruikers wilt delen.

   U kunt slechts één document selecteren. U kunt de koppeling voor meerdere documenten niet tegelijkertijd delen.

1. Klikken **Delen** > **Koppeling proefdrukken**.
1. In de **Koppeling proefdrukken** Voer een van de volgende handelingen uit in het vak dat wordt weergegeven:

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

## Gebruikers aan een proefdruk toevoegen

U kunt elke Workfront-gebruiker aan de proefdruk toevoegen als u bewerkingsrechten hebt op de proefdruk. Als de proefdruk meerdere fasen heeft, voegt u de gebruiker aan een afzonderlijk werkgebied toe

>[!WARNING]
>
>Naast de methoden die in dit artikel worden vermeld, is het mogelijk gebruikers aan een proef toe te voegen door hen in een commentaar van het lusje van Updates van een bestaande proef te etiketteren. Gebruikers die op deze manier aan een proefdruk zijn toegevoegd, ontvangen echter geen e-mailbericht tenzij ze opnieuw worden gelabeld nadat ze aan de proefdrukworkflow zijn toegevoegd.
>
>Daarom raden we u aan gebruikers aan een proefdruk toe te voegen aan de hand van een van de onderstaande methoden, en niet door ze in een opmerking te labelen.
>

>[!NOTE]
>
>Houd rekening met het volgende als u een verouderd Workfront-plan gebruikt waarin proefdrukken voor een gebruiker kan worden in- en uitgeschakeld:
>
>* De ontvangers hoeven geen proef te hebben toegelaten om de proef te herzien.
>* Als Geautomatiseerde workflow is ingeschakeld en u een gebruiker toevoegt aan de proefdruk die geen proefdrukken heeft in Workfront, wordt een nieuw werkgebied gemaakt in de Geautomatiseerde workflow. De gebruiker die u toevoegt, wordt automatisch toegevoegd aan dit nieuwe werkgebied wanneer deze de proefdruk voor het eerst weergeeft. (Zie voor meer informatie [Geautomatiseerd workflowoverzicht](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).)
>

### Gebruikers toevoegen aan een bestaande proefdruk via het tabblad Documenten

1. Selecteer het document met de proefdruk waaraan u gebruikers wilt toevoegen.
1. Als de proefdruk geen geautomatiseerde workflow (stadia) heeft, klikt u op de knop **Meer** in de rechterbovenhoek van de sectie Stage 1, klikt u op **Delen** in het vervolgkeuzemenu.

   of

   Als de proefdruk wel een geautomatiseerde workflow heeft, klikt u op de knop **Meer** in de rechterbovenhoek van het werkgebied waar u de revisor wilt toevoegen, klikt u op **Delen** in het vervolgkeuzemenu.

1. In de **Deze versie delen** vak dat wordt weergegeven onder **Delen** typt u eerst de naam of het e-mailadres van de gebruiker met wie u de proefdruk wilt delen. Klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.

1. (Optioneel) Herhaal deze stap om meerdere gebruikers aan de proefdruk toe te voegen.
1. (Optioneel) Stel een deadline in voor de controleurs.
1. (Optioneel) Controleer of **Personen per e-mail op de hoogte stellen** is geselecteerd als u wilt dat de controleurs weten dat u ze aan de proefdruk hebt toegevoegd.
1. (Optioneel) **Een aangepast bericht toevoegen** naar de e-mail.
1. Als u alle revisoren hebt toegevoegd, klikt u op **Delen**.

### Gebruikers aan een bestaande proefdruk toevoegen vanuit de proefdrukviewer

U kunt gebruikers aan een proefdruk toevoegen terwijl u een proef in de Kijker van het Keuren van het Web en in de Kijker van het Proofing van de Desktop bekijkt.

Zie voor meer informatie [Een proefdruk delen door er gebruikers aan toe te voegen](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) in het artikel [Een proefdruk delen vanuit de proefdrukviewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## Verslag over goedkeuringen voor proefdrukken

U kunt een rapport maken dat rapporten weergeeft over de proefdrukgoedkeuringen die in Workfront zijn gedeeld. Dit rapport bevat de volgende informatie over de proefdrukgoedkeuring in uw systeem:

* Document dat ter goedkeuring is ingediend
* Naam van de fiatteur
* Proefversie
* Proef-id
* Aanmaakdatum proefdrukken

U hebt toegang tot deze goedkeuring wanneer u een rapport maakt dat is gebaseerd op een object, zoals wordt beschreven in [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Voor meer informatie over het rapport van het object Goedkeuringen proef raadpleegt u de [Objecten rapporteren](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) sectie in [Objecten in Adobe Workfront begrijpen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)

## Een gedeelde proefdruk goedkeuren

Wanneer een gebruiker u aan een proef toevoegt en of de rol Fiatteur of Reviewer &amp; Approver gebruikend Geautomatiseerde Workflow verleent, toont het goedkeuringsverzoek op het lusje van Goedkeuringen in uw Huis of Mijn Gebied van het Werk. Vervolgens kunt u het bewijs bekijken en rechtstreeks vanuit Workfront een goedkeuringsbesluit nemen.

Voor informatie over hoe te om goedkeuringsbesluiten van het Mijn gebied van het Werk te nemen, zie [Werk goedkeuren vanuit het thuisgebied](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) of [Goedkeuring van de werkzaamheden](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) in [Goedkeuring van de werkzaamheden](../../../review-and-approve-work/manage-approvals/approving-work.md).
