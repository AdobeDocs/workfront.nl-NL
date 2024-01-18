---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Voorvertoning 4
description: Deze pagina beschrijft alle veranderingen beschikbaar in het milieu van de Voorproef met R1.4 versie. De functionaliteit op deze pagina is op 15 februari 2017 beschikbaar gesteld in de voorvertoningsomgeving.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# R1 Voorvertoning 4

Deze pagina beschrijft alle veranderingen beschikbaar in het milieu van de Voorproef met R1.4 versie. De functionaliteit op deze pagina is op 15 februari 2017 beschikbaar gesteld in de voorvertoningsomgeving.

Voor een lijst van alle veranderingen die in R1 worden aangebracht, zie [De Workfront R1-release](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md).

## Bijgewerkt project, Taak, en Kwestie goedkeurt

Wanneer het creëren van goedkeuringsprocessen voor project, taak, en uitgevende goedkeuringen, zijn de volgende verhogingen en de veranderingen nu beschikbaar: 

* Goedkeuring &quot;Stappen&quot; worden nu goedkeuringsfasen genoemd.
* Meerdere typen fiatteurs per werkgebied opnemen.\
  Dit omvat gebruikers, teams en taakrollen.\
  Vóór deze wijziging kunt u alleen meerdere fiatteurs van hetzelfde type opnemen. U kunt bijvoorbeeld meerdere taakrollen opnemen, maar niet een taakrol en een team.

* De volgende reeds bestaande beperkingen met betrekking tot de wijziging van bestaande algemene goedkeuringsprocedures zijn geschrapt:

   * Het gewijzigde goedkeuringsproces wordt alleen weerspiegeld op objecten in het hele systeem waar het goedkeuringsproces nog niet is gestart of waar het goedkeuringsproces niet is gewijzigd. Objecten waarvan het goedkeuringsproces al is gestart of waar het goedkeuringsproces is gewijzigd, worden niet bijgewerkt met uw wijzigingen.
   * U kunt de status die bepaalt wanneer de goedkeuring start, niet wijzigen.

* Bijgewerkt uiterlijk.

Voor meer informatie over het creëren van goedkeuringsprocessen, zie [Een goedkeuringsproces voor werkitems maken](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Wanneer het associëren van een goedkeuringsproces met een project, een taak, of een kwestie, zijn de volgende verhogingen en de veranderingen nu beschikbaar:

* Bijgewerkt uiterlijk.
* Het goedkeuringsdiagram wordt weergegeven op het tabblad Goedkeuring en geeft een visuele weergave weer van eerdere, huidige en toekomstige goedkeuringsstappen.

Zie voor meer informatie over het koppelen van goedkeuringen aan projecten, taken en problemen [Een nieuw of bestaand goedkeuringsproces koppelen aan werk](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## De status van een project rechtstreeks wijzigen vanaf de projectpagina

U hoeft een project niet meer te bewerken om de projectstatus te wijzigen. U kunt de status van een project nu rechtstreeks wijzigen vanaf de hoofdpagina van het project.

Zie voor meer informatie [De status van een project wijzigen](../../../../manage-work/projects/manage-projects/change-project-status.md).

## Gebruikers plannen voor deactivering

U kunt nu plannen dat gebruikers op een toekomstige datum worden gedeactiveerd.

Vóór deze verbetering, kon u een gebruiker slechts manueel deactiveren onmiddellijk.

Het plannen van een gebruiker om worden gedeactiveerd kan in een verscheidenheid van scenario&#39;s nuttig zijn. Als u bijvoorbeeld in Workfront gebruikers maakt die tijdelijk worden gehuurd, kunt u deze gebruikers instellen op deactivering wanneer hun contract afloopt.

Deze functie is ook beschikbaar voor gebruikers die bulkbewerkingen uitvoeren. 

Voor meer informatie over het plannen van gebruikers voor deactivering, zie [Een gebruiker deactiveren of opnieuw activeren](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) en [Gebruikers toevoegen](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Nieuwe e-maildigest-opties voor &quot;Acties vereist&quot;

De optie Dagelijkse samenvatting is nu beschikbaar in het gedeelte Actie vereist van de instellingen voor Meldingen.

Zie voor meer informatie [Uw eigen e-mailmeldingen wijzigen](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Vergeet niet het e-mailadres bij te werken dat aan uw account is gekoppeld om deze functionaliteit te kunnen testen. Dit is vereist omdat de voorvertoningssandbox de e-mailadressen van alle gebruikers wist.

## Verbetering van prullenbak: opgenomen in de updatestroom en e-mailmelding ontvangen

De volgende verbeteringen zijn toegevoegd bij het herstellen van verwijderde projecten, taken en problemen:

* U ontvangt nu een e-mailbericht nadat u een object hebt teruggezet.\
  Als Workfront-beheerder ontvangt u nu een e-mailbericht nadat u een project, taak of uitgave hebt hersteld die eerder is verwijderd. In het e-mailbericht wordt u geïnformeerd over de status van het herstelproces.\
  Ga voor meer informatie over het herstellen van objecten in Workfront naar [Verwijderde items herstellen](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Wanneer het object is hersteld, wordt het verwijderen en herstellen van het object nu opgenomen in de updatestream van het object zelf en in de updatestream van het bovenliggende object.\
  Eerder werd alleen de verwijdering opgenomen in de updatestream van het bovenliggende object.\
  Wanneer de taak bijvoorbeeld is hersteld, wordt een bericht toegevoegd aan de updatestream van zowel het project als de taak zelf om aan te geven dat de taak is hersteld. (Verwijderen en herstellen worden niet opgenomen bij subtaken. Informatie over het verwijderen en herstellen van subtaken is alleen beschikbaar voor bovenliggende taken.)\
  Zie voor meer informatie [Verwijderde items herstellen](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

 

## Bijgewerkt de Doos van de Dialoog voor het Leiden het Lidmaatschap van de Groep

Er is een nieuwe interface voor het beheer van Groepen en Subgroups die een gemakkelijkere, gebruikersvriendelijkere ervaring aanbiedt.

Het veld Groepseigenaren en het veld Groepsleden worden nu gecombineerd in één veld, met een lijst van hieronder vermelde groepsleden. Bovendien kunt u de lijst met groepsleden filteren en wijzigen of ze eigenaar of lid zijn. 

Voor meer informatie over het toevoegen van subgroepen aan groepen en het aanwijzen van gebruikers als leden of groepseigenaren van groepen, zie [Een groep maken](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) en [Een groep maken](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

 

## Tekst kopiëren in de mobiele toepassing

U kunt tekst kopiëren in de volgende velden van alle objecten die zichtbaar zijn in de mobiele app:

* Naam
* Beschrijving
* Referentienummer
* Opmerkingen

Deze functionaliteit moet in de week van 13 februari worden vrijgegeven voor de App Store van iOS en Android.
