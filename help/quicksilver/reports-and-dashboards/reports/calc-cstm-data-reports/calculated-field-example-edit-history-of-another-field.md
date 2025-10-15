---
content-type: reference
product-area: reporting
keywords: audit,trail,custom,field
navigation-topic: calculate-custom-data-reports
title: 'Voorbeeld van een berekend aangepast veld: bewerkingsgeschiedenis van een veld weergeven'
description: Als gebruikers regelmatig aangepaste velden bijwerken en u wilt een logboek vastleggen van alle wijzigingen die in een veld zijn aangebracht en ook een datum waarop de wijzigingen worden aangebracht, kunt u deze gegevens vastleggen in een berekend aangepast veld.
author: Jenny
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# Voorbeeld van een berekend aangepast veld: bewerkingsgeschiedenis van een veld weergeven

Als gebruikers regelmatig aangepaste velden bijwerken en u wilt een logboek vastleggen van alle wijzigingen die in een veld zijn aangebracht en ook een datum waarop de wijzigingen worden aangebracht, kunt u deze gegevens vastleggen in een berekend aangepast veld.

Het volgende voorbeeld toont u hoe te om Instructies te bouwen geeft Geschiedenis berekende gebied uit om alle verandering te vangen die aan een single-line tekstgebied wordt aangebracht genoemd Instructies.

>[!TIP]
>
>U kunt dit voorbeeld volgen voor alle typen aangepaste velden, niet alleen voor tekstvelden van één regel.

Dit doet het volgende:

* Hiermee beperkt u het veld Instructies > Geschiedenis bewerken tot de meest recente 2000 tekens om binnen de Workfront-databaselimiet te blijven.
* Controleert of de huidige waarde van het veld Instructies overeenkomt met de voorzijde van de waarde van Historie bewerken in Instructies. Hierbij wordt ervan uitgegaan dat deze waarde leeg is. Als dit niet het geval is, wordt het volgende uitgevoerd:

   * Als zij aanpassen, verlaat het de Instructies uitgeven Geschiedenis zoals is;
   * Als zij niet aanpassen, vervangt het de Instructies uitgeven Geschiedenis met de recentste waarde op het gebied van Instructies, die door de huidige datum tussen haakjes, een verticale bar, en de vorige Instructies wordt gevolgd uitgeven Geschiedenis, die de vorige waarde(n) en de datum(s) bewaart toen zij werden ingegaan.

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
   <td> <p>Rechten voor aangepaste formulieren beheren</p></td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Als u een berekend veld met de bewerkingsgeschiedenis van een veld wilt toevoegen aan een aangepast formulier, moet u eerst het volgende doen:

* Het aangepaste formulier maken
* Het veld met de geschiedenis die u wilt vastleggen toevoegen aan het aangepaste formulier

## De bewerkingsgeschiedenis van een veld weergeven

1. Ga naar een aangepast formulier waaraan u het berekende veld wilt toevoegen.

1. Ga als volgt te werk om bijvoorbeeld het aangepaste tekstveld voor een enkele regel te maken:

   1. Klik **Enige lijntekst**.
   1. Specificeer a **Etiket** voor het douanegebied. U kunt de naam bijvoorbeeld &quot;Instructies&quot; geven.
   1. Klik **toepassen**.

1. Klik **Berekend** om een berekend douanegebied aan de vorm toe te voegen.
1. Specificeer a **Etiket** voor het berekende douanegebied. U kunt de instructie bijvoorbeeld &#39;Instructies > Geschiedenis bewerken&#39; noemen.

   Dit is het gebied dat om het even welke veranderingen zal vangen die aan het eerste gebied worden aangebracht u (&quot;Instructies&quot;) creeerde.

1. Klik **sparen en Sluiten**.
1. Klik op de naam van het formulier waaraan u twee velden hebt toegevoegd om het formulier opnieuw te openen.
1. Klik de berekende instructies van het douanegebied **geven Geschiedenis** uit, dan kopieer en kleef het volgende in de **doos van de Berekening**:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Geadviseerd) Deeg de zelfde berekening in het **gebied van Instructies** op het berekende gebied op de vorm.
1. Zorg ervoor dat **Tekst** op het **3} gebied van het Formaat {wordt geselecteerd om het berekende douanegebied als tekst te formatteren.**

   Dit is de standaardinstelling.

1. Klik **sparen en Sluiten**.

   Nu, wanneer u de douaneformulier aan een voorwerp vastmaakt en dan verandert iemand de informatie op het **gebied van Instructies**, geeft het **Instructies Geschiedenis** gebied uit de recentste waarde, die door de huidige datum tussen haakjes, en een verticale bar wordt gevolgd. Als er verdere wijzigingen worden aangebracht, worden deze op dezelfde manier aan deze informatie toegevoegd.

   In de bovengenoemde berekening, kunt u *Instructies* met de nauwkeurige naam van uw enig-lijntekstgebied vervangen de waarvan geschiedenis u wilt volgen, en **de Instructies geven Geschiedenis** met de nauwkeurige naam van uw berekend gebied uit.
