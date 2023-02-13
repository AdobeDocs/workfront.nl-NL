---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,trap-start,kickstart,trap-start
navigation-topic: use-kick-starts
title: 'Kick-start scenario: Aangepaste velden met meerdere opties importeren in Workfront'
description: U kunt aangepaste velden met meerdere opties in Adobe Workfront importeren met de functie Kick-Start.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 80ad604330e8b55037f1607b754cc8bb34f6a3ec
workflow-type: tm+mt
source-wordcount: '2126'
ht-degree: 0%

---


# Kick-Starts-scenario: Aangepaste velden met meerdere opties importeren in Workfront

U kunt aangepaste velden met meerdere opties in Adobe Workfront importeren met de functie Kick-Start.

Voorbeelden van aangepaste velden met meerdere opties zijn:

* Vervolgkeuzelijst met meerdere selecties
* Vervolgkeuzelijst
* Selectievakjes
* Keuzerondjes

Deze velden kunnen soms veel (soms honderden) opties bevatten. Als u ze importeert met de functie Kick-Start, kunt u als Workfront-beheerder veel tijd besparen en fouten voorkomen.

>[!IMPORTANT]
>
>U moet de stappen volgen die in de onderstaande secties worden beschreven, in deze volgorde, om aangepaste velden met meerdere opties te importeren met behulp van een trap-start:
>
>1. Bestaande aangepaste gegevens exporteren uit Workfront (optionele stap)
>1. Het snelstartsjabloon exporteren voor aangepaste gegevens
>1. Piek Excel Kick-Begint spreadsheet
>1. Het Excel-werkblad uploaden naar Workfront



## Bestaande aangepaste gegevens exporteren uit Workfront (optionele stap)

Als u niet bekend bent met de Workfront-databasestructuur of als u niet bekend bent met het bestand voor startende bestanden dat Workfront nodig heeft om informatie te importeren, raden we u aan eerst een bestand met startende informatie uit Workfront te exporteren, vergelijkbaar met de velden die u wilt importeren.

Als u bijvoorbeeld aangepaste formulieren of aangepaste velden wilt importeren, moet u eerst een bestand met een beginnaam exporteren met bestaande aangepaste gegevens.

Wanneer u bestaande gegevens exporteert, kunt u deze eerst scannen en zien hoe de nieuwe gegevens moeten worden opgemaakt.

Als u de Workfront-databaseobjecten en -structuur goed begrijpt, kunt u verdergaan met de onderstaande sectie.

Bestaande gegevens exporteren uit Workfront:

1. Klikken **Hoofdmenu > Instellen** in de rechterbovenhoek van de Workfront-interface.
1. Breid uit **Systeem** links, klikt u op **Gegevens exporteren (Kick-start)**.

   ![](assets/export-data-kick-starts-link-in-setup.png)

1. Selecteren **Aangepaste gegevens** in de **Wat moet u opnemen?** sectie.

   ![](assets/existing-custom-data-box-checked-kick-starts.png)

1. Kies **.xlsx-bestand** in de **Downloadindeling** sectie.

   >[!TIP]
   >
   >    Afhankelijk van hoeveel aangepaste gegevens u in uw systeem hebt, kan dit lang duren.

   ![](assets/download-button-for-kick-starts.png)

1. Klikken **Downloaden**. Een .xlsx-bestand wordt naar de computer gedownload. Navigeer naar en open het.

   ![](assets/existing-data-excel-parameter-sheet.png)

1. Onderzoek het gedownloade dossier en neem nota van de volgende details:

   * Het bestand bevat verschillende bladen. Mogelijk hoeft u de informatie op elk blad niet op de hoogte te zijn, maar u gebruikt enkele bladen om uw gegevens te importeren. Neem de tijd om uzelf vertrouwd te maken met de inhoud en vooral met de indeling van de inhoud in elk vel.
   * Let vooral op de kolomnamen en de notatie waarin de gegevens in elke kolom worden weergegeven.
   * U mag de namen of de volgorde van de kolommen in geen van de bladen wijzigen. De kolomkoppen geven in elke rij de velden aan die u met uw gegevens moet invullen. Als de kolomkop vet wordt weergegeven, is dit een verplicht veld. U moet dus informatie in die kolom hebben.
   >[!IMPORTANT]
   >
   >Sommige kolomkoppen worden mogelijk niet vet weergegeven, maar zijn wel verplicht.

   * Houd het gedownloade bestand ter referentie en ga verder met de volgende sectie.


## De sjabloon Kick-start exporteren voor aangepaste gegevens

Nadat u de informatie over bestaande aangepaste velden in uw systeem hebt gescand, kunt u een nieuwe sjabloon voor het starten van de site voor het importeren downloaden.

