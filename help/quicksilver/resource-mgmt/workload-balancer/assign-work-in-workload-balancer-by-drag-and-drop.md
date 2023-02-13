---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Werk toewijzen in Workload Balancer door slepen en neerzetten
description: U kunt werkitems toewijzen met de Adobe Workfront Workload Balancer door werkitems naar de juiste gebruikers te slepen en neer te zetten.
author: Alina
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: a1ffec0d8a50ff7f025ff23370afa746cf0d6d3f
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# Werk toewijzen in Workload Balancer door slepen en neerzetten

<!--remove production and preview preferences at release-->

U kunt werkitems toewijzen met de Adobe Workfront Workload Balancer door werkitems naar de juiste gebruikers te slepen en neer te zetten.

Voor algemene informatie over het toewijzen van werk aan gebruikers die de Balancer van de Werkbelasting gebruiken, zie [Overzicht van het toewijzen van werk in de werklastverdeler](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan, wanneer het gebruiken van de Balancer van de Werkbelasting voor een team of in het Brongebied </p>
   <p>Werk, wanneer het gebruiken van de Balancer van de Werkbelasting van een project </p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau*</td> 
   <td> <p>Toegang tot het volgende bewerken:</p> 
    <ul> 
     <li> <p>Bronbeheer</p> </li> 
     <li> <p>Projecten</p> </li> 
     <li> <p>Taken</p> </li> 
     <li> <p>Problemen</p> </li> 
    </ul> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute-machtigingen of hoger voor projecten, taken en problemen die Toewijzingen maken bevatten</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Een item toewijzen door het te slepen en neer te zetten

U kunt een item uit het gebied Niet toegewezen werk toewijzen aan een gebruiker of u kunt een reeds toegewezen item opnieuw toewijzen aan een andere gebruiker in het gebied Toegewezen werk.

1. Ga naar Werklastverdeling waar u werk wilt toewijzen.

   U kunt werk aan gebruikers toewijzen gebruikend de Balancer van de Werkbelasting in het gebied van het Middelen, op het project, of op het teamniveau. Ga voor meer informatie over waar de werklastbalans zich in Workfront bevindt naar [De werklastbalans zoeken](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Optioneel) Ga naar de **Niet toegewezen werk** en pas een filter toe om taken en kwesties te bekijken die niet aan gebruikers worden toegewezen

   of

   Ga naar de **Toegewezen werk** en vouw de naam van een gebruiker uit om de aan hen toegewezen het werkpunten te bekijken, als u hun punten opnieuw wilt toewijzen.

1. (Voorwaardelijk) Klik in de taakverdeler van een project op de knop **Alle gebruikers tonen** pictogram ![](assets/show-all-users-icon-project-workload-balancer.png) om alle Workfront-gebruikers weer te geven.

   Alle gebruikers die toegang hebben tot de weergave worden dan weergegeven.

   De gebruikers die ook deel uitmaken van het projectteam en reeds aan punten op het project worden toegewezen hebben het projectpictogram rechts van hun naam in het Toegewezen gebied van het Werk.

   ![](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)


   >[!TIP]
   >
   >* De optie Alle gebruikers weergeven is alleen beschikbaar in Workload Balancer van een project.
   >* Gebruik filters om alleen de gebruikers weer te geven die voor u van belang zijn. Gebruik bijvoorbeeld een filter om alleen gebruikers van uw teams of groepen weer te geven.




1. Klik op de balk van een tijdelijk item dat de geplande of de geprojecteerde tijdlijn aangeeft en sleep dit over de naam van een gebruiker in het deelvenster **Toegewezen** gebied.

   De gebruiker waarop u de muisaanwijzer plaatst om het werkitem naar te zetten, wordt gemarkeerd.

   >[!TIP]
   >
   >De Geplande Uren voor de gebruiker u over update in echt - tijd met het aantal dagelijkse Geplande Uren van het het werkpunt beweegt, om erop te wijzen wat het effect van het toevoegen van een nieuw punt aan hun algemene toewijzing zou kunnen zijn.

   ![](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. Als u klaar bent, zet u het geselecteerde werkitem neer op dezelfde regel als de naam van de gebruiker in het Toegewezen gebied. Het punt wordt toegewezen en de toegewezen Geplande Uren worden bijgewerkt voor de gebruiker met de nieuwe uren van het het werkpunt.

   Als het punt aan een baanrol werd toegewezen die de gebruiker niet kan vervullen, toont het punt onder de naam van de gebruiker in het Toegewezen gebied van het Werk en het blijft ook in het Niet toegewezen gebied van het Werk om erop te wijzen dat de baanrol verbonden aan het nog niet door een gebruiker is vervangen.

   >[!TIP]
   >
   >* Als u Groep door Project op het gebied van Montages toeliet, toont de toegewezen taak onder het overeenkomstige project. Als de instelling is uitgeschakeld, wordt de toegewezen taak weergegeven in het gebruikersgebied.
      >
      >
      >     Het item wordt weergegeven volgens de criteria voor werklastbalans voor het sorteren van werkitems. Zie voor meer informatie [Navigeren door werklastbalans](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).
   >
   >
   >* Als u toeliet toon alle gebruikers in de Balancer van de Werkbelasting van een project en toewees punten aan gebruikers die niet eerder aan punten op het project werden toegewezen, worden de gebruikers toegevoegd aan het Team van het Project. Zie voor meer informatie [Projectteam beheren](../../manage-work/projects/planning-a-project/manage-project-team.md).



1. (Optioneel) Klik op de balk van een tijdelijk item onder de naam van een gebruiker in het gebied Toegewezen werk en sleep het item vervolgens over het gebied Niet toegewezen werk om de toewijzing ongedaan te maken. Het punt is unassigned van de gebruiker, maar het zou nog aan een baanrol kunnen worden toegewezen waarin het in het Unassigned gebied van het Werk toont. Als het punt aan een andere gebruiker wordt toegewezen, blijft het in het Toegewezen gebied van het Werk onder de naam van de gebruiker die nog wordt toegewezen.
1. (Optioneel) Klik op de knop **Toewijzingspictogram tonen** ![](assets/show-allocations-icon-small.png)klikt u op de knop **Het menu Meer** ![](assets/qs-more-menu.png) > **Toewijzingen bewerken**.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   of

   Dubbelklik op een dagelijkse of wekelijkse toewijzing om de hoeveelheid tijd aan te passen die de gebruiker aan het werkitem heeft toegewezen.

   Zie de sectie &quot;Gebruikerstoewijzingen wijzigen&quot; in het artikel voor informatie over het wijzigen van gebruikerstoewijzingen in Workload Balancer [Toewijzingen van gebruikers beheren in Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Voor informatie over het verwijderen van taken uit een werkitem met behulp van Werklastverdeling raadpleegt u [Werklastverdeling ongedaan maken](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

