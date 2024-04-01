---
title: Voorbeeld van het verbinden van recordtypen en records
description: In dit artikel wordt een voorbeeld beschreven van hoe u een verbinding kunt maken tussen een recordtype voor Adobe Workfornt Planning en een Workfront-projectobjecttype. Het beschrijft ook hoe u een verslag van de Planning van Workfront met een individueel project kunt verbinden.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 38509572-72a4-4fce-b3ec-2cb31bb4669a
source-git-commit: e54142e189cd4f407161401203a7f13c752ad404
workflow-type: tm+mt
source-wordcount: '1771'
ht-degree: 0%

---

# Voorbeeld van het verbinden van recordtypen en records

{{maestro-important-intro}}

In dit artikel wordt een voorbeeld van het volgende beschreven:

* Hoe te om een verbinding tussen twee het verslagtypes van de Planning van Workfront en twee verslagen tot stand te brengen.

* Hoe te om een verbinding tussen een het verslagtype van de Planning van Workfront en een het projectobjecten van Workfront, evenals een verbinding tussen een verslag en een project tot stand te brengen.

Zie ook de volgende artikelen voor meer informatie:

* [Verbind recordtypen](../architecture/connect-record-types.md)
* [Connect-records](../records/connect-records.md)

## Twee Workfront-recordtypen en -records verbinden (voorbeeld)

U hebt bijvoorbeeld een recordtype met de naam Campaign als oorspronkelijk recordtype.

U hebt ook een ander recordtype, Product genaamd, dat een valutaveld heeft, Budget.

U wilt een gebied op het verslagtype van Campagne tot stand brengen waar u de waarden van het gebied van de Begroting van het verslagtype Product kunt tonen.

Dit doet u als volgt:

1. Open de tabelweergave voor het recordtype Campagne in een werkruimte.
1. Klik op de knop **+** in de rechterbovenhoek van de tabelweergave om een nieuw veld toe te voegen, klikt u vervolgens op **Nieuwe verbinding** en klik vervolgens op **Product** in de geselecteerde sectie Werkruimte.
1. Voeg bijvoorbeeld de volgende informatie toe:

   * **Recordtype**: Product <!--did they change the casing here?-->
   * **Naam**: Geef het nieuwe veld een naam. Bijvoorbeeld &quot;Productinformatie.&quot; Dit is de naam van het gekoppelde recordveld.
   * **Beschrijving**: Voeg een beschrijving toe voor het nieuwe veld. Bijvoorbeeld, &quot;Dit zijn de Producten die ik mijn campagnes verbonden aan wil.&quot; De beschrijving van het veld wordt weergegeven wanneer u de muisaanwijzer op het veld in de kolomkop plaatst.
   * **Meerdere records toestaan**: Als u deze optie ingeschakeld laat, kunnen gebruikers meerdere records selecteren wanneer het veld voor het gekoppelde recordtype (Productinformatie) in de oorspronkelijke records (campagnes) wordt weergegeven. In ons geval kunnen gebruikers meerdere producten selecteren voor verbinding met één campagne.
   * **Opzoekvelden selecteren**: Als u deze optie ingeschakeld laat, worden de **Opzoekvelden toevoegen** wordt geopend als u productvelden wilt koppelen aan het type Campagne-record. U kunt op **Overslaan** om deze stap over te slaan en productvelden later toe te voegen.

   ![](assets/new-connection-with-product-record-type.png)

