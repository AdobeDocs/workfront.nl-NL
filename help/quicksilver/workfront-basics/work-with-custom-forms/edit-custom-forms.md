---
product-area: projects;user-management
keywords: bewerken,formulieren,rich,tekst,speciaal,indeling,velden,aangepast,informatie,aanpassen,objecten
navigation-topic: work-with-custom-forms
title: Gegevens bewerken in aangepaste formuliervelden
description: U kunt gegevens op een aangepast formulier bewerken nadat het formulier aan een object is gekoppeld. Zie Een aangepast formulier toevoegen aan een object voor informatie over het toevoegen van aangepaste formulieren aan objecten.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 0%

---

# Gegevens bewerken in aangepaste formuliervelden

<!--Audited: 10/2025-->

U kunt gegevens op een aangepast formulier bewerken nadat het formulier aan een object is gekoppeld. Voor informatie over het toevoegen van douaneformulieren aan voorwerpen, zie [&#x200B; een douaneformulier aan een voorwerp &#x200B;](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toevoegen.

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

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

* Uw Workfront-beheerder of een Abonnementsgebruiker met beheerdersrechten voor aangepaste formulieren moet aangepaste formulieren maken in uw omgeving. Voor meer informatie, zie [&#x200B; een douaneformulier &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.
* Er moeten aangepaste formulieren aan een object zijn gekoppeld.

  Voor informatie over hoe te om douaneformulieren op een voorwerp toe te passen, zie [&#x200B; een douaneformulier aan een voorwerp &#x200B;](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toevoegen.

## Informatie bewerken op een aangepast formulier

Het bewerken van gegevens op een aangepast formulier dat aan een object is gekoppeld, is voor de meeste objecten hetzelfde.

Voor informatie over welke voorwerpen een douanevorm kunnen hebben, zie [&#x200B; overzicht van de Vorm van de Douane &#x200B;](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. Ga naar een lijst met objecten waarvoor u gegevens op het aangepaste formulier wilt bewerken, behalve een lijst met herhalingen.
1. Selecteer één of verscheidene voorwerpen in de lijst, dan klik **uitgeven** pictogram ![&#x200B; pictogram &#x200B;](assets/edit-icon.png) bij de bovenkant van de lijst uitgeven.
1. Klik **Forms van de Douane** in het linkerpaneel, binnen **uitgeven &lt; voorwerp >** doos.

   Wanneer er een douaneformulier in bijlage aan het voorwerp is, toont de naam van de vormvertoningen als gebied in de **sectie van de Forms van de Douane**.
1. Voer de gegevens in een veld in waartoe u toegang hebt.

   ![&#x200B; geef doos met douanevormen op het Factureren Verslag uit &#x200B;](assets/edit-box-with-custom-forms-on-billing-record.png)

   Als er meerdere aangepaste formulieren aan het object zijn gekoppeld, doet u dit voor elk formulier.

   Afhankelijk van het type veld waarin u werkt, kunt u het volgende overwegen:

   * U kunt slechts één optie selecteren voor velden met keuzerondjes.
   * U kunt een of meerdere opties selecteren in een selectievakje, afhankelijk van de configuratie van het veld door de maker van het formulier.
   * U kunt een of meerdere opties selecteren in een meerkeuzeveld, afhankelijk van de configuratie van het veld door de maker van het formulier.
   * U kunt tekstvelden alleen opmaken (vet, cursief of onderstrepen) als de gebruiker die het formulier heeft gemaakt, deze heeft ingesteld als een tekstveld met het veldtype Opmaak. Tekstvelden met één regel en tekstvelden met één regel kunnen niet worden opgemaakt.
   * U kunt de tijd van de dag alleen bijwerken in een datumveldtype als de gebruiker die het formulier heeft gemaakt het heeft opgenomen tijdens het maken van het veld.

   >[!NOTE]
   >
   >Velden waarin meerdere selecties zijn toegestaan, beperken mogelijk het aantal opties dat u kunt kiezen. Selectievakjes en meerkeuzevrijheid zijn beperkt tot 5000 selecties.

   Voor informatie over alle gebiedstypes, zie [&#x200B; een douaneformulier &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

1. Klik **sparen**.

   >[!IMPORTANT]
   >
   >U moet alle vereiste velden op het formulier invullen voordat u het formulier kunt opslaan. De naam van een vereist veld wordt gevolgd door een sterretje.
   >
   >![&#x200B; Vereist gebied van de douane &#x200B;](assets/nwe-required-custom-field.png)

   Wanneer iemand gegevens wijzigt in een ander object waarnaar wordt verwezen door berekende aangepaste velden in het object, worden de wijzigingen niet automatisch doorgevoerd in het object. Voor informatie over het manueel bijwerken van alle berekende douanegebieden in uw voorwerp, zie [&#x200B; alle berekende douanegebieden voor een voorwerp &#x200B;](#recalculate-all-calculated-custom-fields-for-an-object) in dit artikel opnieuw berekenen.

   Wanneer afhankelijke velden op de pagina worden gewijzigd, worden berekende velden op het aangepaste formulier dynamisch opnieuw berekend in real-time. U kunt de nieuwe berekende veldwaarde zien zonder het formulier op te slaan, maar deze wordt pas daadwerkelijk toegepast op het formulier en het object als u de wijzigingen opslaat. Dit geldt zowel voor berekende velden op standaardformulieren als voor aangepaste formulieren.

   U kunt ook handmatig alle berekende aangepaste velden voor een object bijwerken wanneer u het object samen met andere objecten in een lijst bulksgewijs bewerkt. Voor instructies, zie [&#x200B; alle berekende douanegebieden voor veelvoudige voorwerpen in een lijst opnieuw berekenen wanneer het uitgeven van de voorwerpen &#x200B;](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) in dit artikel.

1. (Voorwaardelijk) Als u de aangepaste velden voor een aangepaste herhalingsformulier wilt bijwerken, gaat u als volgt te werk:

   1. Ga naar een herhaling.
   1. Klik **Forms van de Douane** in het linkerpaneel.
   1. Om douanevormen toe te voegen, begin de naam van een vorm in **te typen voeg douanevorm** gebied in de hoger-juiste hoek van de pagina toe

      of

      Klik **uitgeven** pictogram op het zelfde gebied om de gebieden op de in bijlage vormen te beginnen uitgeven.

      ![&#x200B; geef de vorm van de iteratie douane &#x200B;](assets/edit-iteration-custom-form.png) uit

   1. Klik **sparen Veranderingen**.

## Aangepaste velden voor objecten opnieuw berekenen

Afhankelijk van wijzigingen die zich kunnen voordoen in aangepaste formulieren of wijzigingen die optreden in velden waarnaar wordt verwezen in aangepaste velden, kunnen de waarden van berekende aangepaste velden periodiek worden verouderd. In dit geval moet u mogelijk aangepaste velden opnieuw berekenen of de aangepaste expressies voor objecten opnieuw berekenen.

In de volgende secties wordt beschreven hoe u aangepaste expressies voor objecten met aangepaste formulieren opnieuw kunt berekenen.

>[!NOTE]
>
>U kunt aangepaste expressies niet opnieuw berekenen voor groepen.

### Alle berekende aangepaste velden opnieuw berekenen op de objectpagina

>[!IMPORTANT]
>
>Er moet een aangepast formulier met berekende velden aan het object zijn gekoppeld voordat u de stappen in deze sectie kunt volgen.

1. Ga naar de hoofdpagina van een van de volgende objecten waarvan u de aangepaste velden opnieuw wilt berekenen:

   * Project
   * Taak
   * Probleem
   * Portfolio
   * Programma
   * Document

1. Klik het **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-icon.png) aan het recht van de naam van de objecten, dan klik **Uitdrukkingen** opnieuw berekenen.

   Hiermee worden alle aangepaste velden op het formulier van het object opnieuw berekend.

### Alle berekende aangepaste velden voor meerdere objecten in een lijst opnieuw berekenen wanneer u de objecten bewerkt {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

Afhankelijk van de objecten waarvoor u de aangepaste expressies opnieuw wilt berekenen, kunt u dit in de volgende gebieden doen:

* In een lijst met objecten klikt u in het menu Meer boven aan de lijst.
* Als u in het vak Bewerken meerdere objecten bulksgewijs selecteert en bewerkt.

U kunt als volgt de aangepaste velden van verschillende objecten handmatig opnieuw berekenen door deze los van een lijst of rapport te bewerken:

1. Ga naar een lijst met de volgende objecttypen waarvan de objecten aangepaste formulieren met berekende velden bevatten:

   * Gebruikers
   * Bedrijven
   * Factureringsgegevens

1. Selecteer de objecten waarvan u de berekende aangepaste velden wilt bijwerken.
1. Klik het **uitgeven pictogram**.
1. Klik **Forms van de Douane** in het linkermenu, dan selecteren **de Uitdrukkingen van de Douane** opnieuw berekenen.
1. Klik **sparen** of **sparen Veranderingen**.

   Workfront berekent alle aangepaste velden voor alle geselecteerde objecten.

Aangepaste expressies opnieuw berekenen in een lijst met objecten:

1. Ga naar een projectlijst of een rapport en selecteer één of verscheidene van de volgende objecten types:

   * Projecten
   * Taken
   * Problemen
   * Portfolio&#39;s
   * Programma&#39;s
   * Uitgaven
1. Klik het **Meer** menu ![&#x200B; Meer menu &#x200B;](assets/more-icon.png), dan klik **opnieuw berekenen de Uitdrukkingen van de Douane**.

![&#x200B; herberekent uitdrukkingschronologie financiert drop-down in projectlijsten &#x200B;](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

Workfront berekent direct alle aangepaste velden voor alle geselecteerde projecten.
Niet alle lijsten met alle objecten hebben deze mogelijkheid.

>[!NOTE]
>
>Bij het opnieuw berekenen van expressies voor meerdere projecten, afhankelijk van de complexiteit ervan, raden we aan om een te groot aantal projecten niet te selecteren voor optimale prestaties.
>
>Sommige dingen die een project te complex zouden kunnen maken zouden veelvoudige gebiedsdelen of taken of een groot aantal douanevelden kunnen zijn.

