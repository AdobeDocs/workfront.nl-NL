---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Een sectie-einde toevoegen aan een aangepast formulier met de oudere formulierbuilder
description: U kunt aangepaste velden en widgets in een aangepast formulier groeperen in secties met koppen. Dit is handig als u gebruikers die het formulier invullen, een geordende ervaring wilt laten zien. Ook, als u toegang tot bepaalde douanegebieden en widgets aan bepaalde gebruikers moet beperken, kunt u hen in een sectie plaatsen en dan toegang tot de sectie verlenen aan slechts die gebruikers.
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 44a52767-60a7-4aaa-b3b8-6b8fb7da7e72
source-git-commit: 961e0451ce9011a8a9f511d7d5da99368d22d6fb
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 0%

---

# Een sectie-einde toevoegen aan een aangepast formulier met de oudere formulierbuilder

U kunt aangepaste velden en widgets in een aangepast formulier groeperen in secties met koppen. Dit is handig als u gebruikers die het formulier invullen, een geordende ervaring wilt laten zien. Ook, als u toegang tot bepaalde douanegebieden en widgets aan bepaalde gebruikers moet beperken, kunt u hen in een sectie plaatsen en dan toegang tot de sectie verlenen aan slechts die gebruikers.

Als u bijvoorbeeld gevoelige informatie wilt bijhouden die alleen systeembeheerders mogen weergeven of bewerken, kunt u een sectie-einde maken met de machtiging Alleen beheerder en de gevoelige velden in die sectie plaatsen.

De toegangsinstellingen die u voor een sectie selecteert, zijn rechtstreeks gekoppeld aan de machtigingen die gebruikers hebben voor het Workfront-object waaraan het aangepaste formulier is gekoppeld. U kunt een sectie verbergen of weergeven op basis van het feit of de gebruiker toegang heeft tot het object, een bijdrage levert aan dat object of dat object beheert. U kunt ook een sectie alleen instellen op Beheerder, zodat alleen gebruikers met een toegangsniveau van de systeembeheerder toegang hebben tot de sectie.

