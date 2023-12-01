---
filename: change-date-format-chrome
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: De datumnotatie wijzigen in [!DNL Adobe Workfront]
description: De datumnotatie voor de datums wijzigen in [!DNL Adobe Workfront] u moet de taalmontages in uw browser veranderen.
feature: Get Started with Workfront
exl-id: 9fac92fb-e3d1-4537-b324-4b35447cef28
source-git-commit: e9a96b6952ca3f128cc723df68787f40c8dcf604
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# De datumnotatie wijzigen in [!DNL Adobe Workfront]

<!--this article used to be called "Change the date format in Adobe Workfront when using Chrome". The team decieded to make it more generic and hide the steps. Also see drafted content below-->

U kunt de datumnotatie wijzigen in [!DNL Adobe Workfront], zoals [!UICONTROL Planned Completion Date], [!UICONTROL Actual Completion Date], of [!UICONTROL Projected Completion Date].

U kunt bijvoorbeeld een datumnotatie wijzigen van _DD/MM/YYYY_ tot _MM/DD/YYYY_ of omgekeerd.
U kunt ook de datumnotatie wijzigen van _MM/DD/YY_ tot _Mon DD, YYYY_.

U kunt datumnotaties op de volgende manieren wijzigen in Workfront, afhankelijk van de wijzigingen die u wilt zien en van de plaats waar u de wijzigingen wilt zien.

* Alle datumnotaties wijzigen voor alle pagina&#39;s in [!DNL Workfront] afhankelijk van uw locatie en taal moet u de taalinstellingen in uw browser wijzigen.

  Als de standaardtaal in uw browser bijvoorbeeld is ingesteld op *[!UICONTROL English (United States)]* De datums worden in de volgende notaties weergegeven:

   * MM/DD/YYYY
   * Mon DD, YYY

  De taalinstellingen wijzigen in [!DNL Chrome] of een andere browser, moet u de instellingen van die browser wijzigen. De stappen voor het wijzigen van de browserinstellingen variëren van browser tot browser. Raadpleeg de [!UICONTROL Help], [!UICONTROL Preferences], of [!UICONTROL Settings] gebieden om te leren hoe u de instellingen kunt wijzigen.

* Als u de datumnotatie alleen wilt wijzigen in rapporten en weergaven, moet u de opdracht [!UICONTROL Field Format] in het dialoogvenster [!UICONTROL Advanced Options] gebied van een kolom, wanneer het opbouwen van het rapport of de mening. Hiermee wijzigt u de datumnotatie niet op basis van de locatie of taal. De datumnotatie wordt gewijzigd in de context van dezelfde locatie of taal.

  ![](assets/field-format-in-advanced-options-of-a-view-highlighted.png)

  Zie voor meer informatie [Een aangepast rapport maken](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Als u de datumnotatie wilt wijzigen in alle uitgaande e-mailmeldingen voor uw hele organisatie, moet u de [!UICONTROL Default Email Locale] in het dialoogvenster [!UICONTROL Customer Info] gebied in [!UICONTROL Setup].

  ![](assets/default-email-locale-field.png)

  Zie voor meer informatie [Basisinformatie voor uw systeem configureren](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Als u de indeling van alle datums in alle uitgaande e-mailberichten voor één gebruiker wilt wijzigen, moet u de [!UICONTROL Email Locale] in het dialoogvenster [!UICONTROL Edit Person] bij het bewerken van het profiel van een gebruiker.

  ![](assets/email-locale-for-user-profile-highlighted.png)

  Zie voor meer informatie [Gebruikersprofiel bewerken](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

<!--drafted because we should not document steps for a third-party application

To change your language settings in Chrome:

1. Click the 3-dots in the top right corner of your Chrome interface, then click **Settings**.
1. On the left area of the Settings page, expand **Advanced**, then click **Languages**.  
   Or  
   Search for *language*&nbsp;at the top of the Settings page, then click **Languages**.

1. In the **Language** list, locate the language and region that use your preferred date format.

   **Example:** If you speak English and you want the date format to be MM/DD/YYYY, you would select **English (United States)**. If you speak English and you want the date format to be DD/MM/YYY, you would select **English (United Kingdom)**.

1. (Conditional) If the language and region you want to use are not visible in the list, click **Add languages** to add it to the list.
1. Click the 3-dot menu next to the language and region you want to use, then click **Move to the top**.
1. Return to the Workfront interface, then refresh the page.  
   The date format is now updated in projects and other areas of Workfront that use MM/DD/YYYY or DD/MM/YYYY format when displaying dates.

   -->
