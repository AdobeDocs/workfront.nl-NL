---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: Ondernemingslidmaatschappen beheren
description: In de [!UICONTROL Companies] in Opstelling, kunt u de leden van een bedrijf toevoegen en verwijderen. U kunt ook hun gebruikersprofielen bewerken, ze eraan herinneren zich te registreren [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] systeem.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 1%

---

# Ondernemingslidmaatschappen beheren

In de [!UICONTROL Companies] gebied in [!UICONTROL Setup], kunt u leden van een bedrijf toevoegen en verwijderen. U kunt ook hun gebruikersprofielen bewerken, ze eraan herinneren zich te registreren [!DNL Workfront], deactiveert u [!DNL Workfront]en verwijdert deze uit de [!DNL Workfront] systeem.

Voor informatie over het creëren van een nieuw bedrijf, zie [Bedrijven maken en bewerken](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## Toegangsvereisten

U moet over het volgende beschikken om bedrijven te kunnen beheren in [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plan*</p> </td> 
   <td>[!UICONTROL Team] of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licentie*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong> </td> 
   <td> <p>Een van de volgende opties:</p> 
    <ul> 
     <li> <p>De [!UICONTROL System Administrator] toegangsniveau, dat u toestaat om het even welk bedrijf in het systeem uit te geven. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>. </p> </li> 
     <li> <p>Administratieve toegang om bedrijven te beheren, die u toestaat om het even welk bedrijf in het systeem uit te geven. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> </li> 
    </ul> <p><b>OPMERKING</b>:  
     <ul> 
      <li> <p>U kunt ook bedrijven beheren die zijn gekoppeld aan een groep waaraan u als groepsbeheerder bent toegewezen.</p> </li> 
      <li> <p>Om gebruikers toe te voegen aan en te verwijderen uit de [!DNL Workfront] -systeem hebt u een van de volgende mogelijkheden:</p> 
       <ul> 
        <li> <p>De [!UICONTROL System Administrator] toegangsniveau. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>. </p> </li> 
        <li> <p>In uw toegangsniveau, [!UICONTROL Edit] moet worden geselecteerd voor de [!UICONTROL Users] instellen. Ook voor de [!UICONTROL Users] instellen, onder [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> de [!UICONTROL Create] en ten minste één van beide [!UICONTROL User Admin] moeten opties zijn ingeschakeld. </p> <p> <img src="assets/access-req-users.png"> </p> <p>Als u het [!UICONTROL User Admin (Group Users)] moet u een groepsbeheerder zijn van een groep waarvan de gebruiker lid is.</p> </li> 
       </ul> <p>Voor informatie over de Gebruikers die in een toegangsniveau plaatsen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Ondernemingslidmaatschappen beheren

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik op **[!UICONTROL Companies]**.
1. Klik op de naam van het bedrijf.
1. Met de **[!UICONTROL Company Members]** in het linkerdeelvenster geselecteerd, voert u een van de volgende handelingen uit:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Een lid toevoegen</td> 
      <td> <p>Klikken <b>[!UICONTROL Add member]</b>Selecteer vervolgens een van de volgende opties in het keuzemenu dat wordt weergegeven:</p> 
       <ul> 
        <li> <p><b>[!UICONTROL New user]</b>: Een gebruiker toevoegen waaraan nog niet is toegevoegd [!DNL Workfront].</p> <p>Voor informatie over het toevoegen van gebruikers aan [!DNL Workfront], zie <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Gebruikers toevoegen</a> en <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Gebruikersprofiel bewerken</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: Voeg een gebruiker toe die al in het systeem bestaat en die u kunt bewerken.</p> <p><b>BELANGRIJK</b>: Als de gebruiker reeds een lid van een ander bedrijf is, treedt de nieuwe taak oude met voeten. De gebruiker verliest toegang tot punten die met het vorige bedrijf worden gedeeld en krijgt toegang tot punten die met dit bedrijf worden gedeeld.</p> </li> 
        <li> <p><b>[!UICONTROL Import Users]</b>: Importeer een gebruiker door een spreadsheet-importbestand te uploaden. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">Gebruikers importeren</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Leden bewerken</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Selecteer ten minste één gebruiker en klik op de knop [!UICONTROL Edit] pictogram <img src="assets/edit-icon.png"> in de werkbalk.</p> </li> 
        <li value="2"> <p>Configureer de opties in het dialoogvenster <b>[!UICONTROL Edit User]</b> weergegeven.</p> <p>Voor informatie over deze opties raadpleegt u <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Gebruikersprofiel bewerken</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lid kopiëren</td> 
      <td> <p>U kunt een lid van het bedrijf tot stand brengen door bestaande te kopiëren. </p> <p><b>OPMERKING</b>:  <p>Wanneer u op deze manier een gebruiker maakt, wordt alle informatie van de oorspronkelijke gebruiker naar de nieuwe gebruiker gekopieerd, behalve de volgende:</p> 
        <ul> 
         <li>De informatie in de [!UICONTROL Personal Info] sectie.</li> 
         <li>[!UICONTROL When I log in, show]: Het standaardlandingslusje voor het toegangsniveau wordt geselecteerd in dit vakje.</li> 
         <li>[!UICONTROL Direct Reports]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>Selecteer de gebruiker en klik op de knop [!UICONTROL Copy] pictogram <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>In de <b>[!UICONTROL New User]</b> de velden die beschikbaar zijn voor de nieuwe gebruiker bewerken.</p> <p>Voor informatie over alle gebieden verbonden aan een gebruiker, zie <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Gebruikersprofiel bewerken</a>.</p> </li> 
        <li value="3"> <p>Klik op <strong>[!UICONTROL Add This User]</strong>.</p> <p>of</p> <p>Klikken <strong>[!UICONTROL Add Person User & Start Another]</strong> om de nieuwe gebruiker op te slaan en een andere gebruiker toe te voegen.</p> </li> 
       </ol> <p>Hiermee maakt u een nieuwe account in [!DNL Workfront] voor de gebruiker.</p> <p>Als u de optie hebt geselecteerd om een uitnodiging naar de gebruiker te verzenden, ontvangen zij een e-mail waarin zij een koppeling kunnen volgen om hun [!DNL Workfront] wachtwoord.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gebruikers verwijderen</td> 
      <td> 
       <div> 
        <p>Selecteer minstens één gebruiker, klik <b>[!UICONTROL Remove users]</b>Selecteer vervolgens een van de volgende opties in het keuzemenu dat wordt weergegeven:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Remove from company]</b>: Hiermee verwijdert u de gebruiker of gebruikers uit het bedrijf.</p> </li> 
         <li> <p><b>[!UICONTROL Delete]</b>: Hiermee verwijdert u de gebruiker of gebruikers uit het dialoogvenster [!DNL Workfront] systeem.</p> <p><b>BELANGRIJK</b>: Als u een gebruiker uit het systeem verwijdert, wordt ook de informatie verwijderd die is gekoppeld aan de gebruiker die u mogelijk wilt behouden. We raden u aan gebruikers te deactiveren in plaats van ze te verwijderen. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Een gebruiker deactiveren of opnieuw activeren</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Opmerkingen verzenden naar gebruikers en hun [!UICONTROL Updates] gebieden</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Selecteer ten minste één gebruiker en klik op de knop [!UICONTROL Comment] pictogram <img src="assets/comment-icon.png"> in de werkbalk.</p> </li> 
        <li value="2"> <p>Typ de opmerking die u naar de gebruikers en naar de [!UICONTROL Updates] van hun gebruikersprofielen.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">De lijst met bedrijfsleden exporteren</td> 
      <td> <p>Klik op de knop [!UICONTROL Export] pictogram <img src="assets/export.png"> Selecteer vervolgens de gewenste indeling voor het geëxporteerde bestand in de werkbalk.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Leden in het systeem deactiveren</td> 
      <td> <p>Selecteer minstens één gebruiker, klik [!UICONTROL More] pictogram <img src="assets/more-icon.png"> in de werkbalk selecteert u vervolgens <b>[!UICONTROL Deactivate]</b>.</p> <p>Zie voor meer informatie <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Een gebruiker deactiveren of opnieuw activeren</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Een gebruiker herinneren zich te registreren in het systeem</td> 
      <td> <p> In de <b>[!UICONTROL Name]</b> kolom, <b>[!UICONTROL Unregistered]</b> wordt weergegeven naast de naam van elke niet-geregistreerde gebruiker. Als u deze gebruikers wilt herinneren zich te registreren in het systeem, selecteert u de gebruikers en klikt u op de knop [!UICONTROL More] pictogram <img src="assets/more-icon.png"> in de werkbalk selecteert u vervolgens <b>[!UICONTROL Remind user to register]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
