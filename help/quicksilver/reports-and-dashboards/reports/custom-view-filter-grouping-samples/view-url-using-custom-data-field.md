---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: externe URL gebruiken van aangepast gegevensveld'
description: U kunt een koppeling naar een interne aangepaste URL weergeven door in een taakweergave een berekend aangepast veld met de naam "Aangepaste URL" te gebruiken.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# Weergave: externe URL gebruiken met aangepast gegevensveld

U kunt een koppeling naar een interne aangepaste URL weergeven met een **Berekend aangepast veld** met de naam &quot;Aangepaste URL&quot; in een **Taakweergave**.

Hierdoor kunt u snel vanuit bepaalde objecten een koppeling maken naar bepaalde delen van de toepassing, rechtstreeks vanuit uw rapporten.

Wanneer u een berekend aangepast veld maakt, moet u eerst het veld maken en vervolgens de weergave maken.

De volgende secties zijn een voorbeeld van een berekend douanegebied voor taken. Het aangepaste veld heet Aangepaste URL. In de aangepaste weergave worden de waarde van het veld en de **URL** veld voor taken.

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

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Het berekende aangepaste veld Aangepaste URL maken

Zie het artikel voor informatie over het maken van een berekend aangepast veld [Berekende gegevens toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Als u toegang hebt om een aangepast formulier te maken, kunt u een berekend aangepast veld maken voor taken die &#39;Aangepaste URL&#39; worden genoemd. Dit veld is rechtstreeks gekoppeld aan de **Overzicht** subtab binnen de **Taakdetails** tab.

1. Maak een berekend aangepast veld.
1. Voer in het veld Berekening de volgende code in:

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&#39;)

1. Vervangen &quot;`<domain>`&quot; met uw werkelijke domeinnaam, zonder de vierkante haakjes.

   De

   ```
   /overview
   ```

   Het gedeelte van deze URL stuurt de koppeling naar het **Overzicht** in het linkerdeelvenster van de taak.

1. Nadat u uw **Berekend aangepast veld**, voegt u de **Aangepast formulier** met dit veld naar verschillende taken in Adobe Workfront die u in de nieuwe weergave wilt weergeven.

## Maak de weergave waarin de velden Aangepaste URL en URL van de taak worden weergegeven

De taak **Weergave** in het onderstaande voorbeeld worden de **Berekend aangepast veld** wordt &quot;Aangepaste URL&quot; genoemd als een directe koppeling naar de **Overzicht** subtab binnen de taak **Details** en de **URL** taakgebied.

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

Deze weergave aanpassen:

1. Ga naar een takenlijst.
1. Breid uit **Weergave** boven aan uw takenlijst.
1. Klikken **Weergave aanpassen**.
1. Verwijder alle kolommen binnen de mening, behalve de eerste kolom.
1. Klik op de kop van de eerste kolom.
1. Klikken **Overschakelen naar tekstmodus** in de rechterbovenhoek van de interface.
1. Klikken **Klik om tekst te bewerken**.
1. Plak de tekstmodus hieronder in uw ene kolom.\
   In dit voorbeeld wordt &#39;&#39;column.1&#39;&#39; geeft de waarde in het veld Aangepaste URL weer als een koppeling naar de taak **Overzicht**. &quot;Kolom.2.&quot; geeft de waarde weer die is opgeslagen in het dialoogvenster **URL-veld** van de taak.
   <pre>column.0.descriptionKey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat= int<br>column.0.link.lookup=link.view<br>column.0.link.valueField= objCode<br>column.0.link.valueFormat= val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=150<br>column.1.description=Custom URL<br>column.1.link.isnewwindow=true<br>column.1.link.url=customDataLabelsAsString(Custom URL)<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString(Custom URL)<br>column.1.name=Custom URL<br>column.1.querysort=URL<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valueField=Custom URL<br>column.1.valueFormat=customDataLabelsAsString<br>column.1.width=150<br>column.2.descriptionKey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valueField=URL<br>column.2.valueFormat=HTML<br>column.2.width=150</pre>

1. Klikken **Weergave opslaan**.
