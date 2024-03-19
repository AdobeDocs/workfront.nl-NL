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
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 0%

---

# Delen voor aangepaste velden en widgets configureren met de oudere formulierbuilder

<span class="preview">De gemarkeerde informatie op deze pagina verwijst naar functionaliteit die nog niet algemeen beschikbaar is. Deze functie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten of in de productieomgeving voor klanten die snelle releases hebben ingeschakeld.</span>

<span class="preview">Voor informatie over snelle versies raadpleegt u [Snelle releases voor uw organisatie in- of uitschakelen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Voor informatie over de huidige versie raadpleegt u [Overzicht tweede release 2024, tweede kwartaal](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Wanneer u een nieuw aangepast veld of een nieuwe aangepaste widget toevoegt aan een aangepast formulier, kan iedereen in het systeem die toegang heeft tot aangepaste formulieren standaard de eigenschappen voor dat item bewerken, zoals het label en de naam. U kunt dit wijzigen door te bepalen met wie het bestand kan worden gedeeld.

Zie voor informatie over aangepaste velden en widgets in aangepaste formulieren [Een aangepast veld toevoegen aan een aangepast formulier met de oudere formulierbuilder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) en [Een elementwidget toevoegen of bewerken in een aangepast formulier met de verouderde formulierbuilder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

## Delen voor een aangepast veld of een aangepaste widget configureren

{{step-1-to-setup}}

1. Klik in het linkerdeelvenster op **Aangepaste Forms**.
1. Als u het delen voor een aangepast veld of een aangepaste widget configureert in de Workfront-instantie van uw organisatie, gaat u als volgt te werk:

   1. Klikken **Velden** het gebied Velden openen.
   1. Selecteer het punt u het delen voor wilt vormen, dan klik **Delen** <span class="preview">of ![Pictogram Delen](assets/share-icon.png).</span>

   Of voer de volgende handelingen uit als u het delen configureert voor een aangepast veld of een aangepaste widget in een bestaand aangepast formulier:

   1. Selecteer het aangepaste formulier en klik op **Bewerken** <span class="preview">of ![Pictogram Bewerken](assets/edit-icon.png).</span>
   1. Selecteer in het formulierbewerkingsgebied aan de rechterkant het item waarvoor u het delen wilt configureren.
   1. Klik in het linkerdeelvenster op **Veld delen**.

1. In de **Aangepaste veldtoegang** vak waarin wordt weergegeven, geeft u aan met wie u het item wilt delen en hoe u het wilt delen:

   1. In de linkerbenedenhoek van het dialoogvenster **Aangepaste veldtoegang** onder **Aangepaste veldtoegang verlenen aan**, typt u de naam van een gebruiker, team, taakrol, groep of bedrijf waarmee u het item wilt delen, en klikt u vervolgens op de naam wanneer het item wordt weergegeven.

      ![](assets/share-field-give-access-to.jpg)

   1. Als u specifieker wilt zijn over hoe u het punt wilt delen, klik de drop-down lijst rechts van de naam, dan gebruik om het even welke volgende opties:

      ![](assets/share-field-view-mng-options.jpg)

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
1. (Optioneel) Klik op het tandwielpictogram ![](assets/gear-icon-settings.png) in de rechterbovenhoek als u een optie voor het delen van het veld voor het hele systeem wilt kiezen.

   Niet alle volgende opties worden tegelijkertijd weergegeven in dit vervolgkeuzemenu. De tweede wordt bijvoorbeeld alleen weergegeven wanneer een van de andere twee is geselecteerd.

   * **Dit bewerkbaar maken voor het hele systeem, zodat iedereen in Workfront het kan bewerken** (de standaardoptie)

     Wanneer u een aangepast veld of een aangepaste widget toevoegt en u het delen ervan niet beperkt, kan iedereen in het systeem die toegang heeft tot aangepaste formulieren deze weergeven en de eigenschappen ervan bewerken.

   * **Toegang tot bewerken in het hele systeem verwijderen**

     Hiermee beperkt u de toegang tot alleen de personen die u aan de lijst hebt toegevoegd.

   * **Dit systeem zo zichtbaar maken dat iedereen in Workfront het kan zien**

1. Klikken **Opslaan** of **Opslaan + Sluiten**.

## Overgenomen toegang tot aangepaste velden en widgets wanneer een aangepast formulier wordt gedeeld

Wanneer iemand een aangepast formulier deelt met een groep, taakrol, team of bedrijf, nemen de ontvangers de toegang van de Weergave over aan aangepaste velden en widgets die zich in het formulier bevinden. Dit toegangsniveau tot deze items op het formulier blijft altijd behouden, zodat het formulier naar wens kan functioneren voor de ontvangers door de persoon die het heeft gemaakt. Dit geldt zelfs voor ontvangers die toegang tot het formulier hebben via Bewerken.

U kunt erachter komen wie toegang tot een aangepast veld of een aangepaste widget heeft geërfd en u kunt de toegang tot dit veld of deze widget verwijderen.

>[!NOTE]
>
>Als een ontvanger beheertoegang heeft tot een aangepast veld of een aangepaste widget op het gedeelde aangepaste formulier, blijft die toegang behouden voor de ontvanger.

* [Ontdek wie toegang tot een aangepast veld of een aangepaste widget heeft geërfd](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [Toegang tot een aangepast veld of aangepaste widget verwijderen in een aangepast formulier dat is gedeeld](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### Ontdek wie toegang tot een aangepast veld of een aangepaste widget heeft geërfd {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Aangepaste Forms**.
1. Klik op de knop **Velden** en selecteert u vervolgens het veld, de afbeelding of de toegangswidget.
1. Klik in het weergegeven vak op **Overgenomen machtigingen** en bekijk de namen die worden weergegeven.
1. Klikken **Annuleren**.

### Toegang tot een aangepast veld of aangepaste widget verwijderen in een aangepast formulier dat is gedeeld {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Als u de toegang tot een aangepast veld of een aangepaste widget in een gedeeld formulier moet verwijderen, moet u het delen van het formulier opheffen. Zie voor instructies in de sectie [Toegang tot een aangepast formulier verwijderen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) in het artikel [Een aangepast formulier delen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