1. Klikken **Hoofdmenu > Instellen** in de rechterbovenhoek van de Workfront-interface.

1. Breid uit **Systeem** links.

1. Klikken **Gegevens importeren (Kick-start)**.

   ![](assets/import-data-kick-starts-link-in-setup.png)

1. In de **Een leeg Kick-startspreadsheet downloaden** gebied, kiest u de **Aangepaste gegevens** selectievakje en klik op **Downloaden**.

   ![](assets/blank-custom-data-option-checked-kick-starts.png)

   Een leeg bestand met de startfunctie wordt naar de computer gedownload.

   >[!NOTE]
   >
   >Het aantal bladen in het bestand, de namen ervan en het aantal kolommen en de namen van de kolommen in elk blad moeten gelijk zijn aan het aantal bladen in de bovenstaande sectie waarin de bestaande aangepaste gegevens staan.

## Piek Excel Kick-Begint spreadsheet

Download de sjabloon voor het starten van de functie voordat u het Excel-spreadsheet vult, zoals beschreven in de bovenstaande sectie.

>[!IMPORTANT]
>
>Probeer geen gegevens te importeren met een speciaal Excel-werkblad. Alle spreadsheets voor het importeren van informatie naar Workfront met de functie voor het starten van de toepassing moeten overeenkomen met de inhoud van de bestanden die u downloadt van Workfront en die in dit artikel worden beschreven.

Om het spreadsheet van Excel met informatie voor de nieuwe douanevelden te bevolken:

1. Open het Excel-werkblad dat u in de vorige sectie hebt gedownload en bekijk een aantal bladen. Elk blad vertegenwoordigt een object in de toepassing.

   >[!INFO]
   >
   >Bijvoorbeeld: **Parameter** (dat verwijst naar Aangepast veld), **Parameteroptie**(dat verwijst naar de optie Aangepast veld), **Categorie** (Dit verwijst naar Aangepast formulier).
   >
   >U moet de namen van de objecten en hun kenmerken schrijven in de indeling die wordt ondersteund door de Workfront-database.
   >
   >Voor informatie over de betekenis van deze objecten raadpleegt u de [Workfront glossary](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).
   >
   >Voor informatie over de namen van de objecten in de Workfront-database raadpleegt u de [API Explorer](../../../wf-api/general/api-explorer.md).
   >
   >![](assets/sheets-included-in-custom-data-export-kick-start-file.png)





1. Zorg ervoor dat de volgende informatie correct is opgemaakt:

   * De eerste rij van elk blad moet leeg blijven, anders genereert het importeren een fout.
   * De kolomkoppen in elk blad vertegenwoordigen kenmerken van de objecten die tijdens het importeren kunnen worden ingesteld. Alle kolomkoppen moeten in de zelfde orde blijven u hen vindt wanneer u het blad uitvoert en zij kunnen niet worden anders genoemd.
   * De kolomkoppen in vet zijn verplichte velden en moeten een waarde hebben.

      >[!TIP]
      >
      >Sommige kolommen zijn vereist, maar niet vet. De `isNew` en `ID` kolommen worden niet vet weergegeven, maar zijn verplichte velden.

