---
product-area: projects
navigation-topic: manage-projects
title: Tijd vereist voor goedkeuring van een project
description: U kunt het project vormen om te vereisen dat de uren tegen het project worden geregistreerd door de Eigenaar van het Project worden goedgekeurd. Als deze configuratie zo is, moeten de uren eerst worden goedgekeurd door de eigenaar van het project voordat ze in aanmerking komen voor gebruik op een factureringsrecord.
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 0%

---

# Tijd vereisen om te worden goedgekeurd voor een project

<!--audited: 08/2024-->

U kunt het project vormen om te vereisen dat de uren tegen het project worden geregistreerd door de Eigenaar van het Project worden goedgekeurd. Als deze configuratie zo is, moeten de uren eerst worden goedgekeurd door de eigenaar van het project voordat ze in aanmerking komen voor gebruik op een factureringsrecord.\
Voor meer informatie over het factureren verslagen, zie het artikel [&#x200B; het factureren verslagen &#x200B;](../../../manage-work/projects/project-finances/create-billing-records.md) creëren.

>[!NOTE]
>
>Als u deze optie inschakelt, wordt de mogelijkheid van een fiatteur voor een tijdpagina om tijd goed te keuren op het tijdblad niet verwijderd. Als de Eigenaar van het Project niet goedkeurt of tijd verwerpen, kan een chronologiefiatteur nog de tijd op een timesheet goedkeuren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Om tijd te vereisen om voor het project te worden goedgekeurd:</p>
   <ul><li><p>Standard</p></li>
   <li><p>Plan</p></li></ul>

<p>Om uren goed te keuren die op een project worden het programma geopend:</p>
   <ul><li><p>Licht of hoger</p></li>
   <li><p>Controleren of hoger</p></li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten bewerken</p>  </td> 
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

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>To require time to be approved on the project:</p>
   <ul><li>New: Standard</li>
   <li>Current: Plan</li></ul>
   
   <p>To approve hours logged on a project:</p>
   <ul><li>New: Light or higher</li>
   <li>Review or higher</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects or higher</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher</p>
  </tr> 
  <tr> 
   <td role="rowheader">Additional access</td> 
   <td> <p>You must meet at least one of the following conditions to approve time on a project:</p> 
    <ul> 
     <li>You are the Project Owner with the access and permissions specified above. In this case, you can do the following if one of the conditions below exists: 
      <ul>
       <li>If you have Manage permissions on the project, you can approve or reject hours logged on the project by any other user.</li>
       <li> If you have Contribute or View access to the project you will be able to approve or reject only the hours logged by you or any other user that reports you.<br></li>
      </ul></li> 
     <li>You have a Plan license with administrative access to Timesheets &amp; Hours. In this case:
      <ul>
       <li>You can approve or reject any hours on the projects you have at least permissions to View. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>-->

## Tijd vereisen om te worden goedgekeurd voor een project

U kunt als volgt de goedkeuring van een projectmanager urenlang voor het project vereisen:

1. Ga naar het project waar u goedkeuring urenlang wilt vereisen.
1. Klik het **Meer** pictogram ![&#x200B; Meer pictogram &#x200B;](assets/more-icon.png) aan het recht van de projectnaam, dan klik **uitgeven**.\
   Het dialoogvenster Project bewerken wordt weergegeven.

1. In de **sectie van de Montages van het Project**, uitgezochte **vereist tijd om voor dit project** worden goedgekeurd.
1. Klik **sparen**.\
   Nu wanneer de tijd wordt geregistreerd en goedgekeurd, worden die uren gesloten en kunnen niet door de gebruiker worden veranderd die hen op het project of timesheet inging. Alleen een Workfront-beheerder kan de opgenomen tijd aanpassen.

## Tijd voor een project goedkeuren en afwijzen

Als projectmanager, kunt u uren goedkeuren of verwerpen die voor taken, kwesties, of het project worden geregistreerd.

Het goedkeuren van de uren op het projectniveau heeft geen invloed op timesheet van om het even welke gebruikers die de uren registreerden. Bijvoorbeeld, kunnen de uren in het project door de projectmanager worden goedgekeurd, maar timesheet is nog te worden goedgekeurd door de manager van de gebruiker of timesheet fiatteur.

Als u opstelling een project om goedkeuring op de geregistreerde uren te vereisen, moet de projectmanager de uren goedkeuren opdat zij beschikbaar zijn om in een factureringsverslag voor het project te worden omvat. Voor meer informatie over het creëren van het factureren verslagen, zie het artikel [&#x200B; het factureren verslagen &#x200B;](../../../manage-work/projects/project-finances/create-billing-records.md) creëren.

Uren voor een project goedkeuren of afwijzen:

1. Ga naar het project.
1. Klik het **gebied van Uren** in het linkerpaneel.

1. De uren die voor kwesties, taken, en de projectvertoning worden geregistreerd en zouden een status van **moeten hebben voorgelegd**.\
   Klik op het vakje links van de uurvermeldingen om de uren te selecteren die u wilt goedkeuren.

1. Klik **goedkeuren** pictogram ![&#x200B; pictogram &#x200B;](assets/approve-hours-icon.png) bij de bovenkant van de uurlijst goedkeuren.\
   Het statuut van de urenveranderingen in **Goedgekeurd**.\
   Als u later de goedgekeurde uren verwerpt, verandert het statuut van de uren in **niet Goedgekeurd**.\
   Wanneer u de goedgekeurde uren in een het facturerings verslag omvat, verandert het statuut van de uren in **In rekening gebracht en goedgekeurd**. De uren die aan een factureringsverslag worden toegevoegd kunnen niet worden geschrapt. Voor meer informatie over het creëren van het factureren verslagen, zie het artikel [&#x200B; het factureren verslagen &#x200B;](../../../manage-work/projects/project-finances/create-billing-records.md) creëren

1. (Facultatief) klik **pictogram van de Weigering** het urenpictogram van de Weigering ![&#x200B; om de tijdingangen op het project te verwerpen.](assets/reject-hours-icon.png)\
   Het statuut van de urenveranderingen in **Afgewezen**.

   >[!NOTE]
   >
   >   Als de geselecteerde uren zijn opgenomen in een factuurrecord die is gemarkeerd als Gefactureerd of Gefactureerd en goedgekeurd, worden de pictogrammen Goedkeuren en Afwijzen niet weergegeven. U kunt alleen uren goedkeuren die nog niet in een factuurrecord zijn gefactureerd.

