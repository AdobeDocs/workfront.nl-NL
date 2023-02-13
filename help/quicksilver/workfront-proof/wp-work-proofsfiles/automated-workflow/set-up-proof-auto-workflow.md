---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: Stel een proefdruk in met een geautomatiseerde workflow in [!DNL Workfront Proof]
description: Dit herhaalt informatie die in het Vormen van proef in Workfront wordt gevonden. Consolideer hier of daar. Misschien beter hier.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 605569df-8e63-476d-a0cd-e73802042011
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1522'
ht-degree: 0%

---

# Stel een proefdruk in met een geautomatiseerde workflow in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Dankzij de geautomatiseerde workflow kunt u de controle en goedkeuring van inhoud gemakkelijker beheren wanneer u complexe revisieprocessen hebt of wanneer u inhoud ter controle regelmatig naar dezelfde groepen personen verzendt.

Als u de proefdruk maakt, gaat deze van het werkgebied naar het werkgebied totdat de eindgoedkeuring is verkregen. De relevante gebruikers worden op elk moment dat zij een goedkeuring moeten verlenen, op de hoogte gebracht.

![stappen_diagram.png](assets/stages-diagram-350x81.png)

U kunt een geautomatiseerde workflow aan een proefdruk toevoegen tijdens het uploaden van het document of nadat het document is geüpload.

## Een proefdruk maken met Geautomatiseerde workflow

1. Maak de proefdruk.
1. In de **[!UICONTROL Share]** sectie, klikt u op **[!UICONTROL Use Automated Workflow]**.

   U kunt deze optie deselecteren om terug te schakelen naar een standaardworkflow.

1. (Optioneel) Als u een geautomatiseerde workflow-sjabloon wilt gebruiken die [!DNL Workfront] beheerder gevormd en met u gedeeld, selecteer het in **[!UICONTROL Select a Workflow template]** vervolgkeuzemenu.

   >[!NOTE]
   >
   >Uw vermogen om het malplaatje te wijzigen hangt van de malplaatjemontages af die door worden gevormd [!DNL Workfront] beheerder. Als de mogelijkheid om de sjabloon te wijzigen is uitgeschakeld, kan alleen de eigenaar van de sjabloon deze wijzigen.

1. Geef de volgende informatie op om de eerste fase van de geautomatiseerde workflow te configureren:

   * **[!UICONTROL Name]:** De naam van het werkgebied wordt weergegeven in het workflowdiagram en is opgenomen in de e-mailmeldingen die worden verzonden aan revisoren.
   * **[!UICONTROL Deadline]:** De functionaliteit van dit veld is afhankelijk van de optie die u in het dialoogvenster **[!UICONTROL Deadline calculated from]** vervolgkeuzelijst.

   * **[!UICONTROL From proof creation]:** Selecteer de uiterste datum voor het bewijs.
   * **[!UICONTROL From stage activation]:** Selecteer het aantal werkdagen dat wordt toegevoegd aan de activeringsdatum van het werkgebied om automatisch een deadline voor de proefdruk in te stellen.
   * **[!UICONTROL Activate stage]:** Voor elke fase van uw workflow kunt u bepalen wanneer deze moet worden geactiveerd. Voor de eerste fase zijn de volgende opties beschikbaar.

      * Bij proefmaken
      * Op een bepaald tijdstip en een bepaalde datum
      * Handmatig\

         Er zijn aanvullende opties beschikbaar voor volgende fasen. Voor deze opties is een hoofdwerkgebied vereist. Het zijn:
      * Wanneer de vorige deadline is bereikt
      * Alle beslissingen worden goedgekeurd of goedgekeurd met wijzigingen
      * Alle besluiten worden goedgekeurd
      * Alle besluiten worden genomen
   * **[!UICONTROL Deadline calculated from]:** De optie die u in deze vervolgkeuzelijst selecteert, bepaalt welke opties beschikbaar zijn in het dialoogvenster **[!UICONTROL Deadline]** veld.

   * **[!UICONTROL Proof creation]:** In de **[!UICONTROL Deadline]** de uiterste datum voor het bewijs te selecteren.

   * **[!UICONTROL Stage activation]:** In de **[!UICONTROL Deadline]** selecteert u het aantal werkdagen dat wordt toegevoegd aan de activeringsdatum van het werkgebied om automatisch een deadline voor de proefdruk in te stellen.

   * **[!UICONTROL Lock stage]:** Selecteer wanneer het werkgebied kan worden vergrendeld.
   * **[!UICONTROL Primary decision maker]:** Selecteer de primaire besluitvormer in het werkgebied. De besluitvormers zijn beschikbaar in de drop-down lijst slechts nadat u recensenten aan het stadium toevoegt.
   * **[!UICONTROL Only one decision required]:** Selecteer deze optie om de revisie te voltooien nadat een van de besluitvormers zijn beslissing heeft genomen.\

      Deze optie is niet beschikbaar als u een gebruiker hebt aangewezen in het dialoogvenster **[!UICONTROL Primary decision maker]** vervolgkeuzemenu.

   * **[!UICONTROL Private stage]:** Als deze optie is geselecteerd, zijn opmerkingen en beslissingen niet zichtbaar voor personen die niet aan dit werkgebied zijn toegevoegd of die geen toezichthouder, beheerder of factuuradbeheerder in de account zijn


