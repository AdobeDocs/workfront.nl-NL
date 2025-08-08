---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Bedrijfslidmaatschap beheren
description: In het gedeelte [!UICONTROL Companies] in Setup kunt u de leden van een bedrijf toevoegen en verwijderen. U kunt hun gebruikersprofielen ook uitgeven, hen eraan herinneren om in  [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront]  systeem te registreren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: 705fc990f2d90ff2102233fc68947fdbe1eb6946
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 1%

---

# Ondernemingslidmaatschappen beheren

In het gebied [!UICONTROL Companies] in [!UICONTROL Setup] kunt u de leden van een bedrijf toevoegen en verwijderen. U kunt ook hun gebruikersprofielen bewerken, ze eraan herinneren zich te registreren in [!DNL Workfront] , ze te deactiveren in [!DNL Workfront] en ze uit het [!DNL Workfront] -systeem verwijderen.

Voor informatie over het creëren van een nieuw bedrijf, zie [ bedrijven ](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md) creëren en uitgeven.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan</p> </td> 
   <td><p>Huidig: [!UICONTROL Team] of hoger</p>
   <p>of</p>
   <p>Nieuw: alle</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licentie</p> </td> 
   <td><p>Huidige: [!UICONTROL Plan]</p>
   <p>of</p>
   <p>Nieuw: [!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong> het niveauconfiguraties van de Toegang </strong> </td> 
   <td> <p>Een van de volgende opties:</p> 
    <ul> 
     <li> <p>Het toegangsniveau van [!UICONTROL System Administrator], dat u toestaat om het even welk bedrijf in het systeem uit te geven.</p> </li> 
     <li> <p>Administratieve toegang om bedrijven te beheren, die u toestaat om het even welk bedrijf in het systeem uit te geven.</p> </li> 
    </ul> <p><b> NOTA </b>:  
     <ul> 
      <li> <p>U kunt ook bedrijven beheren die zijn gekoppeld aan een groep waaraan u als groepsbeheerder bent toegewezen.</p> </li> 
      <li> <p>Als u gebruikers wilt toevoegen aan en verwijderen uit het [!DNL Workfront] -systeem, moet u een van de volgende opties hebben:</p> 
       <ul> 
        <li> <p>Het toegangsniveau van [!UICONTROL System Administrator].</p> </li> 
        <li> <p>In uw toegangsniveau, moet [!UICONTROL Edit] voor het [!UICONTROL Users] plaatsen worden geselecteerd. Voor de instelling [!UICONTROL Users] onder [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> moeten ook de optie [!UICONTROL Create] en ten minste een van de twee opties [!UICONTROL User Admin] zijn ingeschakeld. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Als u de optie [!UICONTROL User Admin (Group Users)] gebruikt, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ondernemingslidmaatschappen beheren

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Companies]**.
1. Klik op de naam van het bedrijf.
1. Klik op **[!UICONTROL Company Members]** in het linkerdeelvenster.
1. Voer een van de volgende handelingen uit:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Een lid toevoegen</td> 
      <td> <p>Klik op <b>[!UICONTROL Add member]</b> en selecteer vervolgens een van de volgende opties in het keuzemenu dat wordt weergegeven:</p> 
       <ul> 
        <li> <p><b>[!UICONTROL New user]</b>: Voeg een gebruiker toe die nog niet aan [!DNL Workfront] is toegevoegd.</p> <p>Voor informatie over het toevoegen van gebruikers aan [!DNL Workfront], zie <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref"> gebruikers </a> toevoegen en <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref"> geef het profiel van een gebruiker </a> uit.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: Voeg een gebruiker toe die al in het systeem bestaat en die u kunt bewerken.</p> <p><b> BELANGRIJK </b>: Als de gebruiker reeds een lid van een ander bedrijf is, treedt de nieuwe taak oude met voeten. De gebruiker verliest toegang tot punten die met het vorige bedrijf worden gedeeld en krijgt toegang tot punten die met dit bedrijf worden gedeeld.</p> </li> 
        <li> <p><b>[!UICONTROL Import Users]</b>: Importeer een gebruiker door een spreadsheet-importbestand te uploaden. Voor meer informatie, zie <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref"> de gebruikers van de Invoer </a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Leden bewerken</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Selecteer ten minste één gebruiker en klik op het pictogram [!UICONTROL Edit] <img src="assets/edit-icon.png"> op de werkbalk.</p> </li> 
        <li value="2"> <p>Configureer de opties in het vak <b>[!UICONTROL Edit User]</b> dat wordt weergegeven.</p> <p>Voor informatie over deze opties, zie <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref"> het profiel van een gebruiker </a> uitgeven.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lid kopiëren</td> 
      <td> <p>U kunt een lid van het bedrijf tot stand brengen door bestaande te kopiëren. </p> <p><b> NOTA </b>:  <p>Wanneer u op deze manier een gebruiker maakt, wordt alle informatie van de oorspronkelijke gebruiker naar de nieuwe gebruiker gekopieerd, behalve de volgende:</p> 
        <ul> 
         <li>De informatie in de sectie [!UICONTROL Personal Info] .</li> 
         <li>[!UICONTROL When I log in, show]: Het standaard landingstabblad voor het toegangsniveau wordt in dit vak geselecteerd.</li> 
         <li>[!UICONTROL Direct Reports]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Selecteer de gebruiker en klik op het pictogram [!UICONTROL Copy] <img src="assets/copy-icon.png"> . </p> </li> 
        <li value="2"> <p>Bewerk in het vak <b>[!UICONTROL New User]</b> dat wordt weergegeven de velden die beschikbaar zijn voor de nieuwe gebruiker.</p> <p>Voor informatie over alle gebieden verbonden aan een gebruiker, zie <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref"> het profiel van een gebruiker </a> uitgeven.</p> </li> 
        <li value="3"> <p>Klik op <strong>[!UICONTROL Add This User]</strong>.</p> <p>of</p> <p>Klik op <strong>[!UICONTROL Add Person User & Start Another]</strong> om de nieuwe gebruiker op te slaan en een andere gebruiker toe te voegen.</p> </li> 
       </ol> <p>Hiermee maakt u een nieuwe account in [!DNL Workfront] voor de gebruiker.</p> <p>Als u de optie hebt geselecteerd om een uitnodiging naar de gebruiker te verzenden, ontvangen zij een e-mail waarin zij een koppeling kunnen volgen om hun [!DNL Workfront] -wachtwoord te maken.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gebruikers verwijderen</td> 
      <td> 
       <div> 
        <p>Selecteer ten minste één gebruiker, klik op <b>[!UICONTROL Remove users]</b> en selecteer vervolgens een van de volgende opties in het vervolgkeuzemenu dat wordt weergegeven:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Remove from company]</b>: Hiermee verwijdert u de gebruiker of gebruikers uit het bedrijf.</p> </li> 
         <li> <p><b>[!UICONTROL Delete]</b>: Hiermee verwijdert u de gebruiker of gebruikers van het [!DNL Workfront] -systeem.</p> <p><b> BELANGRIJK </b>: Het schrappen van een gebruiker uit het systeem schrapt ook informatie verbonden aan de gebruiker die u zou kunnen willen behouden. We raden u aan gebruikers te deactiveren in plaats van ze te verwijderen. Voor meer informatie, zie <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref"> een gebruiker </a> deactiveren of reactiveren.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een opmerking verzenden naar gebruikers en hun [!UICONTROL Updates] gebieden</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Selecteer minstens één gebruiker, dan klik <b> verzenden Update naar Gebruiker </b> in de toolbar.</p> </li> 
        <li value="2"> <p>Typ de opmerking die u naar de gebruikers en naar het gebied [!UICONTROL Updates] van hun gebruikersprofielen wilt verzenden.</p>
         <p>Voor meer informatie, zie <a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md"> directe berichten naar andere gebruikers </a> verzenden.</p></li> 
       </ol>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">De lijst met bedrijfsleden exporteren</td> 
      <td> <p>Klik op het pictogram [!UICONTROL Export] <img src="assets/export.png"> op de werkbalk en selecteer de gewenste indeling voor het geëxporteerde bestand.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Leden in het systeem deactiveren</td> 
      <td> <p>Selecteer ten minste één gebruiker, klik op het pictogram [!UICONTROL More] <img src="assets/more-icon.png"> op de werkbalk en selecteer vervolgens <b>[!UICONTROL Deactivate]</b> .</p> <p>Voor meer informatie, zie <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref"> een gebruiker </a> deactiveren of reactiveren.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Een gebruiker herinneren zich te registreren in het systeem</td> 
      <td> <p> In de kolom <b>[!UICONTROL Name]</b> wordt <b>[!UICONTROL Unregistered]</b> weergegeven naast de naam van elke niet-geregistreerde gebruiker. Als u deze gebruikers wilt herinneren zich te registreren in het systeem, selecteert u de gebruikers, klikt u op het pictogram [!UICONTROL More] <img src="assets/more-icon.png"> op de werkbalk en selecteert u vervolgens <b>[!UICONTROL Remind user to register]</b> .</p> </td> 
     </tr> 
    </tbody> 
   </table>
