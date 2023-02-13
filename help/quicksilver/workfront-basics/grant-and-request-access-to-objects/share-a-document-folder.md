---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Een documentmap delen
description: U kunt een map en de inhoud ervan delen vanuit het gebied Documenten.
author: Alina
feature: Get Started with Workfront
exl-id: c0d318a8-b1cf-4522-b478-acf092687658
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Een documentmap delen

U kunt een map en de inhoud ervan delen vanuit het gebied Documenten.

>[!NOTE]
>
>* De map moet zich in de bovenste vijf niveaus van een maphiërarchie op een object bevinden. Elke map op het zesde niveau of erft de configuraties voor delen van de map direct erboven.
>
>  Zie de sectie voor informatie over het toevoegen van submappen om een mappenhiërarchie te maken [Mappen en submappen maken](../../documents/organizing-documents/create-documents-folder.md#creating-folders) in het artikel [Documentmappen maken](../../documents/organizing-documents/create-documents-folder.md).
>
>* Slimme mappen kunnen niet worden gedeeld.
>* Als u het delen opties voor een documentomslag binnen een malplaatje vormt, en dan leidt iemand tot een project van dat malplaatje, uw het delen configuraties brengen niet naar de documentomslag in het nieuwe project over.
>* Als u het delen opties voor een documentomslag binnen een het werkpunt vormt en dan het het werkpunt kopieert, brengt uw het delen configuraties niet naar de documentomslag in het nieuwe het werkpunt over.
>


## Toegangsvereisten

<!--drafted for P&P
(I am putting Contributor and higher here because this is what I found in testing. Normally, Review equals Light but I found out that Contributor can also have manage rights to documents and can share them.)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Review or higher</p>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Documents</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to an object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten weergeven</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang tot een object weergeven</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Een map delen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Documenten**.

   of

   Open een Workfront-object en klik op **Documenten** in het linkerdeelvenster.

1. Selecteer de map en klik op het pictogram Delen ![](assets/share-icon.png) in de werkbalk.

   De map moet zich in de bovenste vijf niveaus van een maphiërarchie op een object bevinden en kan geen slimme map zijn.

1. In het vak dat wordt weergegeven, onder **Map toegang geven tot**, begin de naam van de gebruiker, het team, de baanrol, de groep, of het bedrijf te typen u de omslag met wilt delen, dan druk **Enter** wanneer de naam wordt weergegeven.
1. Als u de toegang wilt aanpassen voor de gebruiker, het team, de taakrol, de groep of het bedrijf dat u net hebt toegevoegd, klikt u op het vervolgkeuzemenu rechts van de naam en configureert u vervolgens een van de volgende beschikbare opties en een van de geavanceerde instellingen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Weergeven</td> 
      <td> <p>Mogelijkheid om de map en de inhoud ervan weer te geven.</p> <p>Klikken <strong>Geavanceerde instellingen</strong> om op te geven of u het volgende wilt toestaan:</p> 
       <ul> 
        <li><strong>Downloaden</strong>: De map en de inhoud ervan kunnen worden gedownload als ZIP-bestand</li> 
        <li> <p><strong>Delen</strong>: Mogelijkheid om de map te delen met anderen in het systeem</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beheren</td> 
      <td> <p>De map en de inhoud ervan weergeven en bewerken</p> <p>Klikken <strong>Geavanceerde instellingen</strong> om op te geven of u gebruikers wilt toestaan het volgende te doen:</p> 
       <ul> 
        <li><strong>Verwijderen</strong>: De map en de inhoud ervan uit het systeem verwijderen</li> 
        <li><b>Downloaden</b>: De map en de inhoud ervan downloaden als ZIP-bestand</li> 
        <li><strong>Delen</strong>: De map en de inhoud ervan delen met andere gebruikers in het systeem</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Herhaal stap 3-4 om andere namen aan de lijst toe te voegen en hun opties te configureren.
1. (Optioneel) Als u wilt dat iedereen in het systeem de map en de inhoud ervan kan bekijken, klikt u op het tandwielpictogram ![](assets/gear-icon-settings-with-dn-arrow.jpg) in de rechterbovenhoek van het dialoogvenster voor delen klikt u op **Maak dit zichtbaar voor het hele systeem.**

   Als u van mening verandert, kunt u, klikken **Toegang voor het hele systeem verwijderen** (de standaardoptie).

## Hoe gebruikers tot de inhoud van een omslag toegang hebben die met hen wordt gedeeld

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Delete these 2 paragraphs when the story &nbsp;<a href="https://hub.workfront.com/task/622f8d6f000897c9a4a11bdfd9b2cf34/overview">Handle email notification content when a folder is shared</a> goes to Preview:</p>
-->

Als u een map deelt, zien de ontvangers de map momenteel niet in hun documentengebied. Ze hebben echter wel toegang tot de documenten door een documentrapport uit te voeren.

Voor informatie over het runnen van een rapport, zie de sectie [Objecten rapporteren](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) in het artikel [Objecten in Adobe Workfront begrijpen](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md). Zie ook [Een aangepast rapport maken](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Workfront sends a notification email when someone shares a document folder on an object with a user or a team. To access the folder from the email, recipients can click the folder title or the "See it in Workfront" link.</p> <note type="note">
<ul class="preview">
<li> <p>The email notification "Someone shares an object with me" or "Someone shares an object with my team" must be enabled in order for a user or team to receive a notification email about a shared folder.</p> </li>
<li> <p>When someone shares a document folder from the global Documents area, the links in the notification email take the recipient to the global Documents area. Because folders in this area are private, the shared folder is not displayed there, but the recipient can access its documents by creating a document report. </p> <p>For information about running a report, see the section <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects" class="MCXref xref">Report on objects</a> in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. Also see <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li>
<li> <p>Currently, it is not possible to share folders with external users.</p> </li>
</ul>
</note>
</div>
-->

## Overgenomen machtigingen wanneer u een object deelt dat een map bevat

Wanneer u een object deelt dat een documentmap heeft, krijgen de ontvangers ook toegang tot de map:

* Als u aan uw ontvangersToegang van de Mening tot het oudervoorwerp verleent, hebben zij de toegang van de Mening tot de omslag.
* Als u ontvangers Contribute of Manage toegang tot het bovenliggende object geeft, hebben ze beheertoegang tot de map.
* Als u één type toegang (Weergave, Contribute of Beheren) verleent aan het bovenliggende object en een ander type aan de map, hebben uw ontvangers de hoogste van deze twee typen toegang tot documenten in de map

   Als u bijvoorbeeld het bovenliggende object deelt met Weergavetoegang en de map met de toegang Beheren, hebben de ontvangers de optie Beheren voor de documenten in de map.

   >[!NOTE]
   >
   >Een bijgevoegd document neemt alleen machtigingen over van het object waaraan het is gekoppeld. Als u een map voor het object maakt en het document naar de map verplaatst, neemt deze de machtigingen van de map over. Maar als u een map maakt op een bovenliggend of bovenliggend object en het document naar die map verplaatst, worden de machtigingen van die map niet overgenomen.

* Als de optie &quot;nooit documenttoegang van projecten, taken, kwesties, enz. erft&quot;op het toegangsniveau van de ontvanger wordt toegelaten, zullen zij geen toestemmingen aan documenten in een omslag erven die u met hen deelt. Als u ze toegang wilt geven tot een document in de map, moet u het document delen.

   Voor informatie over de optie Nooit overnemen raadpleegt u [Toegang tot Adobe Workfront configureren](../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

   Voor informatie over het delen van een document raadpleegt u [Een document delen](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).
