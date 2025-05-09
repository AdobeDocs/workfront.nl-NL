---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Aangepaste formulieren beheren die zijn gekoppeld aan objecten
description: U kunt de volgorde bijwerken waarin de aangepaste formulieren die aan een object zijn gekoppeld, worden weergegeven, verwijderd of de manier waarop aangepaste formulieren op meerdere objecten worden weergegeven, bulksgewijs bewerken.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 0%

---

# Aangepaste formulieren beheren die zijn gekoppeld aan objecten

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

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
   <td> <p>Toegang bewerken tot de objecten waarvoor u aangepaste formulieren beheert</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute-machtigingen of hoger voor de objecten waarvoor u aangepaste formulieren beheert</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Vereisten

* Uw Workfront-beheerder of een Abonnementsgebruiker met beheerdersrechten voor aangepaste formulieren moet aangepaste formulieren maken in uw omgeving. Voor meer informatie, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.
* Er moeten aangepaste formulieren aan een object zijn gekoppeld.

  Voor informatie over hoe te om douaneformulieren op een voorwerp toe te passen, zie [ een douaneformulier aan een voorwerp ](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toevoegen.

## Meerdere aangepaste formulieren die aan een object zijn gekoppeld opnieuw ordenen {#reorder-multiple-custom-forms-attached-to-an-object}

1. Ga naar het object waar u de volgorde van de toegevoegde aangepaste formulieren wilt wijzigen en bewerk het object.

   **Voorbeeld:** Bijvoorbeeld, om de douaneformulieren van een project te beheren, ga naar het project, klik **Meer** menu ![](assets/more-icon.png), dan klik **uitgeven**.

1. In de **sectie van de Douane Forms van 0&rbrace; &lbrace;voor projecten, taken, en kwesties, klik het ![](assets/move-icon---dots.png) pictogram naast de naam van een douanevorm.** Voor alle andere voorwerpen, klik **leiden Forms**. Deze optie wordt alleen weergegeven als ten minste één aangepast formulier aan het object is gekoppeld.
1. Sleep een formulier ![](assets/move-icon---dots.png) naar een nieuwe locatie in de lijst.
1. Voor projecten, taken, en kwesties douaneformulieren, klik **sparen**.

   Voor alle andere voorwerpen, klik **ik wordt gedaan leidend** > **sparen Veranderingen**.

## Een aangepast formulier verwijderen uit een object {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>Wanneer u een aangepast formulier verwijdert uit een object, gaan alle gegevens die zijn vastgelegd in de aangepaste velden van het formulier verloren en kunnen deze niet worden hersteld.

1. Ga naar het object waar u het aangepaste formulier wilt verwijderen en begin het object te bewerken.

   Bijvoorbeeld, ga naar een project, klik **Meer** menu ![](assets/more-icon.png), dan klik **uitgeven**.

1. Klik **Aangepaste Forms**.
1. Voor projecten, taken, en kwesties douanevormen, klik het **X** pictogram rechts van een vorm om het uit het voorwerp te verwijderen.

   Voor alle andere voorwerpen, klik **leiden Forms**, dan klik het **X** pictogram rechts van een vorm om het uit het voorwerp te verwijderen.

1. Klik **sparen**.

## Meerdere aangepaste formulieren beheren die dezelfde aangepaste velden bevatten

Hetzelfde veld wordt mogelijk weergegeven op meerdere aangepaste formulieren die aan hetzelfde object zijn gekoppeld. Overweeg in dit geval het volgende:

* De waarde van het veld is in alle formulieren identiek.

  U kunt geen verschillende waarden voor dezelfde velden hebben op verschillende formulieren die aan hetzelfde object zijn gekoppeld.

* Als u dezelfde berekende velden op twee verschillende objecten hebt, moeten de berekeningen identiek zijn om fouten te voorkomen. Voor informatie over het toevoegen van berekende gebieden aan douanevormen met inbegrip van veelvoudige vormen, zie [ berekende gebieden aan een vorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) toevoegen.

## Meerdere aangepaste formulieren beheren wanneer objecten voor bulkbewerking

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>Het beheren van aangepaste formulieren op objecten is identiek voor alle objecten, behalve voor projecten.
>
>Voor informatie over het toevoegen van douaneformulieren aan projecten in bulk, zie het artikel [ projecten ](../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

Wanneer u objecten voor bulkbewerking gebruikt waarop meerdere aangepaste formulieren zijn toegepast, kunt u de manier bewerken waarop aangepaste formulieren op deze objecten worden weergegeven en kunt u ook gemeenschappelijke velden bewerken in de aangepaste formulieren.

Alleen de aangepaste formulieren die aan alle geselecteerde objecten zijn gekoppeld, kunnen in een bulkbewerking worden bewerkt.

Meerdere aangepaste formulieren bewerken wanneer objecten bulksgewijs worden bewerkt:

1. In een lijstvoorwerpen, selecteer de voorwerpen waar de douaneformulieren in bijlage zijn, dan klik **geef** pictogram ![](assets/edit-icon.png) uit.
1. Klik **Aangepaste Forms**.

   U kunt alleen de aangepaste formulieren bewerken die zijn gekoppeld aan alle geselecteerde objecten.

   Aangepaste formulieren die alleen aan een aantal objecten zijn gekoppeld, worden niet weergegeven.

1. Velden op aangepaste formulieren bewerken.

   Wanneer velden worden bewerkt, wordt in het veld een visuele indicator weergegeven die aangeeft dat het veld is bewerkt.

   Als een veld op meerdere aangepaste formulieren wordt opgenomen, worden alle waarden van die velden op elk formulier bijgewerkt wanneer u het veld op een van de formulieren bijwerkt.

1. Klik **maak een selectie** drop-down menu en selecteer extra vormen om aan alle geselecteerde voorwerpen toe te voegen.

   Houd rekening met het volgende wanneer u aanvullende formulieren toepast:

   * Objecten kunnen maximaal 10 aangepaste formulieren hebben.
   * U kunt formulieren alleen toepassen als het formulier nog niet is toegepast op een van de objecten die u bewerkt. Een formulier dat al aan een van de objecten is gekoppeld, wordt niet weergegeven in het vervolgkeuzemenu.
   * Nadat u een extra vorm toepast, worden om het even welke gebieden die de vorm met andere vormen gemeenschappelijk heeft getoond in de **Gemeenschappelijke Gebieden** sectie, en zij kunnen worden uitgegeven.

1. (Optioneel) Als u aangepaste formulieren hebt toegevoegd aan alle objecten, maar de objecten nog niet hebt opgeslagen, kunt u de volgorde wijzigen waarin de aangepaste formulieren op de objecten worden weergegeven.

   Voor meer informatie over het veranderen van de orde van de vormen, zie [ veelvoudige douaneformulieren opnieuw ordenen in bijlage aan een voorwerp ](#reorder-multiple-custom-forms-attached-to-an-object) in dit artikel.

1. Klik **verwijderen Vorm** om een douanevorm uit de voorwerpen te verwijderen.

   Voor meer informatie over het verwijderen van douaneformulieren uit voorwerpen, zie [ een douaneformulier uit een voorwerp ](#remove-a-custom-form-from-an-object) verwijderen.

   Houd rekening met het volgende wanneer u bulkformulieren van verschillende objecten verwijdert:

   * Als u wijzigingen in het formulier hebt aangebracht, gaan de wijzigingen verloren en kunnen deze niet worden hersteld.
   * Nadat u een vorm verwijdert, worden om het even welke gebieden uit die vorm die in de **Gemeenschappelijke Gebieden** sectie waren verwijderd uit deze sectie en kunnen niet meer hier worden uitgegeven.

1. Klik **Herstel Vorm** om de vorm aan de staat te herstellen het was binnen alvorens u de voorwerpen uitgeeft.
1. (Optioneel) Klik op de pijl samenvouwen naast de naam van het formulier om één formulier tegelijk samen te vouwen.

   of

   Klik **samenvouwen Forms** om alle vormen tezelfdertijd samen te vouwen.

1. (Optioneel) Klik op de pijl uitvouwen naast de naam van het formulier om één formulier tegelijk uit te vouwen.

   of

   Klik **breid Forms** uit om alle vormen tezelfdertijd uit te breiden. 

1. Klik **sparen Veranderingen**.
