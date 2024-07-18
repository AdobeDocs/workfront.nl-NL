---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: Opstelling een proef met een Geautomatiseerde Werkschema in  [!DNL Workfront Proof]
description: Dit herhaalt informatie die in het Vormen van proef in Workfront wordt gevonden. Consolideer hier of daar. Misschien beter hier.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 605569df-8e63-476d-a0cd-e73802042011
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1522'
ht-degree: 0%

---

# Een proefdruk instellen met behulp van een geautomatiseerde workflow in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [ het Bewijzen ](../../../review-and-approve-work/proofing/proofing.md).

Dankzij de geautomatiseerde workflow kunt u de controle en goedkeuring van inhoud gemakkelijker beheren wanneer u complexe revisieprocessen hebt of wanneer u inhoud ter controle regelmatig naar dezelfde groepen personen verzendt.

Als u de proefdruk maakt, gaat deze van het werkgebied naar het werkgebied totdat de eindgoedkeuring is verkregen. De relevante gebruikers worden op elk moment dat zij een goedkeuring moeten verlenen, op de hoogte gebracht.

![ stage_diagram.png ](assets/stages-diagram-350x81.png)

U kunt een geautomatiseerde workflow aan een proefdruk toevoegen tijdens het uploaden van het document of nadat het document is geüpload.

## Een proefdruk maken met Geautomatiseerde workflow

1. Maak de proefdruk.
1. Klik in de sectie **[!UICONTROL Share]** op **[!UICONTROL Use Automated Workflow]** .

   U kunt deze optie deselecteren om terug te schakelen naar een standaardworkflow.

1. (Optioneel) Als u een automatische werkstroomsjabloon wilt gebruiken die de [!DNL Workfront] -beheerder heeft geconfigureerd en met u heeft gedeeld, selecteert u deze in de vervolgkeuzelijst **[!UICONTROL Select a Workflow template]** .

   >[!NOTE]
   >
   >Uw mogelijkheid om de sjabloon te wijzigen, is afhankelijk van de sjablooninstellingen die door de [!DNL Workfront] -beheerder zijn geconfigureerd. Als de mogelijkheid om de sjabloon te wijzigen is uitgeschakeld, kan alleen de eigenaar van de sjabloon deze wijzigen.

1. Geef de volgende informatie op om de eerste fase van de geautomatiseerde workflow te configureren:

   * **[!UICONTROL Name]:** De werkgebiednaam wordt weergegeven in het werkstroomdiagram en is opgenomen in de e-mailmeldingen die naar revisoren worden verzonden.
   * **[!UICONTROL Deadline]:** de functionaliteit van dit gebied verschilt afhankelijk van welke optie u in de **[!UICONTROL Deadline calculated from]** drop-down lijst selecteert.

   * **[!UICONTROL From proof creation]:** selecteer de deadline voor de proefdruk.
   * **[!UICONTROL From stage activation]:** selecteer het aantal werkdagen dat wordt toegevoegd aan de datum van activering van het werkgebied om automatisch een deadline voor de proefdruk in te stellen.
   * **[!UICONTROL Activate stage]:** Voor elke fase van uw workflow kunt u bepalen wanneer deze moet worden geactiveerd. Voor de eerste fase zijn de volgende opties beschikbaar.

      * Bij proefmaken
      * Op een bepaald tijdstip en een bepaalde datum
      * Handmatig\

        Er zijn aanvullende opties beschikbaar voor volgende fasen. Voor deze opties is een bovenliggende fase vereist. Het zijn:
      * Na vorige deadline is bereikt
      * Alle beslissingen worden goedgekeurd of goedgekeurd met wijzigingen
      * Alle beslissingen worden goedgekeurd
      * Alle beslissingen worden genomen
   * **[!UICONTROL Deadline calculated from]:** de optie die u in deze vervolgkeuzelijst selecteert, bepaalt welke opties beschikbaar zijn in het veld **[!UICONTROL Deadline]** .

   * **[!UICONTROL Proof creation]:** Selecteer in het veld **[!UICONTROL Deadline]** de deadline voor de proefdruk.

   * **[!UICONTROL Stage activation]:** Selecteer in het veld **[!UICONTROL Deadline]** het aantal werkdagen dat wordt toegevoegd aan de activeringsdatum van het werkgebied om automatisch een deadline voor de proefdruk in te stellen.

   * **[!UICONTROL Lock stage]:** selecteer wanneer het werkgebied kan worden vergrendeld.
   * **[!UICONTROL Primary decision maker]:** selecteer de Primaire besluitvormer op het stadium. De besluitvormers zijn beschikbaar in de drop-down lijst slechts nadat u recensenten aan het stadium toevoegt.
   * **[!UICONTROL Only one decision required]:** selecteer deze optie als u de revisie wilt voltooien nadat een van de besluitvormers zijn beslissing heeft genomen.\

     Deze optie is niet beschikbaar als u een gebruiker hebt aangewezen in het vervolgkeuzemenu **[!UICONTROL Primary decision maker]** .

   * **[!UICONTROL Private stage]:** wanneer deze optie wordt geselecteerd, zijn de commentaren en de besluiten niet zichtbaar aan mensen die niet aan dit stadium worden toegevoegd of geen supervisors, Beheerders, of de Beheerders van de Facturering in de rekening zijn