1. (Voorwaardelijk) Als u de optie **Optie Opzoekvelden selecteren** in de vorige stap, uit de lijst van gebieden verbonden aan **Product** recordtype, klikt u op de knop **+** pictogram voor de **Begroting** veld, klik vervolgens op **Velden toevoegen**. Hiermee maakt u een veld met de naam **Begroting (op basis van productinformatie)**, de naam van het gekoppelde veld. Alle informatie voor het productbudget wordt in dit veld weergegeven voor de campagnebestanden.

   ![](assets/add-fields-for-budget-field-for-connector-with-record-type.png)

   >[!TIP]
   >
   >    Als u de begroting van alle geselecteerde producten als één totaal aantal wilt bekijken, selecteer **SUM** in het vervolgkeuzemenu rechts van de veldnaam. Wanneer gebruikers meerdere producten selecteren in het dialoogvenster **Productinformatie** gekoppeld recordveld, **Begroting (op basis van productinformatie)** worden alle begrotingswaarden bij elkaar opgeteld en wordt het totaal weergegeven. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Als u **Geen**, in plaats van **SUM** De afzonderlijke budgetten van de geselecteerde producten worden gescheiden door komma&#39;s.

   Hiermee worden de volgende velden gegenereerd:

   * In de de lijstmening van het verslag van de Campagne en in de verslagpagina van de Campagne van een campagne:

      * **Productinformatie** (het gekoppelde recordveld): hiermee worden de naam of namen van de producten weergegeven wanneer u deze toevoegt.
      * **Begroting (op basis van productinformatie)** (het daaraan gekoppelde veld): Hiermee worden de budgetten van de op het gebied van productinformatie geselecteerde producten weergegeven.

   * In de tabelweergave met productrecord en op de pagina met productrecords van een product:

      * **Campagne**: Dit geeft aan dat het recordtype Product is gekoppeld vanuit het recordtype Campagne.

     ![](assets/example-campaign-information-relationship-fields-from-product-record-table.png)

   >[!TIP]
   >
   >    Gekoppelde recordvelden worden voorafgegaan door het relatiepictogram ![](assets/relationship-field-icon.png).

1. Van de **Campagne** recordtype, maak een campagne door een nieuwe rij toe te voegen in de lijst van het type van verslagpagina van de Campagne.

1. Dubbelklik in het dialoogvenster  **Productinformatie** kolom van de nieuwe campagne .

   ![](assets/connect-other-records-smaller-box-in-table-view.png)

1. Voer een van de volgende handelingen uit:

   * Klik in de lijst op de naam van een verbonden product om dit aan de geselecteerde record toe te voegen. Het product wordt automatisch toegevoegd.
   * Typ de naam van een product en klik erop wanneer het in de lijst wordt weergegeven. Het product wordt automatisch toegevoegd.
   * Klikken **Alles bekijken** om alle producten weer te geven.

1. (Voorwaardelijk) Als u hebt geklikt **Alles bekijken** in de vorige stap **Objecten verbinden** wordt weergegeven.

   ![](assets/connected-objects-table-for-records.png)

1. Typ de naam van een product in het zoekvak en selecteer het product wanneer het in de lijst wordt weergegeven

   of

   Selecteer de productrecords die u wilt koppelen aan de Campagne-records en klik vervolgens op **Objecten verbinden**.

   >[!TIP]
   >
   >    U kunt de verslagpagina van een Campagne openen, het verbonden verslaggebied vinden en klikken **+** in het veld om producten van het type productrecord toe te voegen.

   De volgende kolommen worden bevolkt in de lijst van het het verslagtype van de Campagne:
   * De **Productinformatie** wordt voor de campagnerecord gevuld met de geselecteerde producten.
   * **De begroting (op basis van productinformatie)** wordt gevuld met de begrotingswaarde voor elk geselecteerd product of met een totaal van alle budgetten van de geselecteerde producten (als u SUM hebt geselecteerd voor uw aggregator).

   ![](assets/example-product-information-and-budget-relationship-fields-for-campaign-record-table.png)

   >[!TIP]
   >
   >Wanneer u geen aggregator selecteert voor de meerdere waarden, worden alle waarden van de geselecteerde producten weergegeven, gescheiden door komma&#39;s.

1. Als u de **Campagne** veld van de **Product** de lijstmening, herhaalt stappen 5-7 die van de het verslagtype van het Product lijstmening beginnen en campagneinformatie selecteren. Hiermee werkt u ook het veld Productinformatie in de tabel met recordtypen voor campagne bij. <!--ensure the step numbers remain correct-->


