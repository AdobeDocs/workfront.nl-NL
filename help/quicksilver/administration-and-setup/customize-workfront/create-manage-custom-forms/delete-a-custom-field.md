---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Een aangepast veld of aangepaste widget uit het systeem verwijderen
description: Om de systeemprestaties te verbeteren en formulieren gemakkelijker te gebruiken voor gebruikers, kunt u aangepaste velden en widgets van uw systeem verwijderen wanneer deze niet meer worden gebruikt.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Een aangepast veld of aangepaste widget uit het systeem verwijderen

Om de systeemprestaties te verbeteren en formulieren gemakkelijker te gebruiken voor gebruikers, kunt u aangepaste velden en widgets van uw systeem verwijderen wanneer deze niet meer worden gebruikt.

>[!CAUTION]
>
>Als u een aangepast veld verwijdert, worden ook alle aangepaste gegevens verwijderd die gebruikers in het veld hebben ingevoerd wanneer ze aangepaste formulieren invullen die aan objecten zijn gekoppeld. Die verwijderde gegevens kunnen niet worden hersteld.
>
>U kunt alle aangepaste formulieren en rapporten weergeven die een aangepast veld gebruiken dat u wilt verwijderen, om te beoordelen wat de gevolgen kunnen zijn. Zie voor meer informatie [Alle aangepaste formulieren weergeven die een bepaald aangepast veld of een bepaalde aangepaste widget gebruiken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) en [Alle rapporten weergeven die een bepaald aangepast veld of een bepaalde widget gebruiken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>Of, voor een oplossing kunt u gebruiken om gegevensverlies te vermijden in velden die niet meer worden gebruikt, zie [Een aangepast veld verwijderen zonder gegevens te verliezen die gebruikers hebben ingevoerd](#remove-a-custom-field-without-losing-data-that-users-have-entered) in dit artikel.

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
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> <p>Voor informatie over hoe de beheerders van Workfront deze toegang verlenen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, type licentie of configuraties op toegangsniveau u hebt.

## Een aangepast veld of aangepaste widget uit het systeem verwijderen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Aangepaste Forms.**
1. Klik op de knop **Velden** tab.
1. Selecteer het aangepaste veld of de aangepaste widget en klik vervolgens op **Verwijderen**.
1. Als u zeker weet dat u het item permanent wilt verwijderen en (in het geval van een aangepast veld) alle bijbehorende gegevens op de objecten waar het is gekoppeld, klikt u op **Ja, verwijderen**.

## Een aangepast veld verwijderen zonder gegevens te verliezen die gebruikers hebben ingevoerd {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>Het verwijderen van een aangepast veld uit een aangepast formulier met meer dan 500 velden en widgets kan niet ongedaan worden gemaakt. Als u het veld verwijdert, kunt u het pas opnieuw toevoegen als het formulier minder dan 500 velden en widgets heeft.

1. Bepaal welke aangepaste velden u uit het oorspronkelijke aangepaste formulier wilt verwijderen, maar verwijder deze op dit moment niet.
1. Een nieuw aangepast formulier maken:

   1. Voeg de aangepaste velden toe aan het nieuwe formulier dat u uit het oorspronkelijke aangepaste formulier wilt verwijderen.

      * Als u de aangepaste formulierbuilder gebruikt, raadpleegt u [Een aangepast veld of aangepaste widget opnieuw gebruiken in een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).
      * Als u de formulierontwerper gebruikt, raadpleegt u [Nieuwe of bestaande velden toevoegen aan uw aangepaste formulier](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form).

   1. Sla het nieuwe aangepaste formulier op.

1. De toegang tot het aangepaste formulier beperken tot gebruikers met beheerdersrechten, zoals beschreven in [Een aangepast formulier delen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. Pas het nieuwe aangepaste formulier toe op de objecten waarop het oorspronkelijke aangepaste formulier al is toegepast, zoals beschreven in [Een aangepast formulier toevoegen aan een object](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   Als u het nieuwe aangepaste formulier op deze objecten toepast, worden historische rapportgegevens niet gewijzigd.

1. Wijzig het oorspronkelijke aangepaste formulier en verwijder de aangepaste velden die u aan het nieuwe formulier hebt toegevoegd (in stap 2).

   De velden die u uit het oorspronkelijke aangepaste formulier hebt verwijderd, zijn nu alleen beschikbaar op het nieuwe aangepaste formulier dat u hebt gemaakt. Gebruikers kunnen het aangepaste formulier bekijken op het object, maar gebruikers zonder beheerdersrechten kunnen het aangepaste formulier niet wijzigen.
