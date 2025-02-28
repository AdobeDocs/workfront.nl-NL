---
product-area: projects
navigation-topic: manage-projects
title: Tijd vereisen om te worden goedgekeurd voor een project
description: Tijd vereisen om te worden goedgekeurd voor een project
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '763'
ht-degree: 0%

---

# Tijd vereisen om te worden goedgekeurd voor een project

<!--audited: 08/2024-->

U kunt het project vormen om te vereisen dat de uren tegen het project worden geregistreerd door de Eigenaar van het Project worden goedgekeurd. Als deze configuratie zo is, moeten de uren eerst worden goedgekeurd door de eigenaar van het project voordat ze in aanmerking komen voor gebruik op een factureringsrecord.\
Voor meer informatie over het factureren verslagen, zie het artikel [ het factureren verslagen ](../../../manage-work/projects/project-finances/create-billing-records.md) creëren.

>[!NOTE]
>
>Als u deze optie inschakelt, wordt de mogelijkheid van een fiatteur voor een tijdpagina om tijd goed te keuren op het tijdblad niet verwijderd. Als de Eigenaar van het Project niet goedkeurt of tijd verwerpen, kan een chronologiefiatteur nog de tijd op een timesheet goedkeuren.

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
   <td> <p>Om tijd te vereisen om voor het project te worden goedgekeurd:</p>
   <ul><li>Nieuw: Standaard</li>
   <li>Huidig: Plan</li></ul>

<p>Om uren goed te keuren die op een project worden het programma geopend:</p>
   <ul><li>Nieuw: Licht of hoger</li>
   <li>Controleren of hoger</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten of hoger bewerken</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toestemmingen voor het project of hoger weergeven</p>
  </tr> 
  <tr> 
   <td role="rowheader">Aanvullende toegang</td> 
   <td> <p>U moet aan minstens één van de volgende voorwaarden voldoen om tijd op een project goed te keuren:</p> 
    <ul> 
     <li>U bent de Eigenaar van het Project met de toegang en de toestemmingen hierboven gespecificeerd. In dit geval kunt u het volgende doen als een van de onderstaande voorwaarden bestaat: 
      <ul>
       <li>Als u beheerdersmachtigingen voor het project hebt, kunt u uren die door een andere gebruiker zijn aangemeld, goedkeuren of afwijzen.</li>
       <li> Als u Contribute of de Toegang van de Mening tot het project hebt zult u slechts de uren kunnen goedkeuren of verwerpen die door u of een andere gebruiker worden geregistreerd die u meldt.<br></li>
      </ul></li> 
     <li>U hebt een licentie voor abonnementen met beheerdersrechten voor timesheets en uren. In dit geval:
      <ul>
       <li>U kunt om het even welke uren op de projecten goedkeuren of verwerpen u minstens toestemmingen aan Mening hebt. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Tijd vereisen om te worden goedgekeurd voor een project

U kunt als volgt de goedkeuring van een projectmanager urenlang voor het project vereisen:

1. Ga naar het project waar u goedkeuring urenlang wilt vereisen.
1. Klik het **Meer** pictogram ![ Meer pictogram ](assets/more-icon.png) aan het recht van de projectnaam, dan klik **uitgeven**.\
   Het dialoogvenster Project bewerken wordt weergegeven.

1. In de **sectie van de Montages van het Project**, uitgezochte **vereist tijd om voor dit project** worden goedgekeurd.
1. Klik **sparen**.\
   Nu wanneer de tijd wordt geregistreerd en goedgekeurd, worden die uren gesloten en kunnen niet door de gebruiker worden veranderd die hen op het project of timesheet inging. Alleen een Workfront-beheerder kan de opgenomen tijd aanpassen.

## Tijd voor een project goedkeuren en afwijzen

Als projectmanager, kunt u uren goedkeuren of verwerpen die voor taken, kwesties, of het project worden geregistreerd.

Het goedkeuren van de uren op het projectniveau heeft geen invloed op timesheet van om het even welke gebruikers die de uren registreerden. Bijvoorbeeld, kunnen de uren in het project door de projectmanager worden goedgekeurd, maar timesheet is nog te worden goedgekeurd door de manager van de gebruiker of timesheet fiatteur.

Als u opstelling een project om goedkeuring op de geregistreerde uren te vereisen, moet de projectmanager de uren goedkeuren opdat zij beschikbaar zijn om in een factureringsverslag voor het project te worden omvat. Voor meer informatie over het creëren van het factureren verslagen, zie het artikel [ het factureren verslagen ](../../../manage-work/projects/project-finances/create-billing-records.md) creëren.

Uren voor een project goedkeuren of afwijzen:

1. Ga naar het project.
1. Klik het **gebied van Uren** in het linkerpaneel. Dit zou onder **kunnen worden gevestigd tonen meer** gebied.

1. De uren die voor kwesties, taken, en de projectvertoning worden geregistreerd en zouden een status van **moeten hebben voorgelegd**.\
   Klik op het vakje links van de uurvermeldingen om de uren te selecteren die u wilt goedkeuren.

1. Klik **goedkeuren** pictogram ![](assets/approve-hours-icon.png) bij de bovenkant van de uurlijst.\
   Het statuut van de urenveranderingen in **Goedgekeurd**.\
   Als u later de goedgekeurde uren verwerpt, verandert het statuut van de uren in **niet Goedgekeurd**.\
   Wanneer u de goedgekeurde uren in een het facturerings verslag omvat, verandert het statuut van de uren in **In rekening gebracht en goedgekeurd**. De uren die aan een factureringsverslag worden toegevoegd kunnen niet worden geschrapt. Voor meer informatie over het creëren van het factureren verslagen, zie het artikel [ het factureren verslagen ](../../../manage-work/projects/project-finances/create-billing-records.md) creëren

1. (Facultatief) klik **Afwijzen** pictogram ![](assets/reject-hours-icon.png) om de tijdingangen op het project te verwerpen.\
   Het statuut van de urenveranderingen in **Afgewezen**.

   >[!NOTE]
   >
   >   Als de geselecteerde uren zijn opgenomen in een factuurrecord die is gemarkeerd als Gefactureerd of Gefactureerd en goedgekeurd, worden de pictogrammen Goedkeuren en Afwijzen niet weergegeven. U kunt alleen uren goedkeuren die nog niet in een factuurrecord zijn gefactureerd.

