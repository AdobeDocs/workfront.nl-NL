---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Een geautomatiseerde workflow maken of bewerken voor een bestaande proefdruk
description: Met geautomatiseerde workflows kunt u het revisieproces eenvoudiger beheren als uw proces complex is of als u regelmatig inhoud ter controle naar dezelfde groepen personen verzendt. Wanneer u een proef met een Geautomatiseerde Werkstroom creeert, beweegt de proef zich van stadium aan stadium tot definitieve goedkeuring. Deelnemers krijgen een melding wanneer het hun beurt is om het document te reviseren.
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 0%

---

# Een geautomatiseerde workflow maken of bewerken voor een bestaande proefdruk

Met geautomatiseerde workflows kunt u het revisieproces eenvoudiger beheren als uw proces complex is of als u regelmatig inhoud ter controle naar dezelfde groepen personen verzendt. Wanneer u een proef met een Geautomatiseerde Werkstroom creeert, beweegt de proef zich van stadium aan stadium tot definitieve goedkeuring. Deelnemers krijgen een melding wanneer het hun beurt is om het document te reviseren.

Voor informatie over het creëren van een Geautomatiseerde Workflow voor een nieuw bewijs, zie [Een geavanceerde proefdruk maken met een geautomatiseerde workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Huidig plan: Pro of hoger</p> <p>of</p> <p>Ouder plan: Premium</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Toegang tot proefdrukfunctionaliteit in Workfront</a>.</p> </td> 
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
   <td> <p>Toegang tot documenten bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de beheerder van de Workfront of Workfront-proefdrukken als u wilt weten welk plan, welke rol of welk proefdrukprofiel u hebt.

## Een geautomatiseerde workflow maken of bewerken voor een bestaande proefdruk:

1. Houd de muis boven het document in het gebied Documenten en klik vervolgens op Proofingworkflow.

   of

   Klik op **Workflow** ![](assets/workflow-icon-proofing-viewer.png) in het linkerpaneel, dan klik het Edit pictogram ![](assets/edit-icon-proofing-viewer.png) om de instellingen voor Geautomatiseerde workflow te openen voor de proefdruk.

1. (Voorwaardelijk) Als de proefdruk momenteel een basisworkflow gebruikt (zonder stadia), klikt u op **Omzetten in geautomatiseerde workflow** in het scherm dat wordt weergegeven.

   >[!NOTE]
   >
   >U kunt het eerste werkgebied niet bewerken wanneer u een standaardworkflow omzet in een geautomatiseerde workflow, maar u kunt wel nieuwe fasen toevoegen en configureren.

1. (Voorwaardelijk) om een Geautomatiseerde malplaatje van het Werkschema te gebruiken dat uw beheerder van Adobe Workfront creeerde en met u deelde, klik **Sjabloon toevoegen** selecteert u de sjabloon in het vak dat wordt weergegeven en klikt u vervolgens op **Sjabloon toevoegen**.

   Zie voor meer informatie [Informatie over het gebruik van automatische workflowsjablonen](#about-using-automated-workflow-templates) in dit artikel.

1. Een werkgebied toevoegen aan de automatische workflow:

   1. Klikken **Nieuwe fase** in de rechterbovenhoek.
   1. Typ in het vak dat wordt weergegeven een **Naam** voor het werkgebied.
   1. (Optioneel) Stel een deadline in voor het werkgebied.
   1. In de **Werkgebied activeren** in, kiest u hoe het werkgebied moet worden geactiveerd:


      <table>
      <tbody>
      <tr>
      <td><strong>Bij proefmaken</strong></td>
      <td>Het werkgebied wordt automatisch geactiveerd omdat de proefdruk al is gemaakt.</td>
      </tr>
      <tr>
      <td><strong>Wanneer de deadline van de vorige fase verstrijkt</strong></td>
      <td>Klik op het vorige werkgebied in het dialoogvenster <strong>Bovenliggend werkgebied</strong> vervolgkeuzelijst .</td>
      </tr>
      <tr>
      <td><strong>Op een specifieke datum en tijd</strong></td>
      <td>Klik op de knop <strong>Aan</strong> om de datum te selecteren en klik vervolgens op het vak rechts om de tijd te selecteren.</td>
      </tr>
      <tr>
      <td><strong>Alle beslissingen worden goedgekeurd of goedgekeurd met wijzigingen in het bovenliggende werkgebied</strong></td>
      <td>Klik op het bovenliggende werkgebied in het dialoogvenster <strong>Bovenliggend werkgebied</strong> vervolgkeuzelijst.</td>
      </tr>
      <tr>
      <td><strong>Alle besluiten worden goedgekeurd op ouderstadium</strong></td>
      <td>Klik op het bovenliggende werkgebied in het dialoogvenster <strong>Bovenliggend werkgebied</strong> vervolgkeuzelijst.</td>
      </tr>
      <tr>
      <td><strong>Alle besluiten worden genomen</strong></td>
      <td>Klik op het bovenliggende werkgebied in het dialoogvenster <strong>Bovenliggend werkgebied</strong> vervolgkeuzelijst.</td>
      </tr>
      </tbody>
      </table>


   1. Voer een naam of e-mailadres in en configureer instellingen voor controleurs voor het werkgebied.

      Voor informatie over het toevoegen van revisoren raadpleegt u [Revisoren toevoegen aan een werkgebied](#about-adding-reviewers-to-a-stage) in dit artikel.

   1. Gebruik een van de volgende opties om het werkgebied verder te configureren:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>Deadline-opties</strong> </td>
         <td><p>Als u een deadline voor het werkgebied wilt instellen, klikt u op een optie in het dialoogvenster <strong>Deadline-opties</strong> vervolgkeuzelijst. Vervolgens, onder <strong>Deadline</strong>Voer een van de volgende handelingen uit:</p>
          <ul>
           <li>Als u <strong>Specifieke datum instellen</strong>: Selecteer de gewenste datum en tijd van de deadline.</li>
           <li>Als u <strong>Berekenen vanaf de activeringsdatum van het werkgebied</strong>: Selecteer het aantal werkdagen dat u aan de activeringsdatum van het werkgebied wilt toevoegen om de deadline te bepalen.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Werkgebied vergrendelen</td>
         <td>Geef op wanneer het werkgebied kan worden vergrendeld. </td>
        </tr>
        <tr>
         <td role="rowheader">Primaire beslisser</td>
         <td><p>Selecteer de primaire beslisser in het werkgebied (alleen beschikbaar nadat u ten minste één persoon aan het werkgebied hebt toegevoegd die de rol van fiatteur of hoger heeft). Als u een primaire beslisser selecteert, wordt de <strong>Slechts één besluit vereist</strong> is uitgeschakeld in dit werkgebied.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Slechts één besluit vereist</td>
         <td>Beëindigt het hele herzieningsproces wanneer een van de besluitvormers een besluit neemt.<p>Deze optie is niet beschikbaar als u een gebruiker hebt aangewezen in het dialoogvenster <strong>Primaire beslisser</strong> vervolgkeuzemenu.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Privéstadium</td>
         <td>Hiermee kunnen alleen de volgende personen opmerkingen en beslissingen in deze fase bekijken: Supervisors, Adobe Workfront-beheerders en Workfront Proof-beheerders</td>
        </tr>
        <tr>
         <td role="rowheader">Personen per e-mail op de hoogte stellen</td>
         <td>Hiermee waarschuwt u revisoren met een e-mailmelding wanneer het hun beurt is om aan de proefdruk te werken.</td>
        </tr>
       </tbody>
      </table>

   1. Klikken **Werkgebied toevoegen**.

1. Herhaal desgewenst de vorige stap om meer stappen toe te voegen.

   Aangezien u stadia aan de Geautomatiseerde Werkschema toevoegt, vormt een diagram op het scherm om hen te vertegenwoordigen:

   ![](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. Wanneer u klaar bent met het toevoegen van fasen, klikt u op **Gereed**.

## Informatie over het gebruik van automatische workflowsjablonen {#about-using-automated-workflow-templates}

Overweeg het volgende wanneer u een Geautomatiseerde malplaatje van het Werkschema gebruikt:

1. De instellingen van een automatische werkstroomsjabloon bepalen wat u kunt doen met de geautomatiseerde workflow voor een proefdruk. Als de knop Een werkgebied toevoegen bijvoorbeeld is uitgeschakeld in de sjabloon, is deze niet zichtbaar wanneer u werkt met de instellingen voor Geautomatiseerde workflow voor de proefdruk.
1. Wanneer een persoon wordt toegevoegd aan een werkgebied in een Geautomatiseerde malplaatje van het Werkschema, maar ook reeds als recensent op het bewijs aanwezig is, verwijdert het toepassen van het malplaatje de recensent uit het stadium. Als u geen andere revisor aan het werkgebied toevoegt, wordt u in een bericht gevraagd een revisor toe te voegen.
1. Uw vermogen om een Geautomatiseerde malplaatje van het Werkschema te wijzigen hangt van de malplaatjemontages af die door de beheerder van Workfront worden gevormd, zoals die in wordt beschreven. Als de mogelijkheid om de sjabloon te wijzigen is uitgeschakeld, kan alleen de eigenaar van de sjabloon deze wijzigen.

## Revisoren toevoegen aan een werkgebied {#about-adding-reviewers-to-a-stage}

Houd rekening met het volgende wanneer u revisoren aan een werkgebied toevoegt:

* Nadat u een gebruiker aan een stadium toevoegt, kunt u montages voor die gebruiker op de proef vormen, zoals de proefdrukrol en om het even welke extra toestemmingen zij zouden moeten hebben en het type e-mailalarm zij zullen ontvangen wanneer de mensen commentaren en besluiten over de proef maken.
* U kunt een of meer gebruikers van het ene werkgebied naar het andere slepen. U kunt gebruikers rechtstreeks naar een ander werkgebied slepen of u kunt gebruikers naar een werkgebied in het **Staven** diagram. Druk op Shift+Ctrl (Windows) of Shift+Command (Mac) om meerdere gebruikers te selecteren.
* U kunt een controleur slechts eenmaal aan een proefdruk toevoegen, wat betekent dat u dezelfde persoon niet aan meer dan één werkgebied kunt toevoegen op de proefdruk.
* Revisoren die niet aan een privéfase zijn toegevoegd, kunnen dat stadium niet zien op de proefdruk of de opmerkingen die in dat stadium zijn gemaakt.
* Door gebrek, verleent het toevoegen van een gebruiker aan een stadium die gebruiker toegang om de proef van het ogenblik te bekijken de proef wordt gecreeerd.

   Uw Workfront-beheerder kan gebruikers de toegang tot de proefdruk beperken tot de werkstroom het werkgebied ingaat waar de gebruiker is toegevoegd. Zie voor meer informatie in .
