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

Zie voor meer informatie [Overzicht van voorgangers van taken](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt. Voor meer informatie over toegangsvereisten, zie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Een voorganger maken

1. Ga naar een project.
1. Klikken **Taken** in het linkerdeelvenster.
1. Zorg ervoor dat de huidige weergave de **Voorganger** kolom.

   Als de mening niet de kolom van Predecessors toont, verander in een mening die, of voeg de kolom aan uw mening toe.

1. Selecteer de taak die u als afhankelijke taak wilt aanwijzen.
1. Klik in het dialoogvenster **Predecessors** kolom.
1. Typ het taakaantal dat u als voorganger van de geselecteerde taak wilt aanwijzen, dan druk **Enter**.

   >[!TIP]
   >
   >Ga als volgt te werk om een voorganger voor meerdere projecten toe te voegen:
   >
   >1. Klik op de knop **Abonnementsmodus** pictogram en kies **Automatisch opslaan**.
   >
   >1. Typ het referentienummer van het project van de voorganger gevolgd door een dubbele punt en het nummer van de taak. Bijvoorbeeld: 765021:12. Dit wijst erop dat het Aantal van de Verwijzing van het project van de voorganger 765021 is en voorganger taaantal 12 op het project is.
   >
   >1. Voeg het gebiedstype voor deze voorganger toe. Zie voor meer informatie [Predecessors voor meerdere projecten maken](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
   >
   >Druk **Enter**.
   >
   >**BELANGRIJK**
   >
   >U kunt geen voorganger voor meerdere projecten toevoegen wanneer de taaklijst wordt weergegeven in de modus Handmatig opslaan.

   Het voorgangspictogram wordt groen als de voorganger de markering Voltooid heeft. Dit wijst erop dat de afhankelijke taak klaar voor het werk is.

   Voor meer informatie over de relatietypen beschikbaar in de kolom Predecessors, zie [Overzicht van voorgangers van taken](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) in [Overzicht van voorgangers van taken](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Details voorganger weergeven

U kunt snel details over de voorganger bekijken in de takenlijst.

1. Houd de muisaanwijzer in de takenlijst boven het vorige nummer in het dialoogvenster **Predecessors** kolom.

   Er verschijnt een vak met de details van de voorganger.

   ![Details voorganger](assets/predecessor-details-in-task-list.png)

   De volgende details worden weergegeven:

   **Naam voorganger:** De naam van de voorganger waarnaar wordt verwezen. Het taaknummer van de voorganger wordt opgenomen. Klik op de taaknaam om deze te openen. In het bovenstaande voorbeeld is de voorganger Productie/Uitvoering/Levering.

   **Projectnaam:** De naam van het project waar de voorganger verblijft. Het project wordt geïdentificeerd als het huidige project als predecessor tot de zelfde projecten zoals de taak, of als dwars project behoort, als predecessor tot een verschillend project behoort. In het bovenstaande voorbeeld is de projectnaam Digital Asset Production (Integrated) - Project. Voor meer informatie over predecessors voor meerdere projecten raadpleegt u [Predecessors voor meerdere projecten maken](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   U kunt de projectdetails uitbreiden om de geplande begin en einddata van het project, voorwaarde, status, volledig percentage, en eigenaar te zien. Voor een cross-project kunt u vervolgens op **Zie Project** om het project te openen.

   **ID:** Het referentienummer van het project waar de voorganger zich bevindt.

   **Geplande start:** De geplande begindatum van de voorgaande taak.

   **Gepland uiteinde:** De geplande voltooiingsdatum van de voorgangstaak.

   **Aantal voorgangers:** Het aantal voordecessors voor de voorganger waarnaar wordt verwezen. In het bovenstaande voorbeeld heeft de voorganger waarnaar wordt verwezen 1 voorganger.

   **Aantal opvolgers:** Het aantal (of afhankelijke) opvolgertaken voor de voorganger waarnaar wordt verwezen. In het bovenstaande voorbeeld heeft de voorganger waarnaar wordt verwezen 1 opvolger.