## Een Workfront-planningrecordtype verbinden met een Workfront-projectobjecttype en een record verbinden met afzonderlijke projecten

U hebt bijvoorbeeld een recordtype met de naam Campaign als oorspronkelijk recordtype.

U hebt ook projecten in Workfront met een gebied genoemd &quot;Geplande Inkomsten.&quot;

U wilt een verbindingsgebied op het verslagtype van Campagne tot stand brengen waar u de waarden van het Geplande gebied van Inkomsten van de projecten in Workfront kunt tonen die met campagnes in de Planning van Workfront worden verbonden.

Dit doet u als volgt:

1. Ga naar een Workspace waar u het type Campagne-record wilt koppelen aan Workfront-projecten.
1. Open de tabelweergave voor het type Campagnerecord in de geselecteerde werkruimte.
1. Klik op de knop **+** in de rechterbovenhoek van de tabelweergave om een nieuw veld toe te voegen, klikt u vervolgens op **Nieuwe verbinding** en klik vervolgens op **Project** in de **Workfront-objecttypen** sectie.
1. Voeg bijvoorbeeld de volgende informatie toe:

   * **Recordtype**: Project (van de subsectie Workfront)
   * **Naam**: Geef het nieuwe veld een naam, bijvoorbeeld &quot;Projectinformatie&quot;.
   * **Beschrijving**: Voeg een beschrijving toe voor het nieuwe veld. Bijvoorbeeld: &quot;Dit zijn de projecten waaraan ik mijn campagnes wil koppelen.&quot; De beschrijving wordt weergegeven in de tabelweergave terwijl u de muisaanwijzer op de veldnaam in de kolomkop plaatst.
   * 
      * **Meerdere records toestaan**: Als u deze optie ingeschakeld laat, kunnen gebruikers meerdere projecten selecteren wanneer het veld voor het gekoppelde projecttype (projectinformatie) wordt weergegeven in de oorspronkelijke records (campagnes).
   * **Opzoekvelden selecteren**: Als u deze optie ingeschakeld laat, worden de **Opzoekvelden toevoegen** wordt nu geopend, zodat u de projectvelden kunt koppelen aan het type Campagne-record. U kunt op **Overslaan** om deze stap over te slaan en later projectvelden toe te voegen.

   ![](assets/new-connection-tab-with-workfront-option.png)

1. (Voorwaardelijk) Als u de optie **Optie Opzoekvelden selecteren** in de vorige stap, uit de lijst van gebieden verbonden aan **Project** objecttype, klik op de knop **+** pictogram voor de **Geplande inkomsten** veld, klik vervolgens op **Velden toevoegen**. Hiermee maakt u een veld met de naam **Geplande inkomsten (uit projectinformatie)**, de naam van het gekoppelde veld. Alle informatie uit het veld Geplande inkomsten van project wordt automatisch in dit veld weergegeven voor de campagnebestanden.

   >[!TIP]
   >
   >    Als u de geplande inkomsten van alle geselecteerde projecten wilt weergeven als één totaal getal, selecteert u **SUM** in het vervolgkeuzemenu rechts van de veldnaam. Wanneer de gebruikers veelvoudige projecten in selecteren **Projectinformatie** gekoppeld objectveld, het **Geplande inkomsten (uit productinformatie)** worden alle waarden bij elkaar opgeteld en wordt het totaal weergegeven. <!-- check the shot below - added a bug with a couple of UI changes here-->
   >
   > Als u **Geen**, in plaats van **SUM**, worden de afzonderlijke geplande inkomsten aangegeven met komma&#39;s.

   ![](assets/add-planned-revenue-project-field-to-new-connection.png)

   Hiermee worden de volgende velden gegenereerd:

   * In de de lijstmening van het verslag van de Campagne en in de de verslagpagina van de Campagne:

      * **Projectinformatie** (het veld voor het gekoppelde object): hiermee worden de naam of namen van de projecten weergegeven.
      * **Geplande inkomsten (uit projectinformatie)** (het daaraan gekoppelde veld): Hierin worden de geplande opbrengsten van de geselecteerde projecten in het veld Projectinformatie weergegeven.

   >[!TIP]
   >
   >    Gekoppelde objectvelden worden voorafgegaan door het relatiepictogram ![](assets/relationship-field-icon.png).

