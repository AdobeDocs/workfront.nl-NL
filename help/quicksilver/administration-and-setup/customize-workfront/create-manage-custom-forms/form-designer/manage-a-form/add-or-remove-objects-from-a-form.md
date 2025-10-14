---
title: Objecttypen toevoegen aan of verwijderen uit een bestaand aangepast formulier
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: U kunt objecttypen toevoegen aan of verwijderen uit aangepaste formulieren met de formulierontwerper.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 0%

---

# Objecttypen toevoegen aan of verwijderen uit een bestaand aangepast formulier

U kunt objecttypen toevoegen aan of verwijderen uit een bestaand aangepast formulier met de formulierontwerper.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

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
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td><p>Administratieve toegang tot aangepaste formulieren</p></td> 
  </tr>  
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Objecttypen toevoegen aan een bestaand aangepast formulier

U kunt aanvullende objecttypen aan het formulier toevoegen zodat het aan meerdere objecten kan worden gekoppeld.

>[!NOTE]
>
>Sectie-einden kunnen worden beïnvloed door het objecttype. De beperkte machtiging Bewerken voor afbrekingen van aangepaste formuliersecties is alleen beschikbaar voor de typen projecten, taken, problemen en gebruikersobjecten.
>
>Voor meer informatie, zie [&#x200B; hoe de veelvoudige objecten types sectie kunnen beïnvloeden toestemmingen &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


{{step-1-to-setup}}

1. Klik **Forms van de Douane** in het linkerpaneel.

   In de weergave die wordt weergegeven, kunt u alle aangepaste formulieren bekijken die voor uw organisatie zijn gemaakt. U kunt ook zien wie elk formulier heeft gemaakt, met welk objecttype het werkt en of het actief is.

1. Selecteer de douanevorm u extra objecten types aan wilt toevoegen, dan klik ![&#x200B; uitgeven pictogram &#x200B;](assets/edit-icon2.png).

1. Bij de bovenkant van de vorm, klik het plusteken + na **Types van Objecten**, dan selecteer het type u in het menu wilt dat toont. U kunt dit herhalen om zoveel objecttypen toe te voegen als u wilt.

   ![&#x200B; voeg nieuw voorwerp &#x200B;](assets/add-new-object.png) toe

1. Klik **sparen en Sluiten**.

   >[!TIP]
   >
   >U kunt **klikken toepast** op om het even welk punt terwijl u een douaneformulier creeert om uw veranderingen te bewaren en de vorm open te houden.

## Objecttypen verwijderen op een aangepast formulier

U kunt objecttypen verwijderen uit een bestaand aangepast formulier. Een aangepast formulier moet ten minste één objecttype hebben.

>[!CAUTION]
>
>Als mensen het aangepaste formulier al hebben gekoppeld aan objecten van het type dat u wilt verwijderen, en er gegevens aan hebben toegevoegd, worden die gegevens permanent verwijderd wanneer u dat objecttype op het formulier verwijdert. Het zou historische informatie kunnen omvatten die de gebruikers later zullen vereisen.
>
>Over het algemeen raden we u aan om het aantal keren dat u een aangepast formulier bewerkt dat al in gebruik is, te minimaliseren. Er is geen meldingssysteem om mensen die het aangepaste formulier gebruiken te waarschuwen voor uw wijzigingen.

Een objecttype verwijderen:

{{step-1-to-setup}}

1. Klik **Forms van de Douane** in het linkerpaneel.
1. Selecteer de douanevorm u wilt uitgeven, dan klik ![&#x200B; uitgeven pictogram &#x200B;](assets/edit-icon2.png).
1. Klik X op om het even welke **Types van Objecten** die u van de vorm wilt schrappen.

   ![&#x200B; de objecten van de Schrapping types &#x200B;](assets/delete-object-types.png)

1. (Optioneel) Herhaal de vorige stap voor elk ander objecttype dat u uit het formulier wilt verwijderen.
1. Klik **toepassen**, dan klik **sparen en sluit**.
