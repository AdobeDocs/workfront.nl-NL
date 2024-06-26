---
title: Een formulier ontwerpen op basis van een kopie met de formulierontwerper
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: U kunt een aangepast formulier ontwerpen op basis van een kopie met de formulierontwerper.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
source-git-commit: df6b1e4b362807025f3edb5298e8445c0d44ec69
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Een formulier ontwerpen op basis van een kopie met de formulierontwerper

U kunt een nieuw aangepast formulier ontwerpen dat is gebaseerd op een bestaand formulier. U kunt aangepaste formulieren aan verschillende Workfront-objecten koppelen om gegevens over die objecten vast te leggen.

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
1. Selecteer het aangepaste formulier dat u als basis voor een nieuw aangepast formulier wilt gebruiken en klik op ![Pictogram kopiëren](assets/copy-icon.png).
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
      <p><img src="assets/copy-form-obj-types-040524.png"></p> 
      <p>Het formulier moet aan ten minste één objecttype zijn gekoppeld.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Kopiëren**.

   Als berekende velden in het oorspronkelijke formulier niet compatibel zijn met een objecttype dat u aan het nieuwe formulier toevoegt, wordt u in een bericht gevraagd de berekeningen in die velden te wijzigen.

   Als een toegangsoptie voor een sectie-einde op het oorspronkelijke formulier niet compatibel is met een objecttype dat u toevoegt aan het nieuwe formulier, wordt u in een bericht gevraagd de optie aan te passen.

1. Selecteer het formulier dat u net hebt gekopieerd en klik op ![Pictogram Bewerken](assets/edit-icon.png).
1. Breng wijzigingen aan in het formulier, zoals wordt uitgelegd in de volgende secties van het dialoogvenster [Een formulier ontwerpen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) artikel:

   * [Een bestaand veld of een bestaande widget opnieuw gebruiken die al in een ander aangepast formulier wordt gebruikt](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
      * [Tekstvelden toevoegen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
      * [Berekende velden toevoegen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
      * [Keuzerondjes, groep selectievakjes en vervolgkeuzelijsten toevoegen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
      * [Velden voor typekop en datum toevoegen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
      * [Afbeeldingen, PDF en video&#39;s toevoegen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
      * [Adobe XD-bestanden toevoegen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)

1. (Optioneel) Klik op **Opslaan en sluiten** voegt u het formulier toe aan het object waar u het wilt gebruiken, zoals wordt beschreven in [Een aangepast formulier toevoegen aan een object](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
