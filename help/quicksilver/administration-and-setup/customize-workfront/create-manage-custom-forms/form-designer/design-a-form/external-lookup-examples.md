---
title: Voorbeelden van het externe opzoekveld in een aangepast formulier
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Een extern opzoekveld in een aangepast formulier roept een externe API aan en retourneert waarden als opties in een vervolgkeuzeveld. Dit artikel bevat voorbeelden van het gebruik van het externe opzoekveld om dezelfde instantie van Workfront of een openbare API aan te roepen.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 13880fcb-8523-45d2-9ac6-38453e8e2391
source-git-commit: 3838e355c16275b9e10fb92497f1698ac99c4fa4
workflow-type: tm+mt
source-wordcount: '1414'
ht-degree: 0%

---

# Voorbeelden van het externe opzoekveld in een aangepast formulier

Een extern opzoekveld in een aangepast formulier roept een externe API aan en retourneert waarden als opties in een vervolgkeuzeveld. Gebruikers die werken met het object waaraan het aangepaste formulier is gekoppeld, kunnen een of meer van deze opties in het vervolgkeuzemenu selecteren.

Dit artikel bevat voorbeelden van het gebruik van het externe opzoekveld om dezelfde instantie van Workfront of een openbare API aan te roepen. U kunt de Externe raadpleging ook gebruiken om met een extern systeem zoals Jira, Salesforce, of ServiceNow te communiceren.

Voor meer informatie over het toevoegen van een Extern raadplegingsgebied aan een douaneformulier en extra definities van de externe raadplegingscomponenten, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> </td> 
  </tr>  
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een extern opzoekveld instellen voor dezelfde instantie van Workfront

U kunt de externe zoekopdracht gebruiken om gegevens van uw Workfront-exemplaar over te brengen naar het aangepaste formulier.

<!--When someone accesses the field in the custom form, they will only see in the list of options what they have permissions to see in Workfront. For example, if you are showing a list of projects, the user would only see projects that are shared with them.-->

### Native Workfront-veldwaarden gebruiken in de externe zoekopdracht

In dit voorbeeld wordt getoond hoe u de Workfront API aanroept en een lijst met projecten in een extern opzoekveld vult. Deze lijst wordt gefilterd op status met de waarde van het aangepaste veld Statusquery en een zoekterm via $$QUERY.

1. Open het aangepaste formulier.
1. Op de linkerkant van het scherm, vind **Externe raadpleging** en sleep het aan een sectie op het canvas.
1. Ga het **Etiket** en **Naam** voor het gebied in.
1. Selecteer het **Formaat** voor het gebied.
1. Ga de API vraag op het **Basis API URL** gebied in.

   * Gebruik $$HOST om naar hetzelfde exemplaar van Workfront te verwijzen waar het aangepaste formulier zich bevindt.
   * Gebruik $$QUERY om de resultaten dynamisch te filteren op basis van gebruikersinvoer.

   **de vraag van API van het Voorbeeld**
   `$$HOST/attask/api/v15.0/project/search?status={DE:Status Query}&description=$$QUERY`

1. Herzie de **Afhankelijkheden** voor de gebieden die in de API vraag van verwijzingen worden voorzien.

   Een afhankelijkheidsveld kan elk aangepast of native veld zijn dat beschikbaar is voor het object. Als u bijvoorbeeld een aangepast formulier maakt voor groepen die een extern opzoekveld bevatten, kunnen afhankelijkheidsvelden alle velden bevatten die beschikbaar zijn in een groep.

   In dit voorbeeld wordt `{DE:Status Query}` dynamisch vervangen door de waarde van het aangepaste veld &quot;Statusquery&quot; voor de huidige groep. Wanneer het formulier dus is gekoppeld aan groep A, wordt `{DE:Status Query}` vervangen door de waarde die is ingesteld in het veld Statusquery voor die groep.

1. Selecteer de **Methode van HTTP**.

   Dit zal meestal **krijgen** waarschijnlijk zijn.

1. Ga de **Weg JSON** in om de resultaten van uw API vraag te krijgen.

   **Voorbeeld**
   `$.data[*].name`

   >[!NOTE]
   >
   >**de informatie van de Kopbal** wordt niet vereist voor een vraag aan de zelfde instantie van Workfront.

