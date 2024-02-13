---
title: Gebruikers verwijderen
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Wanneer een gebruiker uw organisatie verlaat, kan die gebruiker uit Workfront verwijderen, hoewel wij adviseren deactiverende gebruikers in plaats van hen te schrappen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: b3717fc89e45983b80471fdd629c79b82086c6ff
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Gebruikers verwijderen

Wanneer een gebruiker uw organisatie verlaat, kunt u die gebruiker uit Adobe Workfront verwijderen.

>[!IMPORTANT]
>
>Als u een gebruiker uit het systeem verwijdert, wordt ook de informatie verwijderd die is gekoppeld aan de gebruiker die u mogelijk wilt behouden. We raden u aan gebruikers te deactiveren in plaats van ze te verwijderen. Zie voor meer informatie [Een gebruiker deactiveren of opnieuw activeren](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
<!--
>* The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].
>
>  For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>  For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
-->

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau voor systeembeheerders. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>. </p> </li> 
     <li> <p><b>Gebruikers</b> het plaatsen in uw toegangsniveau dat wordt gevormd aan <b>Bewerken</b> toegang, met <b>Maken</b> en ten minste één van beide <b>Gebruikersbeheerder</b> opties ingeschakeld onder <b>Uw instellingen nauwkeurig afstellen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Van deze twee opties, als Gebruiker <b>Admin (Groepgebruikers)</b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> <p>Voor meer informatie over de <b>Gebruikers</b> het plaatsen in een toegangsniveau, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Een gebruiker verwijderen of deactiveren

Als u een gebruiker deactiveert, gebeurt het volgende:

* Verwijdert de gebruikerslicenties voor zowel Workfront als Workfront Proof als de Workfront Proof-component aan uw Workfront-account is gekoppeld. Ga voor meer informatie over Workfront Proof naar [Workfront Proof: artikelindex](../../../workfront-proof/workfront-proof.md).
* Aan de gebruiker kan geen werk meer worden toegewezen.
* De gebruiker kan niet meer aan updates worden toegevoegd.
* De gebruiker kan niet meer aan teams of groepen worden toegevoegd.
* Objecten kunnen niet meer met de gebruiker worden gedeeld.
* Hun associatie met de volgende objecten blijft intact:

   * Taken, kwesties, projecten, portefeuilles
   * Dashboards

     >[!NOTE]
     >
     >Als u een gebruiker deactiveert en de aan een gebruiker gekoppelde rapporten of dashboards niet meer kunt weergeven, moet u mogelijk de **Voer dit rapport uit met de toegangsrechten van:** veld.\
     >Zie voor meer informatie de [Waarom heb ik geen toegang tot een rapport dat eigendom is van een gedeactiveerde gebruiker?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) van de [Veelgestelde vragen over rapporten](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) artikel.

   * Documenten
   * Updates
   * Uren

* Als de gebruiker uitgecheckte documenten heeft, blijven de documenten uitgecheckt wanneer u ze deactiveert. Alleen een Workfront-beheerder kan ze weer inchecken. Zie voor meer informatie over het uitchecken van documenten [Documenten controleren](../../../documents/managing-documents/check-out-documents.md).

Wanneer u een gebruiker verwijdert, gebeurt het volgende:

* Verwijdert de gebruikerslicenties voor zowel Workfront als Workfront Proof als de Workfront Proof-component aan uw Workfront-account is gekoppeld. Ga voor meer informatie over Workfront Proof naar [Workfront Proof: artikelindex](../../../workfront-proof/workfront-proof.md).
* Aan de gebruiker kan geen werk meer worden toegewezen.
* De gebruiker kan niet meer aan updates worden toegevoegd.
* De gebruiker kan niet meer aan teams of groepen worden toegevoegd.
* Objecten kunnen niet meer met de gebruiker worden gedeeld.
* Verwijdert de koppeling van die gebruiker met de volgende objecten:

   * Taken, uitgaven, projecten, portfolio
   * Dashboards

     >[!NOTE]
     >
     >U verliest ook toegang tot aangepaste secties die dashboards bevatten die aan de geschrapte gebruiker worden geassocieerd.\
     >Zie voor meer informatie de [Hoe heb ik toegang tot een dashboard dat een rapport bevat dat door een geschrapte gebruiker wordt bezeten?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) van de [Veelgestelde vragen over rapporten](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) artikel.

   * Updates
   * Uren

     >[!NOTE]
     >
     >Deze objecten blijven in Workfront staan, maar de eigenaar van het object is nu leeg.

* Als de gebruiker documenten heeft geüpload onder het gebied Documenten in de algemene navigatiebalk, worden de documenten ook verwijderd.
* Als de gebruiker documenten heeft uitgecheckt die hij of zij bezit en de documenten in het belangrijkste gebied van Documenten (betreden van het Belangrijkste Menu) worden geupload, worden de documenten geschrapt met de gebruiker. Zie voor meer informatie over het uitchecken van documenten [Documenten controleren](../../../documents/managing-documents/check-out-documents.md).

Zie voor meer informatie over het deactiveren van gebruikers [Een gebruiker deactiveren of opnieuw activeren](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

U kunt gebruikers een voor een permanent verwijderen of u kunt meerdere gebruikers tegelijk permanent verwijderen. Wanneer u afzonderlijke gebruikers verwijdert, moet u wachten tot het verwijderingsproces is voltooid voordat u verdergaat met andere activiteiten in Workfront. Het verwijderen van meerdere gebruikers wordt tegelijkertijd als een achtergrondproces uitgevoerd, zodat u Workfront kunt blijven gebruiken terwijl de gebruikers worden verwijderd.

## Een of meer gebruikers verwijderen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) rechtsboven in Adobe Workfront.

1. Klikken **Gebruikers**.
1. Selecteer minstens één gebruiker die u wilt schrappen, klik het Meer menu ![](assets/more-icon.png)en klik vervolgens op **Verwijderen**.
1. Klik in het vak dat wordt weergegeven op **Verwijderen** om de schrapping te bevestigen.

   Het verwijderen van gebruikers wordt als een achtergrondproces uitgevoerd, zodat u Workfront kunt blijven gebruiken terwijl de gebruiker of gebruikers worden verwijderd.

   Afhankelijk van het aantal gebruikers dat u verwijdert, kan het proces enkele minuten of zelfs een paar uur duren.

   Nadat u in Workfront hebt bevestigd dat de gebruikers zijn verwijderd, kunt u ze in het systeem blijven zien totdat het verwijderingsproces op de achtergrond is voltooid.

   Als u later ontdekt dat een of meer gebruikers niet zijn verwijderd, probeert u deze één voor één te verwijderen.
