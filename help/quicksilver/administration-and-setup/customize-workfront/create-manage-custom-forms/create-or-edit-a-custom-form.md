---
title: Een aangepast formulier maken of bewerken met de verouderde formulierbuilder
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: U kunt een nieuw aangepast formulier maken of bewerken.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
source-git-commit: 6b2a2160b5daaa94374707bad4b026daa13edf06
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Een aangepast formulier maken of bewerken met de verouderde formulierbuilder

<!--Audited: 01/2024-->

{{form-designer-default}}

U kunt een nieuw aangepast formulier maken of een bestaand formulier bewerken. Beide taken worden in dit artikel uitgelegd.

Voor informatie over het maken van een nieuw aangepast formulier op basis van een bestaand formulier raadpleegt u [Een aangepast formulier kopiëren om een nieuw formulier te maken met de oudere formulierbuilder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

In dit artikel wordt beschreven hoe u een aangepast formulier kunt maken met de verouderde formulierbuilder. Voor informatie over het maken van een aangepast formulier met de formulierontwerper raadpleegt u [Een formulier ontwerpen met de formulierontwerper](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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
   <td><p>Nieuw: Standaard</p>
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

+++

## Een aangepast formulier maken

{{step-1-to-setup}}

1. Klikken **Aangepaste Forms** in het linkerdeelvenster.

   Aangepaste formulieren worden weergegeven in een lijst. U kunt alle aangepaste formulieren en aangepaste velden bekijken die voor uw organisatie zijn gemaakt. U kunt ook zien wie elk formulier heeft gemaakt, welke objecten eraan zijn gekoppeld en of het actief is.

1. Klikken **Nieuw aangepast formulier.**
1. Selecteer ten minste één objecttype dat u aan het aangepaste formulier wilt koppelen en klik op **Doorgaan**.

   ![](assets/choose-object-type.jpg)

1. Op de **Formulierinstellingen** tab die wordt geopend, typt u een **Formuliertitel** en een facultatieve **Beschrijving** voor het aangepaste formulier.

1. (Optioneel) Als u meer objecttypen aan het formulier wilt toevoegen zodat het aan meer objecten kan worden gekoppeld, klikt u op de knop **plus** aanmelden na **Objecttypen** Selecteer vervolgens het gewenste objecttype in het menu dat wordt weergegeven.

   U kunt dit herhalen om zoveel objecttypen toe te voegen als u wilt.

1. (Optioneel) Klik op de knop **X** op een objecttype om het uit het formulier te verwijderen.

   Voor informatie over het verwijderen van objecttypen uit een aangepast formulier dat u al hebt opgeslagen, raadpleegt u [Objecttypen verwijderen op een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Klikken **Gereed** linksonder in het scherm.

   >[!TIP]
   >
   >U kunt op **Toepassen** op elk gewenst moment tijdens het maken van een aangepast formulier om uw wijzigingen op te slaan en het formulier open te houden.

1. Als u een nieuw aangepast veld aan het formulier wilt toevoegen, gaat u verder met [Een aangepast veld toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) of [Een aangepast veld of aangepaste widget opnieuw gebruiken in een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   of

   Als u uw aangepaste formulier op andere manieren wilt blijven bouwen, gaat u verder naar een van de volgende artikelen:

   * [Een middelenwidget toevoegen of bewerken in een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Aangepaste velden en widgets in een aangepast formulier plaatsen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Een sectie-einde toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Berekende gegevens toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Een bestaand berekend aangepast veld opnieuw gebruiken in een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Weergavelogica toevoegen en logica overslaan naar een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## Een aangepast formulier bewerken starten

U kunt een aangepast formulier op elk gewenst moment na het maken bewerken.

>[!CAUTION]
>
>Zie de sectie voor informatie over het verwijderen van velden uit een aangepast formulier zonder dat gebruikers gegevens verliezen die ze in die velden hebben ingevoerd [Een aangepast veld verwijderen zonder gegevens te verliezen die gebruikers hebben ingevoerd](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove) in het artikel [Een aangepast veld of aangepaste widget uit het systeem verwijderen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
>
>Over het algemeen raden we u aan om het aantal keren dat u een aangepast formulier bewerkt dat al in gebruik is, te minimaliseren. Er is geen meldingssysteem om mensen die het aangepaste formulier gebruiken te waarschuwen voor uw wijzigingen.

{{step-1-to-setup}}

1. Klikken **Aangepaste Forms** in het linkerdeelvenster.

   Aangepaste formulieren worden weergegeven in een lijst. U kunt alle aangepaste formulieren en aangepaste velden bekijken die voor uw organisatie zijn gemaakt. U kunt ook zien wie elk formulier heeft gemaakt, welke objecten eraan zijn gekoppeld en of het actief is.

1. Selecteer het aangepaste formulier dat u wilt bewerken en klik op ![Pictogram Bewerken](assets/edit-icon.png).
1. (Optioneel) Als u de titel en beschrijving van het aangepaste formulier wilt wijzigen, klikt u op de knop **Formulierinstellingen** en typt u vervolgens een **Formuliertitel** en **Beschrijving**.

1. (Optioneel) Als u meer objecttypen aan het formulier wilt toevoegen zodat het aan meer objecten kan worden gekoppeld, klikt u op het plusteken + na **Objecttypen** Selecteer vervolgens de gewenste tekst in het menu dat wordt weergegeven.

   ![](assets/add-object-type-existing-form.png)

   U kunt dit herhalen om zoveel objecttypen toe te voegen als u wilt.

   U kunt ook op de X op een objecttype klikken om het uit het formulier te verwijderen. Dit moet voorzichtig gebeuren als u een objecttype wilt verwijderen uit een aangepast formulier dat u al hebt opgeslagen. Zie voor meer informatie [Objecttypen verwijderen op een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Klikken **Gereed**.

   >[!TIP]
   >
   >U kunt op **Toepassen** op elk gewenst moment tijdens het maken van een aangepast formulier om uw wijzigingen op te slaan en het formulier open te houden.

1. Als u een nieuw aangepast veld aan het formulier wilt toevoegen, gaat u verder met [Een aangepast veld toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) of [Een aangepast veld of aangepaste widget opnieuw gebruiken in een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   of

   Als u uw aangepaste formulier op andere manieren wilt blijven bouwen, gaat u verder naar een van de volgende artikelen:

   * [Een middelenwidget toevoegen of bewerken in een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Aangepaste velden en widgets in een aangepast formulier plaatsen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Een sectie-einde toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Berekende gegevens toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Een bestaand berekend aangepast veld opnieuw gebruiken in een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Weergavelogica toevoegen en logica overslaan naar een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
