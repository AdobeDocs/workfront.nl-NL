---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Een uitgave delen
description: Uw Adobe Workfront-beheerder verleent gebruikers toegang tot weergave- of bewerkingsproblemen wanneer zij toegangsniveaus toewijzen. Zie Toegang verlenen tot problemen voor meer informatie over het verlenen van toegang tot problemen.
author: Courtney
feature: Get Started with Workfront
exl-id: 91ee72e0-20a9-4b06-9f80-a343dd4fbe06
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 0%

---

# Een uitgave delen

Uw Adobe Workfront-beheerder verleent gebruikers toegang tot weergave- of bewerkingsproblemen wanneer zij toegangsniveaus toewijzen. Voor meer informatie over het verlenen van toegang tot kwesties, zie [ Toegang van de Verlening tot kwesties ](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md).

Samen met het toegangsniveau dat gebruikers wordt verleend, kunt u hen toestemmingen aan Mening, Contribute, of Manage ook verlenen specifieke kwesties die u toegang hebt om te delen. Voor meer informatie over toegangsniveaus en toestemmingen, zie [ hoe de toegangsniveaus en de toestemmingen samen ](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) werken.

Machtigingen gelden specifiek voor één item in Workfront en definiëren welke handelingen u op dat item kunt uitvoeren.


## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p> 
   <p>Werk of hoger</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot of hoger weergeven voor de objecten die u wilt delen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen of hoger weergeven voor de objecten die u wilt delen</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het delen van problemen

