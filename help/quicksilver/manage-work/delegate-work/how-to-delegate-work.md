---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: Taken en problemen delegeren
description: U kunt het werk tijdelijk delegeren u aan wordt toegewezen terwijl u uit het bureau bent. In dit artikel wordt beschreven hoe taken kunnen worden gedelegeerd en hoe taken kunnen worden uitgegeven.
author: Lisa
feature: Work Management
exl-id: 42b3112f-4f39-4078-aaa0-623559384a12
source-git-commit: 49bd393af77a67aa1e3a443c4189569178e99ada
workflow-type: tm+mt
source-wordcount: '1407'
ht-degree: 0%

---

# Taak beheren en taken delegeren

<!-- Audited: 1/2024 -->


<!--
<NOTE: 
<you might need to change the tile to Delegate PTI, etc, when that functionality is added. Named it this so it will not conflict with the TOC article for Delegate section which was also "Delegate work"
I wrote this as a "Manage..." article and I did not add three separate articles, to match what we have for delegating approval requests)
-->

U kunt het werk tijdelijk delegeren u aan wordt toegewezen terwijl u uit het bureau bent.

U kunt taken delegeren en taken uitgeven, of u kunt goedkeuringen delegeren. In dit artikel wordt beschreven hoe taken kunnen worden gedelegeerd en hoe taken kunnen worden uitgegeven.

