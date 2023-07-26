---
title: Objecttypen toevoegen aan of verwijderen uit een bestaand aangepast formulier met de formulierontwerper
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: U kunt objecttypen toevoegen aan of verwijderen uit aangepaste formulieren met de formulierontwerper.
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# Objecttypen toevoegen aan of verwijderen uit een bestaand aangepast formulier met de formulierontwerper

U kunt objecttypen toevoegen aan of verwijderen uit een bestaand aangepast formulier met de formulierontwerper.

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-abonnement*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td>
   <p>Huidige abonnement: standaard</p>
   <p>of</p>
   <p>Ouder plan: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td><p>Administratieve toegang tot aangepaste formulieren</p> <p>Ga voor informatie over hoe Workfront-beheerders deze toegang verlenen naar <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, type licentie of configuraties op toegangsniveau u hebt.

## Objecttypen toevoegen aan een bestaand aangepast formulier

U kunt aanvullende objecttypen aan het formulier toevoegen zodat het aan meerdere objecten kan worden gekoppeld.

>[!NOTE]
>
>Sectie-einden kunnen worden beïnvloed door het objecttype. De beperkte machtiging Bewerken voor afbrekingen van aangepaste formuliersecties is alleen beschikbaar voor de typen projecten, taken, problemen en gebruikersobjecten.
>
>Zie voor meer informatie [Hoe meerdere objecttypen de machtigingen voor secties kunnen beïnvloeden](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Aangepaste Forms** in het linkerdeelvenster.

   In de weergave die wordt weergegeven, kunt u alle aangepaste formulieren bekijken die voor uw organisatie zijn gemaakt. U kunt ook zien wie elk formulier heeft gemaakt, met welk objecttype het werkt en of het actief is.

1. Selecteer het aangepaste formulier waaraan u extra objecttypen wilt toevoegen en klik vervolgens op **Bewerken**.

1. Klik boven aan het formulier op het plusteken + na **Objecttypen** Selecteer vervolgens de gewenste tekst in het menu dat wordt weergegeven. U kunt dit herhalen om zoveel objecttypen toe te voegen als u wilt.

   ![](assets/add-new-object.png)

1. Klikken **Opslaan en sluiten**.

   >[!TIP]
   >
   >U kunt op **Toepassen** op elk gewenst moment tijdens het maken van een aangepast formulier om uw wijzigingen op te slaan en het formulier open te houden.

## Objecttypen verwijderen op een aangepast formulier

U kunt objecttypen verwijderen uit een bestaand aangepast formulier. Een aangepast formulier moet ten minste één objecttype hebben.

>[!CAUTION]
>
>Als mensen het aangepaste formulier al hebben gekoppeld aan objecten van het type dat u wilt verwijderen, en er gegevens aan hebben toegevoegd, worden die gegevens permanent verwijderd wanneer u dat objecttype op het formulier verwijdert. Het zou historische informatie kunnen omvatten die de gebruikers later zullen vereisen.
>
>Over het algemeen raden we u aan om het aantal keren dat u een aangepast formulier bewerkt dat al in gebruik is, te minimaliseren. Er is geen meldingssysteem om mensen die het aangepaste formulier gebruiken te waarschuwen voor uw wijzigingen.

Een objecttype verwijderen:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Aangepaste Forms** in het linkerdeelvenster.
1. Selecteer het aangepaste formulier dat u wilt bewerken en klik op **Bewerken**.
1. Klik op de X op een van de **Objecttypen** die u uit het formulier wilt verwijderen, klikt u op **Verwijderen** in het waarschuwingsbericht dat wordt weergegeven.

   ![](assets/delete-object-types.png)

1. (Optioneel) Herhaal de vorige stap voor elk ander objecttype dat u uit het formulier wilt verwijderen.
1. Klikken **Gereed** en klik vervolgens op **Sluiten en opslaan**.
