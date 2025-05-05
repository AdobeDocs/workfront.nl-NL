---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Een tijdpagina goedkeuren
description: Het proces om timesheets goed te keuren geeft managers zichtbaarheid in de werkuren van hun directe rapporten. De fiatteurs kunnen controleren of alle geregistreerde tijd in de juiste gebieden is toegewezen en of er gedurende de periode een voldoende aantal uren is geregistreerd.
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 9d0caff0381ee50bf8dd7060bebafb5354c0f0d8
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 0%

---

# Een tijdschema goedkeuren

<!--Audited: 8/2024-->

Het proces om timesheets goed te keuren geeft managers zichtbaarheid in de werkuren van hun directe rapporten. De fiatteurs kunnen controleren of alle geregistreerde tijd in de juiste gebieden is toegewezen en of er gedurende de periode een voldoende aantal uren is geregistreerd.

Adobe Workfront biedt de mogelijkheid om timesheet-goedkeuringen te configureren voor ondersteuning op dit gebied.

Voor informatie bij het voorleggen van een timesheet, zie [ een timesheet voor goedkeuring ](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md) voorleggen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-plan</p></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td> <p>Nieuw: Standaard</p>
   <p>Huidig: Plan </p> 
   <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Administratieve toegang tot timesheets en uren </p> </td> 
  </tr>

</td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Goedkeuraars voor tijdlijnen aanwijzen

Meestal worden timesheets goedgekeurd door functionele managers of personeel. Tijdschema&#39;s worden gewoonlijk niet goedgekeurd door projectmanagers. De managers van het project kunnen tijd goedkeuren die op projecten wordt geregistreerd, maar het team of de managers van het personeel zouden timesheets moeten goedkeuren.

Er wordt een fiatteur voor het tijdlijnprofiel gedefinieerd. U moet een licentie voor het abonnement hebben die u als fiatteur wilt opgeven.

Voor meer informatie over het aanwijzen van timesheet fiatteurs, zie de sectie [ creeer of geef een timesheet profiel ](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create) in artikel [ uit, geef, en wijs timesheet profielen ](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md) toe.

## Een tijdschema goedkeuren

U kunt alle tijdbladen goedkeuren die zijn verzonden waar u als fiatteur bent aangewezen. Wanneer een timesheet voor goedkeuring wordt voorgelegd, is timesheet vermeld in **Mijn goedkeurt** widget in uw **3&rbrace; gebied van het Huis.** Voor meer informatie, zie [ het goedkeuren van het werk ](../../review-and-approve-work/manage-approvals/approving-work.md).

Als de volgende meldingsinstellingen aanwezig zijn, ontvangt de gebruiker die het tijdspad ter goedkeuring indient een e-mail nadat een tijdsplaat is goedgekeurd:

* De beheerder van Workfront heeft de Goedkeuring van de Tijdopmaak aan Gebruiker en de Afwijzing van de Chronologie aan de gebeurtenismanagers van de Gebruiker toegelaten. Voor informatie over het toelaten van gebeurtenisberichten, zie [ de berichttypes van de Gebeurtenis ](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
* Mijn timesheet wordt goedgekeurd persoonlijk bericht wordt toegelaten op de de profielpagina van de gebruiker. Voor meer informatie, zie [ uw eigen e-mailberichten wijzigen ](/help/quicksilver/workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### Een tijdpagina goedkeuren vanuit het gebied Timesheets

{{step1-to-timesheets}}

Het **gebied van Tijdopnemers** opent.

1. (Voorwaardelijk) als de laatste tijd u toegang had opent, klik **terug naar timesheets** in de upper-left hoek van het scherm.

1. Selecteer **Mijn Goedkeuringen van het Tijdoppervlak** in de hoger-juiste hoek van de pagina om slechts timesheets te bekijken die u goedkeurt

   of

   Selecteer de **Mijn Goedkeuringen van de Chronologie** filter bij de bovenkant van de timesheet lijst.

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >De Mijn optie van Goedkeuringen Timesheet toont niet bij de bovenkant van timesheet lijst of in de lijst van filters als uw beheerder van Workfront of een groepsbeheerder de Mijn filter van de Goedkeuringen van Timesheet van of de Controles van de Lijst in het gebied van de Opstelling of van uw Malplaatje van de Lay-out verwijderde.
   >
   >Voor meer informatie zie [ Filters, Meningen, en Groepen aanpassen gebruikend een lay-outmalplaatje ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Facultatief) klik het **onderzoek** pictogram ![](assets/search-icon.png) bij de bovenkant van de timesheet lijst en typ een sleutelwoord om van specifieke timesheet de plaats te bepalen. U kunt zoeken naar een tijdkader of de naam van een eigenaar of fiatteur.
1. Klik het tijdkader voor timesheet u wilt goedkeuren. De tijdpagina wordt geopend.

   >[!TIP]
   >
   >Tijdschema&#39;s die nog moeten worden goedgekeurd, hebben de status [!UICONTROL Submitted] .


1. Klik **goedkeuren**

   of

   Als u timesheet wilt verwerpen, klik **Weigeren** in de laag-linkerhoek van timesheet.

   Indien goedgekeurd, verandert de chronologiestatus in **Gesloten**.

   Indien verworpen, verandert de chronologiestatus in **Verworpen**.

### Een tijdpagina&#39;s uit het thuisgebied goedkeuren

{{step1-to-home}}

Het gebied Home wordt geopend.

1. Verzeker u **Mijn goedkeurt** widget hebt die aan uw gebied van het Huis wordt toegevoegd. Voor meer informatie, zie [ toevoegen, geef, of verwijder widgets in Nieuw Huis ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md) uit.
1. Zoek naar een timesheet goedkeuring in uw Mijn widget Goedkeuringen.
1. (Facultatief) breid het drop-down menu aan het recht van goedkeurt of verwerpt knopen uit om een commentaar over uw besluit toe te voegen, dan klik **toevoegen**.
1. Klik op een van de volgende knoppen om een goedkeuringsbesluit te nemen:

   * Goedkeuren
   * Afwijzen

   De goedkeuring wordt verwijderd uit **Mijn goedkeurt** widget.


