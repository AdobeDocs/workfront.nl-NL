---
user-type: administrator
product-area: system-administration
keywords: maken,aangepast,formulier,kopiëren,basis,een ander
navigation-topic: create-and-manage-custom-forms
title: Een aangepast formulier kopiëren om een nieuw formulier te maken met de verouderde builder
description: U kunt een nieuw aangepast formulier maken dat is gebaseerd op een bestaand formulier.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 946a726e-af88-413c-abe3-55fbc7486380
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Een aangepast formulier kopiëren om een nieuw formulier te maken met de verouderde builder

<span class="preview">De gemarkeerde informatie op deze pagina verwijst naar functionaliteit die nog niet algemeen beschikbaar is. Deze functie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten of in de productieomgeving voor klanten die snelle releases hebben ingeschakeld.</span>

<span class="preview">Voor informatie over snelle versies raadpleegt u [Snelle releases voor uw organisatie in- of uitschakelen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Voor informatie over de huidige versie raadpleegt u [Overzicht tweede release 2024, tweede kwartaal](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

U kunt een nieuw aangepast formulier maken dat is gebaseerd op een bestaand formulier.

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-plan</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
   <p>Nieuw: Standaard</p>
   <p>of</p>
   <p>Huidig: Plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Een aangepast formulier kopiëren om een nieuw formulier te maken

{{step-1-to-setup}}

1. Klikken **Aangepaste Forms.**
1. Selecteer het aangepaste formulier dat u als basis voor een nieuw aangepast formulier wilt gebruiken en klik op **Kopiëren** <span class="preview">of ![Pictogram kopiëren](assets/copy-icon.png).</span>
1. In de **Aangepast formulier kopiëren** Typ de volgende informatie in het vak dat wordt weergegeven:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Formuliernaam</td> 
      <td>Typ een naam voor het gekopieerde formulier.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Formuliertypen </p> </td> 
      <td> <p>In de <b>Formuliertype</b> Selecteer de objecttypen waarmee u het aangepaste formulier wilt bewerken en klik op de X naast de typen die u wilt verwijderen. Typen die al aan het formulier zijn gekoppeld, worden in de lijst uitgeschakeld.</p> 
      <p><img src="assets/copy-form-obj-types.png"></p> 
      <p>Het formulier moet aan ten minste één objecttype zijn gekoppeld.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Formulier kopiëren**.

   Als berekende velden in het oorspronkelijke formulier niet compatibel zijn met een objecttype dat u aan het nieuwe formulier toevoegt, wordt u in een bericht gevraagd de berekeningen in die velden te wijzigen.

   Als een toegangsoptie voor een sectie-einde op het oorspronkelijke formulier niet compatibel is met een objecttype dat u toevoegt aan het nieuwe formulier, wordt u in een bericht gevraagd de optie aan te passen.

1. Selecteer het formulier dat u net hebt gekopieerd en klik op **Bewerken**.
1. Breng wijzigingen aan in het formulier, zoals wordt uitgelegd in de volgende artikelen:

   * [Een aangepast formulier kopiëren om een nieuw formulier te maken met de oudere formulierbuilder](#Add2)
   * [Berekende gegevens toevoegen aan een aangepast formulier met de oudere formulierbuilder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Aangepaste velden en widgets in een aangepast formulier plaatsen met de oudere formulierbuilder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Een elementwidget toevoegen of bewerken in een aangepast formulier met de verouderde formulierbuilder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Een bestaand berekend aangepast veld opnieuw gebruiken in een aangepast formulier met de oudere formulierbuilder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Weergavelogica toevoegen en logica overslaan naar een aangepast formulier met de oudere formulierbuilder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Een aangepast formulier voorvertonen en invullen met de oudere formulierbuilder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

1. (Optioneel) Klik op **Opslaan en sluiten** voegt u het formulier toe aan het object waar u het wilt gebruiken, zoals wordt beschreven in [Een aangepast formulier toevoegen aan een object](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
