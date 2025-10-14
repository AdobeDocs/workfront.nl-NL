---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Een proefdruk delen in Adobe Workfront
description: U kunt een proefdocument delen in Adobe Workfront door het document te delen of door gebruikers aan de proefdruk toe te voegen.
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: aaf5beb8692b2fdbb797ba908796d78b4ee8866c
workflow-type: tm+mt
source-wordcount: '1231'
ht-degree: 0%

---

# Een proefdruk delen in Adobe Workfront

U kunt een proefdocument delen in Adobe Workfront door het document te delen of door gebruikers aan de proefdruk toe te voegen.

Als u de proefdruk deelt, zoals in dit artikel wordt uitgelegd, heeft de ontvanger dezelfde toegang tot het document en de proefdruk. Bovendien kunt u de ontvanger om goedkeuring vragen voor het bewijs.

>[!TIP]
>
>U kunt ook een proefdruk delen vanuit de proefdrukviewer. Voor instructies, zie [&#x200B; een proef van de het proef kijker &#x200B;](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md) delen.

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
   <td role="rowheader">Rol proefdrukken</td> 
   <td>Auteur of moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, rol, of Profiel van de Toestemming van het Bewijs u hebt, contacteer uw beheerder van Workfront of van Workfront Proof.

+++

## Een proefdrukkoppeling delen

Als u een proefdrukkoppeling deelt, kunnen Workfront-gebruikers toegang bekijken. Gebruikers kunnen opmerkingen maken over de proefdruk en zich abonneren op e-mailmeldingen voor de proefdruk met hun aanmeldingsgegevens voor Workfront. Gebruikers die geen proef maken, kunnen opmerkingen maken en zich abonneren met een e-mailadres en weergavenaam.

>[!IMPORTANT]
>
>De instelling Delen van proefdrukken via een openbare URL of code insluiten moet zijn ingeschakeld.

1. Selecteer het document dat de proefdruk bevat die u met gebruikers wilt delen.

   U kunt slechts één document selecteren. U kunt de koppeling voor meerdere documenten niet tegelijkertijd delen.

1. Klik **Aandeel** > **Verbinding van het Bewijs**.
1. In de **verbinding van het Bewijs** doos die verschijnt, doe één van beiden van het volgende:

   * Om de verbinding aan uw klembord te kopiëren, klik **verbinding van het Exemplaar**.

     U kunt de koppeling nu distribueren via een hulpprogramma van derden, zoals een chat of een e-mailtoepassing.

   * Ga als volgt te werk om de koppeling rechtstreeks vanuit Adobe Workfront te e-mailen:

      1. In het **of e-mailverbinding aan** gebied, begin typend en selecteer de naam van uw ontvanger. Of geef het e-mailadres op van een externe gebruiker met wie u wilt delen.

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
            <td><p>Bevat een knop in het e-mailbericht waarmee gebruikers naar de proefdruk worden geleid in de kijker die ze controleren en waarmee ze toegang krijgen tot de weergave.</p><p>Als <strong> aan bewijs via openbare URL of inbedt code </strong> wordt toegelaten voor de proef, kunnen de gebruikers binnen met hun login van Workfront geloofsbrieven ondertekenen om commentaren aan de proef toe te voegen. Als deze optie is ingeschakeld, kan iedereen die zijn e-mailadres en naam (geen wachtwoord vereist) opgeeft, ondertekenen en opmerkingen toevoegen aan de proefdruk.</p></td>
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

      1. Klik **verzenden**.

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
>* Als Geautomatiseerde workflow is ingeschakeld en u een gebruiker toevoegt aan de proefdruk die geen proefdrukken heeft in Workfront, wordt een nieuw werkgebied gemaakt in de Geautomatiseerde workflow. De gebruiker die u toevoegt, wordt automatisch toegevoegd aan dit nieuwe werkgebied wanneer deze de proefdruk voor het eerst weergeeft. (Voor meer informatie, zie [&#x200B; Geautomatiseerd Overzicht van het Werkschema &#x200B;](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).)
>

### Gebruikers toevoegen aan een bestaande proefdruk via het tabblad Documenten

1. Selecteer het document met de proefdruk waaraan u gebruikers wilt toevoegen.
1. Als de proef geen geautomatiseerd werkschema (stadia) heeft, klik het **Meer** pictogram in de hoger-juiste hoek van Stadium 1 sectie, dan klik **Aandeel** in het drop-down menu.

   of

   Als de proef een Geautomatiseerd Werkschema heeft, klik het **Meer** pictogram in de hoger-juiste hoek van het stadium waar u de recensent wilt toevoegen, dan **Aandeel** in het drop-down menu klikken.

1. In het **Aandeel deze versie** doos die, onder **Aandeel** verschijnt, begint typend de naam of het e-mailadres van een gebruiker die u de proef met wilt delen, dan klik de naam wanneer het in de drop-down lijst verschijnt.

1. (Optioneel) Herhaal deze stap om meerdere gebruikers aan de proefdruk toe te voegen.
1. (Optioneel) Stel een deadline in voor de controleurs.
1. (Facultatief) zorg ervoor **mensen door e-mail** op de hoogte brengt wordt geselecteerd als u de recensenten wilt laten weten u hen aan de proef hebt toegevoegd.
1. (Facultatief) **voeg een douanebericht** aan e-mail toe.
1. Wanneer u alle recensenten hebt toegevoegd, klik **Aandeel**.

### Gebruikers aan een bestaande proefdruk toevoegen vanuit de proefdrukviewer

U kunt gebruikers aan een proefdruk toevoegen terwijl u een proef in de Kijker van het Keuren van het Web en in de Kijker van het Proofing van de Desktop bekijkt.

Voor meer informatie, zie [&#x200B; een proef delen door gebruikers aan het &#x200B;](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) in het artikel [&#x200B; toe te voegen Deel een bewijs van de het proef kijker &#x200B;](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## Verslag over goedkeuringen voor proefdrukken

U kunt een rapport maken dat rapporten weergeeft over de proefdrukgoedkeuringen die in Workfront zijn gedeeld. Dit rapport bevat de volgende informatie over de proefdrukgoedkeuring in uw systeem:

* Document dat ter goedkeuring is ingediend
* Naam van de fiatteur
* Proefversie
* Proef-id
* Aanmaakdatum proefdrukken

U hebt toegang tot deze goedkeuring wanneer het creëren van een rapport dat op een voorwerp wordt gebaseerd, zoals die in [&#x200B; wordt beschreven creeer een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Voor meer informatie over het Proef keurt objecten rapport goed, zie het [&#x200B; Rapport over voorwerpen &#x200B;](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) sectie in [&#x200B; voorwerpen in Adobe Workfront &#x200B;](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) begrijpen

## Een gedeelde proefdruk goedkeuren

Wanneer een gebruiker u aan een proef toevoegt en of de rol Fiatteur of Reviewer &amp; Approver gebruikend Geautomatiseerde Workflow verleent, toont het goedkeuringsverzoek in Mijn widget Goedkeuringen in het gebied van het Huis. Vervolgens kunt u het bewijs bekijken en rechtstreeks vanuit Workfront een goedkeuringsbesluit nemen over het bewijs.

Voor informatie over hoe te om goedkeuringsbesluiten van Mijn widget goedkeurt te nemen, zie [&#x200B; werk van het gebied van het Huis &#x200B;](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) goedkeuren of [&#x200B; werk &#x200B;](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) in [&#x200B; goedkeurend werk &#x200B;](../../../review-and-approve-work/manage-approvals/approving-work.md).
