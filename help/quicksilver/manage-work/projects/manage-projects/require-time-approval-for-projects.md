---
product-area: projects
navigation-topic: manage-projects
title: Tijd vereisen om te worden goedgekeurd voor een project
description: Tijd vereisen om te worden goedgekeurd voor een project
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Tijd vereisen om te worden goedgekeurd voor een project

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN A TOOLTIP IN THE EDIT PROJECT MODAL) </p>
-->

U kunt het project vormen om te vereisen dat de uren tegen het project worden geregistreerd door de Eigenaar van het Project worden goedgekeurd. Als deze configuratie zo is, moeten de uren eerst worden goedgekeurd door de eigenaar van het project voordat ze in aanmerking komen voor gebruik op een factureringsrecord.\
Raadpleeg het artikel voor meer informatie over factureringsrecords [Factureringsrecords maken](../../../manage-work/projects/project-finances/create-billing-records.md).

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
   <td> <p>Plan om tijd te vergen voor goedkeuring van het project</p>
   <p>Controle of hoger om uren goed te keuren die op een project worden geregistreerd</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten of hoger bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen weergeven voor het project of hoger</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
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
     <li>U hebt een licentie voor abonnementen met beheerdersrechten voor timesheets en uren. In dit geval:
      <ul>
       <li>U kunt om het even welke uren op de projecten goedkeuren of verwerpen u minstens toestemmingen aan Mening hebt. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Tijd vereisen om te worden goedgekeurd voor een project

U kunt als volgt de goedkeuring van een projectmanager urenlang voor het project vereisen:

1. Ga naar het project waar u goedkeuring urenlang wilt vereisen.
1. Klik op de knop **Meer** pictogram ![](assets/more-icon.png) rechts van de projectnaam klikt u op **Bewerken**.\
   Het dialoogvenster Project bewerken wordt weergegeven.

1. In de **Projectinstellingen** sectie, selecteert u **Voor dit project goed te keuren tijd vereisen**.
1. Klikken **Opslaan**.\
   Nu wanneer de tijd wordt geregistreerd en goedgekeurd, worden die uren gesloten en kunnen niet door de gebruiker worden veranderd die hen op het project of timesheet inging. Alleen een Workfront-beheerder kan de opgenomen tijd aanpassen.

## Tijd voor een project goedkeuren en afwijzen

Als projectmanager, kunt u uren goedkeuren of verwerpen die voor taken, kwesties, of het project worden geregistreerd.

Het goedkeuren van de uren op het projectniveau heeft geen invloed op timesheet van om het even welke gebruikers die de uren registreerden. Bijvoorbeeld, kunnen de uren in het project door de projectmanager worden goedgekeurd, maar timesheet is nog te worden goedgekeurd door de manager van de gebruiker of timesheet fiatteur. 

Als u opstelling een project om goedkeuring op de geregistreerde uren te vereisen, moet de projectmanager de uren goedkeuren opdat zij beschikbaar zijn om in een factureringsverslag voor het project te worden omvat. Raadpleeg het artikel voor meer informatie over het maken van factureringsrecords [Factureringsrecords maken](../../../manage-work/projects/project-finances/create-billing-records.md).

Uren voor een project goedkeuren of afwijzen:

1. Ga naar het project.
1. Klik op de knop **Uren** in het linkerdeelvenster. Dit kan zich bevinden onder de **Meer weergeven** gebied.

1. De uren die voor kwesties, taken, en de projectvertoning worden geregistreerd en zouden een status van moeten hebben **Verzonden**.\
   Klik op het vakje links van de uurvermeldingen om de uren te selecteren die u wilt goedkeuren.

1. Klikken **Goedkeuren**.\
   De status van de uren verandert in **Goedgekeurd**.\
   Als u de goedgekeurde uren later afwijst, verandert de status van de uren in **Niet goedgekeurd**.\
   Wanneer u de goedgekeurde uren opneemt in een factureringsrecord, verandert de status van de uren in **Gefactureerd en goedgekeurd**. De uren die aan een factureringsverslag worden toegevoegd kunnen niet worden geschrapt. Raadpleeg het artikel voor meer informatie over het maken van factureringsrecords [Factureringsrecords maken](../../../manage-work/projects/project-finances/create-billing-records.md)

1. (Optioneel) Klik op **Afwijzen** om de tijdsinvoer voor het project af te wijzen.\
   De status van de uren verandert in **Geweigerd**.
