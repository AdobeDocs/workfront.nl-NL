---
content-type: reference
product-area: reporting
keywords: audit,trail,custom,field
navigation-topic: calculate-custom-data-reports
title: "Voorbeeld van berekend aangepast veld: de bewerkingsgeschiedenis van een veld weergeven"
description: Als gebruikers regelmatig aangepaste velden bijwerken en u wilt een logboek vastleggen van alle wijzigingen die in een veld zijn aangebracht en ook een datum waarop de wijzigingen worden aangebracht, kunt u deze gegevens vastleggen in een berekend aangepast veld.
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# Voorbeeld van berekend aangepast veld: de bewerkingsgeschiedenis van een veld weergeven

Als gebruikers regelmatig aangepaste velden bijwerken en u wilt een logboek vastleggen van alle wijzigingen die in een veld zijn aangebracht en ook een datum waarop de wijzigingen worden aangebracht, kunt u deze gegevens vastleggen in een berekend aangepast veld.

In het volgende voorbeeld wordt getoond hoe u de *Instructies Geschiedenis bewerken* berekend veld om alle wijzigingen vast te leggen die zijn aangebracht in een tekstveld van één regel, genaamd *Instructies*.

>[!TIP]
>
>U kunt dit voorbeeld volgen voor alle typen aangepaste velden, niet alleen voor tekstvelden van één regel.

Dit doet het volgende: 

* Beperkt de *Instructies Geschiedenis bewerken* tot de meest recente 2000 tekens om binnen de Workfront-databaselimiet te blijven.
* Controleert of de huidige waarde van de *Instructies* komt overeen met de voorzijde van het veld *Instructies Geschiedenis bewerken* waarde; zij gaat ervan uit dat deze leeg is en doet het volgende indien dit niet het geval is: 

   * Als ze overeenkomen, wordt de *Instructies Geschiedenis bewerken* ongewijzigd;
   * Als ze niet overeenkomen, worden de *Instructies Geschiedenis bewerken* met de meest recente waarde in de *Instructies* veld, gevolgd door de huidige datum tussen haakjes, een verticale balk en de vorige *Instructies Geschiedenis bewerken*, waarbij de vorige waarde(n) en de datum(s) waarop ze werden ingevoerd, behouden blijven.

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
   <td><strong>Configuraties op toegangsniveau*</strong> </td> 
   <td> <p>Administratieve toegang tot aangepaste Forms</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Objectmachtigingen</strong> </p> </td> 
   <td> <p>Machtigingen beheren voor de aangepaste formulieren </p> <p>Zie voor meer informatie <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Een aangepast formulier delen</a>.<br></p> </td> 
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

   1. Klikken **Tekstveld met één regel**.
   1. Geef een **Label** voor het aangepaste veld, zoals *Instructies*.
   1. Klikken **Applye**.

1. Selecteren **Veld toevoegen** selecteert u vervolgens **Berekend** om een berekend aangepast veld aan het formulier toe te voegen.
1. Geef een **Label** voor het berekende aangepaste veld, zoals *Instructies Geschiedenis bewerken*.

   Dit is het veld waarin eventuele wijzigingen worden vastgelegd die zijn aangebracht in het eerste veld dat u hebt gemaakt (*Instructies*).

1. Klikken **Opslaan + Sluiten**.
1. Klik op de naam van het formulier waaraan u twee velden hebt toegevoegd om het formulier opnieuw te openen.
1. Klik op het berekende aangepaste veld *Instructies Geschiedenis bewerken,* Kopieer en plak vervolgens het volgende in het vak Berekening:
1. In de **Berekening** geeft u de volgende berekening voor uw aangepaste veld op:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Aanbevolen) Plak dezelfde berekening in de **Instructies** in het berekende veld op het formulier.
1. Controleer of  **Tekst** is geselecteerd in het dialoogvenster **Indeling** veld voor het opmaken van het berekende aangepaste veld als tekst.

   Dit is de standaardinstelling.

1. Klikken **Opslaan en sluiten**.

   Wanneer u het aangepaste formulier nu aan een object koppelt en vervolgens de gegevens in het dialoogvenster *Instructies* in het veld *Instructies > Geschiedenis bewerken&quot; wordt de laatste waarde weergegeven, gevolgd door de huidige datum tussen haakjes en een verticale balk. Als er verdere wijzigingen worden aangebracht, worden deze op dezelfde manier aan deze informatie toegevoegd.

   In de bovenstaande berekening kunt u *Instructies* met de exacte naam van het tekstveld van één regel waarvan u de geschiedenis wilt bijhouden, en *Instructies Geschiedenis bewerken* met de exacte naam van het berekende veld.
