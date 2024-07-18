---
title: Delen voor aangepaste velden en widgets configureren
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Wanneer u een nieuw aangepast veld of een nieuwe aangepaste widget toevoegt aan een aangepast formulier, kan iedereen in het systeem die toegang heeft tot aangepaste formulieren standaard de eigenschappen voor dat item bewerken, zoals het label en de naam. U kunt dit wijzigen door te bepalen met wie het bestand kan worden gedeeld.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 4f591fa3-2cb9-4a22-bfb1-1b50cedfcf3d
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '1087'
ht-degree: 0%

---

# Delen voor aangepaste velden en widgets configureren

Wanneer u een nieuw aangepast veld of een nieuwe aangepaste widget toevoegt aan een aangepast formulier, kan iedereen in het systeem die toegang heeft tot aangepaste formulieren standaard de eigenschappen voor dat item bewerken, zoals het label en de naam. U kunt dit wijzigen door te bepalen met wie het bestand kan worden gedeeld.

Voor informatie over douanegebieden en widgets in douanevormen, zie [ Ontwerp een vorm met de vormontwerper ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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

## Delen van een aangepast veld of aangepaste widget in de lijst met formulieren configureren

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Aangepaste Forms**.
1. Klik **Gebieden** om het gebied van Gebieden te openen.
1. Selecteer het punt u het delen voor wilt vormen, dan klik ![ pictogram van het Aandeel ](assets/share-icon.png).
1. Geef in het vak Aangepaste veldtoegang dat wordt weergegeven op met wie u het item wilt delen en hoe u het wilt delen:

   1. Vlak de laag-linkerhoek van de **doos van de Toegang van het Gebied van de Douane**, onder **geef de toegang van het douanegebied tot**, begin de naam van een gebruiker, een team, een baanrol, een groep, of een bedrijf te typen u het punt met wilt delen, dan de naam klikken wanneer het verschijnt.

      ![ doos van de Toegang van het Gebied van de Douane ](assets/share-field-give-access-to.jpg)

   1. Als u specifieker wilt zijn over hoe u het punt wilt delen, klik de drop-down lijst rechts van de naam, dan gebruik om het even welke volgende opties:

      ![ het Delen opties ](assets/share-field-view-mng-options.jpg)

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
1. (Facultatief) klik het pictogram van de Montages van het tandwielpictogram ![ ](assets/gear-icon-settings.png) in de hoger-juiste hoek als u een systeem-brede het delen optie voor het gebied wilt kiezen.

   Niet alle volgende opties worden tegelijkertijd weergegeven in dit vervolgkeuzemenu. De tweede wordt bijvoorbeeld alleen weergegeven wanneer een van de andere twee is geselecteerd.

   * **maak dit editable systeem-breed zodat iedereen in Workfront het** (de standaardoptie) kan uitgeven

     Wanneer u een aangepast veld of een aangepaste widget toevoegt en u het delen ervan niet beperkt, kan iedereen in het systeem die toegang heeft tot aangepaste formulieren deze weergeven en de eigenschappen ervan bewerken.

   * **verwijder systeem-brede uitgeeft toegang**

     Hiermee beperkt u de toegang tot alleen de personen die u aan de lijst hebt toegevoegd.

   * **maak dit zichtbaar systeem-breed zodat iedereen in Workfront het** kan zien

1. Klik **sparen**.

## Delen van een aangepast veld of aangepaste widget vanuit de formulierontwerper configureren

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Aangepaste Forms**.
1. Open een aangepast formulier of maak een nieuw aangepast formulier.
1. In de vormontwerper, selecteer het punt u het delen voor wilt vormen, dan **Aandeel** op het gebied het uitgeven gebied op het recht klikken.
1. In de doos die toont, onder **de toegang van de douanevorm van de Verlening tot**, begin de naam van de gebruiker, het team, de baanrol, de groep, of het bedrijf te typen u het punt met wilt delen, dan **binnengaan** wanneer de naamvertoningen.
1. Als u specifieker wilt zijn over hoe u het punt deelt, klik het drop-down menu rechts van de naam, dan gebruik om het even welke volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Weergeven</td> 
        <td> <p>Klik <strong> Geavanceerde Montages </strong> om te specificeren of u de gebruikers het punt aan een douaneformulier wilt kunnen toevoegen of het met andere gebruikers delen.</p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Beheren</td> 
        <td> <p>Hiermee kunt u het aangepaste veld bewerken en weergeven in de veldbibliotheek en in de formulierontwerper.</p> <p>Klik <strong> Geavanceerde Montages </strong> om te specificeren of u de gebruikers het punt van het systeem wilt kunnen schrappen of het met andere gebruikers delen.</p> </td> 
       </tr> 
     </tbody> 
    </table>

1. (Optioneel) Herhaal stap 5-6 om andere namen aan de lijst toe te voegen en hun opties te configureren.
1. (Optioneel) Kies een optie voor systeembreed delen voor het veld:

   * **iedereen in het systeem kan** uitgeven (de standaardoptie)

     Wanneer u een aangepast veld of een aangepaste widget toevoegt en u het delen ervan niet beperkt, kan iedereen in het systeem die toegang heeft tot aangepaste formulieren deze weergeven en de eigenschappen ervan bewerken.

   * **iedereen in het systeem kan** bekijken
   * **slechts kunnen de uitgenodigde mensen tot** toegang hebben

     Beperkt de toegang tot slechts die u aan de lijst toevoegde.

   ![ het Delen opties ](assets/share-field-in-designer.png)

1. Klik **sparen**.

## Overgenomen toegang tot aangepaste velden en widgets wanneer een aangepast formulier wordt gedeeld

Wanneer iemand een aangepast formulier deelt met een groep, taakrol, team of bedrijf, nemen de ontvangers de toegang van de Weergave over aan aangepaste velden en widgets die zich in het formulier bevinden. Dit toegangsniveau tot deze items op het formulier blijft altijd behouden, zodat het formulier naar wens kan functioneren voor de ontvangers door de persoon die het heeft gemaakt. Dit geldt zelfs voor ontvangers die toegang tot het formulier hebben via Bewerken.

U kunt erachter komen wie toegang tot een aangepast veld of een aangepaste widget heeft geërfd en u kunt de toegang tot dit veld of deze widget verwijderen.

>[!NOTE]
>
>Als een ontvanger beheertoegang heeft tot een aangepast veld of een aangepaste widget op het gedeelde aangepaste formulier, blijft die toegang behouden voor de ontvanger.

### Ontdek wie toegang tot een aangepast veld of een aangepaste widget heeft geërfd {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Aangepaste Forms**.
1. Klik **Gebieden**, dan selecteer het gebied, het beeld, of de toegangswidget.
1. In de doos die toont, klik **Geërfte Toestemmingen** en bekijk de namen die tonen.
1. Klik **annuleren**.

### Toegang tot een aangepast veld of aangepaste widget verwijderen in een aangepast formulier dat is gedeeld {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Als u de toegang tot een aangepast veld of een aangepaste widget in een gedeeld formulier moet verwijderen, moet u het delen van het formulier opheffen. Voor instructies, zie de sectie [ toegang tot een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#remove-access-to-a-custom-form-from-the-list-of-forms) in het artikel [ om een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md) te delen.