Naast de overwegingen hieronder, zie ook [ Overzicht van het delen van toestemmingen op voorwerpen ](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Een Workfront-beheerder kan machtigingen toevoegen of verwijderen voor alle items in het systeem, zonder de eigenaar van die items te zijn.

* De maker van een uitgave beschikt standaard over de machtiging Beheren.
* U kunt kwesties individueel delen, of u kunt verscheidene van hen tegelijkertijd delen. Delen is hetzelfde als delen van andere objecten in Workfront. Voor meer informatie over het delen van punten in Workfront, zie [ een voorwerp ](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md) delen.
* U kunt de volgende toestemmingen aan een kwestie verlenen:

   * Weergave
   * Contribute
   * Beheren

* Als u een uitgave deelt, nemen alle documenten die aan de uitgave zijn gekoppeld dezelfde machtigingen over.

  De Workfront-beheerder kan opgeven of documenten machtigingen van hogere objecten moeten overnemen op het toegangsniveau van de gebruiker. Voor meer informatie over het beperken van geërfte toestemmingen op documenten, zie [ tot douanetoegangsniveaus ](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

* U kunt overgeërfde machtigingen verwijderen uit een uitgave. Voor meer informatie, zie [ toestemmingen uit voorwerpen ](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md) verwijderen.

## Manieren om een probleem te delen

* Handmatig, wat vergelijkbaar is met het delen van andere objecten in Workfront.
* Automatisch, door één van het volgende te doen:

   * Geef de machtigingen voor een van de bovenliggende objecten van de uitgave op: project, programma of portfolio. De kwesties erven de toestemmingen van hun oudervoorwerpen. Voor informatie over het bekijken van geërfte toestemmingen op voorwerpen, zie [ Mening geërfte toestemmingen op voorwerpen ](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Voeg entiteiten aan het Delen van het Project op een malplaatje toe dat wordt gebruikt om het project tot stand te brengen de kwestie is. Voor informatie over het delen van projecten van malplaatjes, zie [ een malplaatje ](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md) delen.

   * Specificeer de toestemmingen op alle kwesties in een project wanneer u het project uitgeeft. Voor informatie over het beheren van de toegang tot kwesties of verzoeken op het project dat op de toestemmingen van een gebruiker aan het project wordt gebaseerd, zie de [](../../manage-work/projects/manage-projects/edit-projects.md#access) sectie in het artikel [ projecten ](../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

     >[!TIP]
     >
     >Als u niet specificeert welke toestemmingen van de uitgave u gebruikers wilt hebben wanneer zij aan de kwesties op het project worden toegewezen, ontvangen zij de zelfde toestemmingen die zij op het project door gebrek hebben.

   * Geef de machtigingen op die gebruikers ontvangen bij problemen die ze in een aanvraagwachtrij verzenden wanneer ze een aanvraagwachtrij maken. Voor informatie, zie [ een Rij van het Verzoek ](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.

     >[!IMPORTANT]
     >
     >De toestemmingen worden verleend verschillend afhankelijk van al dan niet het project als verzoekrij wordt gepubliceerd:
     >
     >   
     >   
     >   * Wanneer een gebruiker een verzoek naar een project voorlegt dat als verzoekrij wordt gepubliceerd, wordt het Primaire Contact en ingegaan door gebruikers verleend de gespecificeerde toestemming.
     >   * Wanneer een gebruiker een verzoek naar een project indient dat niet als verzoekrij wordt gepubliceerd, wordt het Primaire Contact (als verschillend van ingegaan door gebruiker) de gespecificeerde toestemming verleend, en de Ingegaan door gebruiker wordt verleend leidt toestemmingen aan de kwestie.
     >   
     >

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Automatically share an issue at the project level</h2>
<p>(NOTE: this info duplicates in Edit projects - linked there instead (above).)  </p>
<p>As the Project Owner, you can grant permissions automatically to users as the issues are added to a project.</p>
<ol>
<li value="1">Go to the project whose issues you want to share automatically.</li>
<li value="2"> Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. </li>
<li value="3">In the <strong>Edit Project</strong> box that displays, click <strong>Access</strong>.</li>
<li value="4">In the <strong>When someone is assigned to an ISSUE</strong> field, select from the following permissions levels:
<ul>
<li><strong>View</strong></li>
<li><strong>Contribute</strong></li>
<li><strong>Manage</strong><br>Now, when someone is assigned to an issue on the selected project, they are granted the specified permissions to the issue.  </li>
</ul></li>
<li value="5">(Optional) Select the <strong>Also grant ... access to the project</strong> field to also grant View, Contribute, or Manage permissions to the projects to the user assigned to the issue</li>
<li value="6">In the <strong>When someone submits a REQUEST ...</strong> field, select from the following permissions levels:
<ul>
<li><strong>View</strong></li>
<li><strong>Contribute</strong></li>
<li><p><strong>Manage</strong></p><note type="important">
<p>Permissions are granted differently depending on whether or not the project is published as a request queue:</p>
<ul>
<li>When a user submits a request to a project published as a request queue, the Primary Contact and Entered By users are granted the permission specified.</li>
<li>When a user submits a request to a project not published as a request queue, the Primary Contact (if different from Entered By user) is granted the permission specified, and the Entered By user is granted Manage permissions to the issue.</li>
</ul>
</note></li>
</ul></li>
<li value="7"> <p>(Optional) Select the <strong>People from the same company will inherit the same permissions for all requests</strong> field.</p> <p>People from the same company as the user submitting the request are granted the same permissions on the requests as the user.  </p> </li>
<li value="8">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Automatically share an issue in request queues</h2>
<p>(NOTE: drafted because it's duplicated from Create a Request Queue which is linked above)  </p>
<p>As the Project Owner, you can grant permissions automatically to users as the issues are submitted to a request queue.</p>
<ol>
<li value="1">Go to the project whose issues you want to share automatically.</li>
<li value="2">Click <strong>Edit Project</strong>.</li>
<li value="3">Click <strong>More</strong> then click <strong>Queue Setup</strong>. </li>
<li value="4"> <p>On the <strong>Queue Details</strong> sub-tab, in the drop-down menu under <strong>When someone makes a request, automatically grant</strong>, select from the following permissions levels:</p>
<ul>
<li><strong>View Access</strong> </li>
<li><strong>Contribute Access</strong> </li>
<li> <p><strong>Manage Access</strong> </p> </li>
</ul> <p>Now, when someone submits a request to the selected project, they are granted the specified permissions to the request.</p> </li>
<li value="5"> <p>(Optional) Select the <strong>People from the same company will inherit the same permissions for all requests</strong>.</p> <p>People from the same company as the user submitting the request are granted the same permissions on the requests as the user.  </p> </li>
<li value="6">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Een uitgave delen

1. Navigeer naar de uitgave die u wilt delen.

1. Aan het recht van de voorwaardennaam, klik **Aandeel**. Het **2} dialoogvakje van de Naam van de Uitgave 1} van het Aandeel {opent.[]**

   ![ de kwestie van het Aandeel knoop ](assets/share-issue-button.png)

1. In de **Uitgiftetoegang van de Verlening tot** gebied, begin typend de naam van de gebruiker, het team, de rol, de groep, of het bedrijf u de kwestie met wilt delen, dan klik de naam wanneer het in de drop-down lijst verschijnt.

   >[!TIP]
   >
   >U kunt een kwestie met actieve gebruikers, teams, rollen, of bedrijven slechts delen.


1. (Facultatief) selecteer **wie toegang** drop-down heeft en het de toegangsniveau van de kwestie selecteert:

   * **slechts kunnen de uitgenodigde mensen toegang hebben:** slechts de gebruikers die aan de kwestie worden uitgenodigd kunnen tot het (Gebrek) toegang hebben.
   * **iedereen in het systeem kan** bekijken: Alle gebruikers in het systeem kunnen de kwestie zonder een uitnodiging bekijken.

1. Klik op de vervolgkeuzelijst rechts van de gebruikersnaam en selecteer het machtigingsniveau voor deze uitgave:

   * **Mening**: De gebruiker kan de kwestie herzien en delen.
   * **draag bij** bij: De gebruiker kan updates maken, logboekinformatie, minder belangrijke uitgeven maken, en de kwestie (omvat ook alle toestemmingen van de Mening) delen.
   * **leidt**: De gebruiker heeft volledige toegang tot de kwestie zonder administratieve rechten, die op het toegangsniveau (omvat ook alle toestemmingen van de Mening en van Contribute) worden verleend.

1. (Optioneel) Klik op het pictogram Geavanceerde opties naast het machtigingsniveau dat u hebt toegekend om specifieke machtigingen voor de uitgave te configureren.

   ![ gevormde geavanceerde toestemmingsopties ](assets/advanced-permission-options.png)

1. (Facultatief) om de kwestie snel te delen gebruikend een verbinding, klik **verbinding van het Exemplaar** en door:sturen het aan de ontvanger.

1. Klik **sparen**.

## Problemen bulksgewijs delen

1. Navigeer naar het project dat de kwesties bevat u wilt delen.

1. In het **lusje van Kwesties** op de projectpagina, selecteer de doos links van elke kwestie u wilt delen, dan klik het **pictogram van het Aandeel** ![ Aandeel ](assets/share-icon.png) bij de bovenkant van de pagina. Het deelmodaal wordt geopend.

   ![ Bulk deelt kwesties ](assets/bulk-share-issues.png)

1. In de **Uitgiftetoegang van de Verlening tot** gebied, begin typend de naam van de gebruiker, het team, de rol, de groep, of het bedrijf u de kwesties met wilt delen, dan klik de naam wanneer het in de drop-down lijst verschijnt.

   >[!TIP]
   >
   >U kunt kwesties met actieve gebruikers, teams, rollen, of bedrijven slechts delen.


1. (Facultatief) selecteer **wie toegang** drop-down heeft en het de toegangsniveau van kwesties selecteert:

   * **slechts kunnen de uitgenodigde mensen toegang hebben:** slechts de gebruikers die aan de kwesties worden uitgenodigd kunnen tot hen (Gebrek) toegang hebben.
   * **iedereen in het systeem kan** bekijken: Alle gebruikers in het systeem kunnen de kwesties zonder een uitnodiging bekijken.


1. Klik op de vervolgkeuzelijst rechts van de naam van de gebruiker en selecteer het desbetreffende machtigingsniveau voor de problemen:

   * **Mening**: De gebruiker kan de kwesties herzien en delen.
   * **draag bij** bij: De gebruiker kan updates maken, logboekinformatie, minder belangrijke uitgeven maken, en de kwesties (omvat ook alle toestemmingen van de Mening) delen.
   * **leidt**: De gebruiker heeft volledige toegang tot de kwesties zonder administratieve rechten, die op het toegangsniveau (omvat ook alle toestemmingen van de Mening en van Contribute) worden verleend.

1. (Optioneel) Klik op het pictogram Geavanceerde opties naast het machtigingsniveau dat u hebt toegekend om specifieke machtigingen voor de problemen te configureren.

   ![ gevormde geavanceerde toestemmingsopties ](assets/advanced-permission-options.png)

1. Klik **sparen**.

## Machtigingen geven

In de volgende tabel wordt weergegeven welke machtigingen u gebruikers kunt verlenen wanneer u hen toestaat een uitgave weer te geven, bij te dragen of te beheren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong> Acties </strong> </td> 
   <td><strong> leiden </strong> </td> 
   <td><strong> draagt </strong> bij </td> 
   <td><strong> Mening </strong> </td> 
  </tr> 
  <tr> 
   <td> <p>Problemen toevoegen</p> </td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Verwijderen  </td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Aangepast formulier bijvoegen</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Aangepaste velden bewerken</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Probleem goedkeuren</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Een goedkeuringsproces toevoegen</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Documenten toevoegen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Probleem kopiëren*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Probleem verplaatsen</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Logboekuren</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Omzetten in project*</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Toewijzing accepteren</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Updates/opmerkingen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Geplande datums wijzigen</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Toewijzingen maken</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Delen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Delen in het hele systeem</td> 
   <td>  </td> 
   <td>  </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42; gecontroleerd door de toegangsniveaus en de toestemmingen op het project.
