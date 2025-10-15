---
product-area: projects;user-management
keywords: bewerken,formulieren,rich,tekst,speciaal,indeling,velden,aangepast,informatie,aanpassen,objecten
navigation-topic: work-with-custom-forms
title: Gegevens bewerken in aangepaste formuliervelden
description: U kunt gegevens op een aangepast formulier bewerken nadat het formulier aan een object is gekoppeld. Zie Een aangepast formulier toevoegen aan een object voor informatie over het toevoegen van aangepaste formulieren aan objecten.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '985'
ht-degree: 0%

---

# Gegevens bewerken in aangepaste formuliervelden

<!--Audited: 10/2025-->

U kunt gegevens op een aangepast formulier bewerken nadat het formulier aan een object is gekoppeld. Voor informatie over het toevoegen van douaneformulieren aan voorwerpen, zie [ een douaneformulier aan een voorwerp ](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toevoegen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-pakket</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-licentie</p> </td> 
   <td> <p>Medewerker of hoger</p> 
   <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang bewerken tot het object waarvoor u het aangepaste formulier wilt bewerken</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Objectmachtigingen</p> </td> 
   <td> 
    <ul> 
     <li> <p>Contribute of hoger voor het object waarvoor u het aangepaste formulier wilt bewerken</p> </li> 
     <li><p>Machtigingen weergeven voor de velden die u wilt bewerken.</p></li> 
     <li><p>Machtigingen bewerken voor de secties in het formulier waar de velden die u wilt bewerken zich bevinden</p></li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Team or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront licenses*</p> </td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to the object for which you want to edit the custom form</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> 
    <ul> 
     <li> <p>Contribute or higher permissions on the object for which you want to edit the custom form</p> </li> 
     <li>View permissions on the fields you want to edit. For information about sharing permissions for custom fields, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/share-custom-fields.md" class="MCXref xref">Configure sharing for custom fields and widgets</a>.</li> 
     <li> <p>Edit permissions for the sections on the form where the fields you want to edit are located</p> </li> 
    </ul> <p>For information on requesting additional access for objects, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Vereisten

* Uw Workfront-beheerder of een Abonnementsgebruiker met beheerdersrechten voor aangepaste formulieren moet aangepaste formulieren maken in uw omgeving. Voor meer informatie, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.
* Er moeten aangepaste formulieren aan een object zijn gekoppeld.

  Voor informatie over hoe te om douaneformulieren op een voorwerp toe te passen, zie [ een douaneformulier aan een voorwerp ](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toevoegen.

## Informatie bewerken op een aangepast formulier

Het bewerken van gegevens op een aangepast formulier dat aan een object is gekoppeld, is identiek voor alle objecten. Voor informatie over welke voorwerpen een douanevorm kunnen hebben, zie [ overzicht van de Vorm van de Douane ](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. Ga naar een object waarvan u de gegevens in het aangepaste formulier wilt bewerken.
1. Klik op **`<Object type>`Details** in het linkerdeelvenster.

   Bijvoorbeeld, wanneer het uitgeven van informatie over een vorm van de projectdouane, klik **Details van het Project**.

1. Blader naar het aangepaste formulier. Als er een aangepast formulier aan het object is gekoppeld, wordt de naam van het formulier als een gebied weergegeven in de sectie Details.
1. Klik zo nodig op de pijl ![](assets/expand-arrow-right.png) links van de naam van het aangepaste formulier om het uit te vouwen.
1. Klik in de rechterbovenhoek van de pagina op het pictogram Bewerken ![](assets/edit-icon.png) .
1. Voer de gegevens in een veld in waartoe u toegang hebt.

   ![](assets/click-in-field-to-edit-info-350x132.png)

   of

   Als geen informatie nog op de vorm is ingegaan, klik **Add+** voor om het even welk gebied u toegang tot hebt en begin informatie in te gaan.

   ![](assets/plus-add-to-edit-info-350x180.png)

   Als er meerdere aangepaste formulieren aan het object zijn gekoppeld, kunt u dit voor elk formulier doen.

   Afhankelijk van het type veld waarin u werkt, kunt u het volgende overwegen:

   * U kunt slechts één optie selecteren voor velden met keuzerondjes.
   * U kunt een of meerdere opties selecteren in een selectievakje, afhankelijk van de configuratie van het veld door de maker van het formulier.
   * U kunt een of meerdere opties selecteren in een meerkeuzeveld, afhankelijk van de configuratie van het veld door de maker van het formulier.
   * U kunt tekstvelden alleen opmaken (vet, cursief of onderstrepen) als de gebruiker die het formulier heeft gemaakt, deze heeft ingesteld als een tekstveld met het veldtype Opmaak. Tekstvelden met één regel en tekstvelden met één regel kunnen niet worden opgemaakt.
   * U kunt de tijd van de dag alleen bijwerken in een datumveldtype als de gebruiker die het formulier heeft gemaakt het heeft opgenomen tijdens het maken van het veld.

   Voor informatie over alle gebiedstypes, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

1. Klik **sparen Veranderingen**.

   >[!IMPORTANT]
   >
   >U moet alle vereiste velden op het formulier invullen voordat u het formulier kunt opslaan. De naam van een vereist veld wordt gevolgd door een sterretje.
   >
   >![](assets/nwe-required-custom-field.png)

   Wanneer iemand gegevens wijzigt in een ander object waarnaar wordt verwezen door berekende aangepaste velden in het object, worden de wijzigingen niet automatisch doorgevoerd in het object. Voor informatie over het manueel bijwerken van alle berekende douanegebieden in uw voorwerp, zie [ alle berekende douanegebieden voor een voorwerp ](#recalculate-all-calculated-custom-fields-for-an-object) in dit artikel opnieuw berekenen.

   Wanneer afhankelijke velden op de pagina worden gewijzigd, worden berekende velden op het aangepaste formulier dynamisch opnieuw berekend in real-time. U kunt de nieuwe berekende veldwaarde zien zonder het formulier op te slaan, maar deze wordt pas daadwerkelijk toegepast op het formulier en het object als u de wijzigingen opslaat. Dit geldt zowel voor berekende velden op standaardformulieren als voor aangepaste formulieren.

   U kunt ook handmatig alle berekende aangepaste velden voor een object bijwerken wanneer u het object samen met andere objecten in een lijst bulksgewijs bewerkt. Voor instructies, zie [ alle berekende douanegebieden voor veelvoudige voorwerpen in een lijst opnieuw berekenen wanneer het uitgeven van de voorwerpen ](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) in dit artikel.

## Alle berekende aangepaste velden voor een object opnieuw berekenen  {#recalculate-all-calculated-custom-fields-for-an-object}

1. Ga naar de hoofdpagina van het object waarvan u de aangepaste velden opnieuw wilt berekenen.
1. Klik **Meer** menu ![](assets/more-icon.png) aan het recht van de naam van het voorwerp, dan klik **opnieuw berekende Uitdrukkingen**.

   Hiermee worden alle aangepaste velden op het formulier van het object opnieuw berekend.

## Alle berekende aangepaste velden voor meerdere objecten in een lijst opnieuw berekenen wanneer u de objecten bewerkt {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

U kunt de aangepaste velden van verschillende objecten handmatig opnieuw berekenen door deze los van een lijst of rapport te bewerken.

1. Ga naar een lijst met objecten die aangepaste formulieren met berekende velden bevatten.
1. Selecteer de objecten waarvan u de berekende aangepaste velden wilt bijwerken.
1. Klik het **uitgeven pictogram**.
1. Klik **Forms van de Douane** in het linkermenu, dan selecteren **de Uitdrukkingen van de Douane** opnieuw berekenen.
1. Klik **sparen** **Veranderingen**.

   Workfront berekent alle aangepaste velden voor alle geselecteerde objecten.

>[!TIP]
>
>U kunt aangepaste expressies ook opnieuw berekenen vanuit een lijst met objecten. Bijvoorbeeld, om douaneuitdrukkingen in massa van een lijst van projecten opnieuw te berekenen:
>
>1. Ga naar een projectlijst of rapport en selecteer één of verscheidene projecten.
>1. Klik **Meer** menu ![](assets/more-icon.png), dan klik **opnieuw berekenen de Uitdrukkingen van de Douane**.
>
>![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)
>
>Workfront berekent alle aangepaste velden voor alle geselecteerde projecten.
>>Niet alle lijsten met alle objecten hebben deze mogelijkheid.
>
>Afhankelijk van de complexiteit van uw projecten raden we u aan geen groot aantal projecten te selecteren wanneer u berekende aangepaste velden bulksgewijs herberekent voor optimale prestaties. Sommige dingen die een project te complex zouden kunnen maken zouden veelvoudige gebiedsdelen of taken of een groot aantal douanevelden kunnen zijn.

