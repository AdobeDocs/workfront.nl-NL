---
content-type: reference
product-area: reporting
keywords: audit,trail,custom,field
navigation-topic: calculate-custom-data-reports
title: "Voorbeeld van een berekend aangepast veld: bewerkingsgeschiedenis van een veld weergeven"
description: Als gebruikers regelmatig aangepaste velden bijwerken en u wilt een logboek vastleggen van alle wijzigingen die in een veld zijn aangebracht en ook een datum waarop de wijzigingen worden aangebracht, kunt u deze gegevens vastleggen in een berekend aangepast veld.
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 0%

---

# Voorbeeld van een berekend aangepast veld: bewerkingsgeschiedenis van een veld weergeven

Als gebruikers regelmatig aangepaste velden bijwerken en u wilt een logboek vastleggen van alle wijzigingen die in een veld zijn aangebracht en ook een datum waarop de wijzigingen worden aangebracht, kunt u deze gegevens vastleggen in een berekend aangepast veld.

Het volgende voorbeeld toont u hoe te om de *Instructies te bouwen geeft Geschiedenis* berekend gebied uit om al verandering te vangen die aan een single-line tekstgebied wordt aangebracht genoemd *Instructies*.

>[!TIP]
>
>U kunt dit voorbeeld volgen voor alle typen aangepaste velden, niet alleen voor tekstvelden van één regel.

Dit doet het volgende: 

* Beperkt het *gebied van de Instructies geeft Geschiedenis* tot meest recente 2000 karakters uit om binnen de het gegevensbestandgrens van Workfront te blijven.
* Controleert als de huidige waarde van het *gebied van Instructies* de voorzijde van de *Instructies geeft de waarde van de Geschiedenis* uit; het veronderstelt het leeg is en als het niet is, doet het het volgende: 

   * Als zij aanpassen, verlaat het *Instructies geeft Geschiedenis* uit zoals is;
   * Als zij niet aanpassen, vervangt het *Instructies geeft Geschiedenis* met de recentste waarde in het *gebied van Instructies* uit, die door de huidige datum tussen haakjes, een verticale bar wordt gevolgd, en de vorige *Instructies geeft Geschiedenis* uit, die de vorige waarde(n) en de datum (s) bewaart toen zij werden ingegaan.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-abonnement*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td> <p>Workfront-licentie*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong> het niveauconfiguraties van de Toegang* </strong> </td> 
   <td> <p>Administratieve toegang tot Aangepaste Forms</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> de toestemmingen van Objecten </strong> </p> </td> 
   <td> <p>Rechten voor aangepaste formulieren beheren </p> <p>Voor meer informatie, zie <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref"> een douanevorm </a> delen.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## Vereisten

Als u een berekend veld met de bewerkingsgeschiedenis van een veld wilt toevoegen aan een aangepast formulier, moet u eerst het volgende doen:

* Het aangepaste formulier maken
* Het veld met de geschiedenis die u wilt vastleggen toevoegen aan het aangepaste formulier

## De bewerkingsgeschiedenis van een veld weergeven

1. Ga naar een aangepast formulier waaraan u het berekende veld wilt toevoegen.

1. Ga als volgt te werk om bijvoorbeeld het aangepaste tekstveld voor een enkele regel te maken:

   1. Klik **Enige Gebied van de Tekst van de Lijn**.
   1. Specificeer a **Etiket** voor het douanegebied, zoals *Instructies*.
   1. Klik **Toepassing**.

1. Selecteer **een gebied** toevoegen, dan uitgezocht **Berekend** om een berekend douanegebied aan de vorm toe te voegen.
1. Specificeer a **Etiket** voor het berekende douanegebied, zoals *de Instructies uitgeven Geschiedenis*.

   Dit is het gebied dat om het even welke veranderingen zal vangen die aan het eerste gebied worden aangebracht u (*Instructies*) creeerde.

1. Klik **sparen + Sluiten**.
1. Klik op de naam van het formulier waaraan u twee velden hebt toegevoegd om het formulier opnieuw te openen.
1. Klik de berekende instructies van het douanegebied *uitgeven Geschiedenis,* dan kopiëren en kleef het volgende in de doos van de Berekening:
1. Op het **gebied van de Berekening**, specificeer de volgende berekening voor uw douanegebied:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Geadviseerd) Deeg de zelfde berekening in het **gebied van Instructies** op het berekende gebied op de vorm.
1. Controleer of  **Tekst** wordt geselecteerd op het **3} gebied van het Formaat {om het berekende douanegebied als tekst te formatteren.**

   Dit is de standaardinstelling.

1. Klik **sparen+Sluiten**.

   Nu, wanneer u de douanevorm aan een voorwerp vastmaakt en dan verandert iemand de informatie in het *gebied van Instructies*, geeft het *Instructies uitgeeft Geschiedenis&quot;gebied de recentste waarde uit, die door de huidige datum tussen haakjes, en een verticale bar wordt gevolgd. Als er verdere wijzigingen worden aangebracht, worden deze op dezelfde manier aan deze informatie toegevoegd.

   In de bovengenoemde berekening, kunt u *Instructies* met de nauwkeurige naam van uw enig-lijntekstgebied vervangen de waarvan geschiedenis u wilt volgen, en *de Instructies geven Geschiedenis* met de nauwkeurige naam van uw berekend gebied uit.
