---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Aangepaste formulieren beheren die zijn gekoppeld aan objecten
description: U kunt de volgorde bijwerken waarin de aangepaste formulieren die aan een object zijn gekoppeld, worden weergegeven, verwijderd of de manier waarop aangepaste formulieren op meerdere objecten worden weergegeven, bulksgewijs bewerken.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 78de23b4d5814e5e2ead6bb61a80bba7bd2aed33
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 0%

---

# Aangepaste formulieren beheren die zijn gekoppeld aan objecten

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span>  -->

U kunt de volgorde bijwerken waarin de aangepaste formulieren die aan een object zijn gekoppeld, worden weergegeven, verwijderd of de manier waarop aangepaste formulieren op meerdere objecten worden weergegeven, bulksgewijs bewerken.

## Toegangsvereisten

U moet de volgende toegang hebben om de handelingen uit te voeren die in dit artikel worden beschreven:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang bewerken tot de objecten waarvoor u aangepaste formulieren beheert</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute-machtigingen of hoger voor objecten waarvoor u aangepaste formulieren beheert</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

* Uw Workfront-beheerder of een Abonnementsgebruiker met beheerdersrechten voor aangepaste formulieren moet aangepaste formulieren maken in uw omgeving. Zie voor meer informatie [Een aangepast formulier maken of bewerken](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* Er moeten aangepaste formulieren aan een object zijn gekoppeld.

   Zie voor informatie over het toepassen van aangepaste formulieren op een object [Een aangepast formulier toevoegen aan een object](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Meerdere aangepaste formulieren die aan een object zijn gekoppeld opnieuw ordenen {#reorder-multiple-custom-forms-attached-to-an-object}

1. Ga naar het object waar u de volgorde van de toegevoegde aangepaste formulieren wilt wijzigen en bewerk het object.

   **Voorbeeld:** Als u bijvoorbeeld de aangepaste formulieren van een project wilt beheren, gaat u naar het project en klikt u op de knop **Meer** menu ![](assets/more-icon.png)en klik vervolgens op **Bewerken** .

1. In de **Aangepaste Forms** voor projecten, taken en problemen klikt u op de knop ![](assets/move-icon---dots.png) naast de naam van een aangepast formulier. Voor alle andere objecten klikt u op **Forms beheren**. Deze optie wordt alleen weergegeven als ten minste één aangepast formulier aan het object is gekoppeld.
1. Een formulier slepen ![](assets/move-icon---dots.png) naar een nieuwe locatie in de lijst.
1. Klik voor projecten, taken en aangepaste formulieren **Opslaan**.

   Voor alle andere objecten klikt u op **Ik ben klaar met beheren** > **Wijzigingen opslaan**.

## Een aangepast formulier verwijderen uit een object {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>Wanneer u een aangepast formulier verwijdert uit een object, gaan alle gegevens die zijn vastgelegd in de aangepaste velden van het formulier verloren en kunnen deze niet worden hersteld.

1. Ga naar het object waar u het aangepaste formulier wilt verwijderen en begin met het bewerken van het object.

   Ga bijvoorbeeld naar een project en klik op de knop **Meer** menu ![](assets/more-icon.png)en klik vervolgens op **Bewerken** .

1. Klikken **Aangepaste Forms**.
1. Voor projecten, taken en geeft aangepaste formulieren weer, klikt u op de knop **X** aan de rechterkant van een formulier om het uit het object te verwijderen.

   Voor alle andere objecten klikt u op **Forms beheren** klikt u op de knop **X** aan de rechterkant van een formulier om het uit het object te verwijderen.

1. Klikken **Opslaan** .

## Meerdere aangepaste formulieren beheren die dezelfde aangepaste velden bevatten

Hetzelfde veld wordt mogelijk weergegeven op meerdere aangepaste formulieren die aan hetzelfde object zijn gekoppeld. Overweeg in dit geval het volgende:

* De waarde van het veld is in alle formulieren identiek.

   U kunt geen verschillende waarden voor dezelfde velden hebben op verschillende formulieren die aan hetzelfde object zijn gekoppeld.

* Als u dezelfde berekende velden op twee verschillende objecten hebt, moeten de berekeningen identiek zijn om fouten te voorkomen. Zie voor informatie over het toevoegen van berekende velden aan aangepaste formulieren, inclusief meerdere formulieren [Berekende gegevens toevoegen aan een aangepast formulier](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) .

## Meerdere aangepaste formulieren beheren wanneer objecten voor bulkbewerking

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:

>[!NOTE]
>
><span class="preview">For information about managing custom forms on projects in bulk in the Preview environment, see the article [Edit projects](../../manage-work/projects/manage-projects/edit-projects.md)</span>.

-->

Wanneer u objecten voor bulkbewerking gebruikt waarop meerdere aangepaste formulieren zijn toegepast, kunt u de manier bewerken waarop aangepaste formulieren op deze objecten worden weergegeven en kunt u ook gemeenschappelijke velden bewerken in de aangepaste formulieren.

Alleen aangepaste formulieren die aan alle geselecteerde objecten zijn gekoppeld, kunnen in een bulkbewerking worden bewerkt.

Meerdere aangepaste formulieren bewerken wanneer objecten bulksgewijs worden bewerkt:

1. Selecteer in een lijst de objecten waaraan de aangepaste formulieren zijn gekoppeld en klik op de knop **Bewerken** pictogram ![](assets/edit-icon.png).
1. Klikken **Aangepaste Forms**.

   U kunt alleen de aangepaste formulieren bewerken die zijn gekoppeld aan alle geselecteerde objecten.

   Aangepaste formulieren die alleen aan een aantal objecten zijn gekoppeld, worden niet weergegeven.

1. Velden op aangepaste formulieren bewerken.

   Wanneer velden worden bewerkt, wordt in het veld een visuele indicator weergegeven die aangeeft dat het veld is bewerkt.

   Als een veld op meerdere aangepaste formulieren wordt opgenomen, worden alle waarden van die velden op elk formulier bijgewerkt wanneer u het veld op een van de formulieren bijwerkt.

1. Klik op de knop **Een selectie maken** en selecteert u aanvullende formulieren die u aan alle geselecteerde objecten wilt toevoegen.

   Houd rekening met het volgende wanneer u aanvullende formulieren toepast:

   * Objecten kunnen maximaal 10 aangepaste formulieren hebben.
   * U kunt formulieren alleen toepassen als het formulier nog niet is toegepast op een van de objecten die u bewerkt. Een formulier dat al aan een van de objecten is gekoppeld, wordt niet weergegeven in het vervolgkeuzemenu.
   * Nadat u een aanvullend formulier hebt toegepast, worden alle velden die formulieren gemeen hebben met andere formulieren weergegeven in het dialoogvenster **Algemene velden** en kunnen worden bewerkt.

1. (Optioneel) Als u aangepaste formulieren hebt toegevoegd aan alle objecten, maar de objecten nog niet hebt opgeslagen, kunt u de volgorde wijzigen waarin de aangepaste formulieren op de objecten worden weergegeven.

   Zie voor meer informatie over het wijzigen van de volgorde van de formulieren [Meerdere aangepaste formulieren die aan een object zijn gekoppeld opnieuw ordenen](#reorder-multiple-custom-forms-attached-to-an-object) in dit artikel.

1. Klikken **Formulier verwijderen** om een aangepast formulier uit de objecten te verwijderen.

   Zie voor meer informatie over het verwijderen van aangepaste formulieren uit objecten [Een aangepast formulier verwijderen uit een object](#remove-a-custom-form-from-an-object).

   Houd rekening met het volgende wanneer u bulkformulieren van verschillende objecten verwijdert:

   * Als u wijzigingen in het formulier hebt aangebracht, gaan de wijzigingen verloren en kunnen deze niet worden hersteld.
   * Nadat u een formulier hebt verwijderd, worden alle velden uit dat formulier die zich in het dialoogvenster **Algemene velden** worden verwijderd uit deze sectie en kunnen hier niet meer worden bewerkt.

1. Klikken **Formulier herstellen** om de status van het formulier te herstellen voordat u de objecten hebt bewerkt.
1. (Optioneel) Klik op de pijl samenvouwen naast de naam van het formulier om één formulier tegelijk samen te vouwen.

   of

   Klikken **Forms samenvouwen** om alle formulieren tegelijk samen te vouwen.

1. (Optioneel) Klik op de pijl uitvouwen naast de naam van het formulier om één formulier tegelijk uit te vouwen.

   of

   Klikken **Forms uitbreiden** om alle formulieren tegelijk uit te vouwen. 

1. Klikken **Wijzigingen opslaan**.
