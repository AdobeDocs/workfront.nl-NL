---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Bedrijven van een groep maken en wijzigen
description: Wanneer u een groep bekijkt die u in het gebied van Groepen beheert, kunt u met bedrijven bekijken en werken verbonden aan de groep en om het even welk van zijn subgroups.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Bedrijven van een groep maken en wijzigen

Wanneer u een groep bekijkt die u in het gebied van Groepen beheert, kunt u met bedrijven bekijken en werken verbonden aan de groep en om het even welk van zijn subgroups.

Als er om het even welke groepen boven uw groep zijn, kunnen hun beheerders deze dingen voor uw groep ook doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-abonnement*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> <p>U moet een groepsbeheerder van de groep of een beheerder van Workfront zijn. Voor meer informatie, zie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override=""> de beheerders van de Groep </a> en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override=""> verlenen een gebruiker volledige administratieve toegang </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; als u moet weten welk plan of licentietype u hebt, contacteer uw beheerder van Workfront.

## Bedrijven voor uw groep weergeven, bewerken en maken vanuit het gebied Groepen

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Opstelling** ![](assets/gear-icon-settings.png).

1. In het linkerpaneel, klik **Groepen** ![](assets/groups-icon.png).

1. Klik op de naam van de groep waarvoor u bedrijven wilt maken of wijzigen.
1. In het linkerpaneel, klik **Bedrijven** om van de bedrijven een lijst te maken verbonden aan de groep en om het even welke subgroups het kan hebben.
1. (Facultatief) om een bedrijf toe te voegen, **voeg Bedrijf** toe, dan vorm het bedrijf gebruikend de hieronder vermelde opties. Wanneer u wordt gebeëindigd, klik **tot Bedrijf** leidt.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sectie Basisinformatie</td> 
      <td> 
       <ul> 
        <li> <p><b> Naam van het Bedrijf </b>: Type een naam voor het bedrijf.</p> </li> 
        <li> <p><b> is Actief </b>: Wanneer deze optie wordt toegelaten, kunnen de gebruikers het bedrijf vinden en het aan projecten vastmaken die zij creëren en uitgeven. Een inactief bedrijf kan niet aan projecten worden vastgehouden. Deze optie is standaard ingeschakeld.</p> </li> 
        <li> <p><b> dit is het Primaire Bedrijf </b>: Wijst het bedrijf als primair bedrijf van uw organisatie toe. Het primaire bedrijf vertegenwoordigt doorgaans uw Workfront-account waar de meeste gebruikers werken.</p> <p>Door hun toegangsniveaus te wijzigen, kunt u gebruikers beperken om andere gebruikers te zien:</p> 
         <ul> 
          <li>Alleen in hun primaire onderneming</li> 
          <li> <p>In hun gelieerde onderneming en de primaire onderneming</p> <p>Voor informatie over de primaire bedrijffunctionaliteit binnen de toegangsniveaus van gebruikers, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override=""> douanetoegangsniveaus </a> creëren of wijzigen.</p> <p>U kunt slechts één of geen bedrijf hebben dat als primair bedrijf wordt aangewezen, maar u kunt geen veelvoudige bedrijven hebben die als primaire bedrijven worden aangewezen. Voor meer informatie, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override=""> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </li> 
         </ul> </li> 
        <li> <p><b> Groep </b>: Als er een groep is die zaken met het bedrijf leidt, kunt u de naam van de groep hier toevoegen. Dit is nuttig voor groepsbeheerders die over alle bedrijven moeten rapporteren en beheren die hun groepen zaken doen met.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Het systeem vult in het </strong> gebied van de Groep <strong> {voor het nieuwe bedrijf met de groep u bekijkt.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Als u administratieve toegang tot bedrijven in uw toegangsniveau hebt, kunt u de groep uit het bedrijf verwijderen en een verschillende toewijzen, of het bedrijf zonder een groep verlaten.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Als u geen administratieve toegang tot bedrijven hebt, wordt het <strong> gebied van de Groep </strong> vereist en u kunt slechts de groepen selecteren u of om het even welke subgroepen onder die groepen beheert.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Voor informatie over administratieve toegang tot bedrijven, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override=""> gebruikers administratieve toegang van de Verlening tot bepaalde gebieden </a>.</p> </li> 
        <li> <p><b> Leden van het Bedrijf </b>: Voeg bestaande gebruikers aan het bedrijf toe. Door dit te doen, associeert u deze gebruikers met dit bedrijf.</p> <p>Er is geen beperking aan hoeveel gebruikers u met één bedrijf associeert, maar een gebruiker kan niet met meer dan één bedrijf worden geassocieerd.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Aangepaste Forms-sectie</td> 
      <td> <p>Als er gebieden zijn die u aan uw bedrijf wilt toevoegen die niet in Workfront beschikbaar zijn, kunt u een douaneformulier bouwen en het associëren met uw bedrijf. U kunt dit formulier aan uw bedrijf koppelen door het in de keuzelijst te selecteren. Alleen actieve bedrijven worden vermeld in de keuzelijst. Voor informatie over het creëren van douaneformulieren, zie <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md"> Ontwerp een vorm met de vormontwerper </a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Als u administratieve toegang tot bedrijven in uw toegangsniveau hebt, kunt u ook klikken toevoegt Meer Bedrijven bij de bodem van de lijst. Dit voegt een rij toe waar u het nieuwe bedrijf kunt snel vormen.

1. (Optioneel) Als u bedrijven wilt bewerken of verwijderen, selecteert u ten minste één bedrijf en gebruikt u de werkbalkknoppen om ![](assets/edit-icon.png) het bedrijf te bewerken of te verwijderen. ![](assets/delete.png)

   Voor informatie over het uitgeven van een bedrijf, zie de sectie [ een bedrijf in Workfront ](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) in het artikel [ creëren en uitgeven bedrijven ](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Optioneel) Als u de lijst met bedrijven wilt exporteren, klikt u op het pictogram Exporteren ![](assets/export.png) en selecteert u de gewenste bestandsindeling voor de geëxporteerde lijst.
