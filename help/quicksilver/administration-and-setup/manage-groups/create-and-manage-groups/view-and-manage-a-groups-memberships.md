---
user-type: administrator
product-area: system-administration;user-management
keywords: toevoegen,gebruikers,groep,toevoegen,een andere,toewijzen,beheerder,verwijderen,gebruiker,weergave,rollen,leden,exporteren,lidmaatschap,gegevens
navigation-topic: create-and-manage-groups
title: De lidmaatschappen van een groep weergeven en beheren
description: Als Adobe Workfront-beheerder kunt u leden van elke groep die u beheert, weergeven, toevoegen, verwijderen, exporteren, activeren en deactiveren. U kunt ook hun profielen bewerken, Updates toevoegen aan hun profielen en deze toewijzen als extra groepbeheerders voor de groep.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 1%

---

# De groepslidmaatschappen weergeven en beheren

Als Adobe Workfront-beheerder kunt u leden van elke groep die u beheert, weergeven, toevoegen, verwijderen, exporteren, activeren en deactiveren. U kunt ook hun profielen bewerken, Updates toevoegen aan hun profielen en deze toewijzen als extra groepbeheerders voor de groep.

Als er om het even welke groepen boven uw groep zijn, kunnen hun beheerders deze dingen voor uw groep ook doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

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
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>U moet een groepsbeheerder van de groep of een systeembeheerder zijn.</td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De groepslidmaatschappen weergeven en beheren

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen**.

   In de lijst die wordt weergegeven, kunnen Workfront-beheerders alle groepen en subgroepen zien. Groepbeheerders kunnen alleen de groepen en subgroepen zien die zij beheren.

1. Klik op de naam van de groep die u wilt bewerken.
1. Op de pagina die verschijnt, met **de Leden van de Groep** geselecteerd in het linkermenu, doe om het even welke volgend:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Een gebruiker toevoegen aan de groep</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Klik <strong> toevoegen Leden </strong> <img src="assets/add-icon-plus-in-circle.png">, beginnen de naam van de gebruiker te typen, dan het selecteren wanneer het verschijnt.</li> 
        <li value="2"> <p>Herhaal dit voor alle andere gebruikers die u wilt toevoegen.</p> <p>U kunt op de X rechts van een naam klikken als u besluit die gebruiker niet toe te voegen.</p> </li> 
        <li value="3">Klik <strong> Gedaan </strong> wanneer u wordt gebeëindigd.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een gebruiker uit de groep verwijderen</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Selecteer één of meerdere gebruikersnaam, dan klik <strong> verwijdert lid </strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li value="2"> <p>Klik <strong> verwijderen </strong> in het waarschuwingsbericht dat toont.</p> <p>U kunt een gebruiker vinden u uit de lijst wilt verwijderen door <strong> mensen en groepen van het Onderzoek in de lijst </strong> te klikken, die hun naam in de doos typen, dan de naam te klikken wanneer het verschijnt.</p> <p><b> NOTA </b>:  
          <ul> 
           <li>Als deze groep de thuisgroep is van een gebruiker die u wilt verwijderen, moet u eerst een andere thuisgroep in het gebruikersprofiel toewijzen. Voor meer informatie, zie <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref"> overzicht van de Groepen van het Huis </a> en <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref"> geef het profiel van een gebruiker </a> uit.</li> 
           <li>Als de groep slechts één groepsbeheerder heeft en u moet hem of haar uit de groep verwijderen, moet u een andere groepsbeheerder aan de groep eerst toewijzen.</li> 
           <li>Een gebruiker kan afzonderlijk tot een subgroep evenals tot de oudergroep behoren. Wanneer u iemand uit een subgroep verwijdert, blijven deze deel uitmaken van de bovenliggende groep. Als u ze verwijdert uit de bovenliggende groep, blijven ze ook deel uitmaken van de subgroep. Als u niet wilt dat een gebruiker de toegang voor de oudergroep wordt toegestaan, moet u de gebruiker zowel uit subgroepen als de oudergroep verwijderen, als zij op beide plaatsen individueel vermeld zijn.</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Profielgegevens van een gebruiker bewerken</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Selecteer één of meerdere gebruikersnaam, dan klik <strong> uitgeven </strong> <img src="assets/edit-icon.png">.</li> 
        <li value="2"> <p>Wijzig de profielgegevens van de gebruiker.</p> <p>Voor informatie over de veranderingen u kunt maken, zie <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref"> het profiel van een gebruiker </a> uitgeven.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gebruikerslidmaatschapsgegevens exporteren</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Selecteer één of meerdere gebruikersnaam, dan klik <strong> Uitvoer </strong> <img src="assets/export.png">.</li> 
        <li value="2"> <p>Exporteer de gegevens als een door PDF, Excel of tabs gescheiden bestand.</p> <p>Voor meer informatie over het uitvoeren van gegevens, zie <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref"> Gegevens van de Uitvoer </a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Groeprollen van leden weergeven en bewerken</td> 
      <td> <p>De <strong> kolom van de Rol van de Groep </strong> maakt een lijst van de rol van elk lid. Als groepsbeheerder, kunt u de rol van een lid tweemaal klikken om het te veranderen.</p> <p>Voor leden van de groep die geen groepsbeheerders zijn, is deze kolom niet editable.</p> <p>De beheerders van de groep zijn altijd bij de bovenkant van de lijst.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een opmerking verzenden naar groepsleden</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Selecteer één of meerdere gebruikersnaam, dan klik <strong> Update </strong> <img src="assets/comment-icon.png">.</li> 
        <li value="2">Typ de opmerking.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een gebruiker in Workfront activeren</td> 
      <td>Selecteer één of meerdere inactieve gebruikers, dan klik <strong> activeer gebruiker </strong> om hen in Workfront te activeren. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een gebruiker deactiveren in Workfront</td> 
      <td>Selecteer één of meerdere actieve gebruikers, dan klik <strong> deactivate gebruiker </strong><img src="assets/deactivate-user.png"> om hen in Workfront te deactiveren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sorteren op kolom</td> 
      <td>Klik op de kop van een kolom om de lijst te sorteren op de inhoud in die kolom.</td> 
     </tr> 
    </tbody> 
   </table>
