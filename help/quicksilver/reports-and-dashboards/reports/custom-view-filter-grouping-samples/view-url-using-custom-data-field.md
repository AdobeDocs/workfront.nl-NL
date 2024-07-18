---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: externe URL met gebruik van aangepast gegevensveld'
description: U kunt een koppeling naar een interne aangepaste URL weergeven door in een taakweergave een berekend aangepast veld met de naam "Aangepaste URL" te gebruiken.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Weergeven: externe URL met gebruik van aangepast gegevensveld

U kunt een verbinding aan een interne douane URL tonen door a **Berekend Gebied van de Douane** genoemd &quot;Douane URL&quot;in de Mening van de Taak van a **te gebruiken**.

Hierdoor kunt u snel vanuit bepaalde objecten een koppeling maken naar bepaalde delen van de toepassing, rechtstreeks vanuit uw rapporten.

Wanneer u een berekend aangepast veld maakt, moet u eerst het veld maken en vervolgens de weergave maken.

De volgende secties zijn een voorbeeld van een berekend douanegebied voor taken. Het aangepaste veld heet Aangepaste URL. De douanemening toont de waarde van het gebied evenals het **URL** gebied voor taken.

Met dezelfde stappen kunt u vergelijkbare berekende aangepaste velden en aangepaste weergaven maken voor alle objecten in het systeem die een aangepast formulier hebben.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Verzoek om een weergave te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Het berekende aangepaste veld Aangepaste URL maken

Voor informatie over het creëren van een berekend douanegebied, zie [ berekende gebieden aan een vorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) toevoegen.

Als u toegang hebt om een aangepast formulier te maken, kunt u een berekend aangepast veld maken voor taken die &#39;Aangepaste URL&#39; worden genoemd. Dit gebied verbindt direct met het **Overzicht** subtab binnen de **Details van de Taak** tabel.

1. Maak een berekend aangepast veld.
1. Voer in het veld Berekening de volgende code in:

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&#39;,&#39;/&#39;,&#39;&#39;task/&#39;,ID,&#39;/overview&#39;&#39;)

1. Vervang &quot;`<domain>`&quot;met uw daadwerkelijke domeinnaam, zonder de steunen.

   De

   ```
   /overview
   ```

   Het gedeelte van dit URL leidt de verbinding aan de **sectie van het Overzicht** in het linkerpaneel van de taak.

1. Na het creëren van uw **Berekend Gebied van de Douane**, maak de **Vorm van de Douane** met dit gebied aan verscheidene taken in Adobe Workfront vast die u vertoning in uw nieuwe mening wilt.

## Maak de weergave waarin de velden Aangepaste URL en URL van de taak worden weergegeven

De taak **Mening** in het voorbeeld hieronder toont het **Berekende Gebied van de Douane** geroepen &quot;Douane URL&quot;als directe verbinding aan het **Overzicht** subtab binnen de taak **Details** tabel, evenals het **URL** gebied van de taak.

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

Deze weergave aanpassen:

1. Ga naar een takenlijst.
1. Breid **drop-down Mening** bij de bovenkant van uw taaklijst uit.
1. Klik **aanpassen Mening**.
1. Verwijder alle kolommen binnen de mening, behalve de eerste kolom.
1. Klik op de kop van de eerste kolom.
1. Klik **Schakelaar aan de Wijze van de Tekst** in de hoger-juiste hoek van de interface.
1. Klik **klikken om tekst** uit te geven.
1. Plak de tekstmodus hieronder in uw ene kolom.\
   In dit voorbeeld wordt &#39;&#39;column.1&#39;&#39; toont de waarde op het gebied van &quot;Douane URL&quot;als verbinding in het 0} Overzicht van de taak **.** &quot;Kolom.2.&quot; toont de waarde die in het **wordt opgeslagen gebied URL** van de taak.
   <pre>column.0.descriptionkey=name <br> column.0.link.linkproperty.0.name=ID <br> column.0.link.linkproperty.0.valueField=ID <br> column.0.link.linkproperty.0.valueformat= int <br> column.0.link.lookup=link.view <br> column.0.link.valueField= objCode 5} column.0.link.valueformat= val <br> column.0.linkedname=direct <br> column.0.listsort=string(name) <br> column.0.namekey=name.abbr <br> column.0.querysort=name <br> column.0.shortview=false <br> column.0.stretch=100 {1 2} column.0.valueField=name <br> column.0.valueformat=HTML <br> column.0.width=150 <br> column.1.description=Custom URL <br> column.1.link.isnewwindow=true <br> column.1.link.url=customDataLabelsAsString (Douane)<br> column.1.linkedname=direct <br> column.1.listsort=customDataLabelsAsString (Douane URL) <br> column.1.name=Custom URL <br> column.1.querysort=URL <br> column.1.shortview=false <br> column.1.stretch=0 <br> 1.valueField=Custom URL <br> column.1.valueformat=customDataLabelsAsString <br> column.1.width=150 <br> column.2.descriptionkey=url <br> column.2.linkedname=direct <br> column.2.listsort=string(URL) <br>.2.namekey=url.abbr <br> column.2.querysort=URL <br> column.2.shortview=false <br> column.2.stretch=0 <br> column.2.valueField=URL <br> column.2.valueFormat=HTML <br> column.2.width=150<br><br></pre>

1. Klik **sparen Mening**.