Zie voor informatie over machtigingen voor objecten [Overzicht van het delen van machtigingen voor objecten](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Zie voor informatie over aangepaste velden en widgets in aangepaste formulieren [Een aangepast veld toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) en [Een middelenwidget toevoegen of bewerken in een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

<!--
>[!TIP]
>
>Section breaks that you add to custom forms are saved in your system for re-use. For information about listing them, see [List and edit custom forms and widgets added to custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/list-edit-share-custom-forms-and-custom-fields.md).
-->

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-abonnement*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> <p>Ga voor informatie over hoe Workfront-beheerders deze toegang verlenen naar <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, type licentie of configuraties op toegangsniveau u hebt.

## Toegang voor een sectie in een aangepast formulier maken en configureren

1. Beginnen met het maken of bewerken van een aangepast formulier, zoals beschreven in [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Aangepaste velden en widgets aan het formulier toevoegen, zoals beschreven in [Een aangepast veld toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) en [Een middelenwidget toevoegen of bewerken in een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

1. Tijdens het maken of bewerken van het aangepaste formulier, kunt u op het tabblad **Veld toevoegen** tabblad, klikt u op **Sectie-einde**.

   ![](assets/click-section-break.jpg)

1. Op de **Veldinstellingen** kunt u de gewenste opties voor de sectie instellen:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Vereist) Typ een beschrijvend label dat boven de sectie wordt weergegeven. U kunt het label op elk gewenst moment wijzigen.</p> <p><b>BELANGRIJK</b>: Gebruik geen speciale tekens in dit label. Ze worden niet correct weergegeven in rapporten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td>Typ tekst als u aan gebruikers wilt uitleggen waarvoor de sectie is bedoeld. Dit wordt weergegeven onder het label van de sectie op het aangepaste formulier.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Logica toevoegen</td> 
      <td>Gebruik weergaverelogica om op te geven of de sectie op het formulier moet worden weergegeven, op basis van selecties die gebruikers in meerkeuzevelden maken wanneer ze het formulier invullen. Zie voor meer informatie <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Weergavelogica toevoegen en logica overslaan naar een aangepast formulier</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Toegang verlenen</p> </td> 
      <td> <p> Selecteer de machtigingen die gebruikers nodig hebben voor een object waaraan het aangepaste formulier is gekoppeld, om deze sectie weer te geven en de veldwaarden ervan te bewerken. 
       <p>De volgende machtigingen zijn beschikbaar onder <b>Gebruikers met deze toegang tot het object kunnen veldwaarden weergeven</b>:</p> 
         <ul>
          <li><strong>Weergave</strong>: Machtigingen voor het object weergeven</li>
          <li><p><b>Beperkte bewerking</b>: (Alleen beschikbaar als het object een project, taak, uitgave of gebruiker is):</p> 
          <p>Staat gebruikers toe om aan het voorwerp bij te dragen als het een project, een taak, of een kwestie is.</p>
          <p>Staat gebruikers toe om het profiel uit te geven of de profieltoestemming te bezitten aan het voorwerp als het een gebruiker is.</p></li> 
          <li><b>Bewerken</b>: Rechten voor het object beheren </li> 
          <li><b>Alleen beheerder</b>: Toegangsniveau voor systeembeheerder</li> 
         </ul> </li> 
        <p>De volgende machtigingen zijn beschikbaar onder <b>Gebruikers met deze toegang tot het object kunnen veldwaarden bewerken</b>: </p> 
         <ul> 
          <li> <p><b>Beperkte bewerking</b>: (Alleen beschikbaar als het object een project, taak, uitgave of gebruiker is):</p> 
           <p>Als het voorwerp een project, een taak, of een kwestie, deze toestemming gebruikers toestaat om aan het voorwerp bij te dragen</p>
          <p>Als het object een gebruiker is, kunnen gebruikers met deze machtiging het profiel bewerken of eigenaar zijn van de profielmachtiging voor het object.</p> 
          <li><b>Bewerken</b>: Rechten voor het object beheren </li> 
          <li><b>Alleen beheerder</b>: Toegangsniveau voor systeembeheerder</li> 
         </ul> </li> 
       </ul> 
       <p>Zie voor informatie over machtigingen voor objecten <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overzicht van het delen van machtigingen voor objecten</a>.</p> 
       <p><b>OPMERKING</b>:  
       <ul> 
       <li> <p>Gebruikers zonder de machtigingen die u hier opgeeft, kunnen de aangepaste velden en widgets niet zien in de sectie. </p> <p>Dit is ook het geval als u de waarden van de velden in rapporten weergeeft of deze in berekende velden gebruikt in tekstmodusrapportage.</p> </li> 
       <li> <p>Als u meerdere objecttypen aan uw formulier koppelt, kunt u de weergave- en bewerkingsmachtigingen wijzigen die in deze stappen beschikbaar zijn. Zie voor meer informatie <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Hoe meerdere objecttypen de machtigingen voor secties in een aangepast formulier kunnen beïnvloeden</a> in dit artikel.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Sleep of voeg minstens één aangepast veld of widget toe aan de nieuwe sectie.

   Dit is vereist voordat u de sectie opslaat.

1. Klikken **Gereed**.

   >[!TIP]
   >
   >U kunt op **Toepassen** op elk gewenst moment tijdens het maken van een aangepast formulier om uw wijzigingen op te slaan en het formulier open te houden.

1. Als u uw aangepaste formulier op andere manieren wilt blijven bouwen, gaat u verder naar een van de volgende artikelen:

   * [Een aangepast veld toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [Een middelenwidget toevoegen of bewerken in een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Berekende gegevens toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Aangepaste velden en widgets in een aangepast formulier plaatsen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Weergavelogica toevoegen en logica overslaan naar een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Een aangepast formulier voorvertonen en invullen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

<!--
DRAFTED IN FLARE:
<h2>Configure access for fields without section breaks</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">************This section might get added later. Team decided not to implement.</p>
<p>In a custom form, you can also control users' access to custom fields
and image widgets that are not placed inside a defined section.</p>
<ol>
<li value="1">Begin creating or editing a custom form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</li>
<li value="2">Add custom fields

and widgets

to the form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md" class="MCXref xref">Add a custom field to a custom form</a>.</li>
<li value="3"> <p>While still creating or editing the custom form, open the <b>Form settings</b> tab.</p> <p>SHOW THIS </p> </li>
<li value="4"> <p>Under <b>Grant access</b>, configure the permissions that users need on an object where the custom form is attached, in order to view and edit values in fields not placed under a section break. </p> <p>If you need information about permissions on objects, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects</a>.</p> <note type="note">
<ul>
<li> <p>Users without the permissions you specify here can't see the values of the fields
and image widgets that are not placed in a defined section in the custom form. This is also true if you display the values in reports or use them in calculated fields in text mode reporting.</p> </li>
<li> <p>Associating multiple object types with your form can change the viewing and editing permissions that are available in these steps. For more information, see <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">How multiple object types can affect section break permissions in a custom form</a> in this article.</p> </li>
</ul>
</note>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader"><b>Users with this access to the object can view field values</b> </td>
<td>
<ul>  
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
<tr>
<td role="rowheader">Users with this access to the object can edit field values</td>
<td>
<ul>
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
</tbody>
</table> </li>
<li value="5"> <p>Click Done.</p> <note type="tip">
You can click
<strong>Apply</strong> at any point while you are creating a custom form to save your changes and keep the form open.
</note> </li>
<li value="6"> <p>If you want to continue building your custom form in other ways, continue on to one of the following articles:</p>
<ul>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2" class="MCXref xref">Add a custom field to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md" class="MCXref xref">Add or edit an asset widget in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Add calculated data to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md" class="MCXref xref">Position custom fields and widgets in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md" class="MCXref xref">Preview and complete a custom form</a> </li>
</ul> </li>
</ol>
</div>
-->

## Hoe meerdere objecttypen de machtigingen voor secties kunnen beïnvloeden {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

De beperkte machtiging Bewerken voor afbrekingen van aangepaste formuliersecties is alleen beschikbaar voor de typen projecten, taken, problemen en gebruikersobjecten.

Als u in een aangepast formulier met een sectie-einde dat is geconfigureerd met de machtiging Beperkte bewerking, een van de andere objecttypen aan het formulier toevoegt (Portfolio, Programma, Document, Bedrijf, Factureringsrecord, Iteratie, Kosten of Groep), wordt u gevraagd om over te schakelen naar de machtiging Bewerken. Deze is compatibel met zowel dat objecttype als de bestaande objecttypen op het formulier.

>[!INFO]
>
>**Voorbeeld:** In een douaneformulier verbonden aan het de objecten van het Project type, wordt een sectieonderbreking gevormd met de Beperkte Edit toestemming.
>
>U voegt het objecttype Portfolio aan het formulier toe. Dit betekent dat de optie Beperkte bewerking niet meer beschikbaar is voor het sectie-einde in het formulier.
>
>Een bericht op het scherm zet u ertoe aan om op de Edit toestemming, die het meest gelijkaardig aan Beperkte Edit is, en compatibel met zowel het de objecten van het Project type als het objecten van het Portfolio type is te schakelen.
