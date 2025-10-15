---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: externe URL met aangepast gegevensveld'
description: U kunt een koppeling naar een interne aangepaste URL weergeven door in een taakweergave een berekend aangepast veld met de naam "Aangepaste URL" te gebruiken.
author: Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Weergeven: externe URL met gebruik van aangepast gegevensveld

<!--Audited: 11/2024-->

U kunt een verbinding aan een interne douane URL tonen door a **Berekend Gebied van de Douane** genoemd &quot;Douane URL&quot;in de Mening van de Taak van a **te gebruiken**.

Hierdoor kunt u snel vanuit bepaalde objecten een koppeling maken naar bepaalde delen van de toepassing, rechtstreeks vanuit uw rapporten.

Wanneer u een berekend aangepast veld maakt, moet u eerst het veld maken en vervolgens de weergave maken.

De volgende secties zijn een voorbeeld van een berekend douanegebied voor taken. Het aangepaste veld heet Aangepaste URL. De douanemening toont de waarde van het gebied evenals het **URL** gebied voor taken.

Met dezelfde stappen kunt u vergelijkbare berekende aangepaste velden en aangepaste weergaven maken voor alle objecten in het systeem die een aangepast formulier hebben.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Medewerker of verzoek om een weergave te wijzigen </p>
   <p>Standaard of Plan om een rapport te wijzigen</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Het berekende aangepaste veld Aangepaste URL maken

Voor informatie over het creëren van een berekend douanegebied, zie [ berekende gebieden aan een vorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) toevoegen.

Als u toegang hebt om een aangepast formulier te maken, kunt u een berekend aangepast veld maken voor taken die &#39;Aangepaste URL&#39; worden genoemd. Dit gebied verbindt direct met het **Overzicht** subtab binnen de **Details van de Taak** tabel.

1. Maak een berekend aangepast veld.
1. Voer in het veld Berekening de volgende code in:

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&#39;,&#39;/&#39;,&#39;&#39;task/&#39;,ID,&#39;/overview&#39;&#39;)

1. Vervang &quot;`<domain>`&quot;met uw daadwerkelijke domeinnaam, zonder de steunen. Het `/overview` gedeelte van dit URL leidt de verbinding aan de **2} sectie van het Overzicht {in het linkerpaneel van de taak.**

1. Na het creëren van uw **Berekend Gebied van de Douane**, maak de **Vorm van de Douane** met dit gebied aan verscheidene taken in Adobe Workfront vast die u vertoning in uw nieuwe mening wilt.

## Maak de weergave waarin de velden Aangepaste URL en URL van de taak worden weergegeven

De taak **Mening** in het voorbeeld hieronder toont het **Berekende Gebied van de Douane** geroepen &quot;Douane URL&quot;als directe verbinding aan het **Overzicht** subtab binnen de taak **Details** tabel, evenals het **URL** gebied van de taak.

assets/task-view-with-custom-url-field-quicksilver-350x70.png)

Deze weergave aanpassen:

1. Ga naar een takenlijst.
1. Breid **drop-down Mening** bij de bovenkant van uw taaklijst uit.
1. Klik **aanpassen Mening**.
1. Verwijder alle kolommen binnen de mening, behalve de eerste kolom.
1. Klik op de kop van de eerste kolom.
1. Klik **Schakelaar aan de Wijze van de Tekst** > **uitgeven de Wijze van de Tekst**.
1. Verwijder de tekst in **geeft de Wijze van de Tekst** vakje uit en vervangt het met de volgende code:


   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat= int
   column.0.link.lookup=link.view
   column.0.link.valuefield= objCode
   column.0.link.valueformat= val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.description=Custom URL
   column.1.link.isnewwindow=true
   column.1.link.url=customDataLabelsAsString(Custom URL)
   column.1.linkedname=direct
   column.1.listsort=customDataLabelsAsString(Custom URL)
   column.1.name=Custom URL
   column.1.querysort=URL
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=Custom URL
   column.1.valueformat=customDataLabelsAsString
   column.1.width=150
   column.2.descriptionkey=url
   column.2.linkedname=direct
   column.2.listsort=string(URL)
   column.2.namekey=url.abbr
   column.2.querysort=URL
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=URL
   column.2.valueformat=HTML
   column.2.width=150
   ```

   In dit voorbeeld wordt &#39;&#39;column.1&#39;&#39; De lijnen tonen de waarde op het gebied van de &quot;Douane URL&quot;als verbinding in het 0} Overzicht van de taak **sectie; &quot;column.2.&quot;** toont de waarde die in het **wordt opgeslagen gebied URL** van de taak.

1. Klik **Gedaan** > **sparen Mening**.
