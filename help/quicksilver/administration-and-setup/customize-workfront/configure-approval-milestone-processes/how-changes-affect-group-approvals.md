---
title: De invloed van de wijzigingen in het groeperings- en goedkeuringsproces op toegewezen goedkeuringsproces
user-type: administrator
content-type: reference
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: In dit artikel wordt uitgelegd wat er gebeurt wanneer een goedkeuringsproces al in gebruik is wanneer een Workfront-beheerder (of een gebruiker met beheerdersrechten voor goedkeuringsprocessen) zijn koppeling met een groep wijzigt.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 77b2dce2-1523-4262-a659-0d301059a54c
source-git-commit: 7f719c903ad4079470a6dbd046dce445ba227a5b
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 0%

---

# De invloed van wijzigingen in groep- en goedkeuringsproces op toegewezen goedkeuringsprocessen

Dit artikel verklaart wat gebeurt wanneer een goedkeuringsproces reeds met taken, kwesties, projecten, malplaatjes, of malplaatjetaken wordt geassocieerd en een beheerder van Workfront (of een gebruiker met administratieve toegang tot goedkeuringsprocessen) één van het volgende doet:

* Hiermee wordt het goedkeuringsproces (op groepsniveau) van de ene groep gewijzigd in de andere
* Hiermee wijzigt u de groep die aan het project is gekoppeld
* Verandert het goedkeuringsproces van groepsniveau in systeemniveau
* Verandert het goedkeuringsproces van systeem tot groep-niveau

Het artikel beschrijft ook wat gebeurt wanneer het bewegen van of het kopiëren van taken of kwesties verbonden aan een groep-vlakke goedkeuringsproces tussen twee projecten van verschillende groepen.

