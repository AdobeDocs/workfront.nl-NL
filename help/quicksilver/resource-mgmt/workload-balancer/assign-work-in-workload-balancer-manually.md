---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Handmatig werk toewijzen met Workload Balancer
description: Met de Adobe Workfront Workload Balancer kunt u handmatig werkitems toewijzen aan gebruikers.
author: Alina
feature: Resource Management
role: User
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Handmatig werk toewijzen met Workload Balancer

Met de Adobe Workfront Workload Balancer kunt u handmatig werkitems toewijzen aan gebruikers.

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
   <td> <p>Plan, wanneer het gebruiken van de Balancer van de Werkbelasting in het gebied van de Middelen</p>
   <p>Het werk, wanneer het gebruiken van de Balancer van de Werkbelasting van een team of een project</p>
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

## Werk handmatig toewijzen in Workload Balancer

U kunt werkitems toewijzen die nog niet aan een gebruiker zijn toegewezen of items die aan gebruikers in de werklastbalans zijn toegewezen, opnieuw toewijzen.

1. Ga naar Werklastverdeling waar u werk wilt toewijzen.

   U kunt werk aan gebruikers toewijzen gebruikend de Balancer van de Werkbelasting in het gebied van het Middelen, op het project, of op het teamniveau. Ga voor meer informatie over waar de werklastbalans zich in Workfront bevindt naar [De werklastbalans zoeken](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Optioneel) Ga naar de **Niet toegewezen werk** en pas een filter toe om taken of problemen weer te geven

   of

   Ga naar de **Toegewezen werk** en vouw de naam van een gebruiker uit om de aan hen toegewezen het werkpunten te bekijken, als u hun punten opnieuw wilt toewijzen.

1. Klik op de knop **Het menu Meer** ![](assets/qs-more-menu.png) links van de naam van een tijdelijk onderdeel klikt u op **Deze toewijzen aan**.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >U kunt ook de volgende sneltoetsen gebruiken om taken of problemen toe te wijzen:
   >
   >* In Windows: CTRL+klik op de taak of de uitgiftebalk.
   >* In Mac: CMD+klik op de taak- of uitgavenbalk.

1. Voer een van de volgende handelingen uit:

   * Begin de naam van een gebruiker, baanrol, of team te typen die u aan het punt in wilt toewijzen **Personen, rollen of teams zoeken** , selecteert u het veld wanneer het wordt weergegeven in de lijst en klikt u vervolgens op **Opslaan**.

   >[!TIP]
   >
   >Wanneer u een gebruiker toevoegt, ziet u de avatar, de primaire rol van de gebruiker en hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen.
   >
   >Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt.
   >
   > De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Zie voor meer informatie [Toegang verlenen aan gebruikers](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Als uw Workfront- of groepsbeheerder delegaties in uw omgeving heeft ingeschakeld, gebruikt u het tabblad Toewijzingen om gebruikers toe te wijzen aan de taak of uitgave. Gebruik het tabblad Delegaties om gebruikers weer te geven die zijn gedelegeerd aan het werkitem. Voor informatie over het delegeren van het werk, zie [Taak beheren en taken delegeren](../../manage-work/delegate-work/how-to-delegate-work.md).


   Hiermee wijst u het werkitem toe aan of wijst u het toe aan de opgegeven toewijzingen.

   Als u een punt aan enkel een team of een baanrol toewijst, toont het punt slechts in het Niet toegewezen gebied van het Werk. U moet werkitems toewijzen aan gebruikers om deze weer te geven in het gedeelte Toegewezen werk van Workload Balancer.

   >[!TIP]
   >
   >U kunt meerdere gebruikers, taakrollen of teams toewijzen. U kunt alleen actieve gebruikers, taakrollen en teams toewijzen.
   >
   >
   >Als een gebruiker, een baanrol, of een team werd toegewezen alvorens zij werden gedeactiveerd, blijven zij toegewezen aan het het werkpunt. In dit geval raden we het volgende aan:
   >
   >   
   >   
   >   * Wijs het werkitem opnieuw toe aan actieve bronnen.
   >   * Koppel de gebruikers in een gedeactiveerd team aan een actief team en wijs het het werkpunt aan het actieve team opnieuw toe.
   >   
   >

   * Klikken **Geavanceerd** om toegang te krijgen tot Geavanceerde toewijzingen.

     Voor meer informatie over het maken van Geavanceerde Taken, zie [Geavanceerde toewijzingen maken](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. (Optioneel) Klik op de knop **Toewijzingspictogram tonen** ![](assets/show-allocations-icon-small.png)klikt u op de knop **Het menu Meer** ![](assets/qs-more-menu.png) > **Toewijzingen bewerken**.

   of

   Dubbelklik op een dagelijkse of wekelijkse toewijzing om de hoeveelheid tijd aan te passen die de gebruiker aan het werkitem heeft toegewezen.

   Zie de sectie &quot;Gebruikerstoewijzingen wijzigen&quot; in het artikel voor informatie over het wijzigen van gebruikerstoewijzingen in Workload Balancer [Toewijzingen van gebruikers beheren in Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Voor informatie over het verwijderen van taken uit een werkitem met behulp van Werklastverdeling raadpleegt u [Werklastverdeling ongedaan maken](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
