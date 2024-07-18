---
product-area: documents
navigation-topic: manage-documents
title: Documenten controleren
description: U kunt een document uitchecken om te voorkomen dat andere gebruikers het document verwijderen of een nieuwe versie ervan uploaden. Slechts één gebruiker kan een document tegelijk uitchecken. U kunt elk document dat naar Adobe Workfront is geüpload, uitchecken en documenten die zijn gekoppeld aan externe documentproviders (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint of een andere aangepaste provider).
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Documenten controleren

U kunt een document uitchecken om te voorkomen dat andere gebruikers het document verwijderen of een nieuwe versie ervan uploaden. Slechts één gebruiker kan een document tegelijk uitchecken. U kunt elk document dat naar Adobe Workfront is geüpload, uitchecken en documenten die zijn gekoppeld aan externe documentproviders (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint of een andere aangepaste provider). 

## Toegangsvereisten

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
   <td> <p>Toegang tot documenten bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang tot het document beheren</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Handelingen die zijn toegestaan voor uitgecheckte documenten

Gebruikers met beheerde toegang tot het document kunnen het volgende doen:

* Het document bewerken (documentnaam, beschrijving, aangepaste gegevens)
* Het document verplaatsen
* Het document delen
* Voorbeeld van het document bekijken
* Het document downloaden

  >[!TIP]
  >
  > Hoewel een gebruiker een document kan downloaden wanneer het door een andere gebruiker is uitgecheckt, raden we gebruikers aan te wachten totdat het document opnieuw is ingecheckt voordat het wordt gedownload. Wanneer een document is uitgecheckt, geeft dit vaak aan dat er nog werk wordt verricht in het document. Als u wacht tot een document weer is ingecheckt om het te downloaden, zorgt u ervoor dat de gebruiker de meest recente versie heeft.

* Goedkeuren of een goedkeuring op het document toepassen.
* Het document controleren in de proefdrukviewer

  Voor meer informatie over het proef, zie [ het Bewijzen ](../../review-and-approve-work/proofing/proofing.md)

## Een document uitchecken

Als u beheerdersmachtigingen voor een document hebt, kunt u het uitchecken om bepaalde handelingen in het document te verbieden. 

1. Ga naar het gebied waar het document is opgeslagen en selecteer het document. 

   Voor informatie over het toevoegen van documenten, zie [ documenten aan Adobe Workfront van uw dossiersysteem ](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md) toevoegen.

1. Klik het **Uitchecken** pictogram ![](assets/check-out-25x23.png).

1. Rechts van de documentnaam wordt een vergrendelingspictogram ![](assets/lock-icon-locked-qs.png) weergegeven. Het document blijft uitgecheckt nadat u zich hebt afgemeld bij Workfront.
1. Alleen de gebruiker die het document heeft uitgecheckt of de Workfront-beheerder kan het document inchecken.

## Uitgecheckte documenten beheren

Overweeg het volgende over uitgecheckte documenten:

* Voordat u een object kunt verwijderen waar een uitgecheckt document is opgeslagen, moet u het document eerst weer inchecken. 
* Als de Workfront-beheerder een gebruiker verwijdert die een document heeft uitgecheckt dat hij of zij niet bezat, wordt het document automatisch door Workfront ingecheckt.
* Als de Workfront-beheerder een gebruiker verwijdert die een document dat hij of zij heeft uitgecheckt en het document op een object wordt geüpload, blijft het document uitgecheckt. Alleen een Workfront-beheerder kan deze weer inchecken.
* Als de Workfront-beheerder een gebruiker verwijdert die een document dat hij of zij heeft uitgecheckt en het document alleen wordt geüpload in het gebied Documenten (niet in een object), wordt het document met de gebruiker verwijderd.

  Voor informatie over het schrappen van gebruikers, zie [ gebruikers van de Schrapping ](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* Als de Workfront-beheerder een gebruiker deactiveert, blijven alle uitgecheckte documenten uitgecheckt. Alleen een Workfront-beheerder kan ze weer inchecken. 

## Een document inchecken

U moet een document opnieuw inchecken voordat u een nieuwe versie kunt uploaden of verwijderen. 

Een document inchecken:

1. Ga naar het gebied waar het document is opgeslagen en selecteer het document. 

   Rechts van de documentnaam wordt een vergrendelingspictogram ![](assets/lock-icon-locked-qs.png) weergegeven.

1. Klik het **Controle binnen** pictogram ![](assets/check-in-25x22.png).
