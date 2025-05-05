---
title: Gebruikers verwijderen
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Wanneer een gebruiker uw organisatie verlaat, kan die gebruiker uit Workfront verwijderen, hoewel wij adviseren deactiverende gebruikers in plaats van hen te schrappen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '872'
ht-degree: 0%

---

# Gebruikers verwijderen

>[!IMPORTANT]
>
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet zijn aangemeld bij het Adobe Business Platform. Als u bent aangemeld bij het Adobe Business Platform, moet u gebruikers verwijderen uit de Adobe Admin Console.
>
>Voor een lijst van procedures die verschillen gebaseerd op of uw organisatie aan het Van Bedrijfs Adobe Platform is genegeerd, zie [ Op platform-gebaseerde beleidsverschillen (Adobe Workfront/Adobe Bedrijfs Platform) ](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Wanneer een gebruiker uw organisatie verlaat, kunt u die gebruiker uit Adobe Workfront verwijderen.

>[!IMPORTANT]
>
>Als u een gebruiker uit het systeem verwijdert, wordt ook de informatie verwijderd die is gekoppeld aan de gebruiker die u mogelijk wilt behouden. We raden u aan gebruikers te deactiveren in plaats van ze te verwijderen. Voor meer informatie, zie [ een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) deactiveren of reactiveren.
<!--
>* The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].
>
>  For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/nl/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>  For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
-->

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

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
   <td><p>Nieuw: Standaard</p><p>of</p><p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau voor systeembeheerders. </li> 
     <li> <p><b> Gebruikers </b> het plaatsen in uw toegangsniveau dat aan <b> wordt gevormd geeft </b> toegang uit, met <b> creeert </b> en minstens één van de twee <b> die gebruikers Admin </b> opties onder <b> worden toegelaten verfijnen uw montages </b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Van deze twee opties, als <b> Admin van de Gebruiker (de Gebruikers van de Groep) </b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een gebruiker verwijderen of deactiveren

Als u een gebruiker deactiveert, gebeurt het volgende:

* Hiermee verwijdert u de gebruikerslicenties voor zowel Workfront als Workfront Proof als de Workfront Proof-component aan uw Workfront-account is gekoppeld. Voor meer informatie over Workfront Proof, zie [ Workfront Proof: artikelindex ](../../../workfront-proof/workfront-proof.md).
* Aan de gebruiker kan geen werk meer worden toegewezen.
* De gebruiker kan niet meer aan updates worden toegevoegd.
* De gebruiker kan niet meer aan teams of groepen worden toegevoegd.
* Objecten kunnen niet meer met de gebruiker worden gedeeld.
* Hun associatie met de volgende objecten blijft intact:

   * Taken, kwesties, projecten, portefeuilles
   * Dashboards

     >[!NOTE]
     >
     >Als u een gebruiker deactiveert en niet meer de rapporten of dashboards kan bekijken verbonden aan een gebruiker, kunt u **dit rapport met de Rechten van de Toegang van moeten bijwerken:** gebied.\
     >Om meer te leren, zie [ waarom geen tot een rapport kan toegang hebben dat door een gedeactiveerde gebruiker wordt bezeten?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) sectie van het [ artikel van Veelgestelde vragen van Rapporten ](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

   * Documenten
   * Updates
   * Uren

* Als de gebruiker uitgecheckte documenten heeft, blijven de documenten uitgecheckt wanneer u ze deactiveert. Alleen een Workfront-beheerder kan ze weer inchecken. Voor meer informatie over het controleren van documenten, zie [ Controle uit documenten ](../../../documents/managing-documents/check-out-documents.md).

Wanneer u een gebruiker verwijdert, gebeurt het volgende:

* Verwijdert de gebruikerslicenties voor zowel Workfront als Workfront Proof als de Workfront Proof-component aan uw Workfront-account is gekoppeld. Voor meer informatie over Workfront Proof, zie [ Workfront Proof: artikelindex ](../../../workfront-proof/workfront-proof.md).
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
     >Meer leren, zie [ hoe ik tot een dashboard toegang heb dat een rapport bevat dat door een geschrapte gebruiker wordt bezeten?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) sectie van het [ artikel van Veelgestelde vragen van Rapporten ](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

   * Updates
   * Uren

     >[!NOTE]
     >
     >Deze objecten blijven in Workfront staan, maar de eigenaar van het object is nu leeg.

* Als de gebruiker documenten heeft geüpload onder het gebied Documenten in de algemene navigatiebalk, worden de documenten ook verwijderd.
* Als de gebruiker documenten heeft uitgecheckt die hij of zij bezit en de documenten in het belangrijkste gebied van Documenten (betreden van het Belangrijkste Menu) worden geupload, worden de documenten geschrapt met de gebruiker. Voor meer informatie over het controleren van documenten, zie [ Controle uit documenten ](../../../documents/managing-documents/check-out-documents.md).

Voor meer informatie over het deactiveren van gebruikers, zie [ een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) deactiveren of reactiveren.

U kunt gebruikers een voor een permanent verwijderen of u kunt meerdere gebruikers tegelijk permanent verwijderen. Wanneer u afzonderlijke gebruikers verwijdert, moet u wachten tot het verwijderingsproces is voltooid voordat u verdergaat met andere activiteiten in Workfront. Het verwijderen van meerdere gebruikers wordt tegelijkertijd als een achtergrondproces uitgevoerd, zodat u Workfront kunt blijven gebruiken terwijl de gebruikers worden verwijderd.

## Een of meer gebruikers verwijderen

{{step-1-to-users}}

1. Selecteer minstens één gebruiker die u wilt schrappen, het Meer menu ![ Meer pictogram ](assets/more-icon.png) klikken, dan **Schrapping** klikken.
1. In de doos die verschijnt, klik **Schrapping** om de schrapping te bevestigen.

   Het verwijderen van gebruikers wordt als een achtergrondproces uitgevoerd, zodat u Workfront kunt blijven gebruiken terwijl de gebruiker of gebruikers worden verwijderd.

   Afhankelijk van het aantal gebruikers dat u verwijdert, kan het proces enkele minuten of zelfs een paar uur duren.

   Nadat u in Workfront hebt bevestigd dat de gebruikers zijn verwijderd, kunt u ze in het systeem blijven zien totdat het verwijderingsproces op de achtergrond is voltooid.

   Als u later ontdekt dat een of meer gebruikers niet zijn verwijderd, probeert u deze één voor één te verwijderen.
