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
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '811'
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
   <td> <p>Plan </p> <p>U moet een groepsbeheerder van de groep of een beheerder van Workfront zijn. Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Groepbeheerders</a> en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de Workfront-beheerder als u wilt weten welk abonnement- of licentietype u hebt.

## Bekijk, werk met, en creeer bedrijven voor uw groep van het gebied van Groepen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Groepen** ![](assets/groups-icon.png).

1. Klik op de naam van de groep waarvoor u bedrijven wilt maken of wijzigen.
1. Klik in het linkerdeelvenster op **Bedrijven** een lijst op te stellen van de met de groep verbonden ondernemingen en eventuele subgroepen.
1. (Optioneel) Als u een bedrijf wilt toevoegen, klikt u op **Bedrijf toevoegen** en configureer het bedrijf vervolgens met de onderstaande opties. Als u klaar bent, klikt u op **Bedrijf maken**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sectie Basisinformatie</td> 
      <td> 
       <ul> 
        <li> <p><b>Bedrijfsnaam</b>: Typ een naam voor het bedrijf.</p> </li> 
        <li> <p><b>Is actief</b>: Wanneer deze optie wordt toegelaten, kunnen de gebruikers het bedrijf vinden en het aan projecten vastmaken die zij creëren en uitgeven. Een inactief bedrijf kan niet aan projecten worden vastgehouden. Deze optie is standaard ingeschakeld.</p> </li> 
        <li> <p><b>Dit is het primaire bedrijf</b>: Wijst het bedrijf als primair bedrijf van uw organisatie toe. Het primaire bedrijf vertegenwoordigt doorgaans uw Workfront-account waar de meeste gebruikers werken.</p> <p>Door hun toegangsniveaus te wijzigen, kunt u gebruikers beperken om andere gebruikers te zien:</p> 
         <ul> 
          <li>Alleen in hun primaire onderneming</li> 
          <li> <p>In hun gelieerde onderneming en de primaire onderneming</p> <p>Voor informatie over de primaire bedrijffunctionaliteit binnen de toegangsniveaus van gebruikers, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> <p>U kunt slechts één of geen bedrijf hebben dat als primair bedrijf wordt aangewezen, maar u kunt geen veelvoudige bedrijven hebben die als primaire bedrijven worden aangewezen. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Groep</b>: Als er een groep is die zaken met het bedrijf leidt, kunt u de naam van de groep hier toevoegen. Dit is nuttig voor groepsbeheerders die over alle bedrijven moeten rapporteren en beheren die hun groepen zaken doen met.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Het systeem vult de <strong>Groep</strong> veld voor het nieuwe bedrijf met de groep die u bekijkt.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Als u administratieve toegang tot bedrijven in uw toegangsniveau hebt, kunt u de groep uit het bedrijf verwijderen en een verschillende toewijzen, of het bedrijf zonder een groep verlaten.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Als u geen administratieve toegang tot bedrijven hebt, <strong>Groep</strong> is vereist en u kunt alleen de groepen selecteren die u beheert of subgroepen onder deze groepen.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Voor informatie over administratieve toegang tot bedrijven, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> </li> 
        <li> <p><b>Bedrijfsleden</b>: Voeg bestaande gebruikers toe aan het bedrijf. Door dit te doen, associeert u deze gebruikers met dit bedrijf.</p> <p>Er is geen beperking aan hoeveel gebruikers u met één bedrijf associeert, maar een gebruiker kan niet met meer dan één bedrijf worden geassocieerd.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sectie Factureringstarieven</td> 
      <td> <p>U kunt factureringstarieven met voeten treden verbonden aan uw baanrollen op het bedrijfsniveau. Voor informatie over het creëren van baanrollen en het associëren van hen met het factureren tarieven, zie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" data-mc-variable-override="">Taakrollen maken en beheren</a>.</p> <p>Voor meer informatie over het overschrijven van het factureringstarief op het bedrijfsniveau, zie <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md" class="MCXref xref" data-mc-variable-override="">Factureringstarieven voor de rol van de werknemer op bedrijfsniveau overschrijven</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aangepaste Forms-sectie</td> 
      <td> <p>Als er gebieden zijn die u aan uw bedrijf wilt toevoegen die niet in Workfront beschikbaar zijn, kunt u een Vorm van de Douane bouwen en het associëren met uw bedrijf. U kunt dit formulier aan uw bedrijf koppelen door het in de keuzelijst te selecteren. Alleen actieve bedrijven worden vermeld in het keuzemenu. Ga voor informatie over het maken van aangepaste Forms naar <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">Een aangepast formulier maken of bewerken</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Als u administratieve toegang tot bedrijven in uw toegangsniveau hebt, kunt u ook klikken toevoegt Meer Bedrijven bij de bodem van de lijst. Dit voegt een rij toe waar u het nieuwe bedrijf kunt snel vormen.

1. (Optioneel) Als u bedrijven wilt bewerken of verwijderen, selecteert u ten minste één bedrijf en bewerkt u de werkbalkknoppen ![](assets/edit-icon.png) of verwijderen ![](assets/delete.png) het.

   Zie de sectie voor informatie over het bewerken van een bedrijf [Een bedrijf maken of bewerken in Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) in het artikel [Bedrijven maken en bewerken](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Optioneel) Als u de lijst met bedrijven wilt exporteren, klikt u op het pictogram Exporteren ![](assets/export.png)Selecteer vervolgens de bestandsindeling die u voor de geëxporteerde lijst wilt gebruiken.
