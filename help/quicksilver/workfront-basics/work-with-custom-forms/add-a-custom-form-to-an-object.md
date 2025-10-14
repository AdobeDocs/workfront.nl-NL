---
product-area: projects;user-management
keywords: koppelen, toepassen
navigation-topic: work-with-custom-forms
title: Een aangepast formulier toevoegen aan een object
description: U kunt een bestaand aangepast formulier toevoegen aan de objecten hieronder. Een aangepast formulier bevat aangepaste velden waarin u informatie over het object kunt opslaan.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 7b9989b73f7be46690073f323203ae2d9ca1a4b5
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 0%

---

# Een aangepast formulier toevoegen aan een object

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

U kunt een bestaand aangepast formulier toevoegen aan de objecten hieronder. Een aangepast formulier bevat aangepaste velden waarin u informatie over het object kunt opslaan.

* Projecten (met inbegrip van zakelijke zaken)
* Taken
* Problemen
* Bedrijven
* Portfolio&#39;s
* Programma&#39;s
* Documenten
* Gebruikers
* Groepen
* Herhalingen
* Uitgaven
* Factureringsgegevens

U kunt een aangepast formulier alleen toevoegen aan de typen objecten waarvoor het formulier is gemaakt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de handelingen uit te voeren die in dit artikel worden beschreven:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Adobe Workfront-licentie</td> 
  <td> <p>Nieuw: Medewerker of hoger </p>
 <p>of</p> 
<p>Huidig: Verzoek of hoger </p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang bewerken tot de objecten waarvoor u aangepaste formulieren beheert</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten beheren voor het object waarvoor u een aangepast formulier wilt toevoegen.</p> <p>De mening of de hogere toestemmingen aan de douanevorm, met toestemming <b> verbinden aan de voorwerpen van de Gegevens van de Douane </b> (projecten, taken, en kwesties). Voor meer informatie, zie <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref"> een douanevorm </a> delen.</p> <p>Belangrijk: Als u geen vergunning van het Plan met administratieve toegang tot Aangepast Forms hebt, moet u specifieke toestemmingen hebben om de douanevorm minstens te bekijken, zoals die in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref"> wordt beschreven een douanevorm </a> delen. Deze machtigingen moeten ook aan u worden verleend als het formulier in het hele systeem zichtbaar is. </p> <p>Voor informatie bij het verzoeken van extra toegang, zie <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> Toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Uw Workfront-beheerder of een gebruiker met een licentie en beheerdersrechten voor aangepaste formulieren moet aangepaste formulieren maken in uw omgeving voordat u deze aan objecten kunt toevoegen. Voor meer informatie, zie [&#x200B; een douaneformulier &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

## Een aangepast formulier toevoegen aan een object

U kunt op twee manieren een aangepast formulier aan een object toevoegen:

* [&#x200B; voeg een douanevorm aan een voorwerp toe door het voorwerp uit te geven &#x200B;](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Een aangepast formulier aan een object toevoegen vanuit het gebied Details](#add-a-custom-form-to-an-object-from-the-details-area)

### Een aangepast formulier aan een object toevoegen door het object te bewerken {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Ga naar het object waaraan u het aangepaste formulier wilt toevoegen.
1. Klik **Meer** menu ![](assets/more-icon.png), dan klik **uitgeven** ![](assets/edit-icon.png).
1. Klik **Forms van de Douane** > **Forms** toevoegen, dan selecteren tot 10 vormen van het drop-down menu.

1. (Optioneel) Werk de gegevens in de bewerkbare velden op het aangepaste formulier bij.

   U moet alle vereiste velden bijwerken op de formulieren die u toevoegt.

1. Klik **sparen**.

### Een aangepast formulier aan een object toevoegen vanuit het gebied Details {#add-a-custom-form-to-an-object-from-the-details-area}

1. Ga naar het object waaraan u het aangepaste formulier wilt toevoegen.
1. Klik op de sectie **`<Object type>`Details** in het linkerdeelvenster. Bijvoorbeeld, klik **Details van het Project** om douaneformulieren aan een project toe te voegen of **Details van de Uitgave** om douaneformulieren aan een kwestie toe te voegen.
1. Klik **toevoegen het gebied van de douanevorm** in de hoger-juiste hoek, dan selecteren tot 10 douanevormen van de lijst die toont.

   Als het formulier verplichte velden bevat (gemarkeerd met een rood sterretje), hoeft u deze momenteel niet in te vullen.

   De geselecteerde formulieren worden automatisch aan het object gekoppeld.

1. (Facultatief) werk de informatie op de douanegebieden van de vorm bij, dan klik **sparen Veranderingen**.

## Meerdere aangepaste formulieren voor een object

U kunt maximaal 10 aangepaste formulieren toevoegen aan een bepaald object, zodat u velden ter beschikking kunt stellen van bepaalde gebruikers en niet van andere gebruikers, of u beter kunt voldoen aan de formuliervereisten van meerdere projecten.

**Voorbeeld:** als een bestaand project reeds een douanevorm heeft, en meer douanegebieden voor dit project nodig zijn, die op een andere douanevorm bestaan, kunt u een tweede vorm aan het project met de extra gebieden toevoegen, eerder dan de gebieden aan de bestaande douanevorm toevoegen.

## Een aangepast formulier bulksgewijs aan meerdere objecten toevoegen

U kunt aangepaste formulieren aan meerdere objecten toevoegen door deze in een lijst te selecteren.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>Het toevoegen van aangepaste formulieren aan objecten is hetzelfde voor alle objecten, behalve voor projecten.
>
>Voor informatie over het toevoegen van douaneformulieren aan projecten in bulk, zie het artikel [&#x200B; projecten &#x200B;](../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.


1. Blader naar een lijst met objecten.
1. Selecteer meerdere objecten in de lijst.

1. Klik **Meer** menu ![](assets/more-icon.png), dan klik **uitgeven** pictogram ![](assets/edit-icon.png).

   of

   Klik **uitgeven** pictogram ![](assets/edit-icon.png) bij de bovenkant van de lijst.
1. Klik **Forms van de Douane** in het linkerpaneel.
1. in **maak een selectie** drop-down menu, selecteer de vorm u met alle geselecteerde voorwerpen wilt associëren.

   >[!NOTE]
   >
   >Als u het formulier niet kunt vinden in het vervolgkeuzemenu, betekent dit dat aan ten minste een van de objecten het formulier al is gekoppeld. Bepaal welk object dat is en verwijder het uit de selectie voordat u het formulier aan de overige objecten kunt toevoegen.


1. Klik **sparen Veranderingen**.

   Als het formulier verplichte velden bevat (gemarkeerd met een rood sterretje), hoeft u deze momenteel niet in te vullen.