1. (Optioneel) Voeg revisoren toe aan het werkgebied.
1. Houd rekening met het volgende wanneer u revisoren toevoegt:

   * Een controleur kan slechts eenmaal aan een proefdruk worden toegevoegd. (U kunt dezelfde persoon niet aan meerdere etappes toevoegen op de proefdruk.)
   * Revisoren die aan een privéfase zijn toegevoegd, kunnen alleen het werkgebied zien waaraan ze zijn toegevoegd op de proefdruk en de opmerkingen die in dat werkgebied zijn gemaakt.
   * Door gebrek, verleent het toevoegen van een gebruiker aan een stadium die gebruiker toegang om de proef van het ogenblik te bekijken de proef wordt gecreeerd.\

      De systeembeheerder kan het proefdruksysteem zodanig configureren dat gebruikers geen toegang hebben tot de proefdrukproef totdat de werkstroom het werkgebied bereikt waar de gebruiker is toegevoegd. Zie voor meer informatie

1. (Optioneel) Klik op **[!UICONTROL New stage]** Herhaal vervolgens Stap 4 en Stap 5 om meerdere fasen aan de geautomatiseerde workflow toe te voegen.
1. Ga door met het maken van de proefdruk door de benodigde informatie op te geven in het dialoogvenster [!UICONTROL Organize] en [!UICONTROL More settings] secties over de [!UICONTROL New Proof] pagina, zoals beschreven in

## Geautomatiseerde workflowdiagrammen

Tijdens het instellen van de workflow voor de proefdruk zult u zien dat er een diagram wordt gemaakt. Elk stadium u aan uw proef toevoegt zal in het diagram verschijnen, duidelijk wijzend op de gebiedsdelen tussen de stadia. Privéfasen worden gemarkeerd met een sleutelpictogram.

Het diagram zweeft, wat betekent dat het zichtbaar blijft, zelfs als u de pagina omlaag schuift.

Als u niet het diagram te hoeven zien, kunt u het verbergen (1).

![Figuur.png](assets/diagram-350x93.png)

## Een werkgebied toevoegen

U kunt een extra werkgebied toevoegen aan een werkstroom u creeert of wijzigt.

