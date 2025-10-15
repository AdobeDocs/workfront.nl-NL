---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergeven: Documentrapport met koppeling naar proefafdruk'
description: 'Weergeven: documentrapport met koppeling naar proefdruk'
author: Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Weergeven: documentrapport met koppeling naar proefdruk

<!--Audited: 11/2024-->

In deze documentweergave kunt u een koppeling invoegen naar een proefdruk van de huidige versie van het document.

![ document van de Mening met proefdruk verbinding ](assets/view-document-with-proof-link-350x92.png)

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
   <p>Medewerker of verzoek om een filter te wijzigen </p>
   <p>Standaard of Plan om een rapport te wijzigen</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een documentrapport weergeven met koppeling naar een proefdruk

Deze weergave toepassen:

1. Ga naar een lijst met documenten.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.
1. Klik **toevoegen Kolom**.
1. Klik **Schakelaar aan de Wijze van de Tekst**, dan **geef de Wijze van de Tekst** uit.
1. Verwijder de tekst u in **vindt geef de Wijze van de Tekst** vakje uit, en vervang het met de volgende code:

   ```
   displayname=Proof Link
   shortview=true
   textmode=true
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Vervang &quot;Uw domein&quot; door uw Workfront-domein. Bijvoorbeeld, als URL van Workfront van uw bedrijf *Company.my.workfront.com* is, is uw domein &quot;Bedrijf.&quot;

1. Klik **Gedaan**, dan **sparen Mening**.
1. (Facultatief) werk de meningsnaam bij, dan klik **sparen Mening**.
1. (Optioneel) Als u alleen documenten met proefdrukken wilt weergeven, voegt u een filter toe door het volgende te doen:

   1. Klik het **drop-down menu van de Filter**, dan klik **Nieuwe Filter**.
   1. Klik **toevoegen een Regel van de Filter** en beginnen &quot;Eigenaar van het Bewijs&quot;te typen, dan uitgezochte **identiteitskaart van de Eigenaar van het Bewijs** wanneer het in de lijst toont.
   1. Selecteer **is niet leeg** voor de filterbepaling.
   1. Klik **sparen Filter**.
   1. (Facultatief) werk de filternaam bij, dan klik **sparen Filter**.

1. Klik op de koppeling in de kolom Proefkoppeling voor toegang tot de proefdruk van de laatste versie van het document.
