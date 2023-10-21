---
content-type: overview
product-area: projects
navigation-topic: approvals
title: Overzicht van goedkeuringsproces
description: U kunt een goedkeuringsproces tot stand brengen en het vastmaken aan een voorwerp om ervoor te zorgen dat de aangewezen gebruikers bepaalde veranderingen alvorens het voorwerp vordert herzien.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '1747'
ht-degree: 0%

---

# Overzicht van goedkeuringsproces

U kunt een goedkeuringsproces tot stand brengen en het vastmaken aan een voorwerp om ervoor te zorgen dat de aangewezen gebruikers bepaalde veranderingen alvorens het voorwerp vordert herzien.

Dit is beschikbaar voor de volgende typen objecten in Adobe Workfront:

* Werkitem (project, taak of uitgave, sjabloon, sjabloontaak)
* Document
* Proef

Voor instructies over het maken van een goedkeuringsproces raadpleegt u [Een goedkeuringsproces voor werkitems maken](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Dit artikel bevat algemene informatie over goedkeuringsprocessen die bij werkitems horen.

## Typen goedkeuringsprocedures

Als u een beheerder van Adobe Workfront, of een gebruiker met administratieve toegang tot goedkeuringsprocessen bent, kunt u de volgende goedkeuringsprocessen voor projecten, taken, en kwesties tot stand brengen:

* **Een algemeen goedkeuringsproces op systeemniveau**: Gebruikers kunnen deze koppelen aan:

   * Een project, taak, of kwestie in de sectie van Goedkeuringen
   * In het Edit vakje van het Project, het gebied van het Proces van de Goedkeuring van de Standaard van de Taak
   * In de sectie van de Details van de Rij of van het Onderwerp van de Rij van een project, in de gebieden van het Proces van de StandaardGoedkeuring. Het project moet als verzoekrij worden toegelaten.

* **Een algemeen goedkeuringsproces op groepsniveau**: Gebruikers kunnen deze aan het volgende koppelen:

   * Een project, taak of kwestie die tot de groep behoort die met het goedkeuringsproces in de sectie van Goedkeuringen wordt geassocieerd
   * In het Edit vakje van het Project, het gebied van het Proces van de Goedkeuring van de Standaard van de Taak voor een project dat tot de groep behoort verbonden aan het goedkeuringsproces
   * In de sectie van de Details van de Rij of van het Onderwerp van de Rij van een project, in de gebieden van het Proces van de StandaardGoedkeuring. Het project moet als verzoekrij worden toegelaten en moet tot de groep behoren verbonden aan het goedkeuringsproces.

  Voor informatie over het maken van goedkeuringsproces op systeemniveau of op groepsniveau raadpleegt u [Een goedkeuringsproces voor werkitems maken](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **Een goedkeuringsproces voor eenmalig gebruik**: Voor gebruik met één project, taak, kwestie, malplaatje, of malplaatjetaak. Dit type goedkeuringsproces is alleen van invloed op het object dat eraan is gekoppeld en dat niet beschikbaar is om aan andere objecten te worden gekoppeld.

  Voor informatie over het creëren van een goedkeuringsproces voor eenmalig gebruik, zie [Een nieuw of bestaand goedkeuringsproces koppelen aan werk](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>In dit artikel wordt de term &quot;wereldwijd goedkeuringsproces&quot; gebruikt om een onderscheid te maken tussen &quot;goedkeuringsproces voor eenmalig gebruik&quot;. Een algemeen goedkeuringsproces kan herhaaldelijk worden gebruikt.
>
>De term &quot;mondiaal goedkeuringsproces op groepsniveau&quot; verwijst naar een goedkeuringsproces dat herhaaldelijk kan worden gebruikt voor artikelen en statussen die alleen aan een specifieke groep zijn gekoppeld.

Voor informatie over het creëren van een goedkeuringsproces op systeemniveau of een goedkeuringsproces op groepsniveau raadpleegt u [Een goedkeuringsproces voor werkitems maken](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Overwegingen over goedkeuringsprocedures

* U moet het project, de taak, de kwestie, het malplaatje, of de malplaatjetaak tot stand brengen alvorens het goedkeuringsproces met hen kan worden geassocieerd.
* Een goedkeuringsproces hangt altijd samen met twee essentiële zaken:

   * Elk goedkeuringsproces komt overeen met een bepaalde status van een tijdelijk onderdeel in het Workfront-systeem. Wanneer u de status van een tijdelijk onderdeel wijzigt, moet een bijgevoegde goedkeuring voor die status de statuswijziging bevestigen voordat de nieuwe status aan het onderdeel kan worden toegewezen.

     >[!TIP]
     >
     >
     >   
     >   
     >   * U kunt een goedkeuring op groepsniveau koppelen aan een status op globaal niveau of op groepsniveau.
     >   * U kunt de status van een onderdeel dat een goedkeuringsproces gebruikt, niet wijzigen in een andere status dan de status die is gekoppeld aan het goedkeuringsproces.
     >   
     >   
     >     Bijvoorbeeld, als u een taakgoedkeuring verbonden aan het statuut van Bezig hebt, verandert de taak automatisch zijn status in Bezig wanneer de goedkeuring wordt verleend. De status kan niet automatisch worden gewijzigd in Voltooid of in een andere status die niet aan de goedkeuring is gekoppeld.
     >   
     >   
     >

   * De entiteiten die aan een goedkeuringsproces worden geassocieerd kunnen gebruikers, baanrollen, of teams zijn. De gebruikers zijn uiteindelijk verantwoordelijk voor het goedkeuren of verwerpen van de goedkeuring. U kunt goedkeuringen toewijzen aan gebruikers die een bepaalde rol in het project vervullen. U kunt bijvoorbeeld een goedkeuring toewijzen aan een projecteigenaar of sponsor. Zie voor meer informatie [Een goedkeuringsproces voor werkitems maken](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

     De volgende scenario&#39;s bestaan:

      * Wanneer u een goedkeuring aan baanrollen toewijst, kan om het even welke gebruiker op het Team van het Project die met de baanrol wordt geassocieerd een besluit over de goedkeuring nemen. De aan de goedkeuring gekoppelde rol kan hun primaire rol of een andere rol zijn.

        Voor informatie over het Team van het Project, zie [Overzicht van het projectteam](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * Wanneer u een goedkeuring aan een team toewijst, kan om het even welk lid van dat team een besluit over de goedkeuring nemen. Het team verbonden aan de goedkeuring kan of hun Team van het Huis of om het even welk van hun Andere Teams zijn.

        Voor informatie over de rollen en de teams van een gebruiker, zie [Gebruikersprofiel bewerken](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Wanneer u een het werkpunt creeert, heeft het automatisch geen goedkeuringsproces in bijlage. U moet er handmatig een koppelen als u er een wilt gebruiken. Voor informatie over het bijvoegen van een goedkeuringsproces aan een punt, zie [Een nieuw of bestaand goedkeuringsproces koppelen aan werk](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* De beheerder van Workfront of een gebruiker met administratieve toegang tot goedkeuringsprocessen kunnen een systeem-vlakke globale goedkeuringsprocessen voor gebruik door het systeem tot stand brengen. Een groepsbeheerder met administratieve toegang tot goedkeuringsprocessen kan een globaal goedkeuringsproces op groepsniveau tot stand brengen voor gebruik slechts door een bepaalde groep die zij beheren.
* Als u geen vooraf bepaald systeem-niveau of groep-vlakke globaal goedkeuringsproces voor een het werkpunt wilt gebruiken, kunt u een enig-gebruiks goedkeuringsproces tot stand brengen en vastmaken aan het wanneer u beheertoestemmingen aan het voorwerp hebt waarvoor u het goedkeuringsproces wilt vastmaken.

  >[!NOTE]
  >
  U kunt een goedkeuringsproces voor eenmalig gebruik slechts eenmaal gebruiken voor het specifieke item waarvoor het is gemaakt. U kunt globale statussen evenals groep-vlakke statussen voor enig-gebruiksgoedkeuringsprocessen voor projecten, taken, kwesties, malplaatjes, en malplaatjetaken associëren.

* Wanneer het vastmaken van een goedkeuringsproces op groepsniveau aan een punt gebruikend groep-vlakke douanestatus, zou het veranderen van de Groep van het project een conflict tussen de goedkeuringsstatussen van de vorige groep en die op het systeemniveau kunnen tot stand brengen. U kunt overwegen de goedkeuringsprocessen op groepsniveau voor het project of de taken of problemen ervan te verwijderen voordat u de groep bijwerkt. Voor informatie over het creëren van groep-vlakke goedkeuringsprocessen, zie [Goedkeuringsprocessen op groepsniveau](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). Zie voor informatie over het maken van aangepaste groepsstatussen [Een groepsstatus maken of bewerken](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). Voor informatie over het bijwerken van de Groep van een project, zie [Projecten bewerken](../../manage-work/projects/manage-projects/edit-projects.md).

## De goedkeuringswerkstroom

In deze sectie wordt het volgende uitgelegd over het goedkeuren van werkitems:

* [Hoe goedkeuringsprocessen op statussen vertrouwen](#how-approval-processes-rely-on-statuses)
* [Hoe een typische werkstroom een goedkeuringsproces gebruikt](#how-a-typical-workflow-uses-an-approval-process)

### Hoe goedkeuringsprocessen op statussen vertrouwen {#how-approval-processes-rely-on-statuses}

Als u een status aan een goedkeuringsproces koppelt, zorgt u ervoor dat het onderdeel in de juiste volgorde door de afdelingen wordt geleid.

**Voorbeeld:** U zou een goedkeuringsproces aan de status van de Afdeling van de Marketing kunnen vastmaken die goedkeuring door de afdeling van de Financiën vereist. Dan, wanneer iemand de status voor een het werkpunt in &quot;de Afdeling van de Marketing verandert,&quot;kan het punt niet naar die afdeling bewegen tot de afdeling van de Financiën weg op het ondertekent.

Raadpleeg de volgende artikelen voor meer informatie over statussen van werkitems:

* [Heb toegang tot de lijst van de statussen van het systeemproject](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [De lijst met taakstatussen van het systeem openen](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [Toegang krijgen tot de lijst met systeemuitgiftestatussen](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### Hoe een typische werkstroom een goedkeuringsproces gebruikt {#how-a-typical-workflow-uses-an-approval-process}

In het volgende scenario ziet u hoe gebruikers met een goedkeuringsproces hun werk kunnen goedkeuren terwijl een Workfront-object een workflow doorloopt met verschillende stappen in deze volgorde:

1. De beheerder van Workfront of een gebruiker met administratieve toegang tot de Processen van de Goedkeuring leidt tot een goedkeuringsproces voor een project, een taak, of een kwestie.

   >[!NOTE]
   >
   U kunt processen van de projectgoedkeuring aan een malplaatje, en de processen van de taakgoedkeuring aan een malplaatjetaak vastmaken. Nadat u dit doet, wanneer iemand het malplaatje gebruikt om een project tot stand te brengen, wordt het goedkeuringsproces een project of taakgoedkeuringsproces respectievelijk. Een goedkeuringsproces voor eenmalig gebruik dat aan een sjabloon of sjabloontaak is gekoppeld, blijft een goedkeuringsproces voor projecten en taken voor eenmalig gebruik.

1. Een gebruiker met de machtiging Beheren voor het project, de taak of de uitgave koppelt het goedkeuringsproces aan het onderdeel of maakt een goedkeuring voor één gebruik voor het onderdeel.
1. Een gebruiker die aan het het werkpunt wordt toegewezen verandert zijn status in de status die het goedkeuringsproces in werking stelt en het goedkeuringsproces begint. (De persoon die het goedkeuringsproces tot stand bracht bepaalde het verband tussen de status en het goedkeuringsproces.)
1. De aangewezen fiatteurs ontvangen een melding over het goedkeuringsproces in behandeling en beoordelen het werkitem.
1. Het goedkeuringsproces eindigt nadat de aangewezen fiatteurs alle stappen van het proces goedkeuren. Of als ze een stap afwijzen, wordt de status teruggezet naar een vooraf gedefinieerde status of wordt een uitgave gemaakt. (De persoon die het goedkeuringsproces creeerde bepaalde welke van deze geautomatiseerde stappen na een verwerping gebeuren.)

**Voorbeeld:** Een advertentieteam heeft een status met de naam Ready for Printing en een goedkeuringsproces met de naam Designer/Copywriter Signoff gemaakt die aan deze status zijn gekoppeld. Dit goedkeuringsproces wordt gevormd om:

* Goedkeuring door de ontwerper en copywriter van het team vereisen
* Wordt gestart wanneer iemand de status van een tijdelijk item wijzigt in Gereed voor afdrukken

Een eigenaar van een brochure-project koppelt het goedkeuringsproces voor Designer/Copywriter Signoff aan het brochure-project.

Wanneer iemand in het project de status in Ready for Printing wijzigt, ontvangen de copywriter en de ontwerper meldingen met het verzoek deze goed te keuren of af te wijzen. Tijdens het goedkeuringsproces, wanneer zij of om het goed te keuren of niet bespreken, toont de status van de projecten klaar voor Druk - in afwachting van Goedkeuring.

Nadat beide gebruikers de brochure in Workfront hebben goedgekeurd, verandert de projectstatus in Ready for Printing.

## Goedkeuringsprocedures voor documenten

Goedkeuringen van documenten worden gebruikt voor een meer algemene goedkeuring. Feedback wordt vastgelegd in chatindeling op het tabblad Updates. Met de goedkeuringsknoppen kunt u wijzigingen goedkeuren, afwijzen of goedkeuren.

Als u fiatteurs aan een document wilt toevoegen nadat het naar Workfront is geüpload, raadpleegt u [Documentgoedkeuring aanvragen](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Proefgoedkeuringsprocedures

Goedkeuringen van proefdrukken worden gebruikt voor een diepgaandere revisie en omvatten over het algemeen meer complexe workflows. Feedback wordt vastgelegd met opmaakgereedschappen in de proefdrukviewer. Met de goedkeuringsknoppen kunt u wijzigingen goedkeuren, afwijzen of goedkeuren.

Als u een geautomatiseerde workflow wilt toevoegen aan een proefdruk van een document en bepaalde gebruikers in de workflow wilt toewijzen als fiatteurs van de proefdruk, raadpleegt u [Een geavanceerde proefdruk maken met een geautomatiseerde workflow](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Instellingen configureren voor goedkeuringsprocessen voor werkitems

Als beheerder van Workfront, kunt u globale montages voor werk-punt goedkeuringsprocessen in uw systeem vormen. Deze instellingen bepalen verschillende regels voor goedkeuringsprocessen, zoals hoe lang een goedkeuringsbesluit open moet blijven of hoe u de delegatie van goedkeuring in uw systeem beheert. Zie voor meer informatie over instellingen voor goedkeuringsproces [Algemene goedkeuringsinstellingen configureren](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).