1. Van de **Campagne** een tabelweergave met recordtype maken, een campagne maken door een nieuwe rij in de tabel toe te voegen.

1. Dubbelklik in het dialoogvenster  **Projectinformatie** kolom van de nieuwe campagne .

   ![](assets/connect-projects-smaller-box-in-table.png)

1. Voer een van de volgende handelingen uit:

   * Klik in de lijst op de naam van een project om het toe te voegen aan de geselecteerde record. Het project wordt automatisch toegevoegd.
   * Typ de naam van een project en klik erop wanneer het in de lijst wordt weergegeven. Het project wordt automatisch toegevoegd.
   * Klikken **Alles bekijken** om alle projecten weer te geven.

1. (Voorwaardelijk) Als u hebt geklikt **Alles bekijken** in de vorige stap **Objecten verbinden** wordt weergegeven.

   ![](assets/connect-projects-larger-box.png)

1. Typ de naam van een project in het zoekvak en selecteer het vervolgens wanneer het in de lijst wordt weergegeven

   of

   Selecteer de projectverslagen u met de verslagen van de Campagne wilt verbinden, dan klik **Objecten verbinden**.

   >[!TIP]
   >
   >    U kunt de pagina van een Campagne openen, het verbonden projectgebied vinden en klikken **+** pictogram in het gebied om projecten van het aangesloten verslagtype van het Product toe te voegen.

   Hiermee voegt u het volgende toe aan de geselecteerde werkruimte:

   * In de lijst van het type van verslag van de Campagne:
      * De **Projectinformatie** wordt voor de campagnerecord gevuld met de geselecteerde projecten.
      * De **Geplande inkomsten (uit productinformatie)** wordt gevuld met de begrotingswaarde voor elk geselecteerd product. Dit is een alleen-lezen veld.

   ![](assets/project-linked-field-and-planned-revenue-in-campaign-table-highlighted.png)

   >[!TIP]
   >
   >Wanneer u geen aggregator selecteert voor de meerdere waarden en u meerdere objecten selecteert in het veld voor objectgekoppelde velden, worden alle waarden gescheiden door komma&#39;s weergegeven.

1. Klik de naam van een project op het verbonden verslaggebied.

   Dit opent de read-only pagina van het Project van de Planning van Woekfront.
Informatie over het project controleren. Alleen geselecteerde projectvelden worden weergegeven op de pagina van de record.

1. Klikken **Ga naar bron** in de hoger-juiste hoek van het scherm om het project in Workfront te openen, als u minstens de toestemmingen van de Mening aan het project hebt.
1. (Optioneel) Werk informatie over het project in Workfront bij als u hiervoor gemachtigd bent.

1. (Optioneel) Houd de muisaanwijzer in de tabelweergave Campagne boven de **Projectinformatie** veldkoptekst en klik op de pijl omlaag gericht en klik vervolgens op **Opzoekvelden bewerken.**
1. Klik op de knop **+** pictogram voor om het even welke projectgebieden u aan het verslag van de Planning van Workfront van het Project in wilt toevoegen **Niet-geselecteerde velden** sectie.
1. Klik op de knop **-** pictogram voor om het even welke projectgebieden u uit het verslag van de Planning van het Project van Workfront in wilt verwijderen **Geselecteerde velden** sectie.
1. Klikken **Opslaan**.

   Er worden extra gekoppelde velden toegevoegd aan het type Campagne-record.
