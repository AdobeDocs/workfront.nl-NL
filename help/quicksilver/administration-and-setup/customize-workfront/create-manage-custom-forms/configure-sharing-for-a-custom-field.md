---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Delen voor aangepaste velden en widgets configureren met de oudere formulierbuilder
description: Wanneer u een nieuw aangepast veld of een nieuwe aangepaste widget toevoegt aan een aangepast formulier, kan iedereen in het systeem die toegang heeft tot aangepaste formulieren standaard de eigenschappen voor dat item bewerken, zoals het label en de naam. U kunt dit wijzigen door te bepalen met wie het bestand kan worden gedeeld.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# Delen voor aangepaste velden en widgets configureren met de oudere formulierbuilder

{{form-designer-default}}

Wanneer u een nieuw aangepast veld of een nieuwe aangepaste widget toevoegt aan een aangepast formulier, kan iedereen in het systeem die toegang heeft tot aangepaste formulieren standaard de eigenschappen voor dat item bewerken, zoals het label en de naam. U kunt dit wijzigen door te bepalen met wie het bestand kan worden gedeeld.

Voor informatie over douanegebieden en widgets in douanevormen, zie [ een douanegebied aan een douanevorm met de bouwer van de erfenisvorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) toevoegen en [ een activa widget in een douanevorm met de bouwer van de erfenis ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md) uitgeven of toevoegen.

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

## Delen voor een aangepast veld of een aangepaste widget configureren

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Aangepaste Forms**.
1. Als u het delen voor een aangepast veld of een aangepaste widget configureert in de Workfront-instantie van uw organisatie, gaat u als volgt te werk:

   1. Klik **Gebieden** om het gebied van Gebieden te openen.
   1. Selecteer het punt u het delen voor wilt vormen, dan klik ![ pictogram van het Aandeel ](assets/share-icon.png).

   Of voer de volgende handelingen uit als u het delen configureert voor een aangepast veld of een aangepaste widget in een bestaand aangepast formulier:

   1. Selecteer de douanevorm, dan klik ![ uitgeven pictogram ](assets/edit-icon.png).
   1. Selecteer in het formulierbewerkingsgebied aan de rechterkant het item waarvoor u het delen wilt configureren.
   1. In het linkerpaneel, klik **gebied van het Aandeel**.

1. In het **vakje van de Toegang van het Gebied van de Douane** dat toont, specificeer wie u het punt met wilt delen en hoe u het wilt delen:

   1. Vlak de laag-linkerhoek van de **doos van de Toegang van het Gebied van de Douane**, onder **geef de toegang van het douanegebied tot**, begin de naam van een gebruiker, een team, een baanrol, een groep, of een bedrijf te typen u het punt met wilt delen, dan de naam klikken wanneer het verschijnt.

      ![](assets/share-field-give-access-to.jpg)

   1. Als u specifieker wilt zijn over hoe u het punt wilt delen, klik de drop-down lijst rechts van de naam, dan gebruik om het even welke volgende opties:

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">Weergeven</td> 
         <td> <p>U kunt <strong> Geavanceerde Montages </strong> klikken om te specificeren of u de gebruiker of de gebruikers hun toegang wilt kunnen gebruiken om het punt aan een douanevorm toe te voegen of het met andere gebruikers te delen.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Beheren</td> 
         <td> <p>Hiermee kunt u het aangepaste veld bewerken en weergeven in de veldbibliotheek en op de pagina waar u aangepaste formulieren maakt.</p> <p>U kunt <strong> Geavanceerde Montages </strong> klikken om te specificeren of u de gebruiker of de gebruikers hun toegang wilt kunnen gebruiken om het punt van het systeem te schrappen of het met andere gebruikers te delen.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Optioneel) Herhaal de vorige stap om andere namen aan de lijst toe te voegen en de opties te configureren.
1. (Optioneel) Klik op het tandwielpictogram ![](assets/gear-icon-settings.png) in de rechterbovenhoek als u een optie voor systeembreed delen voor het veld wilt kiezen.

   Niet alle volgende opties worden tegelijkertijd weergegeven in dit vervolgkeuzemenu. De tweede wordt bijvoorbeeld alleen weergegeven wanneer een van de andere twee is geselecteerd.

   * **maak dit editable systeem-breed zodat iedereen in Workfront het** (de standaardoptie) kan uitgeven

     Wanneer u een aangepast veld of een aangepaste widget toevoegt en u het delen ervan niet beperkt, kan iedereen in het systeem die toegang heeft tot aangepaste formulieren deze weergeven en de eigenschappen ervan bewerken.

   * **verwijder systeem-brede uitgeeft toegang**

     Hiermee beperkt u de toegang tot alleen de personen die u aan de lijst hebt toegevoegd.

   * **maak dit zichtbaar systeem-breed zodat iedereen in Workfront het** kan zien

1. Klik **sparen** of **sparen + Sluiten**.

## Overgenomen toegang tot aangepaste velden en widgets wanneer een aangepast formulier wordt gedeeld

Wanneer iemand een aangepast formulier deelt met een groep, taakrol, team of bedrijf, nemen de ontvangers de toegang van de Weergave over aan aangepaste velden en widgets die zich in het formulier bevinden. Dit toegangsniveau tot deze items op het formulier blijft altijd behouden, zodat het formulier naar wens kan functioneren voor de ontvangers door de persoon die het heeft gemaakt. Dit geldt zelfs voor ontvangers die toegang tot het formulier hebben via Bewerken.

U kunt erachter komen wie toegang tot een aangepast veld of een aangepaste widget heeft geërfd en u kunt de toegang tot dit veld of deze widget verwijderen.

>[!NOTE]
>
>Als een ontvanger beheertoegang heeft tot een aangepast veld of een aangepaste widget op het gedeelde aangepaste formulier, blijft die toegang behouden voor de ontvanger.

* [ ontdekt wie toegang tot een douanegebied of widget heeft geërft ](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [Toegang tot een aangepast veld of aangepaste widget verwijderen in een aangepast formulier dat is gedeeld](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### Ontdek wie toegang tot een aangepast veld of een aangepaste widget heeft geërfd {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Opstelling** ![](assets/gear-icon-settings.png).

1. In het linkerpaneel, klik **Aangepaste Forms**.
1. Klik **Gebieden**, dan selecteer het gebied, het beeld, of de toegangswidget.
1. In de doos die toont, klik **Geërfte Toestemmingen** en bekijk de namen die tonen.
1. Klik **annuleren**.

### Toegang tot een aangepast veld of aangepaste widget verwijderen in een aangepast formulier dat is gedeeld {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Als u de toegang tot een aangepast veld of een aangepaste widget in een gedeeld formulier moet verwijderen, moet u het delen van het formulier opheffen. Voor instructies, zie in de sectie [ toegang tot een douaneformulier ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) in het artikel [ verwijdert een douaneformulier ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
