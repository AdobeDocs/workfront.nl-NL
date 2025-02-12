---
title: Aangepaste formuliergegevens overdragen bij het converteren van een object
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Wanneer het werk dat in een het werkpunt wordt bepaald te groot wordt, kunt u het in een groter het werkpunt omzetten.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Aangepaste formuliergegevens overbrengen bij de conversie van een object

Afhankelijk van de bedrijfsbehoeften van uw organisatie, zou het werk dat in een taak of een kwestie wordt bepaald te groot kunnen worden om binnen de taak of de kwestie te leiden. In dit geval kunt u ze omzetten in een groter werkitem:

* U kunt uitgaven in taken of in projecten omzetten
* U kunt taken omzetten in projecten

Als u aangepaste formuliergegevens van een uitgave wilt overbrengen naar een taak of project, moet u de twee taken in dit artikel in de onderstaande volgorde uitvoeren.

Voor meer informatie, zie [ Overzicht van het omzetten van kwesties in Adobe Workfront ](../../../manage-work/issues/convert-issues/convert-issues.md) of [ Overzicht van het omzetten van kwesties in Adobe Workfront ](../../../manage-work/issues/convert-issues/convert-issues.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

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

+++

## Ten eerste: extra objecten toevoegen aan het aangepaste formulier

{{step-1-to-setup}}

1. Klik **Aangepaste Forms**.
1. Vind de vorm u nodig hebt, dan klik ![ uitgeven pictogram ](assets/edit-icon.png).
1. Voeg boven aan het formulier het object toe waarnaar u de taak of uitgave wilt converteren.

   >[!INFO]
   >
   >**Voorbeeld**: Als u de gegevens van de douanevorm aan een project wilt overbrengen, uitgezochte Project.

1. Klik **toepassen** bij de bodem van de vorm.

1. Ga op [ Tweede verder: Zet de kwestie of de taak om en breng de gegevens van de douanevorm ](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data) over.

## Ten tweede: converteer de uitgave of taak en breng de aangepaste formuliergegevens over {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Voeg extra voorwerpen aan de douanevorm op de kwestie of de taak toe u, zoals die in de sectie [ eerst wordt verklaard: Voeg extra voorwerpen aan de douanevorm ](#first-add-additonal-objects-to-the-custom-form) in dit artikel toe.
1. Zet de kwestie of de taak om gebruikend de **optie van Forms van de Douane** in de doos die toont om de douanevorm te selecteren u wenst. Zie de volgende artikelen voor instructies:

   * [Een uitgave converteren naar een project in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Een uitgave converteren naar een taak in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Een taak omzetten in een project](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. In **Bekeerling aan (objecten type)** dialoogdoos die toont, klik **toevoegen Forms** drop-down menu en selecteer de vorm u in de vorige sectie kopieerde.

   De informatie die wordt vastgelegd in de aangepaste velden van de uitgave wordt nu overgebracht naar het aangepaste formulier op de taak.


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->