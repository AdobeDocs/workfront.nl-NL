---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Bedrijven maken en bewerken
description: U kunt bedrijven toevoegen aan [!DNL Workfront] en gebruiken voor financiële planning, rapporteringsdoeleinden, om toestemmingen rond voorwerpen te bepalen, en informatie vertrouwelijk te houden.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '1331'
ht-degree: 0%

---

# Bedrijven maken en bewerken

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Een onderneming is een organisatorische eenheid in [!DNL Adobe Workfront] die uw organisatie, een afdeling binnen de organisatie, of een cliënt kunnen vertegenwoordigen u met werkt. U kunt bedrijven toevoegen aan [!DNL Workfront] en gebruiken voor financiële planning, rapporteringsdoeleinden, om toestemmingen rond voorwerpen te bepalen, en informatie vertrouwelijk te houden.

## Toegangsvereisten

U moet over het volgende beschikken om bedrijven te kunnen beheren in [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan*</p> </td> 
   <td>[!UICONTROL Team] of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licentie*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Een van de volgende opties:</p> 
    <ul> 
     <li> <p>De [!UICONTROL System Administrator] toegangsniveau, dat u toestaat om het even welk bedrijf in het systeem uit te geven. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>. </p> </li> 
     <li> <p>Administratieve toegang om bedrijven te beheren, die u toestaat om het even welk bedrijf in het systeem uit te geven. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> </li> 
    </ul> <p><b>OPMERKING</b>:  
     <ul> 
      <li> <p>U kunt ook bedrijven beheren die zijn gekoppeld aan een groep waaraan u als groepsbeheerder bent toegewezen.</p> </li> 
      <li> <p>Om gebruikers toe te voegen aan en te verwijderen uit de [!DNL Workfront] -systeem hebt u een van de volgende mogelijkheden:</p> 
       <ul> 
        <li> <p>De [!UICONTROL System Administrator] toegangsniveau. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>. </p> </li> 
        <li> <p>In uw toegangsniveau, [!UICONTROL Edit] moet worden geselecteerd voor de [!UICONTROL Users] instellen. Ook voor de [!UICONTROL Users] instellen, onder [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> de [!UICONTROL Create] en ten minste één van beide [!UICONTROL User Admin] moeten opties zijn ingeschakeld. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Als u het [!UICONTROL User Admin (Group Users)] moet u een groepsbeheerder zijn van een groep waarvan de gebruiker lid is.</p> </li> 
       </ul> <p>Voor informatie over de Gebruikers die in een toegangsniveau plaatsen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Voordelen van het toevoegen van gebruikers aan een bedrijf {#benefits-of-adding-users-to-a-company}

* U kunt de organisatieschema van een bedrijf bouwen door gebruikers aan directe rapporten te associëren. Alleen gebruikers van hetzelfde bedrijf kunnen worden toegevoegd als directe rapporten van een andere gebruiker van dat bedrijf.
* Als projectmanager, kunt u beschikbare middelen binnen het zelfde bedrijf identificeren.
* U kunt informatie privé tussen bedrijven houden door één of alle volgende montages te kiezen:

   * Gebruikers van hetzelfde bedrijf kunnen elkaars verzoeken zien.

     Voor meer informatie over hoe een [!DNL Workfront] de beheerder kan gelijkaardige toegang tot verzoeken verlenen die op het bedrijf van gebruikers worden gebaseerd, zie de sectie [Configureer taak- en probleemvoorkeuren voor iedereen in de [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) in het artikel [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

     Voor meer informatie over hoe een groepsbeheerder gelijkaardige toegang tot verzoeken kan verlenen die op het bedrijf van gebruikers worden gebaseerd, zie [Taak- en uitgavevoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * De gebruikers kunnen slechts verzoekrijen zien die met hun bedrijven worden geassocieerd. Voor meer informatie over het beperken van zicht van een verzoekrij, zie [Toegang tot aanvraagwachtrijen bieden](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * U kunt gebruikers beperken tot slechts gebruikers in hun bedrijf of hun bedrijf en het primaire bedrijf zien. Voor informatie over de primaire bedrijffunctionaliteit betreffende gebruikersprivacy, zie [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * Gebruikers kunnen de updates die zij op items maken, beperken tot het zichtbaar zijn voor alleen hun bedrijfsgebruikers. Voor meer informatie over het privé maken van een update aan een bedrijf, zie [Werk bijwerken](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Een bedrijf maken of bewerken in [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

Er is geen limiet aan het aantal bedrijven dat u kunt toevoegen. Nochtans, adviseren wij dat het aantal bedrijven beperkt u wegens problemen gebruikt die met voorwerp kunnen voorkomen toestemmings-teveel de fragmentatie zich in de zichtbaarheid van gebruikers aan het werk punten zou kunnen mengen.

Het bedrijf dat standaard is gekoppeld aan uw instantie van [!DNL Workfront] is al gemaakt in uw [!DNL Workfront] en is het Primaire Bedrijf voor uw organisatie. Deze heeft dezelfde naam als de naam van uw klant. Voor meer informatie over uw klanten in [!DNL Workfront], zie [Basisinformatie voor uw systeem configureren](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

Een bedrijf toevoegen of bewerken:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik op **[!UICONTROL Companies]**.
1. Als u een bedrijf toevoegt, klikt u op **[!UICONTROL New Company]**.

   of

   Als u een bestaand bedrijf bewerkt, selecteert u het bedrijf en klikt u op **[!UICONTROL Edit]**.

1. Gebruik de opties die worden weergegeven om de volgende informatie te configureren:

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
        <li> <p><b>[!UICONTROL This is the Primary Company]</b>: Wijst het bedrijf toe als primair bedrijf van uw organisatie. Het primaire bedrijf vertegenwoordigt doorgaans uw [!DNL Workfront] -account waar de meeste gebruikers werken.</p> <p>U kunt één bedrijf of geen bedrijf hebben dat als primair bedrijf wordt aangewezen, maar u kunt geen veelvoudige bedrijven hebben die als primaire bedrijven worden aangewezen. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> <p><b>OPMERKING</b>: Door hun toegangsniveaus te wijzigen, kunt u gebruikers beperken om andere gebruikers te zien: slechts in hun primair bedrijf, of in hun verbonden bedrijf en het primaire bedrijf. Voor informatie over hoe het primaire bedrijf met de toegangsniveaus van gebruikers werkt, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: Als er een groep is die zaken met het bedrijf leidt, kunt u de naam van de groep hier toevoegen. Dit is nuttig voor groepsbeheerders die over alle bedrijven moeten rapporteren en beheren die hun groepen zaken doen met.</p> <p><b>BELANGRIJK</b>: Als u niet de groep associeert die met dit bedrijf zal werken, kunnen de beheerders voor de groep tot geen toegang hebben tenzij zij administratieve toegang tot bedrijven in hun toegangsniveau hebben. Voor informatie over hoe deze toegang wordt verleend, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Begin de naam van de groep te typen en druk vervolgens op <strong>[!UICONTROL Enter]</strong> wanneer deze wordt weergegeven.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Wanneer u een groep aan een bedrijf toewijst, de groepsbeheerders voor de groepsaanwinst [!UICONTROL Manage] toegang tot het bedrijf. Zie voor meer informatie <a href="#group-administrators-and-companies" class="MCXref xref">Groepsbeheerders en bedrijven</a> in dit artikel.</p> </li> 
        <li> <p><b>[!UICONTROL Company Members]</b>: Voeg bestaande gebruikers toe aan het bedrijf. Door dit te doen, associeert u deze gebruikers met dit bedrijf.</p> <p>Er is geen beperking aan hoeveel gebruikers u met één bedrijf associeert, maar een gebruiker kan niet met meer dan één bedrijf worden geassocieerd.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Forms] sectie</td> 
      <td> <p>Als er gebieden zijn die u aan uw bedrijf wilt toevoegen die niet beschikbaar in zijn [!DNL Workfront]kunt u een aangepast formulier maken en dit koppelen aan uw bedrijf. U kunt dit formulier aan uw bedrijf koppelen door het in de keuzelijst te selecteren. Alleen actieve bedrijven worden vermeld in de keuzelijst. Voor informatie over het maken van aangepaste Forms raadpleegt u <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Een aangepast formulier maken of bewerken</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Als u een nieuw bedrijf maakt, klikt u op **[!UICONTROL Create Company]**.

   of

   Als u een bestaand bedrijf bewerkt, klikt u op **[!UICONTROL Save Changes]**.

## Ondernemingslidmaatschappen beheren

Voor informatie over het beheren van lidmaatschappen voor een bestaand bedrijf, zie [Ondernemingslidmaatschappen beheren](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Factureringssnelheden beheren

Voor informatie over het overschrijden van factureringstarieven op bedrijfsniveau raadpleegt u [Factureringstarieven voor de rol van de werknemer op bedrijfsniveau overschrijven](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## Informatie over het delen van objecten met bedrijven

Er zijn bepaalde machtigingen beschikbaar voor gebruikers die zijn gekoppeld aan een bedrijf, zoals wordt uitgelegd in de sectie [Voordelen van het toevoegen van gebruikers aan een bedrijf](#benefits-of-adding-users-to-a-company). Naast deze machtigingen kunt u gebruikersmachtigingen toestaan om objecten te bekijken, bij te dragen of te bewerken in [!DNL Workfront] door het object met hun bedrijf te delen.

In plaats van een object met één individuele gebruiker tegelijk te delen, kunt u het met het hele bedrijf delen. Elke gebruiker in het bedrijf heeft de zelfde toestemmingen op dat voorwerp.

Zie voor meer informatie over het delen van objecten [Overzicht van het delen van machtigingen voor objecten](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Groepsbeheerders en bedrijven {#group-administrators-and-companies}

Wanneer een [!DNL Workfront] de beheerder wijst een groep aan een bedrijf toe, de groepsbeheerders voor de groepsaanwinst [!UICONTROL Manage] toegang tot het bedrijf in [!UICONTROL Setup]. Hieronder valt ook de toegang tot [!UICONTROL Companies] pagina in [!UICONTROL Setup], waar zij de met hun groep verbonden onderneming kunnen zien en beheren.

Met deze toegang [!UICONTROL Companies] pagina, kan een groepsbeheerder een groep aan een bedrijf toewijzen, maar het moet een bedrijf zijn dat de groepsbeheerder creeerde. Als het de toegangsniveau van de groepsbeheerder niet met administratieve toegang tot bedrijven wordt gevormd, [!UICONTROL Group] Het gebied wordt vereist wanneer de groepsbeheerder tot bedrijf-het is bolded titel wijst op dit:

![](assets/manage-company-group-field-req.jpg)

Voor informatie over hoe de gebruikers administratieve toegang tot bedrijven in hun toegangsniveau verkrijgen, zie [Gebruikers administratieve toegang verlenen tot bepaalde gebieden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Voor informatie over het beheer van een bedrijf in de [!UICONTROL Setup] gebied, zie [Een bedrijf maken of bewerken in [!DNL Workfront]](#create-or-edit-a-company-in-workfront) in dit artikel.
