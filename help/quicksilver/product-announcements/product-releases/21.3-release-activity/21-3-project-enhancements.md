---
title: 21.3 Projectverbeteringen
description: 21.3 Projectverbeteringen
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1df4ccdb-5b74-414c-a622-b0a5ed30a8c4
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 0%

---

# 21.3 Projectverbeteringen

Op deze pagina worden alle projectverbeteringen beschreven die zijn aangebracht met de release 21.3 voor de voorvertoningsomgeving. Deze verbeteringen zijn in de week van 21 juli 2021 beschikbaar gesteld in de productieomgeving.

Voor een lijst van alle veranderingen beschikbaar met de versie 21.3, zie [ overzicht van de Versie 21.3 ](../../../product-announcements/product-releases/21.3-release-activity/21-3-release-overview.md).

## Een sjabloon koppelen aan een groep

>[!NOTE]
>
>Deze functie is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring.

Om u te helpen het proces van de projectverwezenlijking stroomlijnen —en u te helpen gemakkelijker identificeren en rapporteren over welke groepen eigen welke project malplaatjes-wij de capaciteit hebben toegevoegd om een groep aan een projectmalplaatje toe te wijzen.

Wanneer u een groep aan een projectmalplaatje toewijst, worden alle projecten die van het malplaatje worden gecreeerd automatisch geassocieerd met de groep van het malplaatje. Voor meer informatie, zie [ projectmalplaatjes ](../../../manage-work/projects/create-and-manage-templates/edit-templates.md) uitgeven.

Ook, kunt u een proces van de groepsgoedkeuring aan een malplaatje en zijn malplaatjetaken vastmaken als het malplaatje met uw groep wordt geassocieerd. Voor meer informatie, zie [ een nieuw of bestaand goedkeuringsproces met het werk ](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) associëren.

## Velden gemakkelijker bewerken in de sectie Details

>[!NOTE]
>
>Deze functie is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring.

Met de volgende verbeteringen kunt u informatie gemakkelijker bewerken in de sectie Details van elk object:

* Een grijze omtrek rond een veld wanneer u de muisaanwijzer op het veld plaatst, geeft aan dat het veld bewerkbaar is.
* U kunt velden bewerken door er eenmaal op te klikken.

Vóór deze verbetering was het niet duidelijk welke velden bewerkbaar waren en u moest dubbelklikken om een veld te bewerken.

## Overweeg predecessors voor verschillende projecten bij het berekenen van afleveringsdatums

Met een nieuwe verbetering in de manier waarop Adobe Workfront afhandelingsdata voor taken berekent, wordt nu rekening gehouden met de afhankelijkheden tussen projecten.

Eerder werden de wachtdatums alleen berekend op basis van de voorgangers van de taak van hetzelfde project.

Nu, om ervoor te zorgen u altijd een nauwkeurige handoff datum voor een taak met een dwars-project voorganger hebt, moet u de chronologie van het project van de opvolgertaak opnieuw berekenen. Na het opnieuw berekenen van de tijdlijn, berekent de handoff data van de taak rekening houdend met de dwars-projectgebiedsdelen van de taken.

Voor meer informatie over handoff data, zie [ Overzicht van de Datum van de Afhandeling van de Taak ](../../../manage-work/tasks/task-information/handoff-task-date.md).

## Bestaande artikelen en problemen toevoegen vanaf het scrollbord

>[!NOTE]
>
>Deze functie is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring.

U kunt nu een bestaand artikel toevoegen of een bestaand artikel rechtstreeks vanaf het Klembord publiceren. Hierdoor is het gemakkelijker om bestaande artikelen aan uw huidige herhaling toe te voegen zonder dat u naar de achtergrondpagina hoeft te gaan.

Voor meer informatie, zie [ verhalen en kwesties van het board van het Trommel ](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md) toevoegen.

## Nieuwe artikelen en problemen toevoegen vanaf het Klembord

>[!NOTE]
>
>Deze functie is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring.

U kunt nu een nieuw artikel maken of een nieuw artikel rechtstreeks vanaf het tekengebied publiceren. Zo kunt u snel een nieuw artikel aan uw huidige herhaling toevoegen.

Voor meer informatie, zie [ verhalen en kwesties van het board van het Trommel ](../../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md) toevoegen.

## Een artikel of onderwerp verwijderen van het Kanban-bord

>[!NOTE]
>
>Deze functie is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring.

U kunt nu een artikel of uitgave rechtstreeks van uw Kanban-bord verwijderen door op het pictogram Meer van een artikel of uitgiftekaart te klikken en Verwijderen te selecteren. Wanneer u een artikel of uitgave verwijdert, wordt het artikel of de uitgave 30 dagen naar de prullenbak verplaatst en kan het alleen door de systeembeheerder worden hersteld.