1. Klik **toepassen**.

   ![ Opstelling van API vraag aan Workfront in douanevorm ](assets/external-lookup-to-workfront.png)

   Wanneer het aangepaste formulier wordt toegevoegd aan een Workfront-object (in dit voorbeeld een project), ziet het er ongeveer zo uit.

   ![ Vorm van de Douane met extern raadplegingsgebied ](assets/external-lookup-project-status-example1.png)

   ![ Externe raadplegingsopties die op status ](assets/external-lookup-project-status-example2.png) worden gebaseerd

### Aangepaste veldwaarden gebruiken in de externe zoekopdracht

In dit voorbeeld ziet u hoe u de Workfront API aanroept en gegevens van een aangepast veld naar uw externe opzoekveld brengt. Het aangepaste voorbeeldveld wordt &#39;Aangepaste kleuren&#39; genoemd.

1. Open het aangepaste formulier.
1. Op de linkerkant van het scherm, vind **Externe raadpleging** en sleep het aan een sectie op het canvas.
1. Ga het **Etiket** en **Naam** voor het gebied in.
1. Selecteer het **Formaat** voor het gebied.
1. Ga de API URL vraag op het **Basis API URL** gebied in.

   **Voorbeeld**
   `$$HOST/attask/api/v18.0/PORT/search?ID={portfolioID}&fields=parameterValues`

1. Herzie **Afhankelijkheden** voor de gebieden dat dit raadplegingsgebied in API van verwijzingen voorziet.

   Een afhankelijkheidsveld kan elk aangepast of native veld zijn dat op de detailpagina van het object bestaat.

1. Selecteer de **Methode van HTTP**.

   Dit zal meestal **krijgen** waarschijnlijk zijn.

1. Ga de **Weg JSON** in om de resultaten van uw API vraag te krijgen.

   **Voorbeeld**
   `$.data[*].parameterValues.["DE:Combo Colors"]`

   * &quot;parameterValues&quot; verwijst naar elk aangepast veld in Workfront voor het object dat u hebt ingeschakeld.
   * Voor dit voorbeeld, &quot;DE :Combo Kleuren&quot;is het specifieke douanegebied dat de waarden bevat u wilt terugwinnen.

   >[!NOTE]
   >
   >**de informatie van de Kopbal** wordt niet vereist voor een vraag aan de zelfde instantie van Workfront.

1. Klik **toepassen**.

   Wanneer het aangepaste formulier aan een Workfront-object wordt toegevoegd, worden alle waarden in het veld &quot;Combo Colors&quot; weergegeven in het vervolgkeuzemenu Extern opzoekveld.

## Een extern opzoekveld instellen voor de API voor Workfront-planning

Een eindpunt is beschikbaar in de Planning API van Workfront aan onderzoeksverslagen door verslagtype identiteitskaart door Get methode. U kunt dit eindpunt gebruiken om de verslagen van de Planning in Externe raadplegingsgebieden van verwijzingen te voorzien.

* **Basis API URL:** `$$HOST/maestro/api/v1/records/search?recordTypeId={recordTypeID}`
* **Methode van HTTP:** krijgt
* **Weg JSON:** `$.records[*].data.{fieldID}`

  **{fieldID}** is het veld dat in de zoekresultaten voor externe zoekopdrachten op het aangepaste formulier voor eindgebruikers moet worden weergegeven.

Voor meer informatie, zie [ de Planning API van Workfront ](/help/quicksilver/planning/general/planning-api-basics.md).

## Een extern opzoekveld instellen voor een openbare API

U kunt de externe zoekopdracht gebruiken om een externe, openbare API aan te roepen en gegevens op te halen.

