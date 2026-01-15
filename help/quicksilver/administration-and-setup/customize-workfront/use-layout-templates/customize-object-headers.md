---
title: Objectkoppen aanpassen met een lay-outsjabloon
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Adobe Workfront-beheerder of groepsbeheerder kunt u een lay-outsjabloon gebruiken om de velden te configureren die gebruikers in de objectkoptekst zien wanneer ze de pagina van een object openen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: c037b4f9e5530d8dd796bed25021f7073f16061f
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Objectkoppen aanpassen met een lay-outsjabloon

Als Adobe Workfront-beheerder of groepsbeheerder kunt u een lay-outsjabloon gebruiken om de velden te configureren die gebruikers in de objectkoptekst zien wanneer ze de pagina van een object openen.

>[!IMPORTANT]
>
>Het aanpassen van objecten kopballen is momenteel beschikbaar voor projecten, taken, en kwesties.

![&#x200B; de kopbalgebieden van Objecten &#x200B;](assets/object-header-fields.png)

Voor informatie over het creëren van lay-outmalplaatjes, zie [&#x200B; lay-outmalplaatjes &#x200B;](../use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.

Voor informatie over lay-outmalplaatjes voor groepen, zie [&#x200B; tot stand brengen en wijzigen de lay-outmalplaatjes van een groep &#x200B;](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nadat u een lay-outmalplaatje hebt gevormd, moet u het aan gebruikers voor veranderingen toewijzen u aanbracht om aan anderen zichtbaar te zijn. Voor informatie over het toewijzen van een lay-outmalplaatje aan gebruikers, zie [&#x200B; gebruikers aan een lay-outmalplaatje &#x200B;](../use-layout-templates/assign-users-to-layout-template.md) toewijzen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>Om deze stappen op systeemniveau uit te voeren, hebt u het toegangsniveau van de Beheerder van het Systeem nodig.</p>
        <p>Om hen voor een groep uit te voeren, moet u een manager van die groep zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Objectkoppen aanpassen

1. Begin werkend aan een lay-outmalplaatje, zoals die in [&#x200B; wordt beschreven creeer en beheer lay-outmalplaatjes &#x200B;](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. In **pas aan welke gebruikers** drop-down menu zien, selecteren **Projecten**, **Taken**, of **Kwesties**.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. Houd de muisaanwijzer boven de huidige velden in de sectie [!UICONTROL Header fields] en voer een van de volgende handelingen uit:
   * Klik het **x** pictogram om een gebied te verwijderen

     of

   * Klik en houd het **greep** pictogram om het gebied in een nieuwe plaats te slepen en te laten vallen.

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![&#x200B; de kopbalgebieden van Objecten verbergen en bewegen pictogrammen &#x200B;](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. U kunt maximaal vijf velden in de koptekst van een object opnemen.
Als u al vijf velden hebt geselecteerd, moet u een veld verwijderen voordat u een nieuw veld kunt toevoegen.
1. Op **voeg gebied** doos toe, begin de naam van een douanegebied of een inheems gebied van Workfront te typen dat u wilt toevoegen, dan het selecteren wanneer het in de lijst toont. Het veld wordt direct rechts van het veld Toevoegen toegevoegd en wordt weergegeven als het eerste veld in de rechterbovenhoek van de koptekst van het object.

   >[!TIP]
   >
   >* U kunt elk aangepast veld of elk native veld toevoegen dat beschikbaar is in het gedeelte Overzicht van de sectie Details van een object. Alleen problemen hebben bijvoorbeeld het veld Ernst en dat veld is niet beschikbaar om aan projecten of taken toe te voegen.
   >
   >* Wanneer een gebruiker een aangepast veld in de koptekst bewerkt en het bevat in een aangepast formulier dat niet aan het object is gekoppeld, wordt het aangepaste formulier automatisch aan het object toegevoegd.
   >
   >* Wanneer u het veld &quot;Opgelost door&quot; toevoegt aan de koptekst van een probleem, verandert het veld in &quot;Probleem oplossen, Taak of Project&quot; wanneer er een object is dat is gekoppeld aan het probleem.

   ![&#x200B; voeg gebied aan kopbal toe &#x200B;](assets/add-field-to-header-in-lt-list.png)

1. (Optioneel) Sleep de velden in een andere volgorde.

1. Blijf het lay-outmalplaatje aanpassen. U kunt **klikken** op elk ogenblik van toepassing zijn om uw vooruitgang te bewaren.

   of

   Als u wordt gebeëindigd aanpassend, klik **sparen en sluit**.

