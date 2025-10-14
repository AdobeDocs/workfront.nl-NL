---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: de relatie tussen bovenliggende en onderliggende items weergeven in een taak door de taken in te springen'
description: U kunt het onderscheid tussen bovenliggende en onderliggende relaties in een geëxporteerde takenlijst behouden door een aangepaste weergave toe te voegen aan de takenlijst en ervoor te zorgen dat deze weergave is geselecteerd voordat u de lijst exporteert.
author: Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Weergave: de relatie bovenliggend-onderliggend item in een taak weergeven door de taken in te springen

<!--Audited: 11/2024-->

U kunt het onderscheid tussen bovenliggende en onderliggende relaties in een geëxporteerde takenlijst behouden door een aangepaste weergave toe te voegen aan de takenlijst en ervoor te zorgen dat deze weergave is geselecteerd voordat u de lijst exporteert.

![&#x200B; de kindinspringing van de Ouder &#x200B;](assets/parent-child-indented-custom-view-350x94.png)

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p> Huidige: 
   <ul>
   <li>Verzoek om een weergave te wijzigen</li> 
   <li>Plan om een rapport te wijzigen</li>
   </ul>
     </p>
     <p> Nieuw: 
   <ul>
   <li>Medewerker om een weergave te wijzigen</li> 
   <li>Standaard voor het wijzigen van een rapport</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Toon de ouder-kind verhouding in een taak door de taken in te springen

1. Ga naar het project met de taaklijst u zou willen uitvoeren.
1. Klik het **drop-down menu van de Mening**, en selecteer **Nieuwe Mening**.
1. Klik in de **kolomkopbal 0&rbrace; Naam van de Taak &lbrace;.**
1. Selecteer **Schakelaar aan de Wijze van de Tekst** in de hoger-juiste hoek.
1. Klik **uitgeven de Wijze van de Tekst** en verwijder al bestaande tekst.
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

1. Klik **Gedaan** > **sparen Mening**.
