---
content-type: release-notes
navigation-topic: 2019-4-release-activity
title: 2019.4 andere verbeteringen
description: Op deze pagina worden verschillende verbeteringen beschreven die zijn aangebracht met de release van 2019.4. Het wordt in de week van 11 november 2019 beschikbaar gesteld in de productieomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: ed7488f1-2076-4160-97f3-a3da25cccd0f
source-git-commit: e1bf5fbc7dc25bf8ce472b21b9a0906530f82cf0
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# 2019.4 andere verbeteringen

Op deze pagina worden verschillende verbeteringen beschreven die zijn aangebracht met de release van 2019.4. Het wordt in de week van 11 november 2019 beschikbaar gesteld in de productieomgeving.

Voor een lijst met alle wijzigingen die in 2019.4 zijn aangebracht, raadpleegt u [Overzicht van de release 2019.4](../../../../product-announcements/product-releases/quarterly-release-archive/2019.4-release-activity/2019-4-release-activity-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td> <strong>Een automatische proefdrukworkflow starten vanuit een Adobe CC-document</strong> <p>Zonder Adobe CC te verlaten, kunt u een geautomatiseerde testworkflow starten voor een Adobe CC-document dat u hebt gemaakt. Zie de sectie voor meer informatie <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md#generate" class="MCXref xref" xrefformat="{para}">Een proefdruk van Illustrator of InDesign genereren</a> in het artikel <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md" class="MCXref xref" xrefformat="{para}">De extensie Workfront voor Illustrator en InDesign gebruiken</a>.</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td><strong>Workfront G Suite add-on</strong> <p>Now you can manage Workfront objects directly from Gmail, Google Calendar, and Google Drive.</p> <p>When you open a Workfront notification email, instantly view all information about the associated object and take actions, such as reviewing content or updating a status, without leaving your Inbox.</p> <p>When you open a non-Workfront email:</p> 
     <ul> 
      <li>Convert it into a task or issue.</li> 
      <li>Associate it with a project.</li> 
      <li>Assign it as a work item.</li> 
      <li>Add it to a work item as an update.</li> 
      <li>Upload its attachments to Workfront.</li> 
     </ul> <p>Manage Workfront objects without leaving G Suite:</p> 
     <ul> 
      <li>Post updates and replies to comments.</li> 
      <li>View and manage documents associated with a task or issue.</li> 
     </ul> <p>Access and work with object details:</p> 
     <ul> 
      <li>Read the description</li> 
      <li>View the parent object</li> 
      <li>Change the status</li> 
      <li>Access custom data</li> 
      <li>Mark it as complete.</li> 
     </ul> <p>And access your Workfront Home content, including tasks, issues, approvals, and access requests, without leaving G Suite.</p> <p>For more information, see <a href="../../../../workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront for G Suite</a>.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td> <strong>Dubbele e-mailadressen voorkomen</strong> <p>U kunt niet meer hetzelfde e-mailadres gebruiken wanneer u meerdere gebruikers in Workfront maakt, zelfs als deze e-mailadressen per geval verschillen. U kunt bijvoorbeeld niet één gebruiker maken met het e-mailadres JohnDoe@example.com en een andere gebruiker met het e-mailadres johndoe@example.com. </p> <p>Vóór deze wijziging werd het maken van gebruikers met overeenkomende e-mailadressen die alleen per geval verschilden, ondersteund. </p> <p>Opmerking: bestaande gebruikers met overeenkomende e-mailadressen die alleen per geval verschillen, moeten op een toekomstige datum worden bijgewerkt. Als u gebruikers hebt in een Workfront-exemplaar met overeenkomende e-mailadressen die alleen per geval verschillen, neemt Workfront contact met u op met aanvullende informatie en een tijdlijn wanneer deze moeten worden bijgewerkt.</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Aanvullende objecttypen beschikbaar voor Typeahead-velden in een aangepast formulier</strong> 
     <p>Nu, wanneer u een douanegebied van Typeahead creeert, kunt u de volgende objecten types met het gebied associëren: Gebruiker, Bedrijf, Groep, de Rol van de Baan, Portfolio, Programma, Project, en Malplaatje.</p> 
     <p>Eerder kon u alleen het objecttype Gebruiker aan een aangepast Typeahead-veld koppelen.</p> 
     <p>Zie de sectie voor meer informatie <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create" class="MCXref xref" xrefformat="{para}">Een aangepast formulier maken of bewerken</a> in het artikel <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Een aangepast formulier maken of bewerken</a>.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> <strong>Bestandsnaam van de meest recente versie van een weergegeven document</strong> <p>Wanneer u nu een documentversie uploadt met een andere bestandsnaam dan die van de bestaande versie, wordt de nieuwe bestandsnaam weergegeven in Workfront.</p> <p>Eerder, toen u een nieuwe versie met een verschillende filename toevoegde, bleef filename van de vorige versie in Workfront tonen.</p> <p>Zie voor meer informatie <a href="../../../../documents/managing-documents/upload-new-document-version.md" class="MCXref xref" xrefformat="{para}">Een nieuwe versie van een document uploaden</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <strong>Een filter toevoegen aan een Typeahead-veld in een aangepast formulier</strong> <p>Wanneer u nu een Typeahead-veld toevoegt aan een aangepast formulier, kunt u een filter toevoegen om de objecten te beperken die beschikbaar zijn wanneer iemand het veld gebruikt. U kunt het veld bijvoorbeeld beperken, zodat de gebruiker alleen leden van de marketing- en verkoopteams in uw organisatie kan selecteren.</p> <p>Zie de sectie Maken en een nieuw veld toevoegen in het artikel Aangepaste Forms maken voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Het weergavetype van een veld in een aangepast formulier wijzigen</strong> 
     <p>Nu kunt u het weergavetype van een veld in een aangepast formulier wijzigen.</p> 
     <p>Als u bijvoorbeeld een veld Selectievakjes hebt gemaakt, kunt u dit wijzigen in een veld Vervolgkeuzelijst of Keuzerondjes. Deze drie weergavetypen in velden zijn onderling verwisselbaar.</p> 
     <p>Als u een tekstveld Eén regel hebt gemaakt, kunt u dit wijzigen in een tekstveld Alineatekst. Deze twee veldweergavetypen zijn onderling verwisselbaar.</p> 
     <p>Eerder moest u een nieuw veld maken en het oude veld verwijderen om het weergavetype van een aangepast veld te wijzigen. Hiervoor moesten gegevens worden overgedragen, wat vaak tijdrovend was.</p> 
     <p>Zie voor meer informatie <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create" class="MCXref xref" xrefformat="{para}">Een aangepast formulier maken of bewerken</a> in het artikel <a href="../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Een aangepast formulier maken of bewerken</a></p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Tijdschema's en rapporten maken</strong> 
     <p>U kunt nu de tijd van de gebruiker voor betere planning en uitvoering zien. U kunt nieuwe tijd van rapporten en kalenders aan uw dashboards voor een mening in real time van gebruikersbeschikbaarheid ook toevoegen.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
