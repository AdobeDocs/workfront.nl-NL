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

Voor informatie over het creëren van een nieuwe douanevorm van bestaande, zie [ Kopieer een douanevorm om nieuwe tot stand te brengen met de bouwer van de erfenisvorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

In dit artikel wordt beschreven hoe u een aangepast formulier kunt maken met de verouderde formulierbuilder. Voor informatie over het creëren van een douanevorm die de vormontwerper gebruikt, zie [ Ontwerp een vorm met de vormontwerper ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een aangepast formulier maken

{{step-1-to-setup}}

1. Klik **Forms van de Douane** in het linkerpaneel.

   Aangepaste formulieren worden weergegeven in een lijst. U kunt alle aangepaste formulieren en aangepaste velden bekijken die voor uw organisatie zijn gemaakt. U kunt ook zien wie elk formulier heeft gemaakt, welke objecten eraan zijn gekoppeld en of het actief is.

1. Klik **Nieuwe Vorm van de Douane.**
1. Selecteer minstens één objecten type dat u met de douanevorm wilt associëren, dan **blijven** klikken.

   ![](assets/choose-object-type.jpg)

1. Op het **lusje van de Montages van de Vorm** dat opent, typ a **Titel van de Vorm** en een facultatieve **Beschrijving** voor de douanevorm.

1. (Facultatief) als u meer objecten types aan de vorm wilt toevoegen zodat het aan meer voorwerpen kan worden vastgemaakt, klik **plus** teken na **de Types van Objecten**, dan selecteer het objecten type u in het menu wilt dat toont.

   U kunt dit herhalen om zoveel objecttypen toe te voegen als u wilt.

1. (Facultatief) klik **X** op een objecten type om het van de vorm te schrappen.

   Voor informatie over het schrappen van objecten types van een douaneformulier u reeds hebt bewaard, zie [ Objecttypes van de Schrapping op een douaneformulier ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Klik **Gedaan** in de laag-linkerhoek van het scherm.

   >[!TIP]
   >
   >U kunt **klikken toepast** op om het even welk punt terwijl u een douaneformulier creeert om uw veranderingen te bewaren en de vorm open te houden.

1. Als u een nieuw douanegebied aan de vorm wilt toevoegen, ga [ verder een douanegebied aan een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) toevoegen of [ een douanegebied of widget in een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md) opnieuw gebruiken.

   of

   Als u uw aangepaste formulier op andere manieren wilt blijven bouwen, gaat u verder naar een van de volgende artikelen:

   * [ voeg of geef activa widget in een douanevorm toe uit ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [ de douanegebieden en widgets van de Positie in een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [ voeg een sectieonderbreking aan een douanevorm toe ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [ voeg berekende gegevens aan een douanevorm toe ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [ hergebruik een bestaand berekend douanegebied in een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Weergavelogica toevoegen en logica overslaan naar een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## Een aangepast formulier bewerken starten

U kunt een aangepast formulier op elk gewenst moment na het maken bewerken.

>[!CAUTION]
>
>Voor informatie over het verwijderen van gebieden uit een douanevorm zonder gegevens te verliezen die de gebruikers op die gebieden zijn ingegaan, zie de sectie [ een douanegebied verwijderen zonder gegevens te verliezen die de gebruikers ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove) in het artikel [ zijn ingegaan een douanegebied of widget van het systeem ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md) schrappen.
>
>Over het algemeen raden we u aan om het aantal keren dat u een aangepast formulier bewerkt dat al in gebruik is, te minimaliseren. Er is geen meldingssysteem om mensen die het aangepaste formulier gebruiken te waarschuwen voor uw wijzigingen.

{{step-1-to-setup}}

1. Klik **Forms van de Douane** in het linkerpaneel.

   Aangepaste formulieren worden weergegeven in een lijst. U kunt alle aangepaste formulieren en aangepaste velden bekijken die voor uw organisatie zijn gemaakt. U kunt ook zien wie elk formulier heeft gemaakt, welke objecten eraan zijn gekoppeld en of het actief is.

1. Selecteer de douanevorm u wilt uitgeven, dan klik ![ uitgeven pictogram ](assets/edit-icon.png).
1. (Facultatief) om de titel en de beschrijving van de douanevorm te veranderen, klik het **lusje van de Montages van de Vorm**, dan typ a **Titel van de Vorm** en **Beschrijving**.

1. (Facultatief) als u meer objecten types aan de vorm wilt toevoegen zodat het aan meer voorwerpen kan worden vastgemaakt, klik plus teken + na **Types van Objecten**, dan selecteer het type u in het menu wilt dat toont.

   ![](assets/add-object-type-existing-form.png)

   U kunt dit herhalen om zoveel objecttypen toe te voegen als u wilt.

   U kunt ook op de X op een objecttype klikken om het uit het formulier te verwijderen. Dit moet voorzichtig gebeuren als u een objecttype wilt verwijderen uit een aangepast formulier dat u al hebt opgeslagen. Voor meer informatie, zie [ de objecten types van de Schrapping op een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Klik **Gedaan**.

   >[!TIP]
   >
   >U kunt **klikken toepast** op om het even welk punt terwijl u een douaneformulier creeert om uw veranderingen te bewaren en de vorm open te houden.

1. Als u een nieuw douanegebied aan de vorm wilt toevoegen, ga [ verder een douanegebied aan een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) toevoegen of [ een douanegebied of widget in een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md) opnieuw gebruiken.

   of

   Als u uw aangepaste formulier op andere manieren wilt blijven bouwen, gaat u verder naar een van de volgende artikelen:

   * [ voeg of geef activa widget in een douanevorm toe uit ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [ de douanegebieden en widgets van de Positie in een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [ voeg een sectieonderbreking aan een douanevorm toe ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [ voeg berekende gegevens aan een douanevorm toe ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [ hergebruik een bestaand berekend douanegebied in een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Weergavelogica toevoegen en logica overslaan naar een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