1. (Optioneel) Voeg revisoren toe aan het werkgebied.
1. Houd rekening met het volgende wanneer u revisoren toevoegt:

   * Een controleur kan slechts eenmaal aan een proefdruk worden toegevoegd. (U kunt dezelfde persoon niet aan meerdere etappes toevoegen op de proefdruk.)
   * Revisoren die aan een privéfase zijn toegevoegd, kunnen alleen het werkgebied zien waaraan ze zijn toegevoegd op de proefdruk en de opmerkingen die in dat werkgebied zijn gemaakt.
   * Door gebrek, verleent het toevoegen van een gebruiker aan een stadium die gebruiker toegang om de proef van het ogenblik te bekijken de proef wordt gecreeerd.\

     De systeembeheerder kan het proefdruksysteem zodanig configureren dat gebruikers geen toegang hebben tot de proefdrukproef totdat de werkstroom het werkgebied bereikt waar de gebruiker is toegevoegd. Zie voor meer informatie

1. (Optioneel) Klik op **[!UICONTROL New stage]** en herhaal vervolgens Stap 4 en Stap 5 om meerdere fasen aan de geautomatiseerde workflow toe te voegen.
1. Ga door met het maken van de proefdruk door de benodigde informatie op te geven in de secties [!UICONTROL Organize] en [!UICONTROL More settings] op de pagina [!UICONTROL New Proof] , zoals beschreven in

## Geautomatiseerde workflowdiagrammen

Tijdens het instellen van de workflow voor de proefdruk zult u zien dat er een diagram wordt gemaakt. Elk stadium u aan uw proef toevoegt zal in het diagram verschijnen, duidelijk wijzend op de gebiedsdelen tussen de stadia. Privéfasen worden gemarkeerd met een sleutelpictogram.

Het diagram zweeft, wat betekent dat het zichtbaar blijft, zelfs als u de pagina omlaag schuift.

Als u niet het diagram te hoeven zien, kunt u het verbergen (1).

![ Diagram.png ](assets/diagram-350x93.png)

## Een werkgebied toevoegen

U kunt een extra werkgebied toevoegen aan een werkstroom u creeert of wijzigt.

