---
product-area: projects
navigation-topic: approvals
title: Goedkeuringsaanvraag delegeren
description: Het delegeren van goedkeuringsverzoeken staat u toe om een andere gebruiker toe te wijzen om uw verzoeken voor een periode goed te keuren, bijvoorbeeld, als u uit het bureau op vakantie zult zijn.
author: Courtney
feature: Work Management
exl-id: 01b76dd5-98cb-4f0d-97ff-7e665f843a9c
source-git-commit: d04afc0cc55a71e48c357af2ed4446c22dab1ba4
workflow-type: tm+mt
source-wordcount: '1203'
ht-degree: 0%

---

# Goedkeuringsaanvraag delegeren

U kunt het werk tijdelijk delegeren u aan wordt toegewezen terwijl u uit het bureau bent. U kunt taken delegeren en taken uitgeven of u kunt goedkeuringsverzoeken delegeren. Dit artikel beschrijft hoe te om goedkeuringsverzoeken te delegeren. Voor informatie over het delegeren van taak en uitgiftetaken, zie [Taak beheren en taken delegeren](../../manage-work/delegate-work/how-to-delegate-work.md).

>[!NOTE]
>
>Om ervoor te zorgen dat geen inconsistenties met de data voorkomen die u voor uw goedkeuringen plant om worden afgevaardigd, adviseren wij dat de tijdzone van uw gebruikersprofiel dat van uw programma aanpast. Raadpleeg de volgende artikelen voor meer informatie:
>
>* [Een schema maken](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Gebruikersprofiel bewerken](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>


## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-abonnement*</p></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td> <p>Controleren of hoger</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement of licentietype u hebt.

## Gebruikerstoegang voor gedelegeerde goedkeuringen begrijpen

Tijdens de aangewezen goedkeuringsperiode, heeft de gebruiker aan wie u een goedkeuringsverzoek delegeert de volgende capaciteiten:

* Bestaande goedkeuringsaanvragen goedkeuren of afwijzen als er geen besluit is genomen
* Kan nieuwe goedkeuringsaanvragen goedkeuren en afwijzen die gedurende een bepaalde periode zijn ontvangen
* Hiermee krijgt u toegang tot objecten die nog moeten worden goedgekeurd

   >[!NOTE]
   >
   > De Adobe Workfront-beheerder kan gebruikers toegang tot bepaalde objecttypen ontzeggen. Wanneer een gebruiker geen toegang tot een objecttype heeft en een goedkeuring van dat type aan de gebruiker wordt gedelegeerd, heeft de gebruiker geen toegang tot het object weergeven. De gebruiker kan echter nog steeds goedkeuringsaanvragen van de **Home** pagina, zoals beschreven in [Goedkeuring van de werkzaamheden](../../review-and-approve-work/manage-approvals/approving-work.md).\
   Bijvoorbeeld, behoort de Gebruiker A tot Groep A. De Workfront-beheerder heeft de toegangsrechten van groep A beperkt, zodat gebruikers in deze groep geen taken in Workfront kunnen weergeven. Als een verzoek van de taakgoedkeuring aan Gebruiker A wordt gedelegeerd, kan Gebruiker A niet de taak bekijken die de goedkeuring met wordt geassocieerd. Nochtans, kan Gebruiker A het goedkeuringsverzoek van de Homepage goedkeuren of verwerpen.

   Voor informatie over hoe de beheerder van Workfront toegang tot objecten types binnen Opstelling kan beperken, zie  [Aangepaste toegangsniveaus maken of wijzigen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 

Nadat de delegatie van de goedkeuring is gestopt of geannuleerd, heeft de gebruiker die als fiatteur is aangewezen:

* U hebt geen toegang meer tot het goedkeuren van werken voor items die goedkeuring vereisen
* Blijft toegang tot het werk van de Mening tot voorwerpen hebben\
   Gebruikers aan wie via een goedkeuringsdelegatie toegang tot objecten is verleend, behouden die toegang zelfs nadat de goedkeuringsdelegatie is gestopt of teruggeroepen. Als u toegang tot Weergave wilt verwijderen tot alle objecten waartoe de gebruiker toegang had tijdens de periode dat goedkeuringen werden gedelegeerd, moet u naar het object gaan en de toegangsrechten rechtstreeks uit het object verwijderen.

## Goedkeuringsaanvragen delegeren in het thuisgebied

* [Uw goedkeuringen delegeren aan een andere gebruiker](#delegate-your-approvals-to-another-user)
* [Een goedkeuringsdelegatie bijwerken of stoppen](#update-or-stop-an-approval-delegation)
* [Gedelegeerde goedkeuringen weergeven](#view-delegated-approvals)

### Uw goedkeuringen delegeren aan een andere gebruiker {#delegate-your-approvals-to-another-user}

U kunt de volgende typen goedkeuringen delegeren, ongeacht hoe de goedkeuring aan u is toegewezen (of deze rechtstreeks aan u zijn toegewezen, aan een team u lid van, of aan uw baanrol):

* Projectgoedkeuringen
* Taakgoedkeuringen
* Goedkeuring afgeven

U kunt geen timesheet- en documentgoedkeuringen delegeren. 

Overweeg het volgende wanneer het delegeren van goedkeuringen:

* Wanneer u goedkeuringen delegeert, worden al uw goedkeuringen gedelegeerd. U kunt individuele goedkeuringsverzoeken niet delegeren.
* U kunt goedkeuringen aan slechts één gebruiker delegeren; u kunt goedkeuringen niet aan veelvoudige gebruikers tezelfdertijd delegeren.\
   Alle goedkeuringen voor alle projecten, taken, en kwesties worden gedelegeerd aan de gebruiker die u aanwijst.
* Een maximum van 5 gebruikers kan goedkeuringen aan de zelfde gebruiker tezelfdertijd delegeren. Met andere woorden, één gebruiker kan niet tegelijkertijd worden aangewezen als tijdelijke fiatteur voor meer dan vijf gebruikers.
* De activiteit betreffende goedkeuringen toont op de Updates tabel. Systeemupdates tonen moet zijn ingeschakeld. Zowel de gebruiker die de goedkeuring delegeert als de gebruiker aan wie goedkeuringen worden gedelegeerd, ontvangt een e-mailbericht over goedkeuringsactiviteiten.

Goedkeuringen delegeren aan een andere gebruiker:

1. Klik op de knop **Home** pictogram ![](assets/home-icon-30x29.png) in de linkerbovenhoek van Adobe Workfront.

   >[!NOTE]
   Uw Workfront-beheerder kan de volgende wijzigingen aanbrengen in het pictogram Home in uw omgeving:
   * Vervang deze door een afbeelding die is aangepast om uw organisatie te illustreren. In dit geval ziet het pictogram er anders uit dan in dit artikel.
   * De gekoppelde pagina vervangen door een andere pagina. Klik in dit geval op de knop **Hoofdmenu** ![](assets/main-menu-icon.png) in de rechterbovenhoek van de pagina klikt u op **Home**.


   of

   Klik op de knop **Hoofdmenu** pictogram > **uw naam** > **Tijd uit** in het linkerdeelvenster.

1. (Optioneel en voorwaardelijk) Klik in het gebied Home op de knop **Filter** vervolgkeuzemenu en vervolgens op **Goedkeuringen**.

1. (Voorwaardelijk) Klik **Mijn goedkeuring delegeren**

   of

   Als uw systeem of groepsbeheerder de taak en de uitgiftedelegatie toeliet, klik **Delegeren** en klik vervolgens op **Goedkeuringen delegeren**.

   ![](assets/delegate-approvals-nwe.png)

1. Geef de volgende informatie op in de sectie Mijn goedkeuringen delegeren:

   * **Naam**: Typ de naam van de gebruiker aan wie u goedkeuringen wilt delegeren, en klik dan de naam wanneer het in het drop-down menu verschijnt.
   * **Begindatum**: Selecteer de datum waarop goedkeuring moet worden doorgestuurd. Het door:sturen begint om 12:00 op de datum die u selecteert.\
      De begindatum moet de huidige of toekomstige datum zijn.
   * **Einddatum**:Voer een van de volgende handelingen uit:

      * Selecteer de datum waarop goedkeuring niet meer moet worden doorgestuurd. Doorsturen eindigt om 23:59 op de datum die u selecteert.
      * Selecteren **Geen einddatum** om Workfront te configureren voor het voor onbepaalde tijd delegeren van goedkeuringen.

1. Klikken **Opslaan**.

### Een goedkeuringsdelegatie bijwerken of stoppen {#update-or-stop-an-approval-delegation}

1. Klik op de knop **Home** pictogram ![](assets/home-icon-30x29.png) in de linkerbovenhoek van Adobe Workfront.

   >[!NOTE]
   Uw Workfront-beheerder kan de volgende wijzigingen aanbrengen in het pictogram Home in uw omgeving:
   * Vervang deze door een afbeelding die is aangepast om uw organisatie te illustreren. In dit geval ziet het pictogram er anders uit dan in dit artikel.
   * De gekoppelde pagina vervangen door een andere pagina. Klik in dit geval op de knop **Hoofdmenu** ![](assets/main-menu-icon.png) in de rechterbovenhoek van de pagina klikt u op **Home**.


1. Klik op de knop **Filter** vervolgkeuzemenu en vervolgens op **Goedkeuringen**.

1. (Voorwaardelijk) Klik **Delegatie bewerken**

   of

   Als uw systeem of groepsbeheerder taak en uitgiftedelegatie heeft ingeschakeld, klikt u op **Delegatie bewerken** en klik vervolgens op **Goedkeuringen delegeren**.

1. (Voorwaardelijk) doe één van beiden van het volgende:

   * De bestaande delegatie van goedkeuring bijwerken: Wijzig de weergegeven informatie en klik op **Opslaan**.

   * Ophouden van de bestaande delegatie: Klikken **Delegatie stoppen** en klik vervolgens op **Delegatie stoppen** ter bevestiging.

      ![](assets/stop-delegation-nwe.png)

### Gedelegeerde goedkeuringen weergeven {#view-delegated-approvals}

In de werklijst kunt u alleen de volgende typen goedkeuringsdelegaties weergeven:

* Projectgoedkeuringen
* Taakgoedkeuringen
* Goedkeuring afgeven

Gedelegeerde goedkeuringen weergeven:

1. Klik op de knop **Home** pictogram ![](assets/home-icon-30x29.png) in de linkerbovenhoek van Adobe Workfront.

   >[!NOTE]
   Uw Workfront-beheerder kan de volgende wijzigingen aanbrengen in het pictogram Home in uw omgeving:
   * Vervang deze door een afbeelding die is aangepast om uw organisatie te illustreren. In dit geval ziet het pictogram er anders uit dan in dit artikel.
   * De gekoppelde pagina vervangen door een andere pagina. Klik in dit geval op de knop **Hoofdmenu** ![](assets/main-menu-icon.png) in de rechterbovenhoek van de pagina klikt u op **Home**.


1. Klik op de knop **Filter** vervolgkeuzemenu en vervolgens op **Goedkeuringen**.\
   Alle goedkeuringen worden standaard in de lijst weergegeven, inclusief goedkeuringen die aan u zijn toegewezen en goedkeuringen die aan u zijn gedelegeerd.

   ![](assets/delegated-to-me-nwe-350x93.png)
