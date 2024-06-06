---
title: Delen voor aangepaste velden en widgets configureren met de formulierontwerper
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Wanneer u een nieuw aangepast veld of een nieuwe aangepaste widget toevoegt aan een aangepast formulier, kan iedereen in het systeem die toegang heeft tot aangepaste formulieren standaard de eigenschappen voor dat item bewerken, zoals het label en de naam. U kunt dit wijzigen door te bepalen met wie het bestand kan worden gedeeld.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: d80eb802baa6f03ca6e65e542f16b23e9d42444a
workflow-type: tm+mt
source-wordcount: '1095'
ht-degree: 0%

---

# Delen voor aangepaste velden en widgets configureren met de formulierontwerper

{{highlighted-preview-article-level}}

Wanneer u een nieuw aangepast veld of een nieuwe aangepaste widget toevoegt aan een aangepast formulier, kan iedereen in het systeem die toegang heeft tot aangepaste formulieren standaard de eigenschappen voor dat item bewerken, zoals het label en de naam. U kunt dit wijzigen door te bepalen met wie het bestand kan worden gedeeld.

Zie voor informatie over aangepaste velden en widgets in aangepaste formulieren [Een formulier ontwerpen met de formulierontwerper](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Delen van een aangepast veld of aangepaste widget in de lijst met formulieren configureren

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **Aangepaste Forms**.
1. Klikken **Velden** het gebied Velden openen.
1. Selecteer het punt u het delen voor wilt vormen, dan klik ![Pictogram Delen](assets/share-icon.png).
1. Geef in het vak Aangepaste veldtoegang dat wordt weergegeven op met wie u het item wilt delen en hoe u het wilt delen:

   1. In de linkerbenedenhoek van het dialoogvenster **Aangepaste veldtoegang** onder **Aangepaste veldtoegang verlenen aan**, typt u de naam van een gebruiker, team, taakrol, groep of bedrijf waarmee u het item wilt delen, en klikt u vervolgens op de naam wanneer het item wordt weergegeven.

      ![Vak Toegang aangepast veld](assets/share-field-give-access-to.jpg)

   1. Als u specifieker wilt zijn over hoe u het punt wilt delen, klik de drop-down lijst rechts van de naam, dan gebruik om het even welke volgende opties:

      ![Opties voor delen](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">Weergeven</td> 
         <td> <p>U kunt op <strong>Geavanceerde instellingen</strong> om op te geven of de gebruiker of gebruikers toegang moeten kunnen gebruiken om het item toe te voegen aan een aangepast formulier of het te delen met andere gebruikers.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Beheren</td> 
         <td> <p>Hiermee kunt u het aangepaste veld bewerken en weergeven in de veldbibliotheek en op de pagina waar u aangepaste formulieren maakt.</p> <p>U kunt op <strong>Geavanceerde instellingen</strong> om op te geven of de gebruiker of gebruikers toegang moeten kunnen gebruiken om het item uit het systeem te verwijderen of het met andere gebruikers te delen.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Optioneel) Herhaal de vorige stap om andere namen aan de lijst toe te voegen en de opties te configureren.
1. (Optioneel) Klik op het tandwielpictogram ![Instellingenpictogram](assets/gear-icon-settings.png) in de rechterbovenhoek als u een optie voor het delen van het veld voor het hele systeem wilt kiezen.

   Niet alle volgende opties worden tegelijkertijd weergegeven in dit vervolgkeuzemenu. De tweede wordt bijvoorbeeld alleen weergegeven wanneer een van de andere twee is geselecteerd.

   * **Dit bewerkbaar maken voor het hele systeem, zodat iedereen in Workfront het kan bewerken** (de standaardoptie)

     Wanneer u een aangepast veld of een aangepaste widget toevoegt en u het delen ervan niet beperkt, kan iedereen in het systeem die toegang heeft tot aangepaste formulieren deze weergeven en de eigenschappen ervan bewerken.

   * **Toegang tot bewerken in het hele systeem verwijderen**

     Hiermee beperkt u de toegang tot alleen de personen die u aan de lijst hebt toegevoegd.

   * **Dit systeem zo zichtbaar maken dat iedereen in Workfront het kan zien**

1. Klikken **Opslaan**.

## Delen van een aangepast veld of aangepaste widget vanuit de formulierontwerper configureren

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **Aangepaste Forms**.
1. Open een aangepast formulier of maak een nieuw aangepast formulier.
1. Selecteer in de formulierontwerper het item waarvoor u delen wilt configureren, en klik vervolgens op **Delen** in het gebied het uitgeven gebied op het recht.
1. In het vak dat wordt weergegeven, onder **Aangepaste formuliertoegang verlenen aan**, begin de naam van de gebruiker, het team, de baanrol, de groep, of het bedrijf te typen u het punt met wilt delen, dan druk **Enter** wanneer de naam wordt weergegeven.
1. Als u specifieker wilt zijn over hoe u het punt deelt, klik het drop-down menu rechts van de naam, dan gebruik om het even welke volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Weergeven</td> 
        <td> <p>Klikken <strong>Geavanceerde instellingen</strong> om op te geven of gebruikers het item aan een aangepast formulier mogen toevoegen of het met andere gebruikers mogen delen.</p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Beheren</td> 
        <td> <p>Hiermee kunt u het aangepaste veld bewerken en weergeven in de veldbibliotheek en in de formulierontwerper.</p> <p>Klikken <strong>Geavanceerde instellingen</strong> om op te geven of de gebruikers het item uit het systeem moeten kunnen verwijderen of het met andere gebruikers moeten kunnen delen.</p> </td> 
       </tr> 
     </tbody> 
    </table>

1. (Optioneel) Herhaal stap 5-6 om andere namen aan de lijst toe te voegen en hun opties te configureren.
1. (Optioneel) Kies een optie voor systeembreed delen voor het veld:

   * **Iedereen in het systeem kan bewerken** (de standaardoptie)

     Wanneer u een aangepast veld of een aangepaste widget toevoegt en u het delen ervan niet beperkt, kan iedereen in het systeem die toegang heeft tot aangepaste formulieren deze weergeven en de eigenschappen ervan bewerken.

   * **Iedereen in het systeem kan bekijken**
   * **Alleen uitgenodigde personen hebben toegang**

     Beperkt de toegang tot slechts die u aan de lijst toevoegde.

   ![Opties voor delen](assets/share-field-in-designer.png)

1. Klikken **Opslaan**.

## Overgenomen toegang tot aangepaste velden en widgets wanneer een aangepast formulier wordt gedeeld

Wanneer iemand een aangepast formulier deelt met een groep, taakrol, team of bedrijf, nemen de ontvangers de toegang van de Weergave over aan aangepaste velden en widgets die zich in het formulier bevinden. Dit toegangsniveau tot deze items op het formulier blijft altijd behouden, zodat het formulier naar wens kan functioneren voor de ontvangers door de persoon die het heeft gemaakt. Dit geldt zelfs voor ontvangers die toegang tot het formulier hebben via Bewerken.

U kunt erachter komen wie toegang tot een aangepast veld of een aangepaste widget heeft geërfd en u kunt de toegang tot dit veld of deze widget verwijderen.

>[!NOTE]
>
>Als een ontvanger beheertoegang heeft tot een aangepast veld of een aangepaste widget op het gedeelde aangepaste formulier, blijft die toegang behouden voor de ontvanger.

### Ontdek wie toegang tot een aangepast veld of een aangepaste widget heeft geërfd {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **Aangepaste Forms**.
1. Klikken **Velden** Selecteer vervolgens het veld, de afbeelding of de toegangs-widget.
1. Klik in het weergegeven vak op **Overgenomen machtigingen** en bekijk de namen die worden weergegeven.
1. Klikken **Annuleren**.

### Toegang tot een aangepast veld of aangepaste widget verwijderen in een aangepast formulier dat is gedeeld {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Als u de toegang tot een aangepast veld of een aangepaste widget in een gedeeld formulier moet verwijderen, moet u het delen van het formulier opheffen. Zie de sectie voor instructies [Toegang tot een aangepast formulier verwijderen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#remove-access-to-a-custom-form-from-the-list-of-forms) in het artikel [Een aangepast formulier delen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
