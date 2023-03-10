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
source-git-commit: 137165deb0c0e9172224e810c82bc651bb0adfc0
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 0%

---

# Gebruikers verwijderen

Wanneer een gebruiker uw organisatie verlaat, kunt u die gebruiker uit Adobe Workfront verwijderen.

>[!IMPORTANT]
>
>* Als u een gebruiker uit het systeem verwijdert, wordt ook de informatie verwijderd die is gekoppeld aan de gebruiker die u mogelijk wilt behouden. We raden u aan gebruikers te deactiveren in plaats van ze te verwijderen. Zie voor meer informatie [Een gebruiker deactiveren of opnieuw activeren](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
>* De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet aan boord van de Admin Console zijn gegaan. Als uw organisatie is aangemeld bij de Adobe Admin Console, moet u deze handeling uitvoeren via de Adobe Admin Console.
>
>Een gebruiker verwijderen uit het dialoogvenster [!DNL Adobe Admin Console] deactiveert de gebruiker in [!DNL Workfront], maar ze worden niet verwijderd [!DNL Workfront].
>
>  Zie de sectie &quot;Gebruikers definitief verwijderen&quot; in het artikel voor instructies over het verwijderen van een gebruiker in de Adobe Admin Console [Gebruikers individueel beheren](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) of neem contact op met uw Adobe Admin Console-beheerder.
>
>  Voor een lijst met procedures die verschillen afhankelijk van de vraag of uw organisatie al dan niet is aangemeld bij de Adobe Admin Console, raadpleegt u [Op Platform gebaseerde verschillen in beheer (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

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
     <li> <p>Het toegangsniveau van de Beheerder van het Systeem. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>. </p> </li> 
     <li> <p><b>Gebruikers</b> het plaatsen in uw toegangsniveau dat wordt gevormd aan <b>Bewerken</b> toegang, met <b>Maken</b> en ten minste ????n van beide <b>Gebruikersbeheerder</b> opties ingeschakeld onder <b>Uw instellingen nauwkeurig afstellen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Van deze twee opties, als Gebruiker <b>Admin (Groepgebruikers)</b> wordt toegelaten, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> <p>Voor meer informatie over de <b>Gebruikers</b> het plaatsen in een toegangsniveau, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Een gebruiker verwijderen of deactiveren

Als u een gebruiker deactiveert, gebeurt het volgende:

* Verwijdert de gebruikerslicenties voor zowel Workfront als Workfront Proof als de Workfront Proof-component aan uw Workfront-account is gekoppeld. Ga voor meer informatie over Workfront Proof naar [Workfront Proof](../../../workfront-proof/workfront-proof.md).
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

* Als de gebruiker uitgecheckte documenten heeft, blijven de documenten uitgecheckt wanneer u ze deactiveert. Alleen een Workfront-beheerder kan ze weer inchecken. Zie voor meer informatie over het uitchecken van documenten [Documenten uitchecken](../../../documents/managing-documents/check-out-documents.md).

Wanneer u een gebruiker verwijdert, gebeurt het volgende:

* Verwijdert de gebruikerslicenties voor zowel Workfront als Workfront Proof als de Workfront Proof-component aan uw Workfront-account is gekoppeld. Ga voor meer informatie over Workfront Proof naar [Workfront Proof](../../../workfront-proof/workfront-proof.md).
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

* Als de gebruiker documenten heeft ge??pload onder het gebied Documenten in de algemene navigatiebalk, worden de documenten ook verwijderd.
* Als de gebruiker documenten heeft uitgecheckt die hij of zij bezit en de documenten in het belangrijkste gebied van Documenten (betreden van het Belangrijkste Menu) worden geupload, worden de documenten geschrapt met de gebruiker. Zie voor meer informatie over het uitchecken van documenten [Documenten uitchecken](../../../documents/managing-documents/check-out-documents.md).

Voor meer informatie over het deactiveren van gebruikers raadpleegt u [Een gebruiker deactiveren of opnieuw activeren](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

U kunt gebruikers een voor een permanent verwijderen of u kunt meerdere gebruikers tegelijk permanent verwijderen. Wanneer u afzonderlijke gebruikers verwijdert, moet u wachten tot het verwijderingsproces is voltooid voordat u verdergaat met andere activiteiten in Workfront. Het verwijderen van meerdere gebruikers wordt tegelijkertijd als een achtergrondproces uitgevoerd, zodat u Workfront kunt blijven gebruiken terwijl de gebruikers worden verwijderd.

## Een of meer gebruikers verwijderen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront.

1. Klikken **Gebruikers**.
1. Selecteer minstens ????n gebruiker die u wilt schrappen, klik het Meer menu ![](assets/more-icon.png)en klik vervolgens op **Verwijderen**.
1. Klik in het vak dat wordt weergegeven op **Verwijderen** om de schrapping te bevestigen.

   Het verwijderen van gebruikers wordt als een achtergrondproces uitgevoerd, zodat u Workfront kunt blijven gebruiken terwijl de gebruiker of gebruikers worden verwijderd.

   Afhankelijk van het aantal gebruikers dat u verwijdert, kan het proces enkele minuten of zelfs een paar uur duren.

   Nadat u in Workfront hebt bevestigd dat de gebruikers zijn verwijderd, kunt u ze in het systeem blijven zien totdat het verwijderingsproces op de achtergrond is voltooid.

   Als u later ontdekt dat een of meer gebruikers niet zijn verwijderd, probeert u deze ????n voor ????n te verwijderen.