Voor meer informatie, zie [ verhalen of kwesties van de Schrapping van de raad Kanban ](../../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md).

## Updates van Agicard-kopteksten en artikelborden

>[!NOTE]
>
>Deze functie is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring.

Op Kanban- en Scrum-borden zijn nu de volgende verbeteringen beschikbaar:

* De artikelkaarten en de bordkolommen hebben een vaste breedte, zodat de kaartgrootten niet veranderen als u de venstergrootte van de browser aanpast.
* De naam van de kolom Artikelen is gewijzigd in Bovenliggend artikel.
* Elke kaart heeft bovenaan een label waarmee het wordt aangeduid als een bovenliggend artikel, subtaak (gekoppeld aan een bovenliggend artikel), artikel (niet gekoppeld aan een bovenliggend artikel) of uitgave.
* Met achtergrondarcering worden de kolommen visueel gescheiden.

Voor meer informatie, zie [ Overzicht van Herhalingen ](../../../agile/use-scrum-in-an-agile-team/iterations/iterations-overview.md).

## Voorkeuren voor projecten, taken en uitgaven groeperen

Zoals we eerder hebben meegedeeld, hebben we aanpassingen op groepsniveau voor project, taak en voorkeuren voor uitgaven geïmplementeerd in fasen die lopen tot 24 juni 2021. Nu is de rollout volledig en zijn zij beschikbaar in Productie voor alle klanten.

Raadpleeg de volgende artikelen voor meer informatie:

* [ vorm projectvoorkeur voor een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
* [Taak- en uitgavevoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

## Externe gebruikers toestaan een document goed te keuren

>[!NOTE]
>
>Deze functie is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring.

U kunt nu externe e-mailadressen gebruiken om fiatteurs toe te wijzen aan een document in de nieuwe Workfront-ervaring.

Eerder kon u alleen externe gebruikers via e-mailadres toevoegen in Workfront Classic.

Voor meer informatie, zie [ het documentgoedkeuringen van het Verzoek ](../../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Informatie exporteren uit de sectie Details van een portfolio of programma

>[!NOTE]
>
>Deze functie is op 20 mei 2021 beschikbaar gesteld voor de voorvertoningsomgeving. Het zal op 3 juni 2021 worden vrijgegeven in de productieomgeving.

>[!NOTE]
>
>Deze functie is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring.

U kunt nu exporteren naar een .pdf-bestand in het gedeelte Details van portfolio&#39;s en programma&#39;s. Voorafgaand aan deze verbetering, kon u informatie van de sectie van Details slechts van projecten, taken en kwesties uitvoeren.

Voor informatie over het uitvoeren van douanevormen van een voorwerp, zie [ de douanevormen van de Uitvoer en objecten details ](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Tijdstempel Geplande Voltooiingsdatum toegevoegd in koptekst van object

>[!NOTE]
>
>Deze functie is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring.

Om gemakkelijke toegang, gemak en nauwkeurigheid te vergemakkelijken, hebben wij de optie toegevoegd om een timestamp in de Geplande Datum van Voltooiing van de kopbal van projecten, taken, of kwesties te selecteren.

Vóór deze verbetering, toen u de Geplande Datum van Voltooiing van een voorwerp bijwerkte, selecteerde Workfront middernacht als standaardtijd. Nu kunt u zowel de tijd als de voltooiingsdatum aanpassen.

Voor informatie over de objecten kopballen in de nieuwe ervaring van Workfront, zie [ Nieuwe objecten kopballen ](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

## Een aangepast formulier aan een object toevoegen zonder het te bewerken

>[!NOTE]
>
>Deze functie is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring.

We hebben het eenvoudiger gemaakt om een aangepast formulier toe te voegen dat iemand anders invult (of dat u later invult) aan een object. Het formulier wordt niet meer automatisch in de bewerkingsmodus geactiveerd wanneer u het toevoegt. U kunt het lege formulier gewoon opslaan in het object.

Eerder, toen u een aangepast formulier aan een object toevoegde, ging de pagina naar de bewerkingsmodus en moest u alle vereiste velden op het formulier invullen voordat u het naar het object kon opslaan. Dit was lastig toen het formulier bestemd was om door een andere gebruiker te worden ingevuld, of wanneer u nog niet wist wat u een vereist veld op het formulier moest plaatsen.

Voor informatie over het toevoegen van een douanevorm aan een voorwerp, zie [ een douanevorm aan een voorwerp ](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toevoegen.