Voor algemene informatie over het delegeren van het werk, zie [ het werkoverzicht van de Afgevaardigde ](../../manage-work/delegate-work/delegate-work-overview.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

>[!IMPORTANT]
>
>* De gebruikers die u als afgevaardigden selecteert, ontvangen de zelfde toestemmingen zoals uw toestemmingen op de taken en de kwesties u aan hen delegeert.
>* De toestemmingen moeten binnen hun toegangsniveaus werken, en soms zouden hun toegangsniveaus lager kunnen zijn dan van u.
>
>   
>   Bijvoorbeeld, als een gebruiker slechts de toegang van de Mening tot taken op hun toegangsniveau heeft en u hebt leiden toestemmingen op de taken u aan hen delegeert, ontvangen zij leiden toestemmingen aan de taken u aan hen delegeert. Ze kunnen echter niet dezelfde handelingen uitvoeren als u met betrekking tot gedelegeerde taken. Om taken in uw afwezigheid bij te werken, moeten zij Edit toegang tot Taken van de systeembeheerder verzoeken.
>
>   
>   Voor informatie over hoe een systeembeheerder uw toegangsniveau kan wijzigen, zie [ tot douanetoegangsniveaus ](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.
>
>* Voor punten die worden toegewezen nadat de delegatie reeds is begonnen, kan het tot één uur nadat het punt voor [!DNL Workfront] werd toegewezen duren om de onlangs-toegewezen punten met de afgevaardigde te delen.


U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td> <p>Nieuw: Medewerker of hoger</p><p>of</p><p>Huidig: Controleren of hoger</p>

>[!NOTE]
>
>Hoewel u aan het werk kunt worden toegewezen wanneer u een vergunning van het Verzoek hebt, kunt u uw werk niet aan anderen delegeren. [!DNL Workfront] raadt niet aan werk toe te wijzen aan gebruikers van Reviseren, aanvragen of Medewerkers.

</tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken en problemen bewerken 
     </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening of hoger aan de taken of de kwesties die u aan wordt toegewezen</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## Vereisten

Voordat u de in dit artikel beschreven activiteiten kunt uitvoeren, moet u het volgende controleren:

* De [!DNL Workfront] - of groepsbeheerder heeft de instelling [!UICONTROL Allow users to delete tasks & issues with logged hours] ingeschakeld in het [!UICONTROL Setup] -gebied van de [!DNL Workfront] -instantie.

  Voor meer informatie, zie [ taak voor het hele systeem vormen en voorkeur uitgeven ](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Taken en problemen delegeren aan een andere gebruiker

Alvorens het werk aan anderen te delegeren, adviseren wij dat u hen bereikt en hen op de hoogte brengt dat zij als afgevaardigden op uw het werkpunten zullen worden aangewezen. Vraag om hun mondelinge goedkeuring alvorens werk te delegeren om ervoor te zorgen zij de tijd nodig hebben om het werk te voltooien terwijl u uit het bureau bent.

Voor algemene informatie over het delegeren van taken en kwesties, zie [ de taken en kwesties van de Afgevaardigde overzicht ](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

Uw taken en problemen delegeren aan anderen:

1. Ga naar het [!UICONTROL **Begin**] gebied, dan klik [!UICONTROL **Afgevaardigde**] bij de bovenkant van de [!UICONTROL **Lijst van het Werk**].

   ![](assets/delegate-button-in-home.png)

1. In [!UICONTROL **de taken en de kwesties van de Afgevaardigde**] tabel, werk het volgende bij:

   * [!UICONTROL **delegeer uw taken en kwesties aan**]: Begin typend de naam van een gebruiker die u uw taken en kwesties wilt worden gedelegeerd aan, dan het selecteren wanneer het in de lijst toont. U kunt slechts één gebruiker selecteren.

     De gebruiker die u als afgevaardigde selecteert ontvangt de zelfde toestemmingen zoals uw toestemmingen op de taken en de kwesties u aan hen delegeert.

   * [!UICONTROL **datum van het Begin**]: Selecteer een datum van de kalender wanneer de delegatie van uw het werkpunten zou moeten beginnen.

     >[!TIP]
     >
     >De begindatum kan niet in het verleden zijn.

   * [!UICONTROL **Geen einddatum**]: Selecteer deze optie als u niet de einddatum voor uw delegatie wilt specificeren.

   * [!UICONTROL **einddatum**]: Selecteer een datum van de kalender wanneer de delegatie zou moeten ophouden.

     >[!TIP]
     >
     >Als u het veld Einddatum leeg laat en de optie Geen einddatum is niet geselecteerd, wordt de delegatie alleen voor de huidige dag ingesteld.

     ![](assets/delegate-box-expanded-in-home.png)

1. Klik [!UICONTROL **sparen**].

   De volgende dingen gebeuren:

   * Uw werk wordt gedelegeerd aan de opgegeven gebruiker. Eventuele onvolledige taken of problemen die datums hebben binnen de door u geselecteerde tijd (inclusief de nieuw toegewezen taken nadat de delegatie is ingeschakeld) worden gedelegeerd.

     >[!TIP]
     >
     >   Voltooide werkitems met datums binnen de tijdsperiode van de delegatie worden niet gedelegeerd.


   * U ontvangt een bericht in de hoger-juiste hoek van het scherm om te bevestigen dat u de delegatie van uw werk aan een andere gebruiker hebt toegelaten. De naam van de afgevaardigde gebruiker toont in het bevestigingsbericht.

   * Een indicatie dat uw taken en problemen zijn gedelegeerd aan andere gebruikers, wordt weergegeven in de meeste gebieden waar u toewijzingen kunt zien in [!DNL Workfront] . Voor meer informatie over welke gebieden de namen van afgevaardigden niet omvatten, zie [ het werkoverzicht van de Afgevaardigde ](delegate-work-overview.md).

   * De [!UICONTROL **Afgevaardigde**] knoop in het [!UICONTROL Home] gebied verandert in [!UICONTROL **uitgeeft delegatie**] om erop te wijzen dat er een delegatie op zijn plaats is.
   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
   </MadCap:conditionalText>
   -->

   ![](assets/work-delegated-button-in-home.png)

   * Als uw gebeurtenismeldingen en uw persoonlijke meldingen zijn ingeschakeld, ontvangt u ook een e-mailbevestiging van uw delegatie.

   * De gebruiker u als uw afgevaardigde selecteerde ontvangt een e-mail over de delegatie, als hun gebeurtenisberichten worden toegelaten.

     Voor informatie over het toelaten van persoonlijke e-mailberichten, zie [ uw eigen e-mailberichten wijzigen ](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Delegatie bewerken of stoppen

U kunt een delegatie laten verlopen, als u een Einddatum selecteerde, of u kunt het manueel tegenhouden. U kunt ook het tijdkader voor de delegatie wijzigen als de datums voor de delegatie zijn gewijzigd.

1. Ga naar het [!UICONTROL Home] -gebied en klik vervolgens op [!UICONTROL Edit delegation] in de rechterbovenhoek van de werklijst.
1. Voer op het tabblad [!UICONTROL Delegate tasks and issues] een van de volgende handelingen uit:
   * Wijzig de [!UICONTROL **datum van het Begin**] of de [!UICONTROL **datum van het Eind**]
   * Klik [!UICONTROL **delegatie van het Einde**]

   >[!TIP]
   >
   >    U kunt alleen de einddatum van een delegatie bewerken als de delegatie al is gestart.

   ![](assets/stop-delegation-screen-in-home.png)

1. (Voorwaardelijk) klik [!UICONTROL **sparen**] om de nieuwe delegatiedata te bewaren

   of

   Klik [!UICONTROL **delegatie van het Einde**] in de bevestigingsdoos om het tegenhouden van de delegatie te bevestigen.

   De delegatie heeft de datums bijgewerkt of is gestopt en de gedelegeerde gebruikers zijn uit uw taken en problemen verwijderd. Hun machtigingen voor de taken en problemen blijven bestaan.


## Zoeken naar gedelegeerde werkzaamheden en gedelegeerde gegevens

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

Wanneer taken en kwesties worden gedelegeerd, zijn er verscheidene gebieden in [!DNL Workfront] waar u het gedelegeerde werk kunt zien of wie de afgevaardigden zijn.

* [Delegaties zoeken in het vak Toewijzingen](#locate-delegates-in-the-assignments-box)
* [Gedelegeerde werkzaamheden zoeken in [!UICONTROL Home]](#locate-delegated-work-in-home)


### Delegaties zoeken in het vak [!UICONTROL Assignments]

Wanneer uw systeem of groepsbeheerder werkdelegatie in uw systeem toelaat, [!UICONTROL Assignments] toont de doos de volgende lusjes overal u tot het kunt toegang hebben:

* [!UICONTROL **Toewijzingen**]: De gebruikers die aan de taak of de vertoningskwestie hier worden toegewezen.
* [!UICONTROL **Delegaties**]: De gebruikers die als afgevaardigden door de wijzers op de taak worden aangewezen of hier vertoning van de kwestie.

U kunt het vak [!UICONTROL Assignments] openen in de volgende gebieden:

* De taak- of uitgiftekop

  Het veld [!UICONTROL Assignments] in de taak- of uitgiftekop verandert in [!UICONTROL Assignments and delegations] .

  ![](assets/assignments-and-delegates-panel-in-task-header.png)

* De [!UICONTROL Workload Balancer] bij het handmatig toewijzen van taken of uitgaven

  ![](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> U kunt afgevaardigden niet weergeven in de [!UICONTROL Assignments] -sectie van een taak of in het bewerkvak voor uitgaven.

Als een taak of een kwestie wordt gedelegeerd en subtab [!UICONTROL Delegations] leeg is, kan een van de volgende scenario&#39;s bestaan:

* U bent niet toegewezen aan de taak of uitgave.
* De taak of de uitgiftedata zijn buiten het tijdkader van de delegatie.

>[!TIP]
>
>De geplande of Werkelijke Uren voor gedelegeerde taken en kwesties worden niet in hulpmiddelen van het middelbeheer, zoals [!UICONTROL Workload Balancer] of [!DNL Resource Planner] voor de gedelegeerde gebruikers in aanmerking genomen. De uren blijven alleen gekoppeld aan de toegewezen gebruiker.

### Gedelegeerde werkzaamheden zoeken in [!UICONTROL Home]

1. Ga naar het [!UICONTROL **Begin**] gebied, dan klik het filter drop-down menu en selecteer één of meerdere van de volgende opties:
   * [!UICONTROL **Gedelegeerde**]: aan meningstaken en kwesties die aan u of door u worden gedelegeerd.
   * [!UICONTROL ****] Gedelegeerde aan me: aan meningstaken en kwesties die aan u door een andere gebruiker worden gedelegeerd.
   * [!UICONTROL **Gedelegeerde door me**]: aan meningstaken en kwesties die door u aan andere gebruikers worden gedelegeerd.

   ![](assets/delegated-to-me-or-by-me-filters-in-home.png)

1. Klik op het vervolgkeuzemenu [!UICONTROL sorting] om de lijst op de volgende criteria te sorteren:
   * [!UICONTROL Planned Completion]. Dit is de standaardoptie voor sorteren.
   * [!UICONTROL Planned Start]
   * [!UICONTROL Commit Date]
   * [!UICONTROL Project]
   * [!UICONTROL My Priority]
1. Breid de groeperingen in de [!UICONTROL **Lijst van het Werk**] uit om gedelegeerde het werkpunten te bekijken. De volgende scenario&#39;s bestaan:
   * Voor punten die u aan anderen delegeerde, toont de naam van de afgevaardigde in de [!UICONTROL **Lijst van het Werk**] evenals het [!UICONTROL **Toewijzingen en delegaties**] gebied op het recht.

   * Voor punten aan u worden afgevaardigd, toont de naam van de ontvanger in de [!UICONTROL **Lijst van het Werk**] evenals het **[!UICONTROL Assignments and delegations]** gebied op het recht dat.

   >[!TIP]
   >
   >    Als de delegatie op een datum na de datum van vandaag moet beginnen, de begindatum van de delegatie ook in [!UICONTROL Work List] toont. De gedelegeerde items worden weergegeven in de groep die u selecteert voor de [!UICONTROL Work List] , afhankelijk van het type van de groep. Als u bijvoorbeeld groepeert op [!UICONTROL Planned Completion Date] , worden de gedelegeerde items weergegeven in de groep die overeenkomt met de geplande voltooiingsdatums.
