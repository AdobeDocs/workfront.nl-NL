---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Configuratie van gebeurtenismeldingen voor alle groepen ontgrendelen of vergrendelen
description: Als u een Adobe Workfront-beheerder bent, kunt u de mogelijkheid voor groepsbeheerders ontgrendelen of opnieuw vergrendelen om een gebeurtenismelding te configureren voor groepen op hoofdniveau die zij beheren. Configuratie van een gebeurtenismelding bestaat uit het activeren of deactiveren ervan.
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: 325fb9e58d32d1b6cfa1035cd4a25da4b66f6955
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Configuratie van gebeurtenismeldingen voor alle groepen ontgrendelen of vergrendelen

Als u een Adobe Workfront-beheerder bent, kunt u de mogelijkheid voor groepsbeheerders ontgrendelen of opnieuw vergrendelen om een gebeurtenismelding te configureren voor groepen op hoofdniveau die zij beheren. Configuratie van een gebeurtenismelding bestaat uit het activeren of deactiveren ervan.

Als er groepen zijn boven de groep die u beheert, kunnen hun beheerders dit ook voor uw groep doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

Wanneer een beheerder een gebeurtenisbericht voor een groep vormt, beïnvloedt de configuratie gebruikers voor wie die groep, of één van zijn subgroepen, hun Groep van het Huis is. In hun gebruikersprofielen zien deze gebruikers de gebeurtenismeldingen die voor hun thuisgroep zijn geactiveerd in plaats van de gebeurtenismeldingen die voor het hele systeem zijn geactiveerd. Zie voor meer informatie [Gebeurtenismeldingen voor een groep weergeven en configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Een Workfront-beheerder kan de configuratie voor een gebeurtenismelding ontgrendelen en opnieuw vergrendelen in zowel Adobe Workfront Classic als de nieuwe Adobe Workfront-ervaring. Maar een groepsbeheerder kan dat gebeurtenisbericht voor een groep slechts in de nieuwe ervaring van Adobe Workfront vormen. Groepbeheerders die Adobe Workfront Classic gebruiken, kunnen overschakelen naar de nieuwe Adobe Workfront-ervaring om ontgrendelde gebeurtenismeldingen voor een groep te configureren, en vervolgens terugschakelen naar Adobe Workfront Classic om de wijzigingen te zien.
>* Subgroepen erven de configuraties van gebeurtenismeldingen op groepsniveau van de groepen op hoofdniveau erboven.
>

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

## De mogelijkheid om een gebeurtenismelding te configureren ontgrendelen of opnieuw vergrendelen

>[!IMPORTANT]
>
>Wanneer u een bericht opnieuw vergrendelt, nemen alle groepen in het systeem het bericht precies over zoals u het instelt. Dit treedt om het even welke veranderingen met voeten die de groepsbeheerders voor hun groepen zouden kunnen hebben aangebracht, zodat is het een goed idee eerst met hen te raadplegen.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **E-mail** > **Meldingen**.

1. Zorg ervoor dat de **Gebeurtenismeldingen** is geopend.
1. Klik op het pictogram rechts van het bericht om het naar de vergrendelde versie te verplaatsen ![Vergrendelingspictogram](assets/lock-toggle-button.png) of ontgrendeld ![Pictogram Ontgrendelen](assets/unlock-toggle-button.png) positie.

   of

   Als u meerdere meldingen tegelijk wilt ontgrendelen of vergrendelen, selecteert u deze en klikt u op de knop Ontgrendelen ![Pictogram Ontgrendelen](assets/unlock-icon-toolbar.png) of Vergrendelen ![Vergrendelingspictogram](assets/lock-icon-locked-qs.png) in de werkbalk boven de lijst.

1. Klikken **Opslaan**.
1. (Optioneel) Als u het gebeurtenisbericht voor een groep op hoofdniveau wilt configureren in plaats van deze taak over te laten aan de beheerder van de groep, kunt u een van de volgende handelingen uitvoeren:

   * Verwijderen **Systeemgebeurtenismeldingen** in het zoekvak boven de lijst met meldingen zoekt u de naam van de bovenste groep om de meldingen weer te geven. Vervolgens activeert of activeert u de ontgrendelde berichten in de lijst die wordt weergegeven.
   * Klikken **Groepen** in het linkermenu, dan klik de naam van de top-level groep. Klikken **Gebeurtenismeldingen** in het linkerdeelvenster, configureert u vervolgens de ontgrendelde gebeurtenismelding, zoals wordt uitgelegd in [Gebeurtenismeldingen voor een groep weergeven en configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
