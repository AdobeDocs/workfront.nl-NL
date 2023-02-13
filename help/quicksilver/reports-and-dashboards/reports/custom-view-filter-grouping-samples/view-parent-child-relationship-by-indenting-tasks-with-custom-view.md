---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: de ouder-kind verhouding in een taak tonen door de taken in te springen'
description: U kunt het onderscheid tussen bovenliggende en onderliggende relaties in een geëxporteerde takenlijst behouden door een aangepaste weergave toe te voegen aan de takenlijst en ervoor te zorgen dat deze weergave is geselecteerd voordat u de lijst exporteert.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---

# Weergave: de ouder-kind verhouding in een taak tonen door de taken in te springen

U kunt het onderscheid tussen bovenliggende en onderliggende relaties in een geëxporteerde takenlijst behouden door een aangepaste weergave toe te voegen aan de takenlijst en ervoor te zorgen dat deze weergave is geselecteerd voordat u de lijst exporteert.  

![](assets/parent-child-indented-custom-view-350x94.png)

1. Ga naar het project met de taaklijst u zou willen uitvoeren.
1. Klik op de knop **Weergave** en selecteert u **Nieuwe weergave**.

1. Geef het filter een naam in de linkerbovenhoek van het scherm.
1. Klik in het dialoogvenster **Taaknaam** kolomkop.

1. Selecteren **Overschakelen naar tekstmodus** in de rechterbovenhoek.
1. Klik ergens in het tekstvak om tekst te bewerken en alle bestaande tekst te verwijderen.
1. Plak de volgende tekst:

   ```
   displayname=<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br>valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))<br>valueformat=HTML
   ```

1. Klikken **Opslaan**.
1. Klikken **Weergave opslaan**.
