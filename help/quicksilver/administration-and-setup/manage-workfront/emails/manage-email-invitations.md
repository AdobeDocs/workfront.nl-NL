---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: E-mailuitnodigingen beheren voor nieuwe gebruikers
description: Als Adobe Workfront-beheerder kunt u gebruikers toevoegen aan Workfront en ze laten weten dat ze zijn toegevoegd met e-mailuitnodigingen.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---

# E-mailuitnodigingen beheren voor nieuwe gebruikers

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet aan boord van de Admin Console zijn gegaan. Als uw organisatie is aangemeld bij de Adobe Admin Console, moet u deze handeling uitvoeren via de Adobe Admin Console.
>
>Voor een lijst met procedures die verschillen afhankelijk van de vraag of uw organisatie al dan niet is aangemeld bij de Adobe Admin Console, raadpleegt u [Op Platform gebaseerde verschillen in beheer (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als Adobe Workfront-beheerder kunt u gebruikers toevoegen aan Workfront en ze laten weten dat ze zijn toegevoegd met e-mailuitnodigingen.

Met de e-mailuitnodiging kunnen nieuwe gebruikers een koppeling volgen waarin ze een wachtwoord voor hun Workfront-account kunnen kiezen. Ze kunnen dan hun accountinstellingen voltooien.

Voor de beveiliging van de nieuwe accounts raden we u aan e-mailuitnodigingen te gebruiken voor nieuwe gebruikers, zodat deze hun eigen wachtwoord kunnen kiezen. U kunt ook een wachtwoord voor een nieuwe gebruiker selecteren wanneer u een account maakt. Ga voor meer informatie over het toevoegen van nieuwe gebruikers aan Workfront naar [Gebruikers toevoegen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

U kunt de e-mails voor nieuwe gebruikers configureren voor:

* Nieuwe gebruiker toegevoegd aan Workfront
* Gebruikers die aan Workfront zijn toegevoegd met een licentie voor aanvragers

Alle nieuwe gebruikers zien hetzelfde e-mailbericht wanneer een e-mailuitnodiging wordt verzonden.

Voor informatie over het ontvangen van e-mailuitnodigingen raadpleegt u [E-mailuitnodigingen ontvangen en een wachtwoord voor Adobe Workfront maken](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

## Toegangsvereisten

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Systeembeheerder</p> </td> 
  </tr> 
 </tbody> 
</table>

## E-mailuitnodigingen genereren {#generate-email-invitations}

E-mailuitnodigingen worden gegenereerd in de volgende scenario&#39;s:

* Wanneer u een nieuwe gebruiker maakt en **Een uitnodigingsbericht sturen naar deze persoon** op de **Nieuwe gebruiker** formulier. Ga voor meer informatie over het maken van nieuwe gebruikers naar [Gebruikers toevoegen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* Wanneer u meerdere nieuwe gebruikers importeert en u **E-mails met uitnodigingen verzenden aan deze personen** optie. Voor meer informatie over het importeren van meerdere nieuwe gebruikers raadpleegt u [Gebruikers importeren](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
* Nadat de gebruikers zijn gemaakt, kunt u de uitnodigingen handmatig genereren voor gebruikers die hun account nog niet bij Workfront hebben geregistreerd en die nog geen Workfront-wachtwoord hebben ingesteld.\
   Gebruikers die een account hebben gemaakt maar hun account nog niet hebben geregistreerd, worden gemarkeerd als **Niet geregistreerd** in Workfront.

   >[!NOTE]
   >
   >Als u de optie **Een e-mailuitnodiging verzenden aan deze persoon** als u de gebruiker maakt, kan de e-mailuitnodiging niet handmatig worden gegenereerd. Het handmatig doorsturen van de e-mailuitnodigingen is alleen mogelijk voor gebruikers die de oorspronkelijke e-mailuitnodiging hebben ontvangen toen hun account werd gemaakt. Ga voor meer informatie over het maken van nieuwe gebruikers naar [Gebruikers toevoegen](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

E-mailuitnodigingen handmatig genereren voor bestaande niet-geregistreerde gebruikers:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Gebruikers** ![](assets/users-icon-in-main-menu.png).
1. Selecteer de gebruiker die de **Niet geregistreerd** label achter hun naam.

   ![](assets/unreg-user-qs-350x221.png)

1. Klik op het pictogram Meer ![](assets/more-icon.png)en klik vervolgens op **Herinneren aan gebruiker om te registreren**.

   Er wordt een e-mailuitnodiging verzonden naar de nieuwe gebruiker met een nieuwe koppeling waarmee deze zijn Workfront-wachtwoord kan maken.

   >[!NOTE]
   >
   >Als uw organisatie is aangemeld bij de Admin Console en u een gebruiker toevoegt via Workfront, kunt u geen e-mailuitnodiging verzenden naar nieuwe gebruikers.
   >
   >De nieuwe gebruikers van de Adobe worden toegevoegd aan de Admin Console, en de Admin Console levert een e-mail om hen uit te nodigen om het registratieproces te voltooien. Alle gebruikers moeten het registratieproces voltooien om tot om het even welk systeem van de Adobe toegang te hebben.
   >
   >Voor bestaande Adobe-gebruikers kan de gebruiker al dan niet een e-mail ontvangen over de beschikbaarheid van Workfront. Dit is een voorkeur die door de beheerder van de Adobe voor het product wordt gecontroleerd.

## E-mailuitnodigingen configureren {#configure-email-invitations}

Als Workfront-beheerder kunt u het bericht dat u opneemt, configureren met de e-mailuitnodigingen voor nieuwe gebruikers.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in de lijst aan de linkerkant op **E-mail** > **Uitnodigingen**.

1. In de **Algemene opties** in, voert u een van de volgende wijzigingen uit:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Uitnodigingskoppelingen deactiveren na ... dagen</strong> </td> 
      <td> <p>Kies de tijdsduur waarna de e-mailuitnodigingen geen geldige koppeling naar Workfront meer bevatten. Het standaardaantal dagen is 45.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Een bericht en/of servicetermijn opnemen</strong> </td> 
      <td> <p>Selecteer deze optie als u de e-mailuitnodiging wilt wijzigen voor alle nieuwe gebruikers die aan Workfront zijn toegevoegd. Dit geldt niet voor gebruikers met een licentie voor aanvragers.</p> 
       <ul> 
        <li><strong>Bericht</strong>: Als u de e-mailuitnodiging voor alle nieuwe gebruikers wilt wijzigen, geeft u de tekst op die u in uw e-mailuitnodigingen wilt opnemen als de e-mailtekst.</li> 
        <li><strong>Voorwaarden en bepalingen</strong>: Als u de e-mailuitnodiging voor alle nieuwe gebruikers wilt wijzigen, geeft u de tekst op die u in uw e-mailuitnodigingen wilt opnemen als de voorwaarden.<br></li> 
        <li><strong>Inclusief een bericht en/of servicetermijn voor helpdeskgebruikers</strong>: Selecteer deze optie als u de e-mailuitnodiging wilt wijzigen voor alle nieuwe gebruikers die aan Workfront zijn toegevoegd en over een licentie voor aanvragers beschikken.</li> 
        <li><strong>Bericht</strong>: Als u de e-mailuitnodiging voor alle nieuwe gebruikers met een licentie voor de aanvrager wilt wijzigen, geeft u de tekst op die u in uw e-mailuitnodigingen wilt opnemen als de e-mailtekst.</li> 
        <li><strong>Voorwaarden en bepalingen</strong>: Als u ervoor kiest de e-mailuitnodiging voor alle nieuwe gebruikers te wijzigen met een licentie voor de aanvrager, geeft u de tekst op die u in uw e-mailuitnodigingen wilt opnemen als de voorwaarden.<br></li> 
        <li> <p>In de <strong>Uitnodigingsvoorbeeld</strong> kunt u een voorbeeld van uw e-mailuitnodiging bekijken. Als u hebt opgegeven dat u een aangepast bericht wilt opnemen in uw e-mailuitnodiging, wordt het aangepaste bericht in dit gebied weergegeven.</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Opslaan**.
