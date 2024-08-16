---
title: Een formulier ontwerpen op basis van een kopie
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: U kunt een aangepast formulier ontwerpen op basis van een kopie met de formulierontwerper.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
source-git-commit: c1bc2832d1c52885e737056172e7aec93a951e6c
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Een formulier ontwerpen op basis van een kopie

U kunt een nieuw aangepast formulier ontwerpen dat is gebaseerd op een bestaand formulier. U kunt aangepaste formulieren aan verschillende Workfront-objecten koppelen om gegevens over die objecten vast te leggen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een aangepast formulier kopiëren om een nieuw formulier te maken

{{step-1-to-setup}}

1. Klik **Aangepaste Forms.**
1. Selecteer de douanevorm die u als basis voor een nieuwe douanevorm wilt gebruiken, dan klik ![ pictogram van het Exemplaar ](assets/copy-icon.png).
1. In het **vakje van het Exemplaar van de Vorm van de Douane** dat verschijnt, typ de volgende informatie:

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
      <td> <p>In het <b> vakje van het Type van Vorm </b>, selecteer de objecten types die u de douanevorm wilt werken met, en klik X naast om het even welke types die u wilt verwijderen. Typen die al aan het formulier zijn gekoppeld, worden in de lijst uitgeschakeld.</p> 
      <p><img src="assets/copy-form-obj-types-040524.png"></p> 
      <p>Het formulier moet aan ten minste één objecttype zijn gekoppeld.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **Exemplaar**.

   Als berekende velden in het oorspronkelijke formulier niet compatibel zijn met een objecttype dat u aan het nieuwe formulier toevoegt, wordt u in een bericht gevraagd de berekeningen in die velden te wijzigen.

   Als een toegangsoptie voor een sectie-einde op het oorspronkelijke formulier niet compatibel is met een objecttype dat u toevoegt aan het nieuwe formulier, wordt u in een bericht gevraagd de optie aan te passen.

1. Selecteer de vorm die u enkel kopieerde, dan klik ![ uitgeven pictogram ](assets/edit-icon.png).
1. Breng om het even welke veranderingen in de vorm aan, zoals die in de volgende secties van het [ Ontwerp een vorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) artikel wordt verklaard:

   * [Een bestaand veld of een bestaande widget opnieuw gebruiken die al in een ander aangepast formulier wordt gebruikt](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
      * [Tekstvelden toevoegen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
      * [Berekende velden toevoegen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
      * [Keuzerondjes, groep selectievakjes en vervolgkeuzelijsten toevoegen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
      * [Velden voor typekop en datum toevoegen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
      * [Afbeeldingen, PDF en video&#39;s toevoegen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
      * [Adobe XD-bestanden toevoegen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)

1. (Facultatief) nadat u **sparen+Close** klikt, maak de vorm aan het voorwerp vast waar u het wilt gebruiken, zoals die in [ wordt beschreven een douaneformulier aan een voorwerp ](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toevoegen.
