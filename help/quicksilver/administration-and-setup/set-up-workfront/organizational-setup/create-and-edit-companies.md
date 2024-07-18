---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Bedrijven maken en bewerken
description: U kunt bedrijven aan  [!DNL Adobe Workfront]  toevoegen en hen gebruiken voor financiële planning, rapporteringsdoeleinden, om toestemmingen rond voorwerpen te bepalen, en informatie vertrouwelijk te houden.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1400'
ht-degree: 0%

---

# Bedrijven maken en bewerken

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Een bedrijf is een organisatorische eenheid in [!DNL Adobe Workfront] die uw organisatie, een afdeling binnen de organisatie, of een cliënt kan vertegenwoordigen u met werkt. U kunt bedrijven toevoegen aan [!DNL Workfront] en deze gebruiken voor financiële planning, rapporteringsdoeleinden, om machtigingen rond objecten te definiëren en om informatie vertrouwelijk te houden.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet over het volgende beschikken om bedrijven te kunnen beheren in [!DNL Workfront] :

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licentie*</p> </td> 
   <td><p>Huidige: [!UICONTROL Plan]</p>
   of
   <p>Nieuw: [!UICONTROL Standard]</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuratie op toegangsniveau</td> 
   <td> <p>Een van de volgende opties:</p> 
    <ul> 
     <li> <p>Het toegangsniveau van [!UICONTROL System Administrator], dat u toestaat om het even welk bedrijf in het systeem uit te geven. Voor meer informatie, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md"> een gebruiker volledige administratieve toegang verlenen </a>. </p> </li> 
     <li> <p>Administratieve toegang om bedrijven te beheren, die u toestaat om het even welk bedrijf in het systeem uit te geven. Voor meer informatie, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md"> gebruikers administratieve toegang van de Verlening tot bepaalde gebieden </a>.</p> </li> 
    </ul> <p><b> NOTA </b>:  
     <ul> 
      <li> <p>U kunt ook bedrijven beheren die zijn gekoppeld aan een groep waaraan u als groepsbeheerder bent toegewezen.</p> </li> 
      <li> <p>Als u gebruikers wilt toevoegen aan en verwijderen uit het [!DNL Workfront] -systeem, moet u een van de volgende opties hebben:</p> 
       <ul> 
        <li> <p>Het toegangsniveau van [!UICONTROL System Administrator]. Voor meer informatie, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> een gebruiker volledige administratieve toegang verlenen </a>. </p> </li> 
        <li> <p>In uw toegangsniveau, moet [!UICONTROL Edit] voor het [!UICONTROL Users] plaatsen worden geselecteerd. Voor de instelling [!UICONTROL Users] onder [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> moeten ook de optie [!UICONTROL Create] en ten minste een van de twee opties [!UICONTROL User Admin] zijn ingeschakeld. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Als u de optie [!UICONTROL User Admin (Group Users)] gebruikt, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> </li> 
       </ul> <p>Voor informatie over de Gebruikers die in een toegangsniveau plaatsen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> toegang van de Verlening tot gebruikers </a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, licentietype, of configuraties van het toegangsniveau u hebt, contacteer uw [!DNL Workfront] beheerder. Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voordelen van het toevoegen van gebruikers aan een bedrijf {#benefits-of-adding-users-to-a-company}

* U kunt de organisatieschema van een bedrijf bouwen door gebruikers aan directe rapporten te associëren. Alleen gebruikers van hetzelfde bedrijf kunnen worden toegevoegd als directe rapporten van een andere gebruiker van dat bedrijf.
* Als projectmanager, kunt u beschikbare middelen binnen het zelfde bedrijf identificeren.
* U kunt informatie privé tussen bedrijven houden door één of alle volgende montages te kiezen:

   * Gebruikers van hetzelfde bedrijf kunnen elkaars verzoeken zien.

     Voor meer informatie over hoe een [!DNL Workfront] beheerder gelijkaardige toegang tot verzoeken kan geven die op het bedrijf van gebruikers worden gebaseerd, zie de sectie [ taak en kwesties voorkeur voor iedereen binnen  [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) in het artikel [ vormt systeembrede taak en geeft voorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) uit.

     Voor meer informatie over hoe een groepsbeheerder gelijkaardige toegang tot verzoeken kan geven die op het bedrijf van gebruikers worden gebaseerd, zie [ taak vormen en voorkeur voor een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) uitgeven.

   * De gebruikers kunnen slechts verzoekrijen zien die met hun bedrijven worden geassocieerd. Voor meer informatie over het beperken van zicht van een verzoekrij, zie [ toegang verlenen tot verzoekrijen ](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * U kunt gebruikers beperken tot slechts gebruikers in hun bedrijf of hun bedrijf en het primaire bedrijf zien. Voor informatie over de primaire bedrijffunctionaliteit betreffende gebruikersprivacy, zie [ tot douanetoegangsniveaus ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.
   * Gebruikers kunnen de updates die zij op items maken, beperken tot het zichtbaar zijn voor alleen hun bedrijfsgebruikers. Voor meer informatie over het maken van een update privé aan een bedrijf, zie [ het werk van de Update ](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Een bedrijf maken of bewerken in [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

Er is geen limiet aan het aantal bedrijven dat u kunt toevoegen. Nochtans, adviseren wij dat het aantal bedrijven beperkt u wegens problemen gebruikt die met voorwerp kunnen voorkomen toestemmings-teveel de fragmentatie zich in de zichtbaarheid van gebruikers aan het werk punten zou kunnen mengen.

Standaard wordt het bedrijf dat aan uw instantie van [!DNL Workfront] is gekoppeld, al in uw [!DNL Workfront] -systeem gemaakt en is dit het primaire bedrijf voor uw organisatie. Deze heeft dezelfde naam als de naam van uw klant. Voor meer informatie over uw klanteninformatie in [!DNL Workfront], zie [ basisinformatie voor uw systeem ](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md) vormen.

Een bedrijf toevoegen of bewerken:

{#step-1-to-setup}

1. Klik op **[!UICONTROL Companies]**.

   Er wordt een lijst met bedrijven weergegeven.
1. Als u een bedrijf toevoegt, klikt u op **[!UICONTROL New Company]** .

   of

   Als u een bestaand bedrijf bewerkt, selecteert u het bedrijf en klikt u op **[!UICONTROL Edit]** boven aan de lijst met bedrijven.

1. Werk de volgende gegevens bij:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic Info] sectie</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Company Name]</b>: Typ een naam voor het bedrijf.</p> </li> 
        <li> <p><b>[!UICONTROL Is Active]</b>: Wanneer deze optie is ingeschakeld, kunnen gebruikers het bedrijf zoeken en het koppelen aan projecten die ze maken en bewerken. Een inactief bedrijf kan niet aan projecten worden vastgehouden. Deze optie is standaard ingeschakeld.</p> </li> 
        <li> <p><b>[!UICONTROL This is the Primary Company]</b>: Wijst het bedrijf toe als primair bedrijf van uw organisatie. Het primaire bedrijf vertegenwoordigt doorgaans uw [!DNL Workfront] -account waar de meeste gebruikers werken.</p> <p>U kunt één bedrijf of geen bedrijf hebben dat als primair bedrijf wordt aangewezen, maar u kunt geen veelvoudige bedrijven hebben die als primaire bedrijven worden aangewezen. Voor meer informatie, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> <p><b> NOTA </b>: Door hun toegangsniveaus te wijzigen, kunt u gebruikers beperken om andere gebruikers te zien: slechts in hun primair bedrijf, of in hun geassocieerd bedrijf en het primaire bedrijf. Voor informatie over hoe het primaire bedrijf met de toegangsniveaus van gebruikers werkt, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: Als er een groep is die zaken met het bedrijf leidt, kunt u de naam van de groep hier toevoegen. Dit is nuttig voor groepsbeheerders die over alle bedrijven moeten rapporteren en beheren die hun groepen zaken doen met.</p> <p><b> BELANGRIJK </b>: Als u niet de groep associeert die met dit bedrijf zal werken, kunnen de beheerders voor de groep niet tot het bedrijf toegang hebben tenzij zij administratieve toegang tot bedrijven in hun toegangsniveau hebben. Voor informatie over hoe deze toegang wordt verleend, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref"> gebruikers administratieve toegang van de Verlening tot bepaalde gebieden </a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Typ de naam van de groep en druk op <strong>[!UICONTROL Enter]</strong> wanneer deze wordt weergegeven.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Wanneer u een groep toewijst aan een bedrijf, krijgen de groepsbeheerders voor de groepswinst [!UICONTROL Manage] toegang tot het bedrijf. Voor meer informatie, zie <a href="#group-administrators-and-companies" class="MCXref xref"> de beheerders en de bedrijven van de Groep </a> in dit artikel.</p> </li> 
        <li> <p><b>[!UICONTROL Company Members]</b>: Voeg bestaande gebruikers toe aan het bedrijf. Door dit te doen, associeert u deze gebruikers met dit bedrijf.</p> <p>Er is geen beperking aan hoeveel gebruikers u met één bedrijf associeert, maar een gebruiker kan niet met meer dan één bedrijf worden geassocieerd.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Forms] sectie</td> 
      <td> <p>Als er gebieden zijn die u aan uw bedrijf wilt toevoegen die niet beschikbaar in [!DNL Workfront] zijn, kunt u een douaneformulier bouwen en het associëren met uw bedrijf. </p> <p>U kunt dit formulier aan uw bedrijf koppelen door het in de keuzelijst te selecteren. Alleen actieve aangepaste formulieren worden in het menu weergegeven.</p> <p><strong> Nota:</strong> de Geavanceerde eigenschappen van de douanevorm zoals Externe Velden van de Opzoekopdracht en inheemse gebieden van Workfront zijn slechts beschikbaar wanneer u het bedrijfverslag op de detailspagina, niet op de Edit dialoog van het Bedrijf opent. (Klik in de lijst met bedrijven op de bedrijfsnaam om de gegevens te openen.)</p> <p> Voor informatie over het creëren van douaneformulieren, zie <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref"> een douaneformulier </a> creëren of uitgeven. </p> </td>
     </tr> 
    </tbody> 
   </table>

1. (Voorwaardelijk) Als u een bedrijf maakt, klikt u op **[!UICONTROL Create Company]** .

   of

   Als u een bestaand bedrijf bewerkt, klikt u op **[!UICONTROL Save Changes]** .

## Ondernemingslidmaatschappen beheren

Voor informatie over het beheren van lidmaatschappen voor een bestaand bedrijf, zie [ bedrijflidmaatschappen beheren ](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Factureringssnelheden beheren

Voor informatie over het met voeten treden van het factureringspercentages op het bedrijfsniveau, zie [ het factureren van de baanrol van de Opheffing op het bedrijfsniveau ](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## Overzicht van het delen van objecten met bedrijven

Bepaalde toestemmingen zijn beschikbaar aan gebruikers die met een bedrijf worden geassocieerd, zoals verklaard in de sectie [ Voordelen om gebruikers aan een bedrijf ](#benefits-of-adding-users-to-a-company) toe te voegen. Naast deze machtigingen kunt u gebruikersmachtigingen toestaan om objecten in [!DNL Workfront] weer te geven, bij te dragen of te bewerken door het object met hun bedrijf te delen.

In plaats van een object met één individuele gebruiker tegelijk te delen, kunt u het met het hele bedrijf delen. Elke gebruiker in het bedrijf heeft de zelfde toestemmingen op dat voorwerp.

Voor meer informatie over het delen van voorwerpen, zie [ Overzicht van het delen van toestemmingen op voorwerpen ](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Groepsbeheerders en bedrijven {#group-administrators-and-companies}

Wanneer een [!DNL Workfront] beheerder een groep toewijst aan een bedrijf, krijgen de groepsbeheerders voor de groep [!UICONTROL Manage] toegang tot het bedrijf in [!UICONTROL Setup] . Dit omvat toegang tot de [!UICONTROL Companies] pagina in [!UICONTROL Setup] , waar zij het bedrijf kunnen zien en leiden verbonden aan hun groep.

Met deze toegang tot de [!UICONTROL Companies] pagina, kan een groepsbeheerder een groep aan een bedrijf toewijzen, maar het moet een bedrijf zijn dat de groepsbeheerder creeerde. Als het de toegangsniveau van de groepsbeheerder niet met administratieve toegang tot bedrijven wordt gevormd, wordt het [!UICONTROL Group] gebied vereist wanneer de groepsbeheerder tot bedrijf-zijn bolded titel leidt wijst op dit:

![ geef bedrijf ](assets/group-admin-add-company.png) uit

Voor informatie over hoe de gebruikers administratieve toegang tot bedrijven in hun toegangsniveau verkrijgen, zie [ gebruikers administratieve toegang van de Verlening tot bepaalde gebieden ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Voor informatie over het beheren van een bedrijf in het [!UICONTROL Setup] gebied, zie [ creeer of geef een bedrijf in  [!DNL Workfront]](#create-or-edit-a-company-in-workfront) in dit artikel uit.