1. Als u een stadium aan een bestaand bewijs toevoegt, ga naar de de detailpagina van het Bewijs, zoals die op [ wordt beschreven beheert de Details van het Bewijs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Klik in de sectie **[!UICONTROL Workflow]** op **[!UICONTROL New stage]** .

1. Geef informatie voor het werkgebied op, zoals in stap 4 onder de sectie [!UICONTROL Creating a Proof with an Automated Workflow] in dit artikel.
1. Klik op **[!UICONTROL Add stage]** en vervolgens op **[!UICONTROL Done]** .

## Een werkgebied verwijderen

1. Klik op het prullenbakpictogram in de rechterbovenhoek van het werkgebied (1).\
   Het pictogram wordt weergegeven wanneer u de muisaanwijzer op het werkgebied plaatst.\
   ![ het schrappen_a_stage.png ](assets/deleting-a-stage-350x250.png)

## Werkgebiedinstellingen

* **[!UICONTROL Stage name]**: wordt weergegeven in het workflowdiagram en is opgenomen in de e-mailmeldingen die worden verzonden aan revisoren.
* **[!UICONTROL Activate stage]**: Voor elke fase van uw workflow kunt u bepalen wanneer deze moet worden geactiveerd. Voor de eerste fase zijn de volgende opties beschikbaar:

   * Bij proefmaken
   * Op een bepaald tijdstip en een bepaalde datum
   * Handmatig
   * Alleen deze drie opties zijn beschikbaar voor de eerste fase. De andere opties worden beschikbaar wanneer u een tweede fase toevoegt. Hiervoor moet u een bovenliggend werkgebied selecteren.
   * Nadat de vorige deadline is bereikt (moet u een bovenliggende fase kiezen)
   * Alle beslissingen zijn goedgekeurd of [!UICONTROL Approved with changes] (vereist dat u een hoofdwerkgebied selecteert)
   * Alle beslissingen zijn goedgekeurd (hiervoor moet een bovenliggende fase worden gekozen)
   * Alle beslissingen worden genomen (hiervoor moet een bovenliggende fase worden gekozen)

* **[!UICONTROL Deadline]:** U kunt bepalen hoe de deadline voor elke fase van een workflow moet worden berekend. De opties zijn:

   * Van het aanmaken van een proefdruk: in het veld [!UICONTROL deadline] (9) kunt u de deadline voor de proefdruk selecteren.
   * Vanuit werkgebiedactivering: in het vervolgkeuzemenu [!UICONTROL deadline] selecteert u het aantal werkdagen dat wordt toegevoegd aan de activeringsdatum van het werkgebied om automatisch een deadline voor de proefdruk in te stellen.

* **[!UICONTROL Lock]:** Er zijn een aantal opties die bepalen wanneer een werkgebied kan worden vergrendeld. De volgende opties zijn beschikbaar:

   * Handmatige vergrendeling
   * Nooit
   * Wanneer het volgende werkgebied begint
   * Wanneer alle beslissingen worden genomen

**[!UICONTROL Primary decision maker]**: U stelt de primaire beslisser in het werkgebied in. De beschikbare besluitvormers worden pas in de lijst weergegeven nadat u de revisoren aan het werkgebied hebt toegevoegd.

>[!NOTE]
>
>Als u een primaire besluitvormer kiest, is er in dit stadium niet meer slechts één vereiste optie voor een beslissing beschikbaar.

* **[!UICONTROL Only one decision required]**: u kunt deze optie in een werkgebied inschakelen. Dit betekent dat de herziening zal worden afgerond zodra een van de besluitvormers zijn besluit neemt.
* **[!UICONTROL Privacy]:** Elke fase kan privé worden gemaakt. Als een werkgebied privé is, zijn de opmerkingen en beslissingen niet zichtbaar voor personen die niet aan dit werkgebied zijn toegevoegd of die geen toezichthouders, beheerders of factureringsbeheerders in het account zijn. Voor meer informatie, zie [ Geautomatiseerd Overzicht van het Werkschema ](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Revisoren toevoegen aan een werkgebied

1. Voer een naam of e-mailadres in het veld onder aan elk werkgebied in.
1. Klik op het groene plusteken om deze toe te voegen.
1. De rol op de proefdruk instellen.
1. Stel de e-mailwaarschuwing in.
1. Bij het instellen van de eerste fase kunt u ook de eigenaar van de proefdruk wijzigen.

   >[!NOTE]
   >
   >* Een controleur kan slechts eenmaal aan een proefdruk worden toegevoegd. U kunt dezelfde persoon niet aan meer dan één fase op de proefdruk toevoegen.
   >* Revisoren die niet aan een privéfase zijn toegevoegd, kunnen het werkgebied niet zien op de proefdruk of opmerkingen die in dat stadium zijn gemaakt.


## Een proefdruk converteren naar een geautomatiseerde workflow

U kunt een standaardproefdruk naar Geautomatiseerde Werkstroom omzetten.

1. Klik op **[!UICONTROL Convert to Automated Workflow]** op de pagina [!UICONTROL Proof details] .
Nadat de proefdruk is omgezet in een geautomatiseerde workflow, zijn alle fasen actief en openbaar. De optie [!UICONTROL Lock stage] is standaard ingesteld op Handmatig. Alle stadia blijven bij gebruikers en hun instellingen.

   * Het werkgebied activeren is ingesteld op Bij maken van proefdrukken in elke fase.
   * De deadline die wordt berekend op basis van de optie wordt ingesteld op het maken van het bewijs in elke fase.
   * Als op het basisbewijs slechts één beslissingsoptie is geselecteerd, wordt deze in alle stadia geselecteerd.
   * Als er geen proefdruk [!UICONTROL Primary decision maker] is geselecteerd, worden de stappen met die ontvanger ingesteld op Geen en wordt voor alle andere proefdrukken ingesteld op Geen.
   * Werkgebiednaam blijft ongewijzigd.

## Een extra sjabloon toevoegen aan een bestaande automatische workflow

Nadat een standaardproefdruk in Geautomatiseerde Werkschema wordt omgezet, kunt u extra malplaatje aan het toevoegen.

1. Klik op de pagina Proefdrukgegevens in de sectie Workflow op **[!UICONTROL Add template].**

   * De montages van het malplaatje bepalen wat met een proef kan worden gedaan waaraan dit malplaatje werd toegevoegd. Als de [!UICONTROL Add a stage and Add people to stages] -opties voor de sjabloon bijvoorbeeld uitgeschakeld zijn, zijn de knoppen [!UICONTROL add stage] en [!UICONTROL share proof] niet zichtbaar.
   * Als [!UICONTROL Add a stage option] is uitgeschakeld in de opgegeven sjabloon, is de knop [!UICONTROL Add template] niet zichtbaar nadat u deze hebt toegevoegd.
   * Wanneer een persoon aan een stadium in een Geautomatiseerd malplaatje van het Werkschema wordt toegevoegd, maar ook reeds aanwezig op het bewijs toen als dit malplaatje wordt toegepast, zal het systeem deze persoon automatisch uit het stadium verwijderen. Als er verder niemand aan dit specifieke werkgebied wordt toegevoegd, wordt de volgende fout weergegeven omdat het systeem het toevoegen van een leeg werkgebied aan de workflow niet toestaat.

     ![ error_when_adding_template.png ](assets/error-when-adding-template-350x66.png)
