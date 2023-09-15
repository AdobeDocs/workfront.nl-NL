---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: Taken en problemen delegeren
description: U kunt het werk tijdelijk delegeren u aan wordt toegewezen terwijl u uit het bureau bent. In dit artikel wordt beschreven hoe taken kunnen worden gedelegeerd en hoe taken kunnen worden uitgegeven.
author: Alina
feature: Work Management
exl-id: 42b3112f-4f39-4078-aaa0-623559384a12
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1432'
ht-degree: 0%

---

# Taak beheren en taken delegeren

<!--
<NOTE: 
<you might need to change the tile to Delegate PTI, etc, when that functionality is added. Named it this so it will not conflict with the TOC article for Delegate section which was also "Delegate work"
I wrote thhis as a "Manage..." article and I did not add three separate articles, to match what we have for delegating approval requests)
-->

U kunt het werk tijdelijk delegeren u aan wordt toegewezen terwijl u uit het bureau bent.

U kunt taken delegeren en taken uitgeven of u kunt goedkeuringen delegeren. In dit artikel wordt beschreven hoe taken kunnen worden gedelegeerd en hoe taken kunnen worden uitgegeven.

Voor algemene informatie over het delegeren van werk, zie [Overzicht van werkzaamheden delegeren](../../manage-work/delegate-work/delegate-work-overview.md).

## Toegangsvereisten

