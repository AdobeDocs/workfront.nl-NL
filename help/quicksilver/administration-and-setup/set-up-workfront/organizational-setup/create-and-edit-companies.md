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
source-git-commit: 30b61b32add4c6d062b5b524773d309008c9563d
workflow-type: tm+mt
source-wordcount: '1356'
ht-degree: 0%

---

# Bedrijven maken en bewerken

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

Een bedrijf is een organisatorische eenheid in [!DNL Adobe Workfront] die uw organisatie, een afdeling binnen de organisatie, of een cliënt kan vertegenwoordigen u met werkt. U kunt bedrijven toevoegen aan [!DNL Workfront] en deze gebruiken voor financiële planning, rapporteringsdoeleinden, om machtigingen rond objecten te definiëren en om informatie vertrouwelijk te houden.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] package</p> </td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licentie</p> </td> 
   <td><p>[!UICONTROL Plan]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configuratie op toegangsniveau</td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau van [!UICONTROL System Administrator], dat u toestaat om het even welk bedrijf in het systeem uit te geven.</p> </li> 
     <li> <p>Administratieve toegang om bedrijven te beheren, die u toestaat om het even welk bedrijf in het systeem uit te geven.</p> </li> 
    </ul> <p><b> NOTA </b>:  
     <ul> 
      <li> <p>U kunt ook bedrijven beheren die zijn gekoppeld aan een groep waaraan u als groepsbeheerder bent toegewezen.</p> </li> 
      <li> <p>Als u gebruikers wilt toevoegen aan en verwijderen uit het [!DNL Workfront] -systeem, moet u over een van de volgende opties beschikken:</p> 
       <ul> 
        <li> <p>Het toegangsniveau van [!UICONTROL System Administrator]. </p> </li> 
        <li> <p><b>[!UICONTROL Users]</b> het instellen in uw toegangsniveau dat is geconfigureerd voor <b>[!UICONTROL Edit]</b> toegang, waarbij <b>[!UICONTROL Create]</b> en ten minste een van de twee <b>[!UICONTROL User Admin]</b> -opties is ingeschakeld onder <b>[!UICONTROL Fine-tune your settings]</b> <img src="assets/gear-icon-in-access-levels.png"> . </p> <p> <img src="assets/access-req-users.png"> </p> <p>Als <b>[!UICONTROL User Admin (Group Users)]</b> is ingeschakeld, moet u een groepbeheerder zijn van een groep waarvan de gebruiker lid is.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voordelen van het toevoegen van gebruikers aan een bedrijf {#benefits-of-adding-users-to-a-company}

* U kunt de organisatieschema van een bedrijf bouwen door gebruikers aan directe rapporten te associëren. Alleen gebruikers van hetzelfde bedrijf kunnen worden toegevoegd als directe rapporten van een andere gebruiker van dat bedrijf.
* Als projectmanager, kunt u beschikbare middelen binnen het zelfde bedrijf identificeren.
* U kunt informatie privé tussen bedrijven houden door één of alle volgende montages te kiezen:

   * Gebruikers van hetzelfde bedrijf kunnen elkaars verzoeken zien.

     Voor meer informatie over hoe een [!DNL Workfront] beheerder gelijkaardige toegang tot verzoeken kan geven die op het bedrijf van gebruikers worden gebaseerd, zie de sectie [&#x200B; taak en kwesties voorkeur voor iedereen binnen  [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) in het artikel [&#x200B; vormt systeembrede taak en geeft voorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) uit.

     Voor meer informatie over hoe een groepsbeheerder gelijkaardige toegang tot verzoeken kan geven die op het bedrijf van gebruikers worden gebaseerd, zie [&#x200B; taak vormen en voorkeur voor een groep &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) uitgeven.

   * De gebruikers kunnen slechts verzoekrijen zien die met hun bedrijven worden geassocieerd. Voor meer informatie over het beperken van zicht van een verzoekrij, zie [&#x200B; toegang verlenen tot verzoekrijen &#x200B;](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * U kunt gebruikers beperken tot slechts gebruikers in hun bedrijf of hun bedrijf en het primaire bedrijf zien. Voor informatie over de primaire bedrijffunctionaliteit betreffende gebruikersprivacy, zie [&#x200B; tot douanetoegangsniveaus &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.
   * Gebruikers kunnen de updates die zij op items maken, beperken tot het zichtbaar zijn voor alleen hun bedrijfsgebruikers. Voor meer informatie over het maken van een update privé aan een bedrijf, zie [&#x200B; het werk van de Update &#x200B;](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Een bedrijf maken of bewerken in [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

Er is geen limiet aan het aantal bedrijven dat u kunt toevoegen. Nochtans, adviseren wij dat het aantal bedrijven beperkt u wegens problemen gebruikt die met voorwerp kunnen voorkomen toestemmings-teveel de fragmentatie zich in de zichtbaarheid van gebruikers aan het werk punten zou kunnen mengen.

Standaard wordt het bedrijf dat aan uw instantie van [!DNL Workfront] is gekoppeld, al in uw [!DNL Workfront] -systeem gemaakt en is dit het primaire bedrijf voor uw organisatie. Deze heeft dezelfde naam als de naam van uw klant. Voor meer informatie over uw klanteninformatie in [!DNL Workfront], zie [&#x200B; basisinformatie voor uw systeem &#x200B;](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md) vormen.

Een bedrijf toevoegen of bewerken:

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Companies]**.

   Er wordt een lijst met bedrijven weergegeven.

1. Als u een bedrijf toevoegt, klikt u op **[!UICONTROL New Company]** .

   of

   Als u een bestaand bedrijf uitgeeft, selecteer het bedrijf, dan klik het **[!UICONTROL Edit]** pictogram ![&#x200B; uitgeeft pictogram &#x200B;](assets/edit-icon.png) bij de bovenkant van de bedrijflijst.

1. Werk de volgende informatie in de **BasisInfo** sectie bij:

   * **Naam van het Bedrijf**<!--<span class="preview">or **Name**</span>-->: Type een naam voor het bedrijf.
   * **is Actief**: Wanneer deze optie wordt toegelaten, kunnen de gebruikers het bedrijf vinden en het aan projecten vastmaken die zij creëren en uitgeven. Een inactief bedrijf kan niet aan projecten worden vastgehouden. Deze optie is standaard ingeschakeld.
   * **dit is het Primaire Bedrijf**<!--<span class="preview">or **Is Primary**</span>-->: Wijst het bedrijf als primair bedrijf van uw organisatie toe. Het primaire bedrijf vertegenwoordigt doorgaans uw Workfront-account waar de meeste gebruikers werken.

     U kunt één bedrijf of geen bedrijf hebben dat als primair bedrijf wordt aangewezen, maar u kunt geen veelvoudige bedrijven hebben die als primaire bedrijven worden aangewezen. Voor meer informatie, zie [&#x200B; douanetoegangsniveaus &#x200B;](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) creëren en wijzigen.

     >[!NOTE]
     >
     >Door hun toegangsniveaus te wijzigen, kunt u gebruikers beperken om andere gebruikers te zien: slechts in hun primair bedrijf, of in hun verbonden bedrijf en het primaire bedrijf. Voor informatie over hoe het primaire bedrijf met de toegangsniveaus van gebruikers werkt, zie [&#x200B; douanetoegangsniveaus &#x200B;](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) creëren en wijzigen.

   * **Groep**: Als er een groep is die zaken met het bedrijf leidt, kunt u de naam van de groep hier toevoegen. Dit is nuttig voor groepsbeheerders die over alle bedrijven moeten rapporteren en beheren die hun groepen zaken doen met.

     Als u niet de groep associeert die met dit bedrijf zal werken, kunnen de beheerders voor de groep niet tot het bedrijf toegang hebben tenzij zij administratieve toegang tot bedrijven in hun toegangsniveau hebben. Voor informatie over hoe deze toegang wordt verleend, zie [&#x200B; gebruikers administratieve toegang van de Verlening tot bepaalde gebieden &#x200B;](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

     Typ de naam van de groep en selecteer deze wanneer deze wordt weergegeven.

     Wanneer u een groep aan een bedrijf toewijst, leiden de groepsbeheerders voor de groepsaanwinst toegang tot het bedrijf. Voor meer informatie, zie [&#x200B; de beheerders en de bedrijven van de Groep &#x200B;](#group-administrators-and-companies) in dit artikel.

   * **Leden van het Bedrijf**: Voeg bestaande gebruikers aan het bedrijf toe. Door dit te doen, associeert u deze gebruikers met dit bedrijf.

     Typ de naam van een gebruiker en selecteer deze wanneer deze wordt weergegeven.

     Er is geen beperking aan hoeveel gebruikers u met één bedrijf associeert, maar een gebruiker kan niet met meer dan één bedrijf worden geassocieerd.

1. Voeg of werk douaneformulieren in de **sectie van de Douane Forms** bij.

   Als er gebieden zijn die u aan uw bedrijf wilt toevoegen die niet in Workfront beschikbaar zijn, kunt u een douaneformulier bouwen en het associëren met uw bedrijf.

   U kunt dit formulier aan uw bedrijf koppelen door het in de keuzelijst te selecteren. Alleen actieve aangepaste formulieren worden in het menu weergegeven.

   >[!NOTE]
   >
   >Geavanceerde aangepaste formulierfuncties, zoals Externe opzoekvelden en eigen Workfront-velden, zijn alleen beschikbaar als u de bedrijfsrecord opent op de detailpagina en niet in het dialoogvenster Bedrijf bewerken. (Klik in de lijst met bedrijven op de bedrijfsnaam om de gegevens te openen.)

   Voor informatie over het creëren van douaneformulieren, zie [&#x200B; een douaneformulier &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

1. (Voorwaardelijk) Als u een bedrijf maakt, klikt u op **[!UICONTROL Create Company]**<!--<span class="preview">or **Save**</span>-->.

   of

   Als u een bestaand bedrijf bewerkt, klikt u op **[!UICONTROL Save Changes]**<!--<span class="preview">or **Save**</span>-->.

## Ondernemingslidmaatschappen beheren

Voor informatie over het beheren van lidmaatschappen voor een bestaand bedrijf, zie [&#x200B; bedrijflidmaatschappen beheren &#x200B;](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Factureringssnelheden beheren

Voor informatie over het met voeten treden van het factureringspercentages op het bedrijfsniveau, zie [&#x200B; het factureren van de baanrol van de Opheffing op het bedrijfsniveau &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## Overzicht van het delen van objecten met bedrijven

Bepaalde toestemmingen zijn beschikbaar aan gebruikers die met een bedrijf worden geassocieerd, zoals verklaard in de sectie [&#x200B; Voordelen om gebruikers aan een bedrijf &#x200B;](#benefits-of-adding-users-to-a-company) toe te voegen. Naast deze machtigingen kunt u gebruikersmachtigingen toestaan om objecten in [!DNL Workfront] weer te geven, bij te dragen of te bewerken door het object met hun bedrijf te delen.

In plaats van een object met één individuele gebruiker tegelijk te delen, kunt u het met het hele bedrijf delen. Elke gebruiker in het bedrijf heeft de zelfde toestemmingen op dat voorwerp.

Voor meer informatie over het delen van voorwerpen, zie [&#x200B; Overzicht van het delen van toestemmingen op voorwerpen &#x200B;](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Groepsbeheerders en bedrijven {#group-administrators-and-companies}

Wanneer een [!DNL Workfront] beheerder een groep toewijst aan een bedrijf, krijgen de groepsbeheerders voor de groep [!UICONTROL Manage] toegang tot het bedrijf in [!UICONTROL Setup] . Dit omvat toegang tot de [!UICONTROL Companies] pagina in [!UICONTROL Setup] , waar zij het bedrijf kunnen zien en leiden verbonden aan hun groep.

Met deze toegang tot de [!UICONTROL Companies] pagina, kan een groepsbeheerder een groep aan een bedrijf toewijzen, maar het moet een bedrijf zijn dat de groepsbeheerder creeerde. Als het de toegangsniveau van de groepsbeheerder niet met administratieve toegang tot bedrijven wordt gevormd, wordt het [!UICONTROL Group] gebied vereist wanneer de groepsbeheerder tot bedrijf-zijn bolded titel leidt wijst op dit:

![&#x200B; geef bedrijf &#x200B;](assets/group-admin-add-company.png) uit

Voor informatie over hoe de gebruikers administratieve toegang tot bedrijven in hun toegangsniveau verkrijgen, zie [&#x200B; gebruikers administratieve toegang van de Verlening tot bepaalde gebieden &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Voor informatie over het beheren van een bedrijf in het [!UICONTROL Setup] gebied, zie [&#x200B; creeer of geef een bedrijf in  [!DNL Workfront]](#create-or-edit-a-company-in-workfront) in dit artikel uit.

<!-- OLD HTML TABLE
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic Info] section</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Company Name]</b>: Type a name for the company.</p> </li> 
        <li> <p><b>[!UICONTROL Is Active]</b>: When this option is enabled, users can find the company and attach it to projects that they create and edit. An inactive company cannot be attached to projects. This option is enabled by default.</p> </li> 
        <li> <p><b>[!UICONTROL This is the Primary Company]</b>: Assigns the company as your organization's primary company. The primary company typically represents your [!DNL Workfront] account where most of your users work.</p> <p>You can have one company or no company designated as a primary company, but you cannot have multiple companies designated as primary companies. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <p><b>NOTE</b>: By modifying their access levels, you can restrict users to see other users: only in their primary company, or in their associated company and the primary company. For information about how the primary company works with users' access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: If there is a group that conducts business with the company, you can add the name of the group here. This is useful for group administrators who need to report on and manage all the companies that their groups do business with.</p> <p><b>IMPORTANT</b>: If you don't associate the group that will be working with this company, administrators for the group can't access the company unless they have administrative access to companies in their access level. For information about how this access is granted, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Start typing the name of the group, then press <strong>[!UICONTROL Enter]</strong> when it appears.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">When you assign a group to a company, the group administrators for the group gain [!UICONTROL Manage] access to the company. For more information, see <a href="#group-administrators-and-companies" class="MCXref xref">Group administrators and companies</a> in this article.</p> </li> 
        <li> <p><b>[!UICONTROL Company Members]</b>: Add existing users to the company. By doing this, you are associating these users with this company.</p> <p>There is no limit to how many users you associate with one company, but a user cannot be associated with more than one company.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Forms] section</td> 
      <td> <p>If there are fields that you want to add to your company that are not available in [!DNL Workfront], you can build a custom form and associate it with your company. </p> <p>You can attach this form to your company by selecting it from the drop-down menu. Only active custom forms are listed in the menu.</p> <p><strong>Note:</strong> Advanced custom form features such as External lookup fields and Workfront native fields are only available when you open the company record on the details page, not on the Edit Company dialog. (From the list of companies, click the company name to open the details.)</p> <p> For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>
   -->
