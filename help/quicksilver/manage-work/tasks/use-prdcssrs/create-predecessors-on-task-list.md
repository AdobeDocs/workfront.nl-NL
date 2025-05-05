---
product-area: projects
navigation-topic: use-predecessors
title: Een voorganger-relatie maken in de takenlijst
description: U kunt voorgangstaken (of alleen voorgangers) gebruiken om taken te koppelen die afhankelijk zijn van andere taken die moeten worden gestart of voltooid. U wilt bijvoorbeeld geen partij (afhankelijke taak) hosten voordat u de uitnodigingen (voorgangstaak) verzendt.
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---

# Een voorganger-relatie maken in de takenlijst

U kunt voorgangstaken (of alleen voorgangers) gebruiken om taken te koppelen die afhankelijk zijn van andere taken die moeten worden gestart of voltooid. U wilt bijvoorbeeld geen partij (afhankelijke taak) hosten voordat u de uitnodigingen (voorgangstaak) verzendt.

In dit artikel ziet u hoe u voorgangers in de takenlijst kunt maken.

U kunt de voorgangers van taken in de volgende gebieden van Adobe Workfront bekijken:

* In de takenlijst in de kolom Predecessors.
* In de Gantt-grafiek
* In de sectie Predecessors van een afhankelijke taak

Voor meer informatie, zie [ Overzicht van taakvoordecessors ](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Toegangsvereisten

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
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuw: Standaard </p><p>Huidig: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de taken en het project beheren</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront. Voor meer informatie over toegangsvereisten, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Een voorganger maken

1. Ga naar een project.
1. Klik **Taken** in het linkerpaneel.
1. Zorg ervoor dat uw huidige mening de **Predecessor** kolom toont.

   Als de mening niet de kolom van Predecessors toont, verander in een mening die, of voeg de kolom aan uw mening toe.

1. Selecteer de taak die u als afhankelijke taak wilt aanwijzen.
1. Klik binnen de **Predecessors** kolom.
1. Typ het taakaantal dat u als voorganger van de geselecteerde taak wilt aanwijzen, dan druk **binnengaan**.

   >[!TIP]
   >
   >Ga als volgt te werk om een voorganger voor meerdere projecten toe te voegen:
   >
   >1. Klik het **pictogram van de Wijze van het Plan** en kies **Autosave**.
   >
   >1. Typ het referentienummer van het project van de voorganger gevolgd door een dubbele punt en het nummer van de taak. Bijvoorbeeld: 765021:12. Dit wijst erop dat het Aantal van de Verwijzing van het project van de voorganger 765021 is en voorganger taaantal 12 op het project is.
   >
   >1. Voeg het gebiedstype voor deze voorganger toe. Voor meer informatie, zie [ tot dwars-project predecessors ](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md) leiden.
   >
   >Pers **gaat** binnen.
   >
   >**BELANGRIJK**
   >
   >U kunt geen voorganger voor meerdere projecten toevoegen wanneer de taaklijst wordt weergegeven in de modus Handmatig opslaan.

   Het voorgangspictogram wordt groen als de voorganger de markering Voltooid heeft. Dit wijst erop dat de afhankelijke taak klaar voor het werk is.

   Voor meer informatie over de relatietypen beschikbaar in de kolom Predecessors, zie [ Overzicht van taakvoordecessors ](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) in [ Overzicht van taakvoordecessors ](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Details voorganger weergeven

U kunt snel details over de voorganger bekijken in de takenlijst.

1. Voor de taaklijst, houd over het voorgangersaantal in de **1&rbrace; kolom van Predecessors &lbrace;.**

   Er verschijnt een vak met de details van de voorganger.

   ![ Details van de Predecessor ](assets/predecessor-details-in-task-list.png)

   De volgende details worden weergegeven:

   **naam van de Voorganger:** De naam van predecessor die van verwijzingen wordt voorzien. Het taaknummer van de voorganger wordt opgenomen. Klik op de taaknaam om deze te openen. In het bovenstaande voorbeeld is de voorganger Productie/Uitvoering/Levering.

   **naam van het Project:** De naam van het project waar predecessor verblijft. Het project wordt geïdentificeerd als het huidige project als predecessor tot de zelfde projecten zoals de taak, of als dwars project behoort, als predecessor tot een verschillend project behoort. In het bovenstaande voorbeeld is de projectnaam Digital Asset Production (Integrated) - Project. Voor meer informatie over dwars-project predecessors, zie [ creëren dwars-project predecessors ](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   U kunt de projectdetails uitbreiden om de geplande begin en einddata van het project, voorwaarde, status, volledig percentage, en eigenaar te zien. Voor een dwars project, kunt u **dan klikken zie Project** om het project te openen.

   **identiteitskaart:** het aantal van de Verwijzing van het project waar predecessor wordt gevestigd.

   **Geplande Begin:** de Geplande Datum van het Begin van de voorgangstaak.

   **Geplande Eind:** de Geplande Datum van de Voltooiing van de voorgangstaak.

   **Aantal predecessors:** het aantal voordecessors voor voorganger die van verwijzingen worden voorzien. In het bovenstaande voorbeeld heeft de voorganger waarnaar wordt verwezen 1 voorganger.

   **Aantal opvolgers:** het aantal opvolger (of afhankelijke) taken voor voorganger die van verwijzingen worden voorzien. In het bovenstaande voorbeeld heeft de voorganger waarnaar wordt verwezen 1 opvolger.