1. Als u een werkgebied aan een bestaande proefdruk toevoegt, gaat u naar de pagina Proefgegevens, zoals beschreven op [Proofinggegevens beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. In de **[!UICONTROL Workflow]** sectie, klikt u op **[!UICONTROL New stage]**.

1. Geef informatie op voor het werkgebied zoals in stap 4 van de [!UICONTROL Creating a Proof with an Automated Workflow] in dit artikel.
1. Klikken **[!UICONTROL Add stage]** en klik vervolgens op **[!UICONTROL Done]**.

## Een werkgebied verwijderen

1. Klik op het prullenbakpictogram in de rechterbovenhoek van het werkgebied (1).\
   Het pictogram wordt weergegeven wanneer u de cursor op het werkgebied plaatst.\
   ![delete_a_stage.png](assets/deleting-a-stage-350x250.png)

## Werkgebiedinstellingen

* **[!UICONTROL Stage name]**: Wordt weergegeven in het workflowdiagram en is opgenomen in de e-mailmeldingen die worden verzonden aan revisoren.
* **[!UICONTROL Activate stage]**: Voor elke fase van uw workflow kunt u bepalen wanneer deze moet worden geactiveerd. Voor de eerste fase zijn de volgende opties beschikbaar:

   * Bij proefmaken
   * Op een bepaald tijdstip en een bepaalde datum
   * Handmatig
   * Alleen deze drie opties zijn beschikbaar voor de eerste fase. De andere opties worden beschikbaar wanneer u een tweede fase toevoegt. hiervoor moet u een hoofdwerkgebied selecteren.
   * Nadat de vorige deadline is bereikt (moet u een bovenliggende fase kiezen)
   * Alle besluiten zijn goedgekeurd of [!UICONTROL Approved with changes] (vereist het selecteren van een hoofdwerkgebied)
   * Alle beslissingen zijn goedgekeurd (hiervoor moet een bovenliggende fase worden gekozen)
   * Alle beslissingen worden genomen (hiervoor moet een bovenliggende fase worden gekozen)

* **[!UICONTROL Deadline]:** U kunt bepalen hoe de deadline moet worden berekend voor elke fase van een workflow. De opties zijn:

   * Van aanmaak van proefdrukken: In de [!UICONTROL deadline] in veld 9 kunt u de uiterste datum voor de proefdruk selecteren.
   * Vanaf activering van werkgebied: In de [!UICONTROL deadline] in het vervolgkeuzemenu selecteert u het aantal werkdagen dat wordt toegevoegd aan de activeringsdatum van het werkgebied om automatisch een deadline voor de proefdruk in te stellen.

* **[!UICONTROL Lock]:** Er zijn een aantal opties die bepalen wanneer een werkgebied kan worden vergrendeld. U kunt onder andere de volgende opties kiezen:

   * Handmatige vergrendeling
   * Nooit
   * Wanneer het volgende werkgebied begint
   * Wanneer alle beslissingen worden genomen

**[!UICONTROL Primary decision maker]**: U stelt de primaire beslisser in het werkgebied in. De beschikbare besluitvormers worden pas in de lijst weergegeven nadat u de controleurs aan het werkgebied hebt toegevoegd.

>[!NOTE]
>
>Als u een primaire besluitvormer kiest, is slechts één vereiste optie niet meer beschikbaar in dit stadium.

* **[!UICONTROL Only one decision required]**: U kunt deze optie inschakelen in een werkgebied. Dit betekent dat de herziening zal worden afgerond zodra een van de besluitvormers zijn besluit neemt.
* **[!UICONTROL Privacy]:** Elke fase kan privé worden gemaakt. Als een stadium privé is, zullen de commentaren en de besluiten niet zichtbaar aan mensen zijn die niet aan dit stadium worden toegevoegd of geen supervisors, Beheerders of de Beheerders van de Facturering in de rekening zijn. Zie voor meer informatie [Geautomatiseerd workflowoverzicht](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md) .

## Revisoren toevoegen aan een werkgebied

1. Voer een naam of e-mailadres in het veld onder aan elk werkgebied in.
1. Klik op het groene plusteken om deze toe te voegen.
1. De rol op de proefdruk instellen.
1. Stel de e-mailwaarschuwing in.
1. Bij het instellen van de eerste fase kunt u ook de eigenaar van de proefdruk wijzigen.

   >[!NOTE]
   >
   >* Een controleur kan slechts eenmaal aan een proefdruk worden toegevoegd. U kunt niet dezelfde persoon aan meerdere etappes toevoegen op de proefdruk.
   >* Revisoren die niet aan een privéfase zijn toegevoegd, kunnen het werkgebied niet zien op de proefdruk of opmerkingen die in dat stadium zijn gemaakt.



## Een proefdruk converteren naar een geautomatiseerde workflow

U kunt een standaardproefdruk naar Geautomatiseerde Werkstroom omzetten.

1. Klik op **[!UICONTROL Convert to Automated Workflow]** op de pagina [!UICONTROL Proof details].
Nadat het bewijs aan Geautomatiseerde Werkschema wordt herwerkt, zijn alle stadia actief, openbaar en hun [!UICONTROL Lock stage] Deze optie is standaard ingesteld op Handmatig. Alle stadia blijven bij gebruikers en hun montages.

   * Het werkgebied activeren is ingesteld op Bij proefdrukken in elk werkgebied.
   * De termijn die van optie wordt berekend wordt geplaatst aan Aanmaakproef in elk stadium.
   * Als slechts één beslissingsoptie op het basisbewijs is geselecteerd, wordt deze in alle stadia geselecteerd.
   * Indien een basisbewijs [!UICONTROL Primary decision maker] is geselecteerd, worden de fasen met die ontvanger op hen geplaatst en alle andere hebben het geplaatst aan niets.
   * De naam van het werkgebied blijft ongewijzigd.

## Voeg een extra malplaatje aan een bestaand Geautomatiseerd Werkschema toe

Nadat een basisproef in Geautomatiseerde Werkschema wordt omgezet, kunt u extra malplaatje aan het toevoegen.

1. Klik in de sectie Workflow van de pagina Proefgegevens op **[!UICONTROL Add template].**

   * De montages van het malplaatje bepalen wat met een proef kan worden gedaan waaraan dit malplaatje werd toegevoegd. Als de sjabloon bijvoorbeeld het volgende bevat: [!UICONTROL Add a stage and Add people to stages] opties uitgeschakeld, knoppen naar [!UICONTROL add stage] en [!UICONTROL share proof] is niet zichtbaar.
   * Indien [!UICONTROL Add a stage option] is uitgeschakeld in de opgegeven sjabloon nadat u deze hebt toegevoegd aan de [!UICONTROL Add template] zijn niet zichtbaar.
   * Wanneer een persoon aan een stadium in een Geautomatiseerd malplaatje van het Werkschema wordt toegevoegd, maar ook reeds aanwezig op het bewijs toen als dit malplaatje wordt toegepast, zal het systeem deze persoon automatisch uit het stadium verwijderen. Als er verder niemand aan dit specifieke werkgebied wordt toegevoegd, wordt de volgende fout weergegeven omdat het systeem het toevoegen van een leeg werkgebied aan de workflow niet toestaat.

      ![error_when_adding_template.png](assets/error-when-adding-template-350x66.png)
