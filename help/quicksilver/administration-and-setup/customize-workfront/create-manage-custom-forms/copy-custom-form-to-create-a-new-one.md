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
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Een aangepast formulier kopiëren om een nieuw formulier te maken met de verouderde builder

{{form-designer-default}}

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

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

1. Selecteer de vorm die u enkel kopieerde, dan klik **uitgeven**.
1. Breng wijzigingen aan in het formulier, zoals wordt uitgelegd in de volgende artikelen:

   * [ Kopieer een douaneformulier om nieuwe tot stand te brengen met de erfenisvormbouwer ](#Add2)
   * [ voeg berekende gegevens aan een douanevorm met de bouwer van de erfenisvorm toe ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [ de douanegebieden en widgets van de Positie in een douanevorm met de bouwer van de erfenis ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [ voeg of geef activa widget in een douanevorm met de erfenisvormbouwer toe uit ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [ hergebruik een bestaand berekend douanegebied in een douanevorm met de bouwer van de erfenisvorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [ voegt vertoningslogica en overslaat logica aan een douanevorm met de bouwer van de erfenisvorm toe ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Een aangepast formulier voorvertonen en invullen met de oudere formulierbuilder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

1. (Facultatief) nadat u **sparen+Close** klikt, maak de vorm aan het voorwerp vast waar u het wilt gebruiken, zoals die in [ wordt beschreven een douaneformulier aan een voorwerp ](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toevoegen.
