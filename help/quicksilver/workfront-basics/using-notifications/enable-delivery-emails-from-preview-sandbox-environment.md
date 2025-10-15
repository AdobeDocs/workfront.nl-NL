---
navigation-topic: notifications
title: Verzending van e-mails vanuit de voorbeeldsandbox-omgeving inschakelen
description: Als u e-mailmeldingen wilt ontvangen vanuit de omgeving van de voorvertoningssandbox, moet u deze functionaliteit inschakelen in uw gebruikersinstellingen wanneer u bent aangemeld bij Voorvertoning.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: 770e20cf9e32ac9884f5eb320f7067fcf162c63d
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Verzending van e-mails vanuit de voorbeeldsandbox-omgeving inschakelen

[!UICONTROL Adobe Workfront] schakelt alle e-mailcommunicatie uit vanuit de omgeving van de voorvertoning en de aangepaste sandbox. Voor informatie over het milieu van de zandbak van de Voorproef, zie [ het Milieu van Sandbox van de Voorproef van Adobe Workfront ](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). Voor informatie over de Douane verfrist het milieu van Sandbox, zie [ de Douane van Adobe Workfront vernieuwt het milieu van Sandbox ](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Als u de volgende e-mailmeldingen wilt ontvangen vanuit de omgeving van de voorvertoningssandbox, moet u deze functionaliteit inschakelen in uw gebruikersinstellingen wanneer u bent aangemeld bij Voorvertoning:

* E-mailmeldingen die worden geactiveerd door gebeurtenismeldingen
* Herinneringsmeldingen
* Automatische meldingen van late of vroege herinneringen
* E-mailuitnodigingen

U kunt dit voor uzelf of voor elke gebruiker doen die u kunt bewerken. Voor meer informatie over de toegang nodig om gebruikers uit te geven, zie [ toegang van de Verlening tot gebruikers ](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>Leverings- en pushberichten van rapporten op de mobiele app zijn altijd uitgeschakeld voor de voorvertoningssandbox-omgeving. De beheerder van [!DNL Workfront] kan het verzenden van rapporten of pushmeldingen voor de mobiele app niet inschakelen wanneer u de omgeving van de voorvertoningssandbox opent.
>
>Voor informatie over rapportleveringen, zie [ de leveringsoverzicht van het Rapport ](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie</strong></td> 
   <td> 
   <p>Medewerker of hoger om uw eigen instelling te wijzigen</p> <p>Standaard voor het bewerken van de instelling voor andere gebruikers</p> 
   of
   <p> Verzoek of hoger om uw eigen instelling te wijzigen</p> <p>De instelling voor andere gebruikers bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau</strong></td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>Het toegangsniveau van [!UICONTROL System Administrator].</p> </li> 
     <li> <p>In uw toegangsniveau, moet [!UICONTROL Edit] voor het [!UICONTROL Users] plaatsen worden geselecteerd. En voor de instelling [!UICONTROL Users] onder [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> moeten de optie [!UICONTROL Create] en ten minste een van de twee opties [!UICONTROL User Admin] zijn ingeschakeld. </li> 
     <li>Als u de optie [!UICONTROL User Admin (Group Users)] gebruikt, moet u een groepsbeheerder van een groep zijn waar de gebruiker een lid is.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De levering van e-mails vanuit de voorbeeldsandbox-omgeving inschakelen

1. Meld u aan bij de voorbeeldsandbox-omgeving.
1. Klik op de profielafbeelding in de rechterbovenhoek van [!DNL Adobe Workfront] . Klik vervolgens op het menu **[!UICONTROL More]** en selecteer **[!UICONTROL Edit]** .

   of

   Zoek naar een gebruiker in [!DNL Workfront] en klik hun naam. Klik vervolgens op het menu **[!UICONTROL More]** en selecteer **[!UICONTROL Edit]** .

   of

   Voor veelvoudige gebruikers: Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste menupictogram ](assets/main-menu-icon.png) in de hoger-juiste hoek van Workfront, dan klik **[!UICONTROL Users]** ![ pictogram van de Gebruiker ](assets/users-icon-in-main-menu.png).  Selecteer vervolgens meerdere gebruikers en klik op **[!UICONTROL Edit]** .

1. Klik op **[!UICONTROL Preferences]**.
1. Selecteer **[!UICONTROL Receive emails from this test environment]**.

   >[!NOTE]
   >
   >Deze optie is niet beschikbaar als u zich in een productieomgeving bevindt.

1. Klik op **[!UICONTROL Save Changes]**.
