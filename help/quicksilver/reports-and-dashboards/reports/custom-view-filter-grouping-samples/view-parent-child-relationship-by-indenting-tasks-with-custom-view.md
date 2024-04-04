---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: de relatie bovenliggend-onderliggend weergeven in een taak door de taken in te springen'
description: U kunt het onderscheid tussen bovenliggende en onderliggende relaties in een geëxporteerde takenlijst behouden door een aangepaste weergave toe te voegen aan de takenlijst en ervoor te zorgen dat deze weergave is geselecteerd voordat u de lijst exporteert.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 0483230c5d8b7d33f420c6c5f09c4a5aafe37f37
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Weergave: de relatie bovenliggend-onderliggend item in een taak weergeven door de taken in te springen

U kunt het onderscheid tussen bovenliggende en onderliggende relaties in een geëxporteerde takenlijst behouden door een aangepaste weergave toe te voegen aan de takenlijst en ervoor te zorgen dat deze weergave is geselecteerd voordat u de lijst exporteert.

![](assets/parent-child-indented-custom-view-350x94.png)

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
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Toon de ouder-kind verhouding in een taak door de taken in te springen

1. Ga naar het project met de taaklijst u zou willen uitvoeren.
1. Klik op de knop **Weergave** en selecteert u **Nieuwe weergave**.

1. Geef het filter een naam in de linkerbovenhoek van het scherm.
1. Klik in het dialoogvenster **Taaknaam** kolomkop.

1. Selecteren **Overschakelen naar tekstmodus** in de rechterbovenhoek.
1. Klik ergens in het tekstvak om tekst te bewerken en alle bestaande tekst te verwijderen.
1. Plak de volgende tekst:


```
   displayname=
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))
   valueformat=HTML
```

1. Klikken **Opslaan**.
1. Klikken **Weergave opslaan**.
