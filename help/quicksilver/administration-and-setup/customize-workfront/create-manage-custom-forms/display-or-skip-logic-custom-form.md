---
title: Weergavelogica toevoegen en logica overslaan naar een aangepast formulier met de oudere formulierbuilder
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: U kunt bepalen welke secties van een aangepast formulier moeten worden weergegeven of overgeslagen op basis van de keuzes die een gebruiker maakt bij het invullen.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '969'
ht-degree: 0%

---

# Weergavelogica toevoegen en logica overslaan naar een aangepast formulier met de oudere formulierbuilder

{{form-designer-default}}

U kunt bepalen welke secties van een aangepast formulier moeten worden weergegeven of overgeslagen op basis van de keuzes die een gebruiker maakt bij het invullen.

>[!NOTE]
>
>De logica geldt alleen binnen één formulier en kan niet worden gebaseerd op selecties vanuit een ander formulier.

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
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> <p>Voor informatie over hoe de beheerders van Workfront deze toegang verlenen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref"> gebruikers administratieve toegang verlenen tot bepaalde gebieden </a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of configuraties van het toegangsniveau u hebt, contacteer uw beheerder van Workfront.

## Overwegingen bij het gebruik van weergavelogica en het overslaan van logica

* Als u weergavelogica wilt toevoegen aan een aangepast veld, een widget of een sectie-einde, moet ten minste één meerkeuzeveld (keuzerondjes, vervolgkeuzelijst of selectievakjes) vóór dit veld op het formulier worden geplaatst.

  Voor informatie over douanegebieden en widgets in douanevormen, zie [ een douanegebied aan een douanevorm met de bouwer van de erfenisvorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) toevoegen en [ een activa widget in een douanevorm met de bouwer van de erfenis ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md) uitgeven of toevoegen.

* U kunt geen logica overslaan toevoegen aan een widget of sectie-einde. U kunt het alleen toevoegen aan een veld met meerdere keuzen (keuzerondjes, vervolgkeuzelijst of selectievakjes).

* U kunt zowel weergavelogica als logica overslaan aan een aangepast veld toevoegen als het volgende geldt voor het aangepaste veld:

   * Het is een meerkeuzeveld (keuzerondjes, vervolgkeuzelijst of selectievakjes)
   * Voorafgegaan door een veld met meerdere keuzen
   * Het wordt gevolgd door een ander aangepast veld

* Wanneer u formulieren kopieert met logica voor weergave of overslaan, wordt de logica gekopieerd naar het nieuwe aangepaste formulier.
* Wanneer u objecten bulksgewijs bewerkt, worden alle aangepaste velden weergegeven in het vak Objecten bewerken, inclusief de overgeslagen of verborgen velden.
* Houd rekening met het volgende wanneer u een weergaveregel voor een aangepast formulier maakt:

   * Aangepaste velden die niet zijn opgenomen in een logische weergave-instructie, worden standaard weergegeven op een aangepast formulier.
   * U kunt logische instructies voor weergave op meerdere velden maken.
   * Als voor alle velden onder een sectie-einde een weergavelogica is toegepast en alle velden zijn verborgen als gevolg van de logica, wordt de volledige sectie verborgen op het aangepaste formulier.

## Een voorbeeld van een aangepast formulier maken met weergave en logica overslaan

De beste manier om te leren hoe te om vertoning toe te voegen en logica aan een douaneformulier over te slaan is door het praktische voorbeeld dat in de twee volgende secties wordt verklaard:

### Logica weergeven {#display-logic}

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Opstelling** ![](assets/gear-icon-settings.png).

1. In het linkerpaneel, klik **Aangepaste Forms**.

