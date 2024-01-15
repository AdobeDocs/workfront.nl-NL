---
product-area: projects;user-management
keywords: koppelen, toepassen
navigation-topic: work-with-custom-forms
title: Een aangepast formulier toevoegen aan een object
description: U kunt een bestaand aangepast formulier toevoegen aan de objecten hieronder. Een aangepast formulier bevat aangepaste velden waarin u informatie over het object kunt opslaan.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: aec61210cf2c17775738db4975ae8d19223153cc
workflow-type: tm+mt
source-wordcount: '811'
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
* Herhalingen
* Uitgaven
* Factureringsgegevens

U kunt een aangepast formulier alleen toevoegen aan de typen objecten waarvoor het formulier is gemaakt.

## Toegangsvereisten

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
   <td> <p>Rechten beheren voor het object waarvoor u een aangepast formulier wilt toevoegen.</p> <p>Machtigingen voor het aangepaste formulier weergeven of hoger, met toestemming om <b>Koppelen aan aangepaste gegevens</b> objecten (projecten, taken en problemen). Zie voor meer informatie <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Een aangepast formulier delen</a>.</p> <p>Belangrijk: als u geen licentie voor abonnementen hebt met beheerdersrechten voor de aangepaste Forms, moet u specifieke machtigingen hebben om ten minste het aangepaste formulier te kunnen bekijken, zoals beschreven in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Een aangepast formulier delen</a>. Deze machtigingen moeten ook aan u worden verleend als het formulier in het hele systeem zichtbaar is. </p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

Uw Workfront-beheerder of een gebruiker met een licentie en beheerdersrechten voor aangepaste formulieren moet aangepaste formulieren maken in uw omgeving voordat u deze aan objecten kunt toevoegen. Zie voor meer informatie [Een aangepast formulier maken of bewerken](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Een aangepast formulier toevoegen aan een object

U kunt op twee manieren een aangepast formulier aan een object toevoegen:

* [Een aangepast formulier aan een object toevoegen door het object te bewerken](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Een aangepast formulier aan een object toevoegen vanuit het gebied Details](#add-a-custom-form-to-an-object-from-the-details-area)

### Een aangepast formulier aan een object toevoegen door het object te bewerken {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Ga naar het object waaraan u het aangepaste formulier wilt toevoegen.
1. Klik op de knop **Meer** menu ![](assets/more-icon.png)en klik vervolgens op **Bewerken** ![](assets/edit-icon.png).
1. Klikken **Aangepaste Forms** > **Forms toevoegen** Selecteer vervolgens maximaal 10 formulieren in het keuzemenu.

1. (Optioneel) Werk de gegevens in de bewerkbare velden op het aangepaste formulier bij.

   U moet alle vereiste velden bijwerken op de formulieren die u toevoegt.

1. Klikken **Opslaan**.

### Een aangepast formulier aan een object toevoegen vanuit het gebied Details {#add-a-custom-form-to-an-object-from-the-details-area}

1. Ga naar het object waaraan u het aangepaste formulier wilt toevoegen.
1. Klik op de knop **`<Object type>`Details** in het linkerdeelvenster. Klik bijvoorbeeld op **Projectdetails** aangepaste formulieren aan een project of **Probleemdetails** om aangepaste formulieren aan een uitgave toe te voegen.
1. Klik op de knop **Aangepast formulier toevoegen** in de rechterbovenhoek, selecteert u vervolgens maximaal 10 aangepaste formulieren in de lijst die wordt weergegeven.

   Als het formulier verplichte velden bevat (gemarkeerd met een rood sterretje), hoeft u deze momenteel niet in te vullen.

   De geselecteerde formulieren worden automatisch aan het object gekoppeld.

1. (Optioneel) Werk de gegevens bij in de aangepaste velden van het formulier en klik vervolgens op **Wijzigingen opslaan**.

## Meerdere aangepaste formulieren voor een object

U kunt maximaal 10 aangepaste formulieren toevoegen aan een bepaald object, zodat u velden ter beschikking kunt stellen van bepaalde gebruikers en niet van andere gebruikers, of u beter kunt voldoen aan de formuliervereisten van meerdere projecten.

**Voorbeeld:** Als een bestaand project al een aangepast formulier heeft en er meer aangepaste velden nodig zijn voor dit project, dat op een ander aangepast formulier staat, kunt u een tweede formulier aan het project toevoegen met de aanvullende velden in plaats van de velden toe te voegen aan het bestaande aangepaste formulier.

## Een aangepast formulier bulksgewijs aan meerdere objecten toevoegen

U kunt aangepaste formulieren aan meerdere objecten toevoegen door deze in een lijst te selecteren.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>Het toevoegen van aangepaste formulieren aan objecten is hetzelfde voor alle objecten, behalve voor projecten.
>
>Zie het artikel voor informatie over het bulksgewijs toevoegen van aangepaste formulieren aan projecten [Projecten bewerken](../../manage-work/projects/manage-projects/edit-projects.md).


1. Blader naar een lijst met objecten.
1. Selecteer meerdere objecten in de lijst.

1. Klik op de knop **Meer** menu ![](assets/more-icon.png)en klik vervolgens op de knop **Bewerken** pictogram  ![](assets/edit-icon.png).

   of

   Klik op de knop **Bewerken** pictogram ![](assets/edit-icon.png) boven aan de lijst.
1. Klikken **Aangepaste Forms** in het linkerdeelvenster.
1. in de **Een selectie maken** selecteert u het formulier dat u aan alle geselecteerde objecten wilt koppelen.

   >[!NOTE]
   >
   >Als u het formulier niet kunt vinden in het vervolgkeuzemenu, betekent dit dat aan ten minste een van de objecten het formulier al is gekoppeld. Bepaal welk object dat is en verwijder het uit de selectie voordat u het formulier aan de overige objecten kunt toevoegen.


1. Klikken **Wijzigingen opslaan**.

   Als het formulier verplichte velden bevat (gemarkeerd met een rood sterretje), hoeft u deze momenteel niet in te vullen.
