---
user-type: administrator
product-area: system-administration;user-management
keywords: toevoegen,gebruikers,groep,toevoegen,een andere,toewijzen,beheerder,verwijderen,gebruiker,weergave,rollen,leden,exporteren,lidmaatschap,gegevens
navigation-topic: create-and-manage-groups
title: De groepslidmaatschappen weergeven en beheren
description: Als Adobe Workfront-beheerder kunt u leden van elke groep die u beheert, weergeven, toevoegen, verwijderen, exporteren, activeren en deactiveren. U kunt ook hun profielen bewerken, Updates toevoegen aan hun profielen en deze toewijzen als extra groepbeheerders voor de groep.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 1%

---

# De groepslidmaatschappen weergeven en beheren

Als Adobe Workfront-beheerder kunt u leden van elke groep die u beheert, weergeven, toevoegen, verwijderen, exporteren, activeren en deactiveren. U kunt ook hun profielen bewerken, Updates toevoegen aan hun profielen en deze toewijzen als extra groepbeheerders voor de groep.

Als er om het even welke groepen boven uw groep zijn, kunnen hun beheerders deze dingen voor uw groep ook doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-abonnement*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> <p>U moet een groepsbeheerder van de groep of een beheerder van Workfront zijn. Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Groepbeheerders</a> en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de Workfront-beheerder als u wilt weten welk abonnement- of licentietype u hebt.

## De groepslidmaatschappen weergeven en beheren

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Groepen**.

   In de lijst die wordt weergegeven, kunnen Workfront-beheerders alle groepen en subgroepen zien. Groepbeheerders kunnen alleen de groepen en subgroepen zien die zij beheren.

1. Klik op de naam van de groep die u wilt bewerken.
1. Op de pagina die wordt weergegeven, met **Groepsleden** Selecteer in het linkermenu en voer een van de volgende handelingen uit:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Een gebruiker toevoegen aan de groep</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Klikken <strong>Leden toevoegen</strong> <img src="assets/add-icon-plus-in-circle.png">, typt u de naam van de gebruiker en selecteert u deze wanneer deze wordt weergegeven.</li> 
        <li value="2"> <p>Herhaal dit voor alle andere gebruikers die u wilt toevoegen.</p> <p>U kunt op de X rechts van een naam klikken als u besluit die gebruiker niet toe te voegen.</p> </li> 
        <li value="3">Klikken <strong>Gereed</strong> als u klaar bent.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een gebruiker uit de groep verwijderen</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Selecteer een of meer gebruikersnaam en klik op <strong>Lid verwijderen</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li value="2"> <p>Klikken <strong>Verwijderen</strong> in het waarschuwingsbericht dat wordt weergegeven.</p> <p>U kunt een gebruiker vinden u uit de lijst wilt verwijderen door te klikken <strong>Personen en groepen in de lijst zoeken</strong>, typt u de naam in het vak en klikt u vervolgens op de naam wanneer deze wordt weergegeven.</p> <p><b>OPMERKING</b>:  
          <ul> 
           <li>Als deze groep de thuisgroep is voor een gebruiker die u wilt verwijderen, moet u eerst een andere thuisgroep toewijzen in het gebruikersprofiel. Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">Overzicht van thuisgroepen</a> en <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Gebruikersprofiel bewerken</a>.</li> 
           <li>Als de groep slechts één groepsbeheerder heeft en u moet hem of haar uit de groep verwijderen, moet u een andere groepsbeheerder aan de groep eerst toewijzen.</li> 
           <li>Een gebruiker kan afzonderlijk tot een subgroep evenals tot de oudergroep behoren. Wanneer u iemand uit een subgroep verwijdert, blijven deze deel uitmaken van de bovenliggende groep. Als u ze verwijdert uit de bovenliggende groep, blijven ze ook deel uitmaken van de subgroep. Als u niet wilt dat een gebruiker de toegang voor de oudergroep wordt toegestaan, moet u de gebruiker zowel uit subgroepen als de oudergroep verwijderen, als zij op beide plaatsen individueel vermeld zijn.</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Profielgegevens van een gebruiker bewerken</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Selecteer een of meer gebruikersnaam en klik op <strong>Bewerken</strong> <img src="assets/edit-icon.png">.</li> 
        <li value="2"> <p>Wijzig de profielgegevens van de gebruiker.</p> <p>Voor informatie over de wijzigingen die u kunt aanbrengen, raadpleegt u <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Gebruikersprofiel bewerken</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gebruikerslidmaatschapsgegevens exporteren</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Selecteer een of meer gebruikersnaam en klik op <strong>Exporteren</strong> <img src="assets/export.png">.</li> 
        <li value="2"> <p>Exporteer de gegevens als een door PDF, Excel of tabs gescheiden bestand.</p> <p>Voor meer informatie over het exporteren van gegevens raadpleegt u <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Gegevens exporteren</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Groeprollen van leden weergeven en bewerken</td> 
      <td> <p>De <strong>Groepsrol</strong> de kolom maakt een lijst van de rol van elk lid. Als groepsbeheerder, kunt u de rol van een lid tweemaal klikken om het te veranderen.</p> <p>Voor leden van de groep die geen groepsbeheerders zijn, is deze kolom niet editable.</p> <p>De beheerders van de groep zijn altijd bij de bovenkant van de lijst.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een opmerking verzenden naar groepsleden</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Selecteer een of meer gebruikersnaam en klik op <strong>Bijwerken</strong> <img src="assets/comment-icon.png">.</li> 
        <li value="2">Typ de opmerking.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een gebruiker in Workfront activeren</td> 
      <td>Selecteer een of meer inactieve gebruikers en klik op <strong>Gebruiker activeren</strong> om ze te activeren in Workfront. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een gebruiker deactiveren in Workfront</td> 
      <td>Selecteer een of meer actieve gebruikers en klik op <strong>Gebruiker deactiveren</strong><img src="assets/deactivate-user.png"> om ze te deactiveren in Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sorteren op kolom</td> 
      <td>Klik op de kop van een kolom om de lijst te sorteren op de inhoud in die kolom.</td> 
     </tr> 
    </tbody> 
   </table>