In dit voorbeeld wordt getoond hoe u een API van landen (zoals <https://api.first.org/data/v1/countries>) aanroept, zodat u niet alle landnamen in de vervolgkeuzemogelijkheden hoeft te coderen.

1. Open het aangepaste formulier.
1. Op de linkerkant van het scherm, vind **Externe raadpleging** en sleep het aan een sectie op het canvas.
1. Ga het **Etiket** en **Naam** voor het gebied in.
1. Selecteer het **Formaat** voor het gebied.
1. Ga de API URL vraag op het **Basis API URL** gebied in.

   * U kunt $$QUERY toevoegen om vraag het filtreren voor uw eind uit te voeren - gebruikers.

   **Voorbeelden**
Geeft alle landen weer: <https://api.first.org/data/v1/countries>

   Hiermee kan de gebruiker naar een land in het vervolgkeuzevenster zoeken: <https://api.first.org/data/v1/countries?q=$$QUERY>

   Hiermee kan de gebruiker naar een land in een regio zoeken: <https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

   * De beschikbare gebieden worden gedefinieerd in een afzonderlijk aangepast veld in Workfront.
   * Wanneer de gebruiker een gebied op het formulier selecteert, worden in het veld Extern opzoeken alleen de landen in dat gebied weergegeven (in welk land de regio is gedefinieerd in de API). De gebruiker kan ook naar een land in het geselecteerde gebied zoeken.

1. Herzie **Afhankelijkheden** voor de gebieden dat dit raadplegingsgebied in API van verwijzingen voorziet.

   Een afhankelijkheidsveld kan elk aangepast of native veld zijn dat op de detailpagina van het object bestaat.

   In dit voorbeeld wordt `{DE:Region}` vervangen door de waarde van het aangepaste veld Regio.

1. Selecteer de **Methode van HTTP**.

   Dit zal meestal **krijgen** waarschijnlijk zijn.

1. Ga de **Weg JSON** in om de resultaten van uw API vraag te krijgen.

   Met deze optie kunnen gegevens worden opgehaald uit de JSON die door de API-URL wordt geretourneerd. Hiermee kunt u selecteren welke waarden in de JSON-code worden weergegeven in de vervolgkeuzemogelijkheden.

   **Voorbeeld**
   `$.data[*].country`

1. (Optioneel) Klik op **Koptekst toevoegen** en typ of plak het sleutelwaardepaar dat voor verificatie met de API is vereist.

   >[!NOTE]
   >
   >De gebieden van de Kopbal zijn geen veilige plaats om geloofsbrieven op te slaan, en u zou moeten zorgvuldig zijn wat u ingaat en bewaart.

1. (Facultatief) selecteer **multi-Select Vervolgkeuzelijst** om de gebruiker toe te staan om meer dan één waarde in dropdown te selecteren.

1. Klik **toepassen**.

   ![ Opstelling van API vraag aan openbare API in douaneformulier ](assets/external-lookup-to-api-for-countries.png)

   Wanneer het aangepaste formulier wordt toegevoegd aan een Workfront-object (in dit voorbeeld een project), ziet het er ongeveer zo uit.

   ![ Vorm van de Douane met extern raadplegingsgebied ](assets/external-lookup-countries-example1.png)

   ![ Externe raadplegingsopties voor een land dat op gebied ](assets/external-lookup-countries-example2.png) wordt gebaseerd

## Aanvullende gebruiksgevallen voor externe opzoekvelden

Er zijn veel andere gevallen waarin u een externe zoekopdracht kunt maken.

**geval van het Gebruik:** vervang typeahead gebieden, omdat zij problemen met het melden kunnen veroorzaken.
**Oplossing:** gebruik een API vraag aan bestaande voorwerpen in het systeem.

Voorbeeld-basis-API-URL voor sjablonen, ter vervanging van een typeahead-veld:
`$$HOST/attask/api/v17.0/tmpl/search?isActive=true&name_Sort=asc`

**het geval van het Gebruik:** creeer dropdown gebieden met meer eigenschappen (bijvoorbeeld, is er lijnomslag op het Externe onderzoeksgebied).
**Oplossing:** gebruik een API vraag aan bestaande voorwerpen in het systeem, of creeer een nieuw voorwerp en gebruik een API vraag aan dit voorwerp.

**geval van het Gebruik:** bepaal een manier voor gebruikers om hun eigen gebieden buiten het gebied van douaneformulieren te handhaven. Stel het externe opzoekveld in en u kunt gebruikers de objecten geven die het veld vormen. Deze optie is geschikt voor velden en teams met hoog onderhoud.
**Oplossing:** creeer een nieuw voorwerp en gebruik een API vraag aan dit voorwerp.

**geval van het Gebruik:** Integratie met voorwerpen buiten Workfront. Bijvoorbeeld, die tot een ander systeem toegang hebben om de naam van elke gebruiker te krijgen, eerder dan wordt beperkt op een typeahead gebied.
**Oplossing:** automatisering Webhaak/Fusion om met andere systemen te verbinden.

