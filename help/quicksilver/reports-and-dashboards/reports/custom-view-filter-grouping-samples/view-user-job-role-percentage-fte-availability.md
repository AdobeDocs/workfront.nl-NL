---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: percentage gebruikersrol van beschikbare FTE-gegevens'
description: U kunt een kolom aan de mening van een gebruikerslijst toevoegen om een lijst van de Rollen van de Baan te tonen de gebruiker met evenals het percentage van VTE beschikbaarheid voor elke baanrol wordt geassocieerd, zoals die in het gebruikersprofiel wordt bepaald.
author: Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 66de6c952272f52876f8e912c96d1526575b6f0b
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Weergave: percentage gebruikersrol van FTE-beschikbaarheid

<!--Audited: 11/2024-->

U kunt een kolom aan de mening van een gebruikerslijst toevoegen om een lijst van de Rollen van de Baan te tonen de gebruiker met evenals het percentage van VTE beschikbaarheid voor elke baanrol wordt geassocieerd, zoals die in het gebruikersprofiel wordt bepaald.

Voor informatie over het bepalen van het percentage van VTE beschikbaarheid voor gebruikers, zie [&#x200B; het profiel van een gebruiker &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

![&#x200B; user_with_percent_avialbility_per_role.png &#x200B;](assets/user-with-percent-avialbility-per-role-350x138.png)

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

## Het percentage van de Rol van de Taak van de gebruiker van de Mening van VTE beschikbaarheid

1. Ga naar een lijst met gebruikers.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, klik **voegt Kolom** toe.

1. Klik de kopbal van de nieuwe kolom, dan klik **Schakelaar aan de Wijze van de Tekst** > **geeft de Wijze van de Tekst** uit.
1. Verwijder de tekst u in **vindt geef de Wijze van de Tekst** vakje uit, en vervang het met de volgende code:

   ```
   displayname=Roles Time Percentage
   listdelimiter=
   listmethod=nested(userRoles).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({role},'-',{timePercentage},'%')
   valueformat=HTML
   ```

1. Klik **Gedaan**, dan **sparen Mening**.

1. (Facultatief) werk de meningsnaam bij, dan klik **sparen Mening**.