1. Het aangepaste voorbeeldformulier maken:

   1. Klik **Nieuwe Vorm van de Douane**, dan klik **Project** in de drop-down lijst.

   1. In de **doos van de Titel van de Vorm 0}, type** de douanevorm van de Steekproef - het leren vertoningslogica en overslaat logica **.**

   1. Klik **voeg een Gebied** in de hogere linkerhoek toe.
   1. Voeg een dropdown gebied toe genoemd *Gebied van de Uitgave* door **Dropdown** te klikken, dan het typen **gebied van de Uitgave** in de **doos van het Etiket**.

   1. Onder **Keuzen**, voeg de volgende keuzen in de tekstvakjes toe:

      Onderzoek vereist

      Geen onderzoek meer

   1. Klik **sparen + Sluiten** in de lagere linkerhoek.

1. Selecteer de nieuwe **douanevorm van de Steekproef - het Leren vertoningslogica en overslaan logica** douanevorm, dan klik **uitgeven**.

1. Voeg een nieuw enkel gebied van de lijntekst toe genoemd *Ander Onderzoek* door **Enig Gebied van de Tekst van de Lijn** te klikken, dan het typen **Ander Onderzoek** in de **doos van het Etiket**.

1. Klik **toevoegen Logica** dichtbij de laag-linkerkant van **geef het scherm van de Vorm van de Douane uit**.

1. In de doos die verschijnt, met het **open lusje van de Logica van de Vertoning**, opstelling de logica voor wanneer het **Andere gebied van het Onderzoek** op de vorm zal verschijnen door **gebied van de Uitgave** in de eerste drop-down te klikken, **Onderzoek nodig** in de tweede drop-down, en **Geselecteerd** in de derde drop-down.
1. Klik **sparen** om het **Logische van het Gebied** venster te sluiten, dan klik **Gedaan** op het **gebied van de Montages van het Gebied**.

   Nu, wanneer iemand **Onderzoek nodig** op het **gebied van de Uitgave** drop-down selecteert, zal het **Andere gebied van het Onderzoek** tonen.

1. Klik **Voorproef** om ervoor te zorgen de logica verschijnt de manier u het op de vorm wilt.
1. Klik **Voorproef van het Eind** wanneer u vindt dat de logica zoals verwacht werkt.
1. Klik **sparen + Sluiten** op **geef het venster van de Vorm van de Douane uit** om de vorm te bewaren, dan verdergaat op [ logica van de Overslaan ](#skip-logic) hieronder.

### Logica overslaan {#skip-logic}

Logische functies voor overslaan zijn vergelijkbaar met die voor de weergave van logica, maar fungeren als het omgekeerde: in plaats van dat specifieke aangepaste multikeuze-velden worden weergegeven op basis van specifieke selecties, bepaalt u welke velden moeten worden overgeslagen op basis van de selecties van de gebruikers.

Om over dit te leren, blijf werkend aan de vorm van de steekproefdouane u in de sectie [ logica van de Vertoning ](#display-logic) in dit artikel creeerde:

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Opstelling** ![](assets/gear-icon-settings.png).

1. Klik **Aangepaste Forms**.
1. Selecteer de vorm **douanevorm van de Steekproef - het Leren vertoningslogica en overslaan logica** die u in de stappen hierboven creeerde, dan klik **uitgeven**.

1. Selecteer het drop-down gebied u genoemd *gebied van de Uitgave* creeerde.
1. Klik **toevoegen Logische** knoop in **de Montages van het Gebied** sidebar.

1. In de **Logische doos van het Gebied**, zorg ervoor **Skip Logische** tabel wordt geselecteerd.

1. Plaats eerste drop-down aan **geen meer onderzoek** en tweede drop-down aan **Geselecteerd**.

1. In **dan Skip aan** drop-down, uitgezochte **Einde van vorm.**

   Nu, wanneer iemand **geen meer onderzoek** op het **gebied van de Uitgave** drop-down gebied selecteert, zal de vorm direct aan het eind van de vorm zonder het **Andere gebied van het Onderzoek** te tonen overslaan.

1. Klik **sparen**.
1. Klik **Voorproef** om ervoor te zorgen de logica de manier toepast u het wilt.
1. Klik **Gedaan** in de lagere linkerkant van de vorm.
