---
product-area: projects
navigation-topic: manage-issues
title: Gebruikerstoewijzingen wijzigen voor meerdere uitgaven in een lijst
description: Gebruikerstoewijzingen wijzigen voor meerdere uitgaven in een lijst
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 0%

---

# Gebruikerstoewijzingen wijzigen voor meerdere uitgaven in een lijst

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

U kunt gebruikerstoewijzingen aan veelvoudige kwesties gelijktijdig wijzigen. Zie ook de volgende artikelen voor informatie over het bewerken van uitgaven of het een voor een toewijzen van uitgaven:

* [&#x200B; geeft kwesties &#x200B;](../../../manage-work/issues/manage-issues/edit-issues.md) uit
* [Problemen toewijzen](../../../manage-work/issues/manage-issues/assign-issues.md)

Voor algemene informatie over het toewijzen van kwesties, zie [&#x200B; Overzicht van het wijzigen van uitgiftetaken &#x200B;](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>U moet ten minste over Contribute-machtigingen beschikken om een uitgave te kunnen toewijzen aan de uitgave.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenties*</td> 
   <td> <p>Nieuw: Standaard </p>
   <p>Huidig: Verzoek of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot problemen bewerken</p> <p>De mening of de hogere toegang tot Projecten en Taken om één kwestie toe te wijzen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het probleem beheren</p> <p>Contribute-machtigingen of hoger voor het project of de taak waar de uitgave zich bevindt, wanneer u meerdere uitgaven toewijst.</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:&nbsp;drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of&nbsp;reasons, including the following:</p>
<ul>
<li>Users join or leave&nbsp;your team</li>
<li>A user takes a vacation that extends beyond the issue&nbsp;due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## Toewijzingen wijzigen voor meerdere problemen

1. Ga naar de lijst van de kwestie die de kwesties bevat waarvan taken u wilt wijzigen.
1. (Optioneel) Maak een filter om alleen uitgaven weer te geven die zijn toegewezen aan de ontvanger die u wilt wijzigen.

   U kunt bijvoorbeeld een filter maken om alleen uitgaven weer te geven die een specifieke rol als toegewezen persoon hebben. Vervolgens kunt u de rol vervangen door een specifieke gebruiker. Ga als volgt te werk:

   1. Klik de **drop-down lijst van de Filter**, dan klik **Nieuwe Filter**.

      Het dialoogvenster Nieuw filter wordt weergegeven.

   1. Klik **toevoegen een Regel van de Filter.**
   1. Om voor een specifieke rol te filtreren, breid **Rollen van de Taak uit,** dan **identiteitskaart**

      of

      Om voor een specifieke gebruiker te filtreren, breid **Gebruikers van de Taak uit,** dan **identiteitskaart**

      >[!TIP]
      >
      >Gebruik niet **Toegewezen aan** omdat dit gebied slechts naar de Eigenaar van de Uitgave en niet naar alle toegewezen verwijst.

   1. In de drop-down lijst, uitgezochte **Gelijk** als filterkwalificatie.
   1. Typ de naam van de gebruiker of rol waarvoor u wilt filteren en klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.
   1. Klik **sparen Filter.**

1. Selecteer de kwesties waarvoor u taken wilt wijzigen, dan klik **uitgeven** pictogram ![&#x200B; uitgeven pictogram &#x200B;](assets/qs-edit-icon.png).

   **geeft Kwesties** vertoningen uit. De items die worden bewerkt, worden in de linkerbovenhoek van de pagina weergegeven.

1. Ga naar de **sectie van Taken**, dan uitgezochte **Ontvanger**.

   ![&#x200B; gebied van Taken &#x200B;](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. Voer een van de volgende handelingen uit:

   1. Een nieuwe ontvanger toevoegen:

      1. Begin de naam van een gebruiker, een rol, of een team te typen, dan het te selecteren wanneer het in de lijst toont. De toewijzing wordt toegevoegd en vervangt de huidige toewijzingen voor de geselecteerde uitgaven niet.

         >[!TIP]
         >
         >U kunt meerdere gebruikers, taakrollen of teams toewijzen. U kunt alleen actieve gebruikers, taakrollen en teams toewijzen.
         >
         >Als een gebruiker, een baanrol, of een team werd toegewezen alvorens zij werden gedeactiveerd, blijven zij toegewezen aan het het werkpunt. In dit geval raden we het volgende aan:
         >
         >* Wijs het werkitem opnieuw toe aan actieve bronnen.
         >* Koppel de gebruikers in een gedeactiveerd team aan een actief team en wijs het het werkpunt aan het actieve team opnieuw toe.

         Informatie die algemeen is voor alle geselecteerde uitgaven, wordt weergegeven. Bijvoorbeeld, als de zelfde gebruiker aan alle kwesties wordt toegewezen, toont die gebruiker in de **Assignee** kolom. Als er geen algemene informatie wordt weergegeven over de geselecteerde problemen.

   1. Afzonderlijke toewijzingen verwijderen:

      1. Klik het **pictogram van X** naast de naam van de ontvanger die u wilt verwijderen als de bestemmingsvertoningen in de lijst van Taken.

         of

         (Voorwaardelijk) als de ontvanger die u wilt verwijderen niet in de sectie van Taken toont omdat de ontvanger aan slechts enkele kwesties wordt toegewezen die u hebt geselecteerd, **verwijdert Assignee** en begint de naam van de ontvanger te typen die u wilt verwijderen, dan klikken de naam wanneer het in de drop-down lijst verschijnt.

      1. Klik **verwijder opnieuw Ontvanger** om een andere te verwijderen ontvanger toe te voegen.

   1. Alle bestaande toewijzingen verwijderen:

      1. Klik **verwijderen Alle Bestaande Toewijzers**, dan klik **ja, schrap Alle Toewijzers**.

         Hierdoor worden niet alleen algemene toewijzingen (toewijzingen die in het dialoogvenster Bewerken worden weergegeven), maar ook alle toewijzingen voor alle geselecteerde problemen verwijderd.

1. (Optioneel) Wijzig een of meer van de volgende opties voor de toewijzingen die u hebt geselecteerd om aan de problemen te koppelen:

   * **Eigenaar van de Uitgave:** selecteer het radioknoop om erop te wijzen welke ontvanger als Eigenaar van Uitgave wordt aangewezen. Als deze optie niet is geselecteerd, wijst Adobe Workfront de eerste toegewezen persoon aan als de eigenaar van de uitgave. Dit is niet beschikbaar voor teamtoewijzingen.
   * **Rol van de Ontvanger**: Selecteer een rol van de drop-down lijst. Als deze optie niet is geselecteerd, selecteert Workfront automatisch de primaire rol van de gebruiker.

1. Klik **sparen Veranderingen**.