1. Selecteer `**PARAM Parameter`** werkblad en voeg informatie over de nieuwe aangepaste velden toe in de volgende vereiste kolommen:

   * **`isNew`** = enter **`TRUE`** in deze kolom voor elke regel die een nieuw aangepast veld vertegenwoordigt. Dit geeft aan dat het veld nieuw is en niet bestaat in Workfront.

      >[!TIP]
      >
      >    Als een regel een bestaand veld vertegenwoordigt dat al in Workfront voorkomt, voert u **`isNew`** = **`FALSE`**.

   * **`ID`** = moet een uniek getal zijn voor elke regel die een nieuw veld vertegenwoordigt. U kunt elk nummer gebruiken dat begint met 1, zolang elk nieuw veld een uniek nummer heeft.
   * **`setDataType`** = voor elke regel die een nieuw veld vertegenwoordigt, voert u het gegevenstype in dat het veld ondersteunt. Het gegevenstype moet worden ingevoerd zoals het in de database wordt weergegeven. Selecteer een van de volgende gegevenstypen:
      * **`NMBR`** for Number
      * **`CURC`** voor Valuta
      * **`TEXT`** voor tekst
   * `**setDisplaySize**`= de weergavegrootte (&#39;**setDisplaySize**&#39;) voor meerdere opties is aangepaste velden altijd 0.
   * **`setDisplayType`** = voor elke regel die een nieuw veld vertegenwoordigt, voert u het weergavetype van het veld in. Het weergavetype moet worden ingevoerd zoals het in de database wordt weergegeven.

      Selecteer een van de volgende opties voor aangepaste velden met meerdere opties:

      * **`MULT`** voor Vervolgkeuzelijst met meerdere selecties
      * **`SLCT`** voor Vervolgkeuzelijst
      * **`RDIO`** voor keuzerondjes
      * **`CHCK`** voor selectievakjes
      >[!TIP]
      >
      >Als u de informatie over Gegevenstype en Weergavetype wilt vinden, raadpleegt u de [API Explorer](../../../wf-api/general/api-explorer.md), breid de **Parameter** -object, en zoek deze kenmerken onder de **velden** tab.

   * **`setName`** = voert u de naam in van de aangepaste velden die u in Workfront wilt weergeven.

      >[!INFO]
      >
      >We kunnen bijvoorbeeld twee aangepaste velden importeren, genaamd _Merk_, een veld voor het selectievakje, en _Media_, een veld voor keuzerondjes.

   * De **`setName`** en de **`setValue`** de kolommen bevatten gewoonlijk de zelfde informatie en zij zouden op de namen moeten wijzen die in de interface van Workfront voor uw nieuw gebied worden gewenst.
   De waarde van een veld is de naam die wordt weergegeven in rapporten, terwijl de naam wordt weergegeven in de aangepaste formulieren die aan objecten zijn gekoppeld.

   Zie voor meer informatie [Een aangepast veld toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).

   ![](assets/parameter-sheet-filled-out-kick-starts.png)

1. Selecteer **`POPT Parameter Options`** Voeg in de volgende vereiste kolommen informatie toe over de opties van elk aangepast veld:

   * **`isNew`** = enter **`TRUE`** in deze kolom voor elke regel die een nieuwe veldoptie vertegenwoordigt.

      >[!TIP]
      >
      >    Als een lijn een bestaande optie vertegenwoordigt, zou u ingaan **`isNew`** = **`FALSE`**.

   * **`ID`** = moet een uniek getal zijn voor elke regel die een nieuwe optie vertegenwoordigt. U kunt elk nummer gebruiken dat begint met 1, zolang elke nieuwe optie een uniek nummer heeft.
   * **`setIsDefault`** = enter `TRUE` voor de opties die u standaard wilt weergeven, en `FALSE` voor alle andere opties, voor elk gebied.  Wij willen bijvoorbeeld _Nike_ de standaardoptie voor _Merk_ en _Afdrukken_ de standaardoptie voor _Media_.

      >[!TIP]
      >
      >Er kan slechts één standaardoptie voor elk veld zijn.

   * **`setParameterID`** = de opties die overeenkomen met de _Merk_ aangepast veld bevat een **`setParameterID`** van 1, en de opties die overeenkomen met de _Media_ hebben een **`setParameterID`**van 2. De `PARAM` en `POPT` bladen verwijzen naar elkaar om aan te geven welke opties tot welk aangepast veld behoren.
   * **`setDisplayOrder`**= de kolom met de weergavevolgorde geeft de volgorde aan waarin de opties in het aangepaste veld worden weergegeven. U kunt beginnen met 1 en in oplopende volgorde verdergaan voor alle opties, ongeacht tot welke velden ze behoren. Het is belangrijk dat er voor elke optie unieke nummers zijn.
   * De **`setLabel`** en de `**setValue`** de kolommen bevatten gewoonlijk de zelfde informatie en zij zouden op de namen moeten wijzen die in Workfront UI worden gewenst. De waarde van een optie is de naam die in rapporten wordt weergegeven, terwijl het label in de aangepaste formulieren wordt weergegeven wanneer het aan een object is gekoppeld. Zie voor meer informatie [Een aangepast veld toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
   * **`setIsHidden`** = enter `TRUE` als u een van de opties wilt verbergen.
   ![](assets/parameter-option-sheet-filled-out-kick-starts.png)


1. (Optioneel) Als u ook een aangepast formulier wilt maken waarin u de nieuwe velden later kunt toevoegen, selecteert u de optie  **`CTGY Category`** De volgende vereiste kolommen voor de aangepaste formuliergegevens in een werkblad plaatsen en bijwerken:

   * **`isNew`** = enter **`TRUE`** in deze kolom voor elke regel die een nieuw aangepast formulier vertegenwoordigt.
   * **`ID`** = voer een uniek nummer in voor elke regel die een nieuw formulier vertegenwoordigt. U kunt elk nummer gebruiken dat begint met 1, zolang elke nieuwe optie of regel een uniek nummer heeft.
   * **`setGroupID`** = voeg identiteitskaart van de Groep voor uw Groep van het Huis, of een andere groep in het systeem toe de waarvan leden u toegang tot dit formulier wilt hebben. Dit is een verplicht veld.
   Als u de opdracht `ID` van een Groep, kunt u of een rapport van de Groep bouwen en toevoegen `ID` in Weergave of navigeer naar een groep en zoek de URL voor de groep. De groep-id staat in de URL van de pagina van de groep. Als de URL van de groep bijvoorbeeld `https://companyName.my.workfront.com/group/575b000800467a6f66e747932c807464/members`, de groep-id is `575b000800467a6f66e747932c807464`.

   * **`setCatObjCode` **= dit is de objectcode voor het objecttype waarvoor u het formulier wilt maken. Voer een code uit de volgende opties in:
      * **`CMPY`** voor Bedrijf
      * **`TASK`** voor taak
      * **`PROJ`** voor project
      * **`PORT`** voor Portfolio
      * **`PRGM`** voor programma
      * **`USER`** voor gebruiker
      * **`DOCU`** voor document
      * **`OPTASK`** voor uitgifte
      * **`EXPNS`** voor kosten
      * **`ITRN`** voor herhaling
      * **`BILL`** voor factureringsrecords
      * **`GROUP`** voor groep
      >[!NOTE]
      >
      >Voor formulieren met meerdere objecten voert u het eerste object in dat u zou selecteren bij het maken van een formulier in de gebruikersinterface. Stel bijvoorbeeld de `setCatObjCode` tot `TASK`, als u Taken selecteert in de interface van Workfront en vervolgens, uitgave, Portfolio, enz., maar u wilt niet dat het formulier beschikbaar is voor Projecten.

   * **`setName`** = dit is de naam van het aangepaste formulier zoals u het wilt weergeven in de Workfront-interface.

      ![](assets/category-sheet-filled-out-kick-starts.png)



1. Sla het spreadsheet op als een .xls- of .xlsx-bestand op uw computer. Uw Excel-werkblad is ingevuld en kan nu worden geïmporteerd in Workfront.


## Het Excel-werkblad uploaden naar Workfront

Nadat u de in de vorige secties beschreven stappen hebt uitgevoerd, gaat u als volgt verder om de nieuwe velden en formulieren te uploaden naar Workfront:

1. Klikken **Gegevens importeren** **(Kick-Starts) ** onder de **Hoofdmenu > Instellen > Systeem** -menu.

1. Klikken **Bestand kiezen** onder de sectie **Gegevens uploaden met werkblad Kick-Start**.

1. Blader naar het Excel-werkblad dat u hebt voorbereid, op uw computer en selecteer het werkblad wanneer u het hebt gevonden.  Wanneer het bestand wordt herkend door Workfront, wordt de knop Uploaden blauw.
1. Klikken **Uploaden.**

   ![](assets/kick-start-file-selected-and-upload-blue-button.png)

1. Er wordt een melding weergegeven dat het importeren is gelukt. Afhankelijk van hoeveel informatie u invoert, zou deze stap een paar seconden aan een minuut kunnen vergen.

   ![](assets/kick-start-successful.png)

   De nieuwe aangepaste velden en formulieren staan nu in uw Workfront-systeem. U kunt ze vinden in het gedeelte Aangepaste Forms van Setup.

   >[!NOTE]
   >
   >De nieuwe formulieren en de geïmporteerde velden hebben nog geen verbinding. Het formulier wordt geïmporteerd zonder aangepaste velden. U moet de velden handmatig toevoegen aan het nieuwe aangepaste formulier of aan een ander bestaand aangepast formulier.


   Voor informatie over het toevoegen van velden aan aangepaste formulieren raadpleegt u [Een aangepast veld toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).

1. (Voorwaardelijk) Als het importeren niet is gelukt, wordt een foutbericht weergegeven waarin het probleem is aangegeven. Probeer het veld, het blad en het rijnummer te identificeren waarin het probleem is opgetreden en corrigeer de gegevens in het Excel-bestand. Probeer het bestand vervolgens nog een keer te importeren.

   ![](assets/kick-start-error.png)

1. (Voorwaardelijk) Afhankelijk van wat het probleem is, zoals vermeld in het foutbericht, kunnen sommige gegevens al worden geïmporteerd. U moet een van de volgende handelingen uitvoeren voordat u het blad opnieuw kunt importeren:

   * Verwijder de informatie die uit Workfront is geïmporteerd uit het gebied Aangepaste Forms en breng de correctie aan die wordt aangegeven door het foutbericht.
   * Geef aan dat er al een veld of formulier in het systeem staat voor de velden of formulieren die al zijn geïmporteerd, en breng vervolgens de correctie aan.
Als u wilt aangeven dat een veld of aangepast formulier al in Workfront is, moet u ervoor zorgen dat de optie `inNew` veld is gemarkeerd als `FALSE` in bladen die informatie over het formulier bevatten (`CTGY`) of het veld (`PARAM`) op het schoppen van het invoerblad.
