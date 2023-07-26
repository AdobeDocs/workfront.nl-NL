---
title: Aangepaste formuliergegevens overbrengen bij de conversie van een object
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Wanneer het werk dat in een het werkpunt wordt bepaald te groot wordt, kunt u het in een groter het werkpunt omzetten.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Aangepaste formuliergegevens overbrengen bij de conversie van een object

Afhankelijk van de bedrijfsbehoeften van uw organisatie, zou het werk dat in een taak of een kwestie wordt bepaald te groot kunnen worden om binnen de taak of de kwestie te leiden. In dit geval kunt u ze omzetten in een groter werkitem:

* U kunt uitgaven in taken of in projecten omzetten
* U kunt taken omzetten in projecten

Als u aangepaste formuliergegevens van een uitgave wilt overbrengen naar een taak of project, moet u de twee taken in dit artikel in de onderstaande volgorde uitvoeren.

Zie voor meer informatie [Overzicht van conversie van problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md) of [Overzicht van conversie van problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

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
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> <p>Ga voor informatie over hoe Workfront-beheerders deze toegang verlenen naar <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, type licentie of configuraties op toegangsniveau u hebt.

## Eerste: extra objecten toevoegen aan het aangepaste formulier

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Aangepaste Forms**.
1. Zoek het formulier dat u nodig hebt en klik op **Bewerken**.
1. Voeg boven aan het formulier het object toe waarnaar u de taak of uitgave wilt converteren.
   >[!INFO]
   >
   >**Voorbeeld**: Selecteer Project als u de aangepaste formuliergegevens naar een project wilt overbrengen.

1. Klikken **Toepassen** onder aan het formulier.

1. Doorgaan naar [Ten tweede: converteer de uitgave of taak en breng de aangepaste formuliergegevens over](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Ten tweede: converteer de uitgave of taak en breng de aangepaste formuliergegevens over {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Voeg aanvullende objecten toe aan het aangepaste formulier voor de uitgave of taak die u converteert, zoals wordt uitgelegd in de sectie [Ten eerste: extra objecten toevoegen aan het aangepaste formulier](#first-add-additonal-objects-to-the-custom-form) in dit artikel.
1. Converteer het probleem of de taak met de opdracht **Aangepaste Forms** in het vak dat wordt weergegeven om het aangepaste formulier te selecteren dat u nodig hebt. Zie de volgende artikelen voor instructies:

   * [Een uitgave converteren naar een project in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Een uitgave converteren naar een taak in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Een taak omzetten in een project](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. In de **Omzetten in (objecttype)** klikt u op het dialoogvenster dat wordt weergegeven **Forms toevoegen** en selecteert u het formulier dat u in de vorige sectie hebt gekopieerd.

   De informatie die wordt vastgelegd in de aangepaste velden van de uitgave wordt nu overgebracht naar het aangepaste formulier op de taak.


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see the section [Start editing a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) in the article [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->