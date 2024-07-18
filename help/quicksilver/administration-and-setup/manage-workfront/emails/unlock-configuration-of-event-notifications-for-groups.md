---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Configuratie van gebeurtenismeldingen voor alle groepen ontgrendelen of vergrendelen
description: Als u een Adobe Workfront-beheerder bent, kunt u de mogelijkheid voor groepsbeheerders ontgrendelen of opnieuw vergrendelen om een gebeurtenismelding te configureren voor groepen op hoofdniveau die zij beheren. Configuratie van een gebeurtenismelding bestaat uit het activeren of deactiveren ervan.
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Configuratie van gebeurtenismeldingen voor alle groepen ontgrendelen of vergrendelen

Als u een Adobe Workfront-beheerder bent, kunt u de mogelijkheid voor groepsbeheerders ontgrendelen of opnieuw vergrendelen om een gebeurtenismelding te configureren voor groepen op hoofdniveau die zij beheren. Configuratie van een gebeurtenismelding bestaat uit het activeren of deactiveren ervan.

Als er groepen zijn boven de groep die u beheert, kunnen hun beheerders dit ook voor uw groep doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

Wanneer een beheerder een gebeurtenisbericht voor een groep vormt, beïnvloedt de configuratie gebruikers voor wie die groep, of één van zijn subgroepen, hun Groep van het Huis is. In hun gebruikersprofielen zien deze gebruikers de gebeurtenismeldingen die voor hun thuisgroep zijn geactiveerd in plaats van de gebeurtenismeldingen die voor het hele systeem zijn geactiveerd. Voor meer informatie, zie [ Mening en vorm gebeurtenisberichten voor een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

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

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Opstelling** ![](assets/gear-icon-settings.png).

1. Klik **E-mail** > **Meldingen**.

1. Zorg ervoor de **Berichten van de Gebeurtenis** tabel open is.
1. Klik het pictogram aan het recht van het bericht om het aan het gesloten ![ pictogram van het Slot ](assets/lock-toggle-button.png) of ontgrendelde ![ te schakelen ontgrendelen pictogram ](assets/unlock-toggle-button.png) positie.

   of

   Als u veelvoudige berichten wilt ontgrendelen of sluiten allen in één keer, hen selecteren, dan klik het pictogram van de Ontgrendeling ](assets/unlock-icon-toolbar.png) of van het Slot ![ het pictogram van het Slot ](assets/lock-icon-locked-qs.png) knoop dat in de toolbar boven de lijst toont.![

1. Klik **sparen**.
1. (Optioneel) Als u het gebeurtenisbericht voor een groep op hoofdniveau wilt configureren in plaats van deze taak over te laten aan de beheerder van de groep, kunt u een van de volgende handelingen uitvoeren:

   * Schrap {de Berichten van de Gebeurtenis van het 0} Systeem **in het onderzoeksvakje boven de lijst van berichten, onderzoek naar en selecteer de naam van de top-level groep om van zijn berichten een lijst te maken, dan activeer of inactiveer de ontgrendelde berichten in de lijst die toont.**
   * Klik **Groepen** in het linkermenu, dan klik de naam van de top-level groep. Klik {de Meldingen van de Gebeurtenis 0} **in het linkerpaneel, dan vormen het ontgrendelde gebeurtenisbericht, zoals die in [ worden verklaard Mening en vormen gebeurtenisberichten voor een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).**