Voor informatie over de 3 types van goedkeuringsprocessen kunt u in Workfront gebruiken, zie [&#x200B; overzicht van het proces van de Goedkeuring &#x200B;](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

>[!NOTE]
>
>Als het project, of zijn taken of kwesties reeds met een groep-vlakke goedkeuringsproces gebruikend groep-vlakke douanestatus worden geassocieerd, zou het veranderen van de groep een conflict tussen de goedkeuringsstatussen van de vorige groep en die op het systeemniveau kunnen tot stand brengen.
>
>Als een goedkeuringsproces bijvoorbeeld twee paden bevat, een voor een status op systeemniveau en een tweede voor een status op groepsniveau die gelijk is aan dezelfde status op systeemniveau, leidt het wijzigen van de groep van het oorspronkelijke project ertoe dat Workfront problemen ondervindt met het begrijpen van de status die specifiek is voor een groep en die mogelijk niet bestaat voor de tweede groep. In dit geval treedt er een fout op.
>
>U kunt overwegen de goedkeuringsprocessen op groepsniveau voor het project of de taken of problemen ervan te verwijderen voordat u de groep van het project bijwerkt.
>
>Voor informatie over het creëren van groep-vlakke goedkeuringsprocessen, zie [&#x200B; groep-vlakke goedkeuringsprocessen &#x200B;](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).
>
>Voor informatie over het creëren van een groep-vlakke douanestatus, zie [&#x200B; een groepsstatus &#x200B;](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md) creëren of uitgeven

## Een groepsspecifiek goedkeuringsproces van de ene groep naar de andere wijzigen

De volgende scenario&#39;s komen voor wanneer een groep-specifiek goedkeuringsproces reeds op een voorwerp wordt gebruikt en iemand het aan een verschillende groep opnieuw toewijst:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Gebied of voorwerp waar het goedkeuringsproces is verbonden</th> 
   <th>Goedkeuringsobject</th> 
   <th>Wijziging in het goedkeuringsproces voor het object of gebied</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Goedkeuring van project of sjabloon </td> 
   <td>Project</td> 
   <td>Wordt een goedkeuringsproces voor eenmalig gebruik</td> 
  </tr> 
  <tr> 
   <td>Taak- of sjabloontaakgoedkeuring </td> 
   <td>Taak</td> 
   <td>Wordt een goedkeuringsproces voor eenmalig gebruik </td> 
  </tr> 
  <tr> 
   <td>Goedkeuring afgeven</td> 
   <td>Probleem</td> 
   <td>Wordt een goedkeuringsproces voor eenmalig gebruik</td> 
  </tr> 
  <tr> 
   <td>Het gedeelte Taken in het vak Project bewerken of Sjabloon bewerken</td> 
   <td>Taak</td> 
   <td> <p>Het veld Standaardgoedkeuringsproces taak wordt opnieuw ingesteld op n.v.t.</p> <p>Door gebrek, worden geen goedkeuringsprocessen geassocieerd met nieuwe taken op het project.</p> </td> 
  </tr> 
  <tr> 
   <td>De sectie van de Details van de rij van een project of een malplaatje</td> 
   <td>Probleem</td> 
   <td> <p>Het veld Standaardgoedkeuring wordt teruggezet op N.v.t.</p> <p>Door gebrek, worden geen goedkeuringsprocessen geassocieerd met nieuwe kwesties of verzoeken op het project.</p> </td> 
  </tr> 
  <tr> 
   <td>De sectie van het Onderwerp van de rij van een project of een malplaatje</td> 
   <td>Probleem</td> 
   <td> <p>Het veld Standaardgoedkeuring wordt teruggezet op N.v.t.</p> <p>Er zijn geen goedkeuringsprocessen gekoppeld aan nieuwe problemen of verzoeken over het project die standaard worden uitgevoerd.</p> </td> 
  </tr> 
 </tbody> 
</table>

## De groep wijzigen die aan een project is gekoppeld

Wanneer iemand de groep wijzigt die aan een project is gekoppeld, gebeurt het volgende:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Gebied of object waaraan het goedkeuringsproces al is gekoppeld</th> 
   <th>Goedkeuringsobject</th> 
   <th>Wijziging in het goedkeuringsproces van het object of gebied</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Goedkeuring van project of sjabloon </td> 
   <td>Project</td> 
   <td>Wordt een goedkeuringsproces voor eenmalig gebruik en de status die eraan is gekoppeld, wordt bijgewerkt zodat deze overeenkomt met een vergelijkbare status voor de nieuwe groep.</td> 
  </tr> 
  <tr> 
   <td>Taak- of sjabloontaakgoedkeuring </td> 
   <td>Taak</td> 
   <td>Wordt een goedkeuringsproces voor eenmalig gebruik en de status die eraan is gekoppeld, wordt bijgewerkt zodat deze overeenkomt met een vergelijkbare status voor de nieuwe groep.</td> 
  </tr> 
  <tr> 
   <td>Goedkeuring afgeven</td> 
   <td>Probleem</td> 
   <td>Wordt een goedkeuringsproces voor eenmalig gebruik en de status die eraan is gekoppeld, wordt bijgewerkt zodat deze overeenkomt met een vergelijkbare status voor de nieuwe groep.</td> 
  </tr> 
  <tr> 
   <td>Het gedeelte Taken in het vak Project bewerken of Sjabloon bewerken</td> 
   <td>Taak</td> 
   <td> <p>Het veld Standaardgoedkeuringsproces taak wordt opnieuw ingesteld op N.V.</p> <p>Door gebrek, worden geen goedkeuringsprocessen geassocieerd met nieuwe taken op het project</p> </td> 
  </tr> 
  <tr> 
   <td>De sectie van de Details van de rij van een project of een malplaatje</td> 
   <td>Probleem</td> 
   <td> <p>Het veld Standaardgoedkeuringsproces wordt opnieuw ingesteld op N.V.</p> <p>Door gebrek, worden geen goedkeuringsprocessen geassocieerd met nieuwe kwesties of verzoeken over het project</p> </td> 
  </tr> 
  <tr> 
   <td>De sectie van het Onderwerp van de rij van een project of een malplaatje</td> 
   <td>Probleem</td> 
   <td> <p>Het veld Standaardgoedkeuringsproces wordt opnieuw ingesteld op N.V.</p> <p>Door gebrek, worden geen goedkeuringsprocessen geassocieerd met nieuwe kwesties of verzoeken over het project</p> </td> 
  </tr> 
 </tbody> 
</table>

## Een goedkeuringsproces wijzigen van groepsniveau in systeemniveau

Wanneer iemand de optie Groep in een groep-specifiek goedkeuringsproces in &quot;Alle groepen verandert,&quot;wordt het goedkeuringsproces systeembreed en het volgende voorkomt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Gebied of voorwerp waar het goedkeuringsproces is verbonden</th> 
   <th>Goedkeuringsobject</th> 
   <th>Wijziging in het goedkeuringsproces van het object of gebied</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Goedkeuring van project of sjabloon </td> 
   <td>Project</td> 
   <td>Geen wijziging</td> 
  </tr> 
  <tr> 
   <td>Taak- of sjabloontaakgoedkeuring </td> 
   <td>Taak</td> 
   <td>Geen wijziging</td> 
  </tr> 
  <tr> 
   <td>Goedkeuring afgeven</td> 
   <td>Probleem</td> 
   <td>Geen wijziging</td> 
  </tr> 
  <tr> 
   <td>Het gedeelte Taken in het vak Project bewerken of Sjabloon bewerken</td> 
   <td>Taak</td> 
   <td> <p>Geen verandering in het goedkeuringsproces maar, door gebrek, wordt het geassocieerd met nieuwe taken op het project</p> </td> 
  </tr> 
  <tr> 
   <td>De sectie van de Details van de rij van een project of een malplaatje</td> 
   <td>Probleem</td> 
   <td> <p>Geen wijziging in het goedkeuringsproces, maar is standaard gekoppeld aan nieuwe kwesties of verzoeken in het project</p> </td> 
  </tr> 
  <tr> 
   <td>De sectie van het Onderwerp van de rij van een project of een malplaatje</td> 
   <td>Probleem</td> 
   <td> <p>Geen wijziging in het goedkeuringsproces, maar is standaard gekoppeld aan nieuwe kwesties of verzoeken in het project</p> </td> 
  </tr> 
 </tbody> 
</table>

## Een goedkeuringsproces wijzigen van systeemniveau in groepsniveau

Wanneer iemand de beschikbaarheid van een systeembreed goedkeuringsproces van &quot;Alle groepen&quot;in een specifieke groep verandert, wordt het goedkeuringsproces groep-specifiek en het volgende komt voor:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Gebied of voorwerp waar het goedkeuringsproces is verbonden</th> 
   <th>Goedkeuringsobject</th> 
   <th>Wijziging in het goedkeuringsproces van het object of gebied</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Project, taak, kwestie, malplaatje, of malplaatjetaak die tot de groep van het goedkeuringsproces behoort</td> 
   <td> <p>Project, taak of uitgave</p> </td> 
   <td>Geen wijziging</td> 
  </tr> 
  <tr> 
   <td>Het gebied van taken in Edit Project of geeft het vakje van het Malplaatje voor een project of een malplaatje uit dat tot de groep van het goedkeuringsproces behoort</td> 
   <td>Taak</td> 
   <td> <p>Geen verandering in het goedkeuringsproces maar, door gebrek, wordt het geassocieerd met nieuwe taken op het project</p> </td> 
  </tr> 
  <tr> 
   <td>De sectie van de Details van de rij voor een project of een malplaatje dat tot de groep van het goedkeuringsproces behoort</td> 
   <td>Probleem</td> 
   <td> <p>Geen wijziging in het goedkeuringsproces, maar is standaard gekoppeld aan nieuwe kwesties of verzoeken in het project</p> </td> 
  </tr> 
  <tr> 
   <td>De sectie van het Onderwerp van de rij voor een project of een malplaatje dat tot de groep van het goedkeuringsproces behoort</td> 
   <td>Probleem</td> 
   <td> <p>Geen wijziging in het goedkeuringsproces, maar is standaard gekoppeld aan nieuwe kwesties of verzoeken in het project</p> </td> 
  </tr> 
  <tr> 
   <td>Project, taak, kwestie, malplaatje, of malplaatjetaak die tot een groep buiten de groep van het goedkeuringsproces behoort</td> 
   <td> <p>Projecten</p> <p>Taken</p> <p>Problemen</p> </td> 
   <td>Wordt een goedkeuringsproces voor eenmalig gebruik</td> 
  </tr> 
  <tr> 
   <td>Het gebied van taken in Edit Project of geeft het vakje van het Malplaatje voor een project of een malplaatje uit dat tot een groep buiten de groep van het goedkeuringsproces behoort</td> 
   <td>Taken</td> 
   <td> <p>Het veld Standaardgoedkeuringsproces taak wordt opnieuw ingesteld op n.v.t.</p> <p>Door gebrek, worden geen goedkeuringsprocessen geassocieerd met nieuwe taken op het project.</p> </td> 
  </tr> 
  <tr> 
   <td>De sectie van de Details van de rij voor een project of een malplaatje dat tot een groep buiten de groep van het goedkeuringsproces behoort</td> 
   <td>Problemen</td> 
   <td> <p>Het veld Standaardgoedkeuring wordt teruggezet op N.v.t.</p> <p>Door gebrek, worden geen goedkeuringsprocessen geassocieerd met nieuwe kwesties of verzoeken op het project.</p> </td> 
  </tr> 
  <tr> 
   <td>De sectie van het Onderwerp van de rij voor een project of een malplaatje dat tot een groep buiten de groep van het goedkeuringsproces behoort</td> 
   <td>Problemen</td> 
   <td> <p>Het veld Standaardgoedkeuring wordt teruggezet op N.v.t.</p> <p>Door gebrek, worden geen goedkeuringsprocessen geassocieerd met nieuwe kwesties of verzoeken op het project.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Een taak of een probleem verplaatsen of kopiëren naar een project met een andere groep dan die van het goedkeuringsproces

Het bewegen of het kopiëren van een taak of een kwestie van een project aan een andere zou bestaande goedkeuringsprocessen op de taak of de kwestie afhankelijk van de groepen van de twee projecten kunnen beïnvloeden. In de volgende tabel worden de mogelijke scenario&#39;s weergegeven:

| Oorspronkelijke taak of goedkeuringsproces van afgifte | Groepen van de twee projecten | Wijzigingen in het goedkeuringsproces nadat de taak of uitgave naar een ander project is verplaatst |
|---|---|---|
| Goedkeuringsprocedure voor eenmalig gebruik in combinatie met een systeembrede status | Projecten bevinden zich in dezelfde of verschillende groepen | Geen wijziging |
| Goedkeuringsprocedure voor eenmalig gebruik in verband met een groepsspecifieke status | Projecten bevinden zich in verschillende groepen | De goedkeuring blijft een goedkeuringsproces voor eenmalig gebruik en de status die aan de goedkeuring is gekoppeld, wordt bijgewerkt zodat deze overeenkomt met een vergelijkbare status voor de nieuwe groep. |
| Goedkeuringsprocedure voor het hele systeem | Projecten bevinden zich in dezelfde of verschillende groepen | Geen wijziging |
| Groepsspecifieke goedkeuringsprocedure | Projecten bevinden zich in dezelfde groep | Geen wijziging |
| Groepsspecifieke goedkeuringsprocedure | Projecten bevinden zich in verschillende groepen en de groepen hebben verschillende groepsspecifieke statussen | De goedkeuring wordt een goedkeuringsproces voor eenmalig gebruik en de status die aan de goedkeuring is gekoppeld, wordt bijgewerkt zodat deze overeenkomt met een vergelijkbare status voor de nieuwe groep. |
| Groepsspecifieke goedkeuringsprocedure | De projecten zijn in verschillende groepen en er is een status met de zelfde sleutel in de nieuwe groep zoals de status verbonden aan het goedkeuringsproces van de eerste groep | Geen wijziging |
