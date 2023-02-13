---
title: Weergavelogica toevoegen en logica overslaan naar een aangepast formulier
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: U kunt bepalen welke secties van een aangepast formulier moeten worden weergegeven of overgeslagen op basis van de keuzes die een gebruiker maakt bij het invullen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
source-git-commit: 59e3b958dd81f2f068bc06c3fe439de0084f9ce4
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# Weergavelogica toevoegen en logica overslaan naar een aangepast formulier

U kunt bepalen welke secties van een aangepast formulier moeten worden weergegeven of overgeslagen op basis van de keuzes die een gebruiker maakt bij het invullen.

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
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> <p>Ga voor informatie over hoe Workfront-beheerders deze toegang verlenen naar <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, type licentie of configuraties op toegangsniveau u hebt.

## Overwegingen bij het gebruik van weergavelogica en het overslaan van logica

* Als u weergavelogica wilt toevoegen aan een aangepast veld, een widget of een sectie-einde, moet ten minste één meerkeuzeveld (keuzerondjes, vervolgkeuzelijst of selectievakjes) vóór dit veld op het formulier worden geplaatst.

   Voor informatie over aangepaste velden en widgets in aangepaste formulieren raadpleegt u [Een aangepast veld toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) en [Een middelenwidget toevoegen of bewerken in een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* U kunt geen logica overslaan toevoegen aan een widget of sectie-einde. U kunt het alleen toevoegen aan een veld met meerdere keuzen (keuzerondjes, vervolgkeuzelijst of selectievakjes).

* U kunt zowel weergavelogica als logica overslaan aan een aangepast veld toevoegen. Dit geldt voor alle volgende zaken in het aangepaste veld:

   * Het is een meerkeuzeveld (keuzerondjes, vervolgkeuzelijst of selectievakjes)
   * Voorafgegaan door een veld met meerdere keuzen
   * Het wordt gevolgd door een ander aangepast veld

* Wanneer u formulieren kopieert met logica voor weergave of overslaan, wordt de logica gekopieerd naar het nieuwe aangepaste formulier.
* Houd rekening met het volgende wanneer u een weergavelogische regel voor een aangepast formulier maakt

   * Aangepaste velden die niet zijn opgenomen in een logische weergave-instructie, worden standaard weergegeven op een aangepast formulier.
   * U kunt logische instructies voor weergave op meerdere velden maken.

* Wanneer u objecten bulksgewijs bewerkt, worden alle aangepaste velden weergegeven in het vak Objecten bewerken, inclusief de overgeslagen of verborgen velden.

## Een voorbeeld van een aangepast formulier maken met weergave en logica overslaan

De beste manier om te leren hoe te om vertoning toe te voegen en logica aan een douaneformulier over te slaan is door het praktische voorbeeld dat in de twee volgende secties wordt verklaard:

* [Logica weergeven](#display-logic)
* [Logica overslaan](#skip-logic)

### Logica weergeven {#display-logic}

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Aangepaste Forms** ![](assets/custom-forms-icon.png).

1. Het aangepaste voorbeeldformulier maken:

   1. Klikken **Nieuw aangepast formulier** en klik vervolgens op **Project** in de vervolgkeuzelijst.

   1. In de **Formuliertitel** vak, tekst **Aangepast voorbeeldformulier - Leren werken met weergavelogica en logica overslaan**.

   1. Klikken **Veld toevoegen** in de linkerbovenhoek.
   1. Een vervolgkeuzeveld toevoegen met de naam *Probleemveld* door te klikken **Vervolgkeuzelijst** en typt u **Probleemveld** in de **Label** doos.

   1. Onder **Keuzen** voegt u de volgende opties toe aan de tekstvakken:

      Onderzoek vereist

      Geen onderzoek meer

   1. Klikken **Opslaan + Sluiten** in de linkerbenedenhoek.

1. Selecteer de nieuwe **Aangepast voorbeeldformulier - Leren werken met weergavelogica en logica overslaan** aangepast formulier, klik vervolgens op **Bewerken**.

1. Een nieuw tekstveld met één regel toevoegen met de naam *Ander onderzoek* door te klikken **Tekstveld met één regel** en typt u **Ander onderzoek** in de **Label** doos.

1. Klikken **Logica toevoegen** aan de linkerbenedenzijde van het **Aangepast formulier bewerken** scherm.

1. In het vak dat wordt weergegeven, **Weergavelogica** open, opstelling de logica voor wanneer **Ander onderzoek** wordt op het formulier weergegeven door op **Probleemveld** in de eerste vervolgkeuzelijst, **Onderzoek vereist** in de tweede vervolgkeuzelijst, en **Geselecteerd** in de derde vervolgkeuzelijst.
1. Klikken **Opslaan** om de **Field Logic** venster, klik vervolgens op **Gereed** in de **Veldinstellingen** gebied.

   Nu, wanneer iemand selecteert **Onderzoek vereist** in de **Probleemveld** de **Ander onderzoek** wordt weergegeven.

1. Klikken **Voorvertoning** om ervoor te zorgen dat de logica op de gewenste manier op het formulier wordt weergegeven.
1. Klikken **Voorvertoning beëindigen** wanneer u ontdekt dat de logica zoals verwacht werkt.
1. Klikken **Opslaan + Sluiten** op de **Aangepast formulier bewerken** venster om het formulier op te slaan, en ga vervolgens door naar [Logica overslaan](#skip-logic) hieronder.

### Logica overslaan {#skip-logic}

Logische functies overslaan werkt net als logica voor weergave, maar fungeert als omgekeerd: in plaats van specifieke aangepaste meerkeuzevelden te laten verschijnen op basis van specifieke selecties, bepaalt u welke velden moeten worden overgeslagen op basis van de selecties van de gebruikers.

U leert dit door te werken aan het voorbeeldformulier dat u in de sectie hebt gemaakt [Logica weergeven](#display-logic) in dit artikel :

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Aangepaste Forms**.
1. Selecteer het formulier **Aangepast voorbeeldformulier - Leren werken met weergavelogica en logica overslaan** die u in de bovenstaande stappen hebt gemaakt, klikt u op **Bewerken**.

1. Selecteer het drop-down gebied u genoemde creeerde *Probleemveld*.
1. Klik op de knop **Logica toevoegen** in de **Veldinstellingen** zijbalk.

1. In de **Field Logic** de **Logica overslaan** is geselecteerd.

1. Eerste vervolgkeuzelijst instellen op **Geen onderzoek meer** en de tweede vervolgkeuzelijst naar **Geselecteerd**.

1. In de **Vervolgens overslaan naar** vervolgkeuzelijst, selecteert u **Einde van formulier.**

   Nu, wanneer iemand selecteert **Geen onderzoek meer** in de **Probleemveld** vervolgkeuzelijst, wordt het formulier direct naar het einde van het formulier overgeslagen zonder dat het de **Ander onderzoek** veld.

1. Klikken **Opslaan**.
1. Klikken **Voorvertoning**  om ervoor te zorgen dat de logica op de gewenste manier wordt toegepast.
1. Klikken **Gereed** linksonder in het formulier.
