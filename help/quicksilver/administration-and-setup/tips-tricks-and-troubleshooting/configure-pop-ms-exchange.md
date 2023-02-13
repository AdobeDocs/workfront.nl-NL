---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: POP configureren in Microsoft Exchange
description: Een POP-e-mailaccount in [!DNL Microsoft Exchange] is uitgeschakeld.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# POP-in configureren [!DNL Microsoft Exchange]

## Probleem

Een POP-e-mailaccount in [!DNL Microsoft Exchange] is uitgeschakeld.

## Oplossing

Voordat u tijd besteedt aan het oplossen van problemen, moet u ervoor zorgen dat de POP-account van de gebruiker correct is geconfigureerd. Als u problemen blijft ervaren nadat u hebt bevestigd dat de POP-account correct is geconfigureerd, neemt u contact op met [!DNL Microsoft] Steun of één van hun partners voor extra hulp.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder. Zie voor meer informatie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## POP-in configureren [!DNL Microsoft Exchange]

>[!NOTE]
>
>De volgende stappen kunnen als algemene gids voor het vormen van POP binnen worden gebruikt [!DNL Microsoft Exchange] voor een productie [!DNL Workfront] systeem. De stappen kunnen aanzienlijk verschillen, afhankelijk van de Exchange-versie of de wijzigingen in de code die Microsoft aanbrengt.

1. Begin en laat de POP3 dienst op de server van de Uitwisseling toe 2010.

   >[!NOTE]
   >
   >De POP3-service is standaard niet gestart.

   1. Start [!DNL Microsoft]Serverbeheer.
   1. Navigeren: **[!UICONTROL Server Manager]** > **[!UICONTROL Configuration]** >**[!UICONTROL Windows Firewall with Advanced Security]** > **[!UICONTROL Services]**.

   1. Klikken met rechtermuisknop **[!DNL Microsoft Exchange]POP3** en klik vervolgens op **[!UICONTROL Properties]**.

   1. (Voorwaardelijk) Om ervoor te zorgen dat de POP-service automatisch wordt gestart op de knop **[!UICONTROL General]** tabblad, stelt u de **[!UICONTROL Startup]** tekst naar [!UICONTROL Automatic].

1. Vorm POP3 voor de server.

   1. Start de [!DNL Microsoft Exchange] Beheerconsole.
   1. Navigeren: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Server Configuration]** > **[!UICONTROL Client Access]**.

   1. Kies **[!UICONTROL POP3]**.

      POP3 staat op de lijst onder [!UICONTROL POP3] en [!UICONTROL IMAP4] tabs.

   1. Rechts onder **[!UICONTROL Actions]**, selecteert u **[!UICONTROL POP3]** en kiest u **[!UICONTROL Properties]**.

   1. Klikken **[!UICONTROL POP3 Properties]** en open vervolgens de **[!UICONTROL Binding]** tab.

      Alle beschikbare IP adressen en havenaantallen die voor de POP3 serververtoning worden gevormd. In het bovenste vak ziet u de optie Niet gecodeerd en in het onderste vak ziet u de IP en poorten voor SSL/TLS-verbindingen.

   1. Klikken **[!UICONTROL POP3 Properties]** en open vervolgens de **[!UICONTROL Authentication]** tab.

   1. **[!UICONTROL Select Secure]** aanmelden.

      Een TLS-verbinding is vereist voor verificatie door de client op de server.

1. Gebruikers toestaan of toestaan verbinding te maken met POP.

   1. Start de [!DNL Microsoft Exchange] Beheerconsole.
   1. Navigeren: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Recipient Configuration]** > **[!UICONTROL Mailbox]**.

      Er wordt een lijst met postvakken of gebruikers weergegeven.

   1. Markeer de e-mail die binnen wordt gebruikt [!DNL Workfront].
   1. Rechts onder **[!UICONTROL Actions]**, selecteert u **[!UICONTROL Properties]** en open vervolgens de **[!UICONTROL Mailbox Features]** tab.

   1. (Voorwaardelijk) Als POP3 is uitgeschakeld, klikt u op **[!UICONTROL POP3]** en klik vervolgens op **[!UICONTROL Enable]**.

      Er wordt een lijst met postvakken of gebruikers weergegeven.

1. Vorm ontvang schakelaars.

   1. Start [!DNL Microsoft Exchange] Beheerconsole.
   1. Navigeren: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Server Configuration]** > **[!UICONTROL Hub Transport]**.

      Een lijst van ontvangt schakelaars toont.

   1. Bevestig de ontvangstaansluiting *Client* *EX01* is ingeschakeld.

      Wanneer *Client* *EX01* is de naam van uw server van de Uitwisseling.

   1. Selecteren *Client EX01* en vervolgens rechts onder **[!UICONTROL Actions]**, selecteert u **[!UICONTROL Properties]**.

   1. Open de **[!UICONTROL Authentication]** tab, zorg er dan voor **[!UICONTROL Transport Layer Security (TLS)]** is ingeschakeld.

      >[!NOTE]
      >
      >Om Basisauthentificatie te hebben, kunt u TLS en de Geïntegreerde Authentificatie van Vensters moeten beginnen.
