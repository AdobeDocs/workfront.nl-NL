---
title: Aangepaste Forms- en objectgegevens exporteren
description: U kunt het overzicht en de aangepaste formuliergegevens vanuit de sectie Details van een object exporteren naar een PDF-bestand. U kunt de PDF vervolgens afdrukken of delen met andere gebruikers.
author: Alina
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 0%

---

# Aangepaste formulieren en objectdetails exporteren

<!--Audited: 10/2025-->

U kunt het overzicht en de aangepaste formuliergegevens vanuit de sectie Details van een object exporteren naar een PDF-bestand. U kunt de PDF vervolgens afdrukken of delen met andere gebruikers.

Deze functionaliteit wordt ondersteund voor de volgende objecten:

* Projecten
* Taken
* Problemen
* Portfolio
* Programma&#39;s

<!--
* Billing records</p> <p>After you open a billing record on a project, you can use the Details area to attach a custom form to the record and fill it out. You can also export billing record information from the Details area.</p> </li>
  -->

>[!NOTE]
>
>De velden in de sectie Details die uw Workfront of groepsbeheerder heeft verwijderd met een lay-outsjabloon, worden niet weergegeven.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-pakket</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-licentie</p> </td> 
   <td><p>Voor problemen:</p>
   <ul><li><p>Medewerker of hoger</p></li>
   <li><p>Aanvrager of hoger</p> </li></ul>
   <p>Voor projecten en taken:</p>
   <ul><li><p>Licht of hoger</p></li>
   <li><p>Revisor of hoger</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Weergave of hoger voor projecten, taken en problemen</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Objectmachtigingen</p> </td> 
   <td> <p>Geef meer of meer machtigingen weer voor het project, de taak of de uitgave waarvan u het formulier wilt exporteren</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Request or higher for issues</p> <p>Review or higher for projects and tasks</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Access level configurations*</strong> </td> 
   <td> <p>View or higher for Projects, Tasks, and Issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> <p>View or higher permissions to the project, task, or issue whose form you want to export</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Vereisten

Voordat u begint, moet u beschikken over alle volgende opties:

1. Er is een aangepast formulier gemaakt voor een specifiek object waaruit u het wilt exporteren.
1. Het aangepaste formulier aan het object laten koppelen

   of

   U hebt de juiste toegang om een aangepast formulier toe te voegen en de gegevens op het formulier te bewerken.

Voor informatie over het creëren van douaneformulieren, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

Voor informatie over het vastmaken van vormen aan voorwerpen, zie [ een douanevorm aan een voorwerp ](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toevoegen.

## Informatie exporteren in de sectie Details

Informatie exporteren uit de sectie Details van een object is identiek voor alle objecten waarvoor dit wordt ondersteund.

1. Ga naar een project, een taak, een portefeuille, een programma, of een kwestie waarvoor u minstens de toestemmingen van de Mening hebt.
1. Klik het **&quot;Details&quot;punt** op het linkerpaneel, zoals **Details van de Taak**.
1. (Facultatief) als er geen douaneformulier in bijlage aan het voorwerp is, begin de naam van een douaneformulier in **te typen voeg douanevormgebied** toe, dan het te klikken wanneer het in de lijst verschijnt.

   U kunt maximaal 10 formulieren toevoegen.

1. (Facultatief) de informatie van de update in de sectie van Details, dan klik **sparen Veranderingen**.
1. Klik het **drop-down menu van de Uitvoer** in de hoger-juiste hoek, uitgezocht **Overzicht**, of de vormen u wilt uitvoeren, dan klik **Uitvoer**.

   U kunt **selecteren allen** ook selecteren als u het gebied van het Overzicht en alle douaneformulieren wilt uitvoeren.

   ![ de knoop van de de douanevorm van de Uitvoer ](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >De volgende scenario&#39;s kunnen bestaan:
   >
   >   * Wanneer uw groep of Workfront-beheerder de selectie van alle velden in het gebied Overzicht opheft en voor het object aangepaste formulieren zijn gekoppeld, wordt de sectie Overzicht niet weergegeven.
   >   * Wanneer uw groep of Workfront-beheerder de selectie van alle velden in het gebied Overzicht opheft en er geen aangepaste formulieren zijn gekoppeld voor het object, is het vervolgkeuzemenu Exporteren niet zichtbaar.
   >   * Als voor het object geen aangepaste formulieren zijn gekoppeld, kunt u alleen het gebied Overzicht exporteren.
   >   * Aangepaste velden die achter logica staan en niet zichtbaar zijn op het formulier, worden niet geëxporteerd. Voor informatie over het toevoegen van logica aan een douaneformulier, zie [ logische regels aan douaneformulieren en gebieden ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md) toevoegen.

   Er wordt een PDF-bestand gemaakt en naar de computer gedownload. Het PDF-bestand bevat de volgende informatie:

   * De naam van het object waaraan het formulier is gekoppeld
   * De naam van de gebruiker die de PDF heeft geëxporteerd
   * Datum en tijdstip waarop de PDF is geproduceerd
   * De naam van de geëxporteerde formulieren
   * Informatie uit de velden die op het formulier zijn ingevuld
