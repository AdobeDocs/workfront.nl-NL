---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: POP configureren in Microsoft Exchange
description: Een POP e-mailrekening in  [!DNL Microsoft Exchange]  wordt onbruikbaar gemaakt.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# POP configureren in [!DNL Microsoft Exchange]

## Probleem

Een POP-e-mailaccount in [!DNL Microsoft Exchange] is uitgeschakeld.

## Oplossing

Voordat u tijd besteedt aan het oplossen van problemen, moet u ervoor zorgen dat de POP-account van de gebruiker correct is geconfigureerd. Als u problemen blijft ervaren nadat u hebt bevestigd dat de POP-account correct is geconfigureerd, neemt u contact op met de [!DNL Microsoft] Support of een van de partners voor extra hulp.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td>
   <p>Nieuw: Standaard</p>
   <p>of</p>
   <p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## POP configureren in [!DNL Microsoft Exchange]

>[!NOTE]
>
>De volgende stappen kunnen worden gebruikt als algemene richtlijn voor het configureren van POP in [!DNL Microsoft Exchange] voor een productie [!DNL Workfront] -systeem. De stappen kunnen aanzienlijk verschillen, afhankelijk van de Exchange-versie of de wijzigingen in de code die Microsoft aanbrengt.

1. Begin en laat de POP3 dienst op de server van de Uitwisseling toe 2010.

   >[!NOTE]
   >
   >De POP3-service is standaard niet gestart.

   1. Start [!DNL Microsoft]&#39;s Server Manager.
   1. Navigeer: **[!UICONTROL Server Manager]** > **[!UICONTROL Configuration]** > **[!UICONTROL Windows Firewall with Advanced Security]** > **[!UICONTROL Services]** .

   1. Klik met de rechtermuisknop op **[!DNL Microsoft Exchange]POP3** en klik vervolgens op **[!UICONTROL Properties]** .

   1. (Voorwaardelijk) Om ervoor te zorgen dat de POP-service automatisch wordt gestart, stelt u op het tabblad **[!UICONTROL General]** het **[!UICONTROL Startup]** type in op [!UICONTROL Automatic] .

1. Vorm POP3 voor de server.

   1. Start de [!DNL Microsoft Exchange] Management-console.
   1. Navigeer: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Server Configuration]** > **[!UICONTROL Client Access]** .

   1. Kies **[!UICONTROL POP3]** .

      POP3 staat in de lijst onder de tabbladen [!UICONTROL POP3] en [!UICONTROL IMAP4] .

   1. Selecteer rechts onder **[!UICONTROL Actions]** de optie **[!UICONTROL POP3]** en kies vervolgens **[!UICONTROL Properties]** .

   1. Klik op **[!UICONTROL POP3 Properties]** en open vervolgens het tabblad **[!UICONTROL Binding]** .

      Alle beschikbare IP adressen en havenaantallen die voor de POP3 serververtoning worden gevormd. In het bovenste vak ziet u de optie Niet gecodeerd en in het onderste vak ziet u de IP en poorten voor SSL/TLS-verbindingen.

   1. Klik op **[!UICONTROL POP3 Properties]** en open vervolgens het tabblad **[!UICONTROL Authentication]** .

   1. **[!UICONTROL Select Secure]** aanmelden.

      Een TLS-verbinding is vereist voor verificatie door de client op de server.

1. Gebruikers toestaan of toestaan verbinding te maken met POP.

   1. Start de [!DNL Microsoft Exchange] Management-console.
   1. Navigeer: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Recipient Configuration]** > **[!UICONTROL Mailbox]** .

      Er wordt een lijst met postvakken of gebruikers weergegeven.

   1. Markeer de e-mail die binnen [!DNL Workfront] wordt gebruikt.
   1. Selecteer rechts onder **[!UICONTROL Actions]** de optie **[!UICONTROL Properties]** en open vervolgens de tab **[!UICONTROL Mailbox Features]** .

   1. (Voorwaardelijk) Als POP3 is uitgeschakeld, klikt u op **[!UICONTROL POP3]** en vervolgens op **[!UICONTROL Enable]** .

      Er wordt een lijst met postvakken of gebruikers weergegeven.

1. Vorm ontvang schakelaars.

   1. Start [!DNL Microsoft Exchange] Management Console.
   1. Navigeer: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Server Configuration]** > **[!UICONTROL Hub Transport]** .

      Een lijst van ontvangt schakelaars toont.

   1. Bevestig de ontvangen schakelaar *Cliënt* *EX01* wordt toegelaten.

      Waar *de Cliënt* *EX01* de naam van uw server van de Uitwisseling is.

   1. Selecteer *Cliënt EX01*, dan op het recht onder **[!UICONTROL Actions]**, uitgezocht **[!UICONTROL Properties]**.

   1. Open het tabblad **[!UICONTROL Authentication]** en controleer of **[!UICONTROL Transport Layer Security (TLS)]** is ingeschakeld.

      >[!NOTE]
      >
      >Om Basisauthentificatie te hebben, kunt u TLS en de Geïntegreerde Authentificatie van Vensters moeten beginnen.
