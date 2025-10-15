---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: Percentage gebruikersrol van FTE-beschikbaarheid'
description: U kunt een kolom aan de mening van een gebruikerslijst toevoegen om een lijst van de Rollen van de Baan te tonen de gebruiker met evenals het percentage van VTE beschikbaarheid voor elke baanrol wordt geassocieerd, zoals die in het gebruikersprofiel wordt bepaald.
author: Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Weergave: percentage gebruikersrol van FTE-beschikbaarheid

<!--Audited: 11/2024-->

U kunt een kolom aan de mening van een gebruikerslijst toevoegen om een lijst van de Rollen van de Baan te tonen de gebruiker met evenals het percentage van VTE beschikbaarheid voor elke baanrol wordt geassocieerd, zoals die in het gebruikersprofiel wordt bepaald.

Voor informatie over het bepalen van het percentage van VTE beschikbaarheid voor gebruikers, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

![ user_with_percent_avialbility_per_role.png ](assets/user-with-percent-avialbility-per-role-350x138.png)

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Medewerker of verzoek om een weergave te wijzigen </p>
   <p>Standaard of Plan om een rapport te wijzigen</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


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
