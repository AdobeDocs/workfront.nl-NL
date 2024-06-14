---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: De weergave-instellingen voor de startagenda configureren
description: U kunt de montages van de Kalender van het Huis vormen om met een Web-based versie van Vooruitzichten te integreren en u te helpen uw werkbelasting tegen uw beschikbare werkuren volgen.
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Configureer uw [!UICONTROL Home Calendar] weergave-instellingen

<!--Audited: 01/2024-->

U kunt de [!UICONTROL Home Calendar] instellingen om het volgende te doen:

* Integreren met een webversie van [!DNL Outlook] in de cloud [!DNL Office 365] of [!DNL Outlook Live]. U kunt alle gebeurtenissen van uw kalender van Vooruitzichten en om het even welke bijbehorende kalenders tonen u in uw selecteert [!UICONTROL Home Calendar] in Adobe Workfront.
* Help u uw werkbelasting te volgen op basis van uw beschikbare werkuren op de [!UICONTROL Allocation] bar.

Ga voor meer informatie over de Home-agenda naar [[!UICONTROL Home Calendar] weergave](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

In dit artikel wordt beschreven hoe u de instellingen van de agenda van het begin kunt configureren en de startagenda kunt integreren met uw externe Outlook-agenda.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>Huidige: [!UICONTROL Work] of hoger</p> 
   of
   <p>Nieuw: [!UICONTROL Standard]</p> 
   </td> 
  </tr> 
   </tbody> 
</table>

*Neem contact op met uw [!DNL Workfront] beheerder. Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Over integratie [!DNL Microsoft Outlook] kalenders

Overweeg het volgende aangezien u uw Kalender van het Huis met uw vormt [!DNL Microsoft Outlook] kalender:

* U kunt alleen een webversie integreren van [!DNL Outlook] in de cloud [!DNL Office 365] of [!DNL Outlook Live].

  Op locatie [!DNL Outlook] en [!DNL Outlook] over een cloudgebaseerde onderneming [!DNL Exchange] server wordt niet ondersteund.

  Als uw organisatie Single Sign-On gebruikt, hebt u [!DNL Microsoft 365 E3] of [!DNL E5].

* Bijlagen die zijn gekoppeld aan uw [!DNL Outlook] gebeurtenissen zijn niet gekoppeld aan de [!DNL Outlook] gebeurtenissen in uw startagenda.
* Integratie met een [!DNL Outlook] De kalender moet voor elke gebruiker afzonderlijk worden ingevuld.
* Gebeurtenissen die worden weergegeven in het dialoogvenster [!UICONTROL Due] wordt niet weergegeven op uw [!DNL Microsoft] kalender tenzij u hen van hebt gesleept [!UICONTROL Work List] aan uw [!DNL Adobe Workfront] Kalender. Zie voor meer informatie [[!UICONTROL Due] bar](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) en [Lijst met werkzaamheden op de [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) in [[!UICONTROL Home Calendar] weergave](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* Wanneer u de integratie met [!DNL Outlook], alleen werkitems die naar de [!UICONTROL Home Calendar] vanaf dat moment zal de synchronisatie worden uitgevoerd . Items die zich vóór het inschakelen van de integratie in de startagenda bevonden, worden niet weergegeven en u moet ze opnieuw naar de startagenda slepen als u deze wilt weergeven in [!DNL Outlook].
* Wanneer u een [!DNL Outlook] kalender met andere mensen, of wanneer u het toestemmingsniveau voor een kalender verandert u met anderen deelt, beïnvloedt deze verandering hun kalenders ongeveer 30 minuten niet. Voor meer informatie raadpleegt u de [!DNL Microsoft Outlook] documentatie.\
   Daarom moet u bij de integratie [!DNL Workfront] Kalender met een [!DNL Outlook] kalender die u met andere gebruikers deelt, zullen zij niet uw [!DNL Workfront] Kalenderitems gedurende ongeveer 30 minuten.

>[!NOTE]
>
>De [!DNL Outlook] De kalenderconfiguratie is volledig los van [!DNL Outlook] Add-in ([!UICONTROL [!DNL Outlook] Integration] of [!DNL Workfront Outlook]). Er is geen installatie vereist om de kalender te vormen, maar er is een installatie nodig voor [!DNL Outlook] Add-in. Voor meer informatie over de [!DNL Outlook] Add-in, zie [Instellen [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Configureer uw [!UICONTROL Home Calendar] weergave-instellingen en deze integreren met Outlook-kalenders

1. In de [!UICONTROL Home Calendar] klik op de knop **[!UICONTROL Settings]** tandwielpictogram ![Kalender_Instellingen_versnelling_pictogram.png](assets/calendar-settings-gear-icon.png) in de rechterbovenhoek om de **[!UICONTROL Calendar settings]** aan de rechterkant.

   Als u informatie nodig hebt over de toegang tot de [!UICONTROL Home Calendar] bekijken, zie [De weergave [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Optioneel) Om uw [!DNL Microsoft Outlook] kalender, klik **[!UICONTROL Add account]** in de rechterbovenhoek van het **[!UICONTROL Calendar settings]** deelvenster. Voer vervolgens uw [!DNL Microsoft Outlook] aanmeldingsgegevens. U kunt deze stap herhalen om meerdere [!DNL Outlook] rekeningen.

   >[!NOTE]
   >
   >U moet [!DNL Workfront] toegang tot uw [!DNL Outlook] kalender. Toestemming verlenen is toegestaan [!DNL Workfront] om toegang tot kalendergegevens te behouden, lees uw [!DNL outlook] en lees en werk uw [!DNL Microsoft] kalender.

1. Vernieuw het browservenster om informatie van uw [!DNL Outlook] in de kalender en in de [!UICONTROL Calendar settings] deelvenster.
1. Klik op de knop **[!UICONTROL Settings]** tandwielpictogram weer in de rechterbovenhoek om het **[!UICONTROL Calendar settings]** deelvenster. ![Kalender_Instellingen_versnelling_pictogram.png](assets/calendar-settings-gear-icon.png)

1. (Optioneel) Onder elke [!DNL Microsoft] account dat u in de vorige stap hebt toegevoegd, selecteert u **[!UICONTROL View]** of **[!UICONTROL Sync]**:

   * **[!UICONTROL View]**: Dit is een alleen-lezen optie die wordt weergegeven [!DNL Microsoft] agendagebeurten [!UICONTROL Home Calendar].
   * **[!UICONTROL Sync]**: Met deze optie is het mogelijk te synchroniseren in twee richtingen tussen uw [!DNL Microsoft] en [!UICONTROL Home] kalenders. Met andere woorden: [!DNL Workfront] [!UICONTROL Home Calendar] objecten exporteren naar je [!DNL Microsoft] kalender en [!DNL Microsoft] Kalender-items importeren naar je Workfront [!UICONTROL Home Calendar] in real time.

     ![](assets/view-sync-checkboxes-qs.png)

1. (Optioneel) Onder uw [!DNL Workfront] of een geïntegreerde account, selecteert u de bijbehorende kalenders die u op uw [!UICONTROL Home Calendar] (zoals uw PTO-, Verjaars- of feestdagen-kalender) en klik vervolgens op de agenda van uw browser [!UICONTROL Refresh] of [!UICONTROL Reload] om uw wijzigingen te zien.

1. (Optioneel) In het dialoogvenster **[!UICONTROL General]** deel onder **[!UICONTROL Start Week On]**, selecteert u de dag die u wilt weergeven als de eerste dag van uw werkweek in de startagenda.

   ![](assets/general-section-home-calendar-settings-panel.png)

1. Configureer de volgende opties:

   * **[!UICONTROL My Work Days]:** Selecteer de dagen die u werkt.
   * **[!UICONTROL My Usual Start Time]:** Selecteer het tijdstip waarop u uw werkdag start.
   * **[!UICONTROL My Usual End Time]:** Selecteer de tijd waarop u uw werkdag wilt beëindigen.

   [!DNL Workfront] gebruikt deze drie instellingen om het aantal uren te berekenen dat u in een week werkt. Dit getal is van invloed op de [!UICONTROL Allocation] -balk, waarmee u uw werklast kunt bijhouden op basis van uw beschikbare werkuren. Zie voor meer informatie [[!UICONTROL Allocation] bar](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) in het artikel [[!UICONTROL Home Calendar] weergave](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Klik buiten de **[!UICONTROL Calendar settings]** te sluiten.

   [!DNL Workfront] Hiermee slaat u uw wijzigingen automatisch op.

Voor informatie over het gebruik van de [!UICONTROL Calendar] om uw werktoewijzingen en geïntegreerde kalendergebeurtenissen te beheren, raadpleegt u [Gebruik de [!UICONTROL Home Calendar] weergave](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
