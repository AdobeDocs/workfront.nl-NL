---
content-type: reference
product-area: reporting
keywords: audit,trail,custom,field
navigation-topic: calculate-custom-data-reports
title: 'Voorbeeld van een berekend aangepast veld: bewerkingsgeschiedenis van een veld weergeven'
description: If users update custom fields on a regular basis and you want to capture a log of all the changes made to a field as well as a date when the changes happen, you can capture this information in a calculated custom field.
author: Courtney
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# Voorbeeld van een berekend aangepast veld: bewerkingsgeschiedenis van een veld weergeven

If users update custom fields on a regular basis and you want to capture a log of all the changes made to a field as well as a date when the changes happen, you can capture this information in a calculated custom field.

Het volgende voorbeeld toont u hoe te om Instructies te bouwen geeft Geschiedenis berekende gebied uit om alle verandering te vangen die aan een single-line tekstgebied wordt aangebracht genoemd Instructies.

>[!TIP]
>
>U kunt dit voorbeeld volgen voor alle typen aangepaste velden, niet alleen voor tekstvelden van één regel.

Dit doet het volgende:

* Hiermee beperkt u het veld Instructies > Geschiedenis bewerken tot de meest recente 2000 tekens om binnen de Workfront-databaselimiet te blijven.
* Controleert of de huidige waarde van het veld Instructies overeenkomt met de voorzijde van de waarde van Historie bewerken in Instructies. Hierbij wordt ervan uitgegaan dat deze waarde leeg is. Als dit niet het geval is, wordt het volgende uitgevoerd:

   * Als zij aanpassen, verlaat het de Instructies uitgeven Geschiedenis zoals is;
   * If they do not match, it replaces the Instructions Edit History with the latest value in the Instructions field, followed by the current date in parentheses, a vertical bar, and the previous Instructions Edit History, which preserves the previous value(s) and the date(s) when they were entered.

## Toegangsvereisten

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-pakket</p> </td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-licentie</p> </td> 
   <td>
      <p>Standard</p>
      <p>Plan</p></td>
  </tr> 
  <tr> 
   <td><p>Configuraties op toegangsniveau</p></td> 
   <td> <p>Administratieve toegang tot Aangepaste Forms</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objectmachtigingen</p> </td> 
   <td> <p>Manage permissions on the custom forms</p></td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

To add a calculated field that displays a field&#39;s edit history to a custom form, you must first:

* Het aangepaste formulier maken
* Het veld met de geschiedenis die u wilt vastleggen toevoegen aan het aangepaste formulier

## De bewerkingsgeschiedenis van een veld weergeven

1. Ga naar een aangepast formulier waaraan u het berekende veld wilt toevoegen.

1. Ga als volgt te werk om bijvoorbeeld het aangepaste tekstveld voor een enkele regel te maken:

   1. Klik **Enige lijntekst**.
   1. Specify a **Label** for the custom field. U kunt de naam bijvoorbeeld &quot;Instructies&quot; geven.
   1. Klik **toepassen**.

1. Click **Calculated** to add a calculated custom field to the form.
1. Specify a **Label** for the calculated custom field. For example, you can name it &quot;Instructions Edit History&quot;.

   Dit is het gebied dat om het even welke veranderingen zal vangen die aan het eerste gebied worden aangebracht u (&quot;Instructies&quot;) creeerde.

1. Klik **sparen en Sluiten**.
1. Klik op de naam van het formulier waaraan u twee velden hebt toegevoegd om het formulier opnieuw te openen.
1. Klik de berekende instructies van het douanegebied **geven Geschiedenis** uit, dan kopieer en kleef het volgende in de **doos van de Berekening**:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Geadviseerd) Deeg de zelfde berekening in het **gebied van Instructies** op het berekende gebied op de vorm.
1. Zorg ervoor dat **Tekst** op het **3&rbrace; gebied van het Formaat &lbrace;wordt geselecteerd om het berekende douanegebied als tekst te formatteren.**

   Dit is de standaardinstelling.

1. Klik **sparen en Sluiten**.

   Now, when you attach the custom form to an object and then someone changes the information in the **Instructions** field, the **Instructions Edit History** field displays the latest value, followed by the current date in parentheses, and a vertical bar. If further changes are made, they are added to this information in the same way.

   In the above calculation, you can replace *Instructions* with the exact name of your single-line text field whose history you want to track, and **Instructions Edit History** with the exact name of your calculated field.
