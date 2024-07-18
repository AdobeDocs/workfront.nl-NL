---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Een aangepast veld of aangepaste widget uit het systeem verwijderen
description: Om de systeemprestaties te verbeteren en formulieren gemakkelijker te gebruiken voor gebruikers, kunt u aangepaste velden en widgets van uw systeem verwijderen wanneer deze niet meer worden gebruikt.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Een aangepast veld of aangepaste widget uit het systeem verwijderen

Om de systeemprestaties te verbeteren en formulieren gemakkelijker te gebruiken voor gebruikers, kunt u aangepaste velden en widgets van uw systeem verwijderen wanneer deze niet meer worden gebruikt.

>[!CAUTION]
>
>Als u een aangepast veld verwijdert, worden ook alle aangepaste gegevens verwijderd die gebruikers in het veld hebben ingevoerd wanneer ze aangepaste formulieren invullen die aan objecten zijn gekoppeld. Die verwijderde gegevens kunnen niet worden hersteld.
>
>U kunt alle aangepaste formulieren en rapporten weergeven die een aangepast veld gebruiken dat u wilt verwijderen, om te beoordelen wat de gevolgen kunnen zijn. Voor meer informatie, zie [ Mening alle douanevormen die een bepaald douanegebied of widget ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) en [ gebruiken Mening alle rapporten die een bepaald douanegebied of widget ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md) gebruiken.
>
>Of, voor een alternerende actie kunt u gebruiken om het verliezen van gegevens op niet meer gebruikte gebieden te vermijden, zie [ een douanegebied verwijderen zonder gegevens te verliezen die de gebruikers ](#remove-a-custom-field-without-losing-data-that-users-have-entered) in dit artikel zijn ingegaan.

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

## Een aangepast veld of aangepaste widget uit het systeem verwijderen

{{step-1-to-setup}}

1. Klik **Aangepaste Forms.**
1. Klik **Gebieden** om het gebied van Gebieden te openen.
1. Selecteer het douanegebied of widget, dan klik **Schrapping**.
1. Als u zeker bent u het punt en (in het geval van een douanegebied) alle bijbehorende gegevens over voorwerpen permanent wilt schrappen waar het in bijlage was, ja klikken **, schrap het**.

## Een aangepast veld verwijderen zonder gegevens te verliezen die gebruikers hebben ingevoerd {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>Het verwijderen van een aangepast veld uit een aangepast formulier met meer dan 500 velden en widgets kan niet ongedaan worden gemaakt. Als u het veld verwijdert, kunt u het pas opnieuw toevoegen als het formulier minder dan 500 velden en widgets heeft.

1. Bepaal welke aangepaste velden u uit het oorspronkelijke aangepaste formulier wilt verwijderen, maar verwijder deze op dit moment niet.
1. Een nieuw aangepast formulier maken:

   1. Voeg de aangepaste velden toe aan het nieuwe formulier dat u uit het oorspronkelijke aangepaste formulier wilt verwijderen.

      Voor informatie, zie de sectie [ nieuwe of bestaande gebieden aan uw douanevorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form) in [ Ontwerp een vorm met de vormontwerper ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) toevoegen.

   1. Sla het nieuwe aangepaste formulier op.

1. De toegang van de beperking tot de douanevorm tot slechts gebruikers met administratieve toegang, zoals die in [ wordt beschreven Deel een douanevorm ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. Pas de nieuwe douanevorm op de voorwerpen toe waar de originele douanevorm reeds wordt toegepast, zoals die in [ wordt beschreven voeg een douanevorm aan een voorwerp ](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toe.

   Als u het nieuwe aangepaste formulier op deze objecten toepast, worden historische rapportgegevens niet gewijzigd.

1. Wijzig het oorspronkelijke aangepaste formulier en verwijder de aangepaste velden die u aan het nieuwe formulier hebt toegevoegd (in stap 2).

   De velden die u uit het oorspronkelijke aangepaste formulier hebt verwijderd, zijn nu alleen beschikbaar op het nieuwe aangepaste formulier dat u hebt gemaakt. Gebruikers kunnen het aangepaste formulier bekijken op het object, maar gebruikers zonder beheerdersrechten kunnen het aangepaste formulier niet wijzigen.
