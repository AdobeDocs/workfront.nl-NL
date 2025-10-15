---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: De bedrijven van een groep maken en wijzigen
description: Wanneer u een groep bekijkt die u in het gebied van Groepen beheert, kunt u met bedrijven bekijken en werken verbonden aan de groep en om het even welk van zijn subgroups.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: 1554c067afcc548c7f7abd03dbc3a49404e3c89c
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Bedrijven van een groep maken en wijzigen

Wanneer u een groep bekijkt die u in het gebied van Groepen beheert, kunt u met bedrijven bekijken en werken verbonden aan de groep en om het even welk van zijn subgroups.

Als er om het even welke groepen boven uw groep zijn, kunnen hun beheerders deze dingen voor uw groep ook doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

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
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>U moet een groepsbeheerder van de groep of een systeembeheerder zijn.</td>
  </tr>
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bedrijven voor uw groep weergeven, bewerken en maken vanuit het gebied Groepen

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen** ![&#x200B; Groepen &#x200B;](assets/groups-icon.png).

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
        <li> <p><b> Groep </b>: Als er een groep is die zaken met het bedrijf leidt, kunt u de naam van de groep hier toevoegen. Dit is nuttig voor groepsbeheerders die over alle bedrijven moeten rapporteren en beheren die hun groepen zaken doen met.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Het systeem vult in het <strong> gebied van de Groep </strong> &lbrace;voor het nieuwe bedrijf met de groep u bekijkt.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Als u administratieve toegang tot bedrijven in uw toegangsniveau hebt, kunt u de groep uit het bedrijf verwijderen en een verschillende toewijzen, of het bedrijf zonder een groep verlaten.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Als u geen administratieve toegang tot bedrijven hebt, wordt het <strong> gebied van de Groep </strong> vereist en u kunt slechts de groepen selecteren u of om het even welke subgroepen onder die groepen beheert.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Voor informatie over administratieve toegang tot bedrijven, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override=""> gebruikers administratieve toegang van de Verlening tot bepaalde gebieden </a>.</p> </li> 
        <li> <p><b> Leden van het Bedrijf </b>: Voeg bestaande gebruikers aan het bedrijf toe. Door dit te doen, associeert u deze gebruikers met dit bedrijf.</p> <p>Er is geen beperking aan hoeveel gebruikers u met één bedrijf associeert, maar een gebruiker kan niet met meer dan één bedrijf worden geassocieerd.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Aangepaste Forms-sectie</td> 
      <td> <p>Als er gebieden zijn die u aan uw bedrijf wilt toevoegen die niet in Workfront beschikbaar zijn, kunt u een douaneformulier bouwen en het associëren met uw bedrijf. U kunt dit formulier aan uw bedrijf koppelen door het in de keuzelijst te selecteren. Alleen actieve bedrijven worden vermeld in de keuzelijst. Voor informatie over het creëren van douaneformulieren, zie <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md"> een douaneformulier </a> creëren. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Als u administratieve toegang tot bedrijven in uw toegangsniveau hebt, kunt u ook klikken toevoegt Meer Bedrijven bij de bodem van de lijst. Dit voegt een rij toe waar u het nieuwe bedrijf kunt snel vormen.

1. (Facultatief) om bedrijven uit te geven of te schrappen, om minstens één bedrijf te selecteren, dan de toolbarknopen gebruiken om ![&#x200B; uit te geven pictogram &#x200B;](assets/edit-icon.png) uitgeven of ![&#x200B; schrap pictogram &#x200B;](assets/delete.png) het.

   Voor informatie over het uitgeven van een bedrijf, zie de sectie [&#x200B; een bedrijf in Workfront &#x200B;](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) in het artikel [&#x200B; creëren en uitgeven bedrijven &#x200B;](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Facultatief) om de lijst van bedrijven uit te voeren, klik het pictogram van de Uitvoer ![&#x200B; &#x200B;](assets/export.png), dan selecteer het dossierformaat u voor de uitgevoerde lijst wilt.
