---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Beheren [!DNL Adobe Workfront] meldingen in [!DNL Microsoft] Teams
description: U kunt meldingen ontvangen van [!DNL Adobe Workfront] over items die u moet goedkeuren, toewijzingen die u hebt gekregen of opmerkingen en wijzigingen in items waaraan u bent gekoppeld.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1212'
ht-degree: 0%

---

# Beheren [!DNL Adobe Workfront] meldingen in [!DNL Microsoft Teams]

U kunt meldingen ontvangen van [!DNL Adobe Workfront] over items die u moet goedkeuren, toewijzingen die u hebt gekregen of opmerkingen en wijzigingen in items waaraan u bent gekoppeld.

Deze meldingen bevatten [!DNL Workfront] acties die u kunt uitvoeren binnen [!DNL Microsoft Teams] zonder weg te navigeren van [!DNL Microsoft Teams] om ze te verwezenlijken.

>[!NOTE]
>
>[!DNL Microsoft Teams] niet meer ondersteund [!DNL Internet Explorer]. Als u de opdracht [!DNL Adobe Workfront for Microsoft Teams integration]moet u een andere webbrowser gebruiken dan [!DNL Internet Explorer].


## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Vereisten voor ontvangst [!DNL Workfront] Meldingen in [!DNL Microsoft Teams]

U kunt [!DNL Workfront] meldingen in [!DNL Microsoft Teams] indien aan de volgende voorwaarden is voldaan:

* Een teameigenaar heeft geïnstalleerd en geconfigureerd [!DNL Workfront for Microsoft Teams] voor uw team.
* U bent aangemeld [!DNL Workfront] van [!DNL Microsoft Teams].
* U hebt directe meldingen ingeschakeld in [!DNL Workfront]. Voor informatie over het inschakelen van instant notifications raadpleegt u [Uw eigen e-mailmeldingen wijzigen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Voor informatie over installeren [!DNL Workfront for Microsoft Teams] en aanmelden bij [!DNL Workfront from Microsoft Teams], zie [Installeren [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Beheer [!DNL Workfront] Meldingen in [!DNL Microsoft Teams]

Wanneer de [!DNL Workfront for Microsoft Teams] app is geïnstalleerd, een [!DNL Workfront] chatkanaal wordt gemaakt in [!DNL Microsoft Teams] voor elk lid van dat team. Wanneer een bepaalde handeling wordt uitgevoerd in [!DNL Workfront]kunt u de instellingen configureren voor [!DNL Workfront for Microsoft Teams] om meldingen over die actie te ontvangen in het [!DNL Workfront] chatkanaal [!DNL Microsoft Teams].

Houd rekening met het volgende wanneer u werkt met [!DNL Workfront] meldingen van [!DNL Microsoft Teams]:

* U kunt niet allen ontvangen, maar slechts een geselecteerd aantal van [!DNL Workfront] meldingen in [!DNL Microsoft Teams].
* Alle meldingen die u ontvangt van [!DNL Workfront] worden weergegeven in de [!DNL Workfront] bot chatten kanaal.

  Voor informatie over het installeren van de [!DNL Workfront] beide kanalen, zie [Aanmelden bij [!DNL Workfront] van [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) sectie in [Installeren [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) artikel.

* Er kan een vertraging van maximaal 5 minuten zijn tussen het tijdstip waarop een update wordt uitgevoerd [!DNL Workfront] en wanneer u hierover een melding ontvangt in [!DNL Microsoft Teams].
* Voor elke [!DNL Microsoft Teams] bericht, u ontvangt ook een e-mailbericht.

Om het [!DNL Workfront] meldingen die u kunt ontvangen in [!DNL Microsoft Teams]:

1. Klik op de knop **[!UICONTROL More added]** (driepuntpictogram) op de linkernavigatiebalk in [!DNL Microsoft Teams].

1. Klikken [!DNL Workfront] in de lijst die wordt weergegeven.
1. Selecteer de **[!UICONTROL Settings]** tab.

   ![](assets/ms-teams-settings-tab-350x552.png)

1. Schakel een van de meldingen uit die u niet wilt ontvangen. U kunt groepen meldingen in- of uitschakelen, zoals informatie of goedkeuringsmeldingen, of u kunt meldingen afzonderlijk beheren.

   Alle meldingen zijn standaard ingeschakeld.

   De instellingen voor meldingen voor [!DNL Workfront for Microsoft] Teams worden automatisch opgeslagen.

   >[!NOTE]
   >
   >U kunt geen meldingen meer toevoegen aan de meldingen die standaard beschikbaar zijn.

## Reageren op [!DNL Workfront] Meldingen en goedkeuringsverzoeken in [!DNL Microsoft Teams]

1. Aanmelden bij [!DNL Workfront] van [!DNL Microsoft Teams].\
   Voor informatie over aanmelden bij [!DNL Workfront], zie [Installeren [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Ga naar de **[!UICONTROL Chat]** en klik op **[!DNL Workfront]** beide kanalen.\
   Dit kanaal is bedoeld voor uw persoonlijke chat met de [!DNL Workfront] bot. Alles [!DNL Workfront] hier worden meldingen weergegeven.
1. Afhankelijk van het type kennisgeving dat u ontvangt, gaat u verder naar de desbetreffende sectie:

   * [Goedkeuringsmeldingen](#approval-notifications-approval-notifications)
   * [Toewijzingsmeldingen](#assignment-notifications-assignment-notifications)
   * [Opmerkingen](#comment-notifications-comment-notifications)
   * [Meldingen bijwerken](#update-notifications-update-notifications)
   * [Meldingen wijzigen](#date-change-notifications-date-change-notifications)

### Goedkeuringsmeldingen {#approval-notifications}

U ontvangt goedkeuringsberichten wanneer u wordt gevraagd om een voorwerp, zoals een taak, een timesheet, of een proef goed te keuren. U kunt echter nog steeds opmerkingen maken over het bericht.Vanaf het goedkeuringsbericht kunt u de volgende handelingen uitvoeren:

* **[!UICONTROL Approve]**: Klik om het item goed te keuren.
* **[!UICONTROL Change]**: Klik om het item met wijzigingen goed te keuren.
* **[!UICONTROL Reject]**: Klik om het item af te wijzen.
* **[!UICONTROL Comment]**: Klik om een opmerking te maken. Uw opmerking wordt ook weergegeven in [!DNL Workfront] als een update van het object waar het bericht over gaat.
* **[!UICONTROL Go to Proof]**: Klik om de proefdruk te openen. Vervolgens kunt u rechtstreeks in het bewijs een beslissing nemen. Zie voor meer informatie [Beslissen op een bewijs in de professionele drukker](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

>[!NOTE]
>
>Nadat u een goedkeuringsbesluit hebt genomen, kunt u dit niet meer wijzigen in de melding.

#### Acties beschikbaar voor specifieke goedkeuringskennisgevingen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Melding</th> 
   <th>[!UICONTROL Approve]</th> 
   <th>[!UICONTROL Reject]</th> 
   <th> <p>[!UICONTROL Change]</p> </th> 
   <th> <p>[!UICONTROL Go to Proof] </p> </th> 
   <th>[!UICONTROL Comment]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">U moet een project goedkeuren</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">U moet een taak goedkeuren</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">U moet een probleem goedkeuren</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">U moet een document goedkeuren</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">U moet de toegang tot een object goedkeuren</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">U moet een timesheet goedkeuren</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Iemand wil dat je deze proefdruk goedkeurt</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uw tijdschema is afgewezen</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uw timesheet is opnieuw geopend</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Een verzoek om goedkeuring van een document dat u hebt aangevraagd, is goedgekeurd</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Een verzoek om goedkeuring van een document dat u hebt aangevraagd, wordt goedgekeurd met wijzigingen</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Een verzoek om documentgoedkeuring dat u hebt aangevraagd, wordt afgewezen</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uw timesheet is goedgekeurd</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Toewijzingsmeldingen {#assignment-notifications}

U ontvangt toewijzingsmeldingen wanneer u, of een team dat u hebt ingeschakeld, wordt toegewezen aan een taak of uitgave in Workfront. Vanuit het toewijzingsbericht kunt u de volgende handelingen uitvoeren:

* **[!UICONTROL Work on it]**: Selecteer deze optie om aan het item te werken. Een bericht wordt kort weergegeven om te bevestigen dat een nieuw onderdeel aan uw werklijst is toegevoegd.
* **[!UICONTROL View in [!DNL Workfront]]**: Selecteer deze optie om de toegewezen uitgave of taak in Workfront weer te geven. Er wordt dan een nieuw tabblad geopend.
* **[!UICONTROL Start]**: Klik om aan het item te werken. Een bericht wordt kort weergegeven om te bevestigen dat een nieuw onderdeel aan uw werklijst is toegevoegd.
* **[!UICONTROL Comment]**: Klik om een opmerking over het item te maken. Uw opmerking wordt ook weergegeven in de updatestream van het item in Workfront.
* **[!UICONTROL Status]**: Klik en selecteer vervolgens de nieuwe status voor het werkitem in het keuzemenu.

#### Handelingen beschikbaar voor specifieke toewijzingsmeldingen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Melding</th> 
   <th>[!UICONTROL Start]</th> 
   <th>[!UICONTROL Comment]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">U bent toegewezen aan een taak</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">U bent toegewezen aan een uitgave</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Een team waaraan u wordt toegewezen ontvangt een het werkverzoek voor een taak</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Een team waaraan u bent toegewezen ontvangt een het werkverzoek voor een kwestie</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Opmerkingen {#comment-notifications}

U ontvangt een melding wanneer iemand opmerkingen maakt over een onderdeel waaraan u bent gekoppeld, of u opneemt in een update. Via het communicatiemelding kunt u de volgende handelingen uitvoeren:

* **Repalleen**: Klik om te reageren op de opmerking of [!UICONTROL update]. Uw antwoord wordt ook weergegeven in de updatestream waarin de opmerking wordt weergegeven in Workfront.
* **[!UICONTROL View in Workfront]**: Selecteer deze optie om de opmerking en het item in Workfront weer te geven. Dit item wordt op een nieuw tabblad geopend.
* **[!UICONTROL Status]**: Klik en selecteer vervolgens een nieuwe status voor het werkitem waar de opmerking of update over gaat.

#### Acties die beschikbaar zijn voor specifieke communicatiemiddelen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Melding</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Op uw verzoek is een opmerking geplaatst</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Er is een antwoord op uw werkverzoek geplaatst</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Iemand reageert op een thread waarin u zich bevindt</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Iemand heeft commentaar op een van je werk.</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Iemand reageert op een door u goedgekeurde tijdpagina</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Een opmerking wordt toegevoegd aan de pagina met gebruikersprofielen of door meerdere gebruikers bulksgewijs te bewerken</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Een opmerking wordt toegevoegd op een van uw updates</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Er wordt een opmerking toegevoegd aan uw tijdspagina</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### Meldingen bijwerken {#update-notifications}

Je ontvangt een bericht als er een update is van een object waaraan je bent gekoppeld, maar je hoeft geen actie te ondernemen. Vanuit het informatieve bericht kunt u de volgende handelingen uitvoeren:

* **[!UICONTROL Reply]**: Klik om te reageren op de [!UICONTROL update]. Uw antwoord wordt ook weergegeven in de updatestream van het item in Workfront.
* **Weergeven in Workfront**: Selecteer deze optie om de opmerking en het item in Workfront weer te geven. Dit item wordt op een nieuw tabblad geopend.
* **[!UICONTROL Status]**: Klik en selecteer vervolgens de nieuwe status voor het item in het keuzemenu.

#### Beschikbare acties op het gebied van specifieke kennisgevingen van informatie:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Melding</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Er wordt een update uitgevoerd voor een taak, uitgave of project waarop u een abonnement hebt</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Iemand neemt u op een geleide update</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Iemand neemt uw team op een [!UICONTROL directed update]</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### Meldingen wijzigen {#date-change-notifications}

U ontvangt een melding over een datumwijziging wanneer de datum verandert in een tijdelijk onderdeel waaraan u bent toegewezen. Vanaf het datumwijzigingsbericht kunt u de volgende handelingen uitvoeren.

* **[!UICONTROL Comment]**: Klik om een opmerking over het item te maken. Uw opmerking wordt ook weergegeven in de updatestream van het item in Workfront.
* **[!UICONTROL Status]**: Klik en selecteer vervolgens de nieuwe status voor het werkitem in het keuzemenu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Melding</th> 
   <th> <p>[!UICONTROL Comment]</p> </th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">De wijzigingen op de vervaldatum in een taak die u toewijst aan</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
