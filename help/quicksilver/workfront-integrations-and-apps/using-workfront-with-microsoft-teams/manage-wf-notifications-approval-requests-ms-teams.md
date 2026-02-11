---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Beheer  [!DNL Adobe Workfront]  berichten in  [!DNL Microsoft]  Teams
description: U kunt berichten van  [!DNL Adobe Workfront]  over punten ontvangen u moet goedkeuren, taken u, of commentaren en veranderingen in punten hebt gegeven u met wordt geassocieerd.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 7720d51864428e6d7cf493f88bbee13b5203774b
workflow-type: tm+mt
source-wordcount: '1404'
ht-degree: 0%

---

# [!DNL Adobe Workfront] -meldingen beheren in [!DNL Microsoft Teams]

>[!IMPORTANT]
>
>Als [ Microsoft overgangen aan de Nieuwe cliënt van Teams ](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability), zal de Klassieke cliënt van Teams niet meer beschikbaar na 1 Juli, 2025 zijn. Als u Microsoft Teams en geïntegreerde toepassingen zoals Workfront wilt blijven gebruiken, moeten klanten vóór deze datum overstappen naar de New Teams-client.
>
>De bijgewerkte Workfront-integratie is nu beschikbaar en volledig compatibel met de New Teams-ervaring. In de meeste gevallen wordt Workfront automatisch weergegeven wanneer gebruikers een overgang hebben gemaakt. Als dit niet het geval is, kan de integratie handmatig worden geïnstalleerd vanaf de Microsoft Teams App Store. Om de integratie van Workfront in de Nieuwe cliënt van Teams te installeren of te verifiëren, zie [  [!DNL Adobe Workfront]  installeren voor Microsoft Teams ](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

U kunt meldingen ontvangen van [!DNL Adobe Workfront] over items die u moet goedkeuren, toewijzingen die u hebt gekregen of opmerkingen en wijzigingen in items waaraan u bent gekoppeld.

Deze meldingen bevatten [!DNL Workfront] -acties die u binnen [!DNL Microsoft Teams] kunt uitvoeren zonder van [!DNL Microsoft Teams] af te navigeren om ze te voltooien.

>[!NOTE]
>
>[!DNL Microsoft Teams] biedt geen ondersteuning meer voor [!DNL Internet Explorer] . Als u [!DNL Adobe Workfront for Microsoft Teams integration] wilt gebruiken, moet u een andere webbrowser gebruiken dan [!DNL Internet Explorer] .




## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p>
   <p>Werk of hoger</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten voor het ontvangen van [!DNL Workfront] meldingen in [!DNL Microsoft Teams]

U kunt [!DNL Workfront] -meldingen ontvangen in [!DNL Microsoft Teams] als aan de volgende voorwaarden is voldaan:

* Een teameigenaar heeft [!DNL Workfront for Microsoft Teams] voor uw team geïnstalleerd en geconfigureerd.
* U bent aangemeld bij [!DNL Workfront] vanuit [!DNL Microsoft Teams] .
* U hebt expresmeldingen ingeschakeld in [!DNL Workfront] . Voor informatie bij het toelaten van onmiddellijke berichten, zie [ uw eigen e-mailberichten wijzigen ](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Voor informatie over het installeren van [!DNL Workfront for Microsoft Teams] en het programma openen aan [!DNL Workfront from Microsoft Teams], zie [ installeren  [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## [!DNL Workfront] Meldingen beheren in [!DNL Microsoft Teams]

Wanneer de app [!DNL Workfront for Microsoft Teams] is geïnstalleerd, wordt in [!DNL Workfront] chat channel gemaakt voor elk lid van dat team. [!DNL Microsoft Teams] Wanneer een bepaalde handeling wordt uitgevoerd in [!DNL Workfront] , kunt u de instellingen voor [!DNL Workfront for Microsoft Teams] configureren voor het ontvangen van meldingen over die handeling in het [!DNL Workfront] chatkanaal van [!DNL Microsoft Teams] .

Houd rekening met het volgende wanneer u werkt met [!DNL Workfront] -meldingen van [!DNL Microsoft Teams] :

* U kunt niet alle berichten ontvangen, maar alleen een geselecteerd aantal [!DNL Workfront] meldingen in [!DNL Microsoft Teams] .
* Alle meldingen die u ontvangt van [!DNL Workfront] , worden weergegeven in het chatkanaal van [!DNL Workfront] .

  Voor informatie bij het installeren van het [!DNL Workfront] bot kanaal, zie het [ Aanmelden aan  [!DNL Workfront]  van  [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) sectie in [ het Installeren van  [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) artikel.

* Er kan een vertraging van maximaal 5 minuten optreden tussen het tijdstip waarop een update wordt uitgevoerd in [!DNL Workfront] en het tijdstip waarop u de melding hierover ontvangt in [!DNL Microsoft Teams] .
* Voor elke [!DNL Microsoft Teams] -melding ontvangt u ook een e-mailmelding.

De [!DNL Workfront] -meldingen beheren die u kunt ontvangen in [!DNL Microsoft Teams] :

1. Klik op het pictogram **[!UICONTROL More added]** (met drie punten) voor apps op de linkernavigatiebalk in [!DNL Microsoft Teams] .

1. Klik op [!DNL Workfront] in de lijst die wordt weergegeven.
1. Selecteer het tabblad **[!UICONTROL Settings]**. 

   ![ de montages tabel van de Teams van MS ](assets/ms-teams-settings-tab-350x552.png)

1. Schakel een van de meldingen uit die u niet wilt ontvangen. U kunt groepen meldingen in- of uitschakelen, zoals informatie of goedkeuringsmeldingen, of u kunt meldingen afzonderlijk beheren.

   Alle meldingen zijn standaard ingeschakeld.

   De instellingen voor meldingen voor [!DNL Workfront for Microsoft] -teams worden automatisch opgeslagen.

   >[!NOTE]
   >
   >U kunt geen meldingen meer toevoegen aan de meldingen die standaard beschikbaar zijn.

## Reageren op [!DNL Workfront] Meldingen en goedkeuringsverzoeken in [!DNL Microsoft Teams]

1. Meld u aan bij [!DNL Workfront] vanuit [!DNL Microsoft Teams] .\
   Voor informatie over het programma openen aan [!DNL Workfront], zie [ installeren  [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Ga naar het **[!UICONTROL Chat]** -gebied en klik op het **[!DNL Workfront]** -beide kanaal.\
   Dit kanaal is voor je persoonlijke chat met de [!DNL Workfront] bot. Alle [!DNL Workfront] -meldingen worden hier weergegeven.
1. Afhankelijk van het type kennisgeving dat u ontvangt, gaat u verder naar de desbetreffende sectie:

   * [Goedkeuringsmeldingen](#approval-notifications-approval-notifications)
   * [Toewijzingsmeldingen](#assignment-notifications-assignment-notifications)
   * [Opmerkingen](#comment-notifications-comment-notifications)
   * [Meldingen bijwerken](#update-notifications-update-notifications)
   * [Meldingen wijzigen](#date-change-notifications-date-change-notifications)

### Goedkeuringsmeldingen {#approval-notifications}

U ontvangt goedkeuringsberichten wanneer u wordt gevraagd om een voorwerp, zoals een taak, een timesheet, of een proef goed te keuren. U kunt echter nog steeds opmerkingen maken over het bericht.Vanaf het goedkeuringsbericht kunt u de volgende handelingen uitvoeren:

* **[!UICONTROL Approve]**: klik om het item goed te keuren.
* **[!UICONTROL Change]**: klik om het item met wijzigingen goed te keuren.
* **[!UICONTROL Reject]**: klik om het item af te wijzen.
* **[!UICONTROL Comment]**: klik om een opmerking te maken. Uw opmerking wordt ook in [!DNL Workfront] weergegeven als een update van het object waar het bericht over gaat.
* **[!UICONTROL Go to Proof]**: klik om de proefdruk te openen. Vervolgens kunt u rechtstreeks in het bewijs een beslissing nemen. Voor meer informatie, zie [ een besluit over een bewijs in de het proef kijker ](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) nemen.

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
   <td role="rowheader">Een verzoek om goedkeuring van een document dat u hebt aangevraagd, is goedgekeurd*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Een verzoek om goedkeuring van een document dat u hebt aangevraagd, wordt goedgekeurd met wijzigingen*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Een verzoek om goedkeuring van een document dat u hebt aangevraagd, is afgewezen*</td> 
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

*Deze meldingen verwijzen naar goedkeuringen van oudere documenten. Unieke meldingen voor documentgoedkeuring worden momenteel niet ondersteund in [!DNL Microsoft Teams] . Voor meer informatie over de verschillende goedkeuringssystemen in Workfront, zie [ Beschikbare functionaliteit voor documentgoedkeuringen ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md).

### Toewijzingsmeldingen {#assignment-notifications}

U ontvangt toewijzingsmeldingen wanneer u, of een team dat u hebt ingeschakeld, wordt toegewezen aan een taak of uitgave in Workfront. Vanuit het toewijzingsbericht kunt u de volgende handelingen uitvoeren:

* **[!UICONTROL Work on it]**: Selecteer deze optie om vast te leggen of u aan het item wilt werken. Een bericht wordt kort weergegeven om te bevestigen dat een nieuw onderdeel aan uw werklijst is toegevoegd.
* **[!UICONTROL View in [!DNL Workfront]]**: selecteer deze optie om de toegewezen uitgave of taak in Workfront weer te geven, waardoor een nieuw tabblad wordt geopend.
* **[!UICONTROL Start]**: klik om te beginnen met werken aan het item. Een bericht wordt kort weergegeven om te bevestigen dat een nieuw onderdeel aan uw werklijst is toegevoegd.
* **[!UICONTROL Comment]**: klik om een opmerking over het item te maken. Uw opmerking wordt ook weergegeven in de updatestream van het item in Workfront.
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

* **Weg **: Klik om op de commentaar of [!UICONTROL update] te antwoorden. Uw antwoord wordt ook weergegeven in de updatestream waarin de opmerking wordt weergegeven in Workfront.
* **[!UICONTROL View in Workfront]**: selecteer deze optie om de opmerking en het item in Workfront weer te geven. Dit item wordt op een nieuw tabblad geopend.
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

* **[!UICONTROL Reply]**: klik om te reageren op [!UICONTROL update] . Uw antwoord wordt ook weergegeven in de updatestream van het item in Workfront.
* **Mening in Workfront**: Uitgezocht om de commentaar en het punt in Workfront te bekijken, die in een nieuw lusje wordt geopend.
* **[!UICONTROL Status]**: Klik en selecteer vervolgens de nieuwe status voor het item in het vervolgkeuzemenu.

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

* **[!UICONTROL Comment]**: klik om een opmerking over het item te maken. Uw opmerking wordt ook weergegeven in de updatestream van het item in Workfront.
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
