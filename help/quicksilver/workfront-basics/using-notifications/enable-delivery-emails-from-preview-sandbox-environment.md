---
navigation-topic: notifications
title: Verzending van e-mails vanuit de voorbeeldsandbox-omgeving inschakelen
description: Als u e-mailmeldingen wilt ontvangen vanuit de omgeving van de voorvertoningssandbox, moet u deze functionaliteit inschakelen in uw gebruikersinstellingen wanneer u bent aangemeld bij Voorvertoning.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Verzending van e-mails vanuit de voorbeeldsandbox-omgeving inschakelen

[!UICONTROL Adobe Workfront] Hiermee schakelt u alle e-mailcommunicatie uit vanuit de omgeving van de sandbox Voorvertoning en Aangepast vernieuwen. Voor informatie over de omgeving van de voorvertoningssandbox raadpleegt u [De Adobe Workfront Preview Sandbox-omgeving](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). Voor informatie over de omgeving van de Aangepaste sandbox vernieuwen raadpleegt u [De aangepaste vernieuwingssandbox van Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Als u de volgende e-mailmeldingen wilt ontvangen vanuit de omgeving van de voorvertoningssandbox, moet u deze functionaliteit inschakelen in uw gebruikersinstellingen wanneer u bent aangemeld bij Voorvertoning:

* E-mailmeldingen die worden geactiveerd door gebeurtenismeldingen
* Herinneringsmeldingen
* Automatische meldingen van late of vroege herinneringen
* Uitnodigingen e-mailen

U kunt dit voor uzelf of voor elke gebruiker doen die u kunt bewerken. Voor meer informatie over de toegang nodig om gebruikers uit te geven, zie [Toegang verlenen aan gebruikers](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>Leverings- en pushberichten van rapporten op de mobiele app zijn altijd uitgeschakeld voor de voorvertoningssandbox-omgeving. Noch u noch de [!DNL Workfront] De beheerder kan levering van rapporten of dupberichten voor mobiele app toelaten wanneer u tot de milieu van de Sandbox van de Voorproef toegang hebt.
>
>Voor informatie over rapportleveringen raadpleegt u [Overzicht van levering rapporteren](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Request] of hoger om uw eigen instelling te wijzigen</p> <p>[!UICONTROL Plan] om het plaatsen voor andere gebruikers uit te geven</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>U moet een van de volgende opties hebben:</p> 
    <ul> 
     <li> <p>De [!UICONTROL System Administrator] toegangsniveau.</p> <p> Voor informatie over dit toegangsniveau, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>. </p> </li> 
     <li> <p>In uw toegangsniveau, [!UICONTROL Edit] moet worden geselecteerd voor de [!UICONTROL Users] instellen. En voor de [!UICONTROL Users] instellen, onder [!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> de [!UICONTROL Create] en ten minste één van beide [!UICONTROL User Admin] moeten opties zijn ingeschakeld. </p> <p>Als u het [!UICONTROL User Admin (Group Users)] moet u een groepsbeheerder zijn van een groep waarvan de gebruiker lid is.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>Voor informatie over de [!UICONTROL Users] het plaatsen in een toegangsniveau, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Toegang verlenen aan gebruikers</a>.</p> </li> 
    </ul> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## De levering van e-mails vanuit de voorbeeldsandbox-omgeving inschakelen

1. Meld u aan bij de omgeving van de voorvertoningssandbox.
1. Klik op de profielafbeelding in de rechterbovenhoek van [!DNL Adobe Workfront]. Klik vervolgens op de knop **[!UICONTROL More]** en selecteert u **[!UICONTROL Edit]**.

   of

   Zoeken naar een gebruiker in [!DNL Workfront] en klik op hun naam. Klik vervolgens op de knop **[!UICONTROL More]** en selecteert u **[!UICONTROL Edit]**.

   of

   Voor meerdere gebruikers: Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **[!UICONTROL Users]** ![](assets/users-icon-in-main-menu.png).  Selecteer vervolgens meerdere gebruikers en klik op **[!UICONTROL Edit]**.

1. Klik op **[!UICONTROL Preferences]**.
1. Selecteren **[!UICONTROL Receive emails from this test environment]**.

   >[!NOTE]
   >
   >Deze optie is niet beschikbaar als u zich in een productieomgeving bevindt.

1. Klik op **[!UICONTROL Save Changes]**.