>[!IMPORTANT]
>
>* De gebruikers die u als afgevaardigden selecteert, ontvangen de zelfde toestemmingen zoals uw toestemmingen op de taken en de kwesties u aan hen delegeert.
>* De toestemmingen moeten binnen hun toegangsniveaus werken, en soms zouden hun toegangsniveaus lager kunnen zijn dan van u.
>
>   
>   Bijvoorbeeld, als een gebruiker slechts de toegang van de Mening tot taken op hun toegangsniveau heeft en u hebt leiden toestemmingen op de taken u aan hen delegeert, ontvangen zij leiden toestemmingen aan de taken u aan hen delegeert. Ze kunnen echter niet dezelfde handelingen uitvoeren als u met betrekking tot gedelegeerde taken. Zij moeten om Edit toegang tot Taken van de systeembeheerder verzoeken om taken in uw afwezigheid bij te werken.
>
>   
>   Voor informatie over hoe een kan uw toegangsniveau wijzigen, zie [Aangepaste toegangsniveaus maken of wijzigen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
>
>* Voor punten die na de delegatie reeds begonnen worden toegewezen, kan het tot één uur duren nadat het punt werd toegewezen voor [!DNL Workfront] om de onlangs-toegewezen punten met de afgevaardigde te delen.


U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>Controleren of hoger</p>

>[!NOTE]
>
>Hoewel u aan het werk kunt worden toegewezen wanneer u een vergunning van het Verzoek hebt, kunt u uw werk niet aan anderen delegeren. [!DNL Workfront] adviseert niet het toewijzen van werk aan het Overzicht of van het Verzoek gebruikers.

</tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Geef toegang tot Taken en Kwesties uit als u nog geen toegang hebt, vraag uw [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening of hoger aan de taken of de kwesties die u aan wordt toegewezen</p> 
    <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw [!DNL Workfront] beheerder.

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## Vereisten

Voordat u de in dit artikel beschreven activiteiten kunt uitvoeren, moet u het volgende controleren:

* Uw [!DNL Workfront] of groepsbeheerder de optie [!UICONTROL Allow users to delete tasks & issues with logged hours] in het dialoogvenster [!UICONTROL Setup] gebied van uw [!DNL Workfront] -instantie.

  Zie voor meer informatie [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Taken en problemen delegeren aan een andere gebruiker

Alvorens het werk aan anderen te delegeren, adviseren wij dat u hen bereikt en hen op de hoogte brengt dat zij als afgevaardigden op uw het werkpunten zullen worden aangewezen. Vraag om hun mondelinge goedkeuring alvorens werk te delegeren om ervoor te zorgen zij de tijd nodig hebben om het werk te voltooien terwijl u uit het bureau bent.

Voor algemene informatie over het delegeren van taken en kwesties, zie [Overzicht van taken en problemen delegeren](delegate-work.md).

Uw taken en problemen delegeren aan anderen:

1. Ga naar de [!UICONTROL **Home**] gebied, klik vervolgens op [!UICONTROL **Delegeren**] boven aan het dialoogvenster [!UICONTROL **Werklijst**].

   ![](assets/delegate-button-in-home.png)

1. In de [!UICONTROL **Taken en problemen delegeren**] kunt u het volgende bijwerken:

   * [!UICONTROL **Uw taken en problemen delegeren aan**]: Typ de naam van een gebruiker waaraan u uw taken en uitgaven wilt delegeren en selecteer deze vervolgens wanneer deze in de lijst wordt weergegeven. U kunt slechts één gebruiker selecteren.\

     De gebruiker die u als afgevaardigde selecteert ontvangt de zelfde toestemmingen zoals uw toestemmingen op de taken en de kwesties u aan hen delegeert. Zie voor meer informatie [Taak- en probleemoverzicht delegeren](delegate-work-overview.md).

   * [!UICONTROL **Begindatum**]: Selecteer een datum in de kalender waarop de delegatie van uw werkitems moet beginnen.

     >[!TIP]
     >
     >De begindatum kan niet in het verleden zijn.

   * [!UICONTROL **Geen einddatum**]: Selecteer deze optie als u de einddatum voor uw delegatie niet wilt opgeven.

   * [!UICONTROL **Einddatum**]: Selecteer een datum in het rooster waarop de delegatie moet stoppen.

     >[!TIP]
     >
     >Als u geen einddatum selecteert, wordt de delegatie alleen voor de huidige dag ingeschakeld.

     ![](assets/delegate-box-expanded-in-home.png)

1. Klikken [!UICONTROL **Opslaan**].

   De volgende dingen gebeuren:

   * Uw werk wordt gedelegeerd aan de opgegeven gebruiker. Eventuele onvolledige taken of problemen die datums hebben binnen de door u geselecteerde tijd (inclusief de nieuw toegewezen taken nadat de delegatie is ingeschakeld) worden gedelegeerd.

   >[!TIP]
   >
   >   Voltooide werkitems met datums binnen de tijdsperiode van de delegatie worden niet gedelegeerd.


   * U ontvangt een bericht in de hoger-juiste hoek van het scherm om te bevestigen dat u de delegatie van uw werk aan een andere gebruiker hebt toegelaten. De naam van de afgevaardigde gebruiker toont in het bevestigingsbericht.

   * Een aanwijzing dat uw taken en problemen zijn gedelegeerd aan andere gebruikers die op de meeste gebieden worden weergegeven waar u toewijzingen kunt zien in [!DNL Workfront]. Voor meer informatie over welke gebieden de namen van afgevaardigden niet omvatten, zie [Taak- en probleemoverzicht delegeren](delegate-work-overview.md).

   * De [!UICONTROL **Delegeren**] in de [!UICONTROL Home] gebied verandert in [!UICONTROL **Delegatie bewerken**] aan te geven dat er een delegatie bestaat .
   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
   </MadCap:conditionalText>
   -->

   ![](assets/work-delegated-button-in-home.png)

   * Als uw gebeurtenismeldingen en uw persoonlijke meldingen zijn ingeschakeld, ontvangt u ook een e-mailbevestiging van uw delegatie.

   * De gebruiker u als uw afgevaardigde selecteerde ontvangt een e-mail over de delegatie, als hun gebeurtenisberichten worden toegelaten.

     Voor informatie over het inschakelen van persoonlijke e-mailmeldingen raadpleegt u [Uw eigen e-mailmeldingen wijzigen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).




## Delegatie bewerken of stoppen

U kunt een delegatie laten verlopen, als u een Einddatum selecteerde, of u kunt het manueel tegenhouden. U kunt ook het tijdkader voor de delegatie wijzigen als de datums voor de delegatie zijn gewijzigd.

1. Ga naar de [!UICONTROL Home] gebied, klik vervolgens op [!UICONTROL Edit delegation] in de rechterbovenhoek van de werklijst.
1. In de [!UICONTROL Delegate tasks and issues] voert u een van de volgende handelingen uit:
   * Wijzig de [!UICONTROL **Begindatum**] of de [!UICONTROL **Einddatum**]
   * Klikken [!UICONTROL **Delegatie stoppen**]

   >[!TIP]
   >
   >    U kunt alleen de einddatum van een delegatie bewerken als de delegatie al is gestart.

   ![](assets/stop-delegation-screen-in-home.png)

1. (Voorwaardelijk) klik [!UICONTROL **Opslaan**] om de nieuwe delegatiedata op te slaan

   of

   Klikken [!UICONTROL **Delegatie stoppen**] in het bevestigingsvak om te bevestigen dat de delegatie wordt stopgezet.

   De delegatie heeft de datums bijgewerkt of is gestopt en de gedelegeerde gebruikers zijn uit uw taken en problemen verwijderd. Hun machtigingen voor de taken en problemen blijven bestaan.


## Zoeken naar gedelegeerde werkzaamheden en gedelegeerde gegevens

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

Wanneer taken en kwesties worden gedelegeerd, zijn er verscheidene gebieden in [!DNL Workfront] waar u het gedelegeerde werk kunt zien of wie de afgevaardigden zijn.

* [Delegaties zoeken in het vak Toewijzingen](#locate-delegates-in-the-assignments-box)
* [Gedelegeerde werkzaamheden zoeken in [!UICONTROL Home]](#locate-delegated-work-in-home)


### Delegaties zoeken in het dialoogvenster [!UICONTROL Assignments] box

Wanneer uw systeem of groepsbeheerder werkdelegatie in uw systeem toelaat, [!UICONTROL Assignments] worden de volgende tabbladen weergegeven, overal waar u toegang tot deze tabbladen hebt:

* [!UICONTROL **Toewijzingen**]: Gebruikers die hier zijn toegewezen aan de taak- of uitgifteweergave.
* [!UICONTROL **Delegaties**]: De gebruikers die door de wijzers op de taak worden aangewezen of vertoning van de kwestie hier worden aangewezen als afgevaardigden.

U hebt toegang tot [!UICONTROL Assignments] in de volgende gebieden:

* De taak- of uitgiftekop

  ![](assets/assignments-and-delegates-panel-in-task-header.png)

  De [!UICONTROL Assignments] in de taak of geeft de koptekst van de uitgave aan [!UICONTROL Assignments and delegations].

* De [!UICONTROL Workload Balancer] bij het handmatig toewijzen van taken of problemen

  ![](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> U kunt geen afgevaardigden weergeven in het dialoogvenster [!UICONTROL Assignments] sectie van een taak of uitgeeft uitgeeft vakje.

Als een taak of een kwestie wordt gedelegeerd en [!UICONTROL Delegations] subtab is leeg, kan een van de volgende scenario&#39;s bestaan:

* U bent niet toegewezen aan de taak of uitgave.
* De taak of de uitgiftedata zijn buiten het tijdkader van de delegatie.

>[!TIP]
>
>De geplande of Werkelijke Uren voor gedelegeerde taken en kwesties worden niet in de hulpmiddelen van het middelbeheer in aanmerking genomen, zoals [!UICONTROL Workload Balancer] of de [!DNL Resource Planner] voor de gedelegeerde gebruikers. De uren blijven alleen gekoppeld aan de toegewezen gebruiker.

### Gedelegeerde werkzaamheden zoeken in [!UICONTROL Home]

1. Ga naar de [!UICONTROL **Home**] klikt u op de vervolgkeuzelijst met filters en selecteert u een of meer van de volgende opties:
   * [!UICONTROL **Gedelegeerde**]: om taken en problemen te bekijken die aan u of door u zijn gedelegeerd.
   * [!UICONTROL **Aan mij gedelegeerd**]: om taken en kwesties te bekijken die aan u door een andere gebruiker worden gedelegeerd.
   * [!UICONTROL **Gedelegeerde**]: om taken en problemen weer te geven die u aan andere gebruikers hebt gedelegeerd.

   ![](assets/delegated-to-me-or-by-me-filters-in-home.png)

1. Klik op de knop [!UICONTROL sorting] vervolgkeuzelijst om de lijst op de volgende criteria te sorteren:
   * [!UICONTROL Planned Completion]. Dit is de standaardoptie voor sorteren.
   * [!UICONTROL Planned Start]
   * [!UICONTROL Commit Date]
   * [!UICONTROL Project]
   * [!UICONTROL My Priority]
1. Breid de groeperingen in uit [!UICONTROL **Werklijst**] om gedelegeerde werkitems weer te geven. De volgende scenario&#39;s bestaan:
   * Voor punten die u aan anderen delegeerde, toont de naam van de afgevaardigde in [!UICONTROL **Werklijst**] en de [!UICONTROL **Toewijzingen en delegaties**] aan de rechterkant.

   * Voor aan u gedelegeerde items wordt de naam van de ontvanger weergegeven in het dialoogvenster [!UICONTROL **Werklijst**] en de **[!UICONTROL Assignments and delegations]** aan de rechterkant.

   >[!TIP]
   >
   >    Als de delegatie op een datum na de datum van vandaag moet beginnen, wordt de begindatum van de delegatie ook weergegeven in het [!UICONTROL Work List]. De gedelegeerde items worden weergegeven in de groep die u selecteert voor de [!UICONTROL Work List], afhankelijk van het type van de groep. Als u bijvoorbeeld groepeert op [!UICONTROL Planned Completion Date], worden de gedelegeerde items weergegeven in de groep die overeenkomt met de geplande voltooiingsdatums.
