---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: Instellingen voor e-mailmeldingen configureren in [!DNL Workfront Proof]
description: Via e-mailberichten die zijn gegenereerd door Workfront Proof worden medewerkers op de hoogte gebracht van recente activiteiten op proefdrukken, zoals opmerkingen, antwoorden of besluiten.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: b4991b649a68ede587e47da2ebb7470aab3b5913
workflow-type: tm+mt
source-wordcount: '1773'
ht-degree: 0%

---

# Instellingen voor e-mailmeldingen configureren in [!DNL Workfront Proof]

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Via e-mailmeldingen worden medewerkers op de hoogte gebracht van recente activiteiten op proefdrukken, zoals opmerkingen, antwoorden of besluiten.

U kunt e-mailmeldingen instellen voor revisoren in de volgende gebieden:

* De pagina Nieuwe proefdruk
* De [!UICONTROL New version] page
* De [!UICONTROL Workflow] van de [!UICONTROL Proof details] pagina.

Zie voor meer informatie [Proefdrukken genereren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Proefdrukken genereren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [Proefdrukken genereren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Proofinggegevens beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

Elke gebruiker kan ook zijn eigen instellingen voor e-mailwaarschuwingen instellen die automatisch worden toegepast wanneer een proefdruk met hem wordt gedeeld. <!--If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a proof default on the users details pages.-->

>[!NOTE]
>
>Deze instellingen worden voorgesteld wanneer gebruikers de proefdrukken maken en deze deelnemers toevoegen. Dit zijn echter alleen suggesties, zodat ze op elk moment tijdens het herzieningsproces kunnen worden aangepast en de wijzigingen van toepassing zijn op alle activiteiten die na de wijziging worden verricht. De standaardinstellingen voor proefdrukken worden overschreven door de instellingen op proefdrukniveau.

Gebruikers met [!UICONTROL Administrator] of [!UICONTROL Billing Administrator] kunnen ook de standaardwaarden voor proefdrukken instellen voor andere gebruikers in hun account vanuit de accountinstellingen.

Zie voor informatie over profielen [Profielen met proefmachtigingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

* [Standaardwaarden voor proefdrukken configureren in persoonlijke instellingen ([!DNL Workfront Proof] alleen gebruikers)](#configure-proof-defaults-in-personal-settings-workfront-proof-users-only)
* [E-mailwaarschuwingen voor een ontvanger wijzigen](#change-email-alerts-for-a-recipient)
* [Standaardwaarden voor proefdrukken voor een gebruiker configureren](#configure-proof-defaults-for-a-user)

## Standaardwaarden voor proefdrukken configureren in persoonlijke instellingen ([!DNL Workfront Proof] alleen gebruikers)

U kunt proefdrukinstellingen configureren voor proefdrukken die u maakt.

<!--For information about proof settings the [!DNL Workfront] administrator or [!DNL Workfront Proof] administrator can configure, see .-->

1. Klikken **[!UICONTROL Settings]** > **[!UICONTROL Personal settings]**.

1. Klik op de knop **[!UICONTROL Proofing defaults]** tab.
1. Klikken **[!UICONTROL Default email notification settings]** om het uit te breiden.
1. Selecteer in de vervolgkeuzelijst rechts van de volgende twee instellingen een van de opties die in de onderstaande tabel worden beschreven.

   * **[!UICONTROL Default email alert]**: beïnvloedt elke proef die met u wordt gedeeld. Deze instelling kan worden overschreven op proefdrukniveau.
   * **[!UICONTROL Default email alert for new guest reviewers]**: Heeft gevolgen voor controleurs die voorheen niet als contactpersonen in uw account bestonden.

   >[!NOTE]
   >
   >Als u geen van de volgende opties kiest, [!DNL Workfront Proof] geeft u dagelijks een overzicht van de activiteiten op uw proefdrukken.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All activity]</td> 
      <td>[!UICONTROL Workfront] stuurt een e-mail naar de controleur telkens wanneer er activiteiten aan het bewijs, zoals een nieuwe commentaar, een antwoord, of een besluit zijn. <p>Dit is een goede optie voor de persoon die het proefdrukproces beheert omdat het hen toestaat om de activiteit te zien aangezien het gebeurt. </p><p>Gebruikers ontvangen geen e-mailbericht over hun eigen activiteiten.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Replies to my comments]</td> 
      <td>Een e-mail wordt alleen naar de controleur verzonden als iemand uitdrukkelijk op zijn opmerking reageert (dit sluit zijn eigen reacties op zijn eigen opmerkingen uit). Dit betekent dat als iemand op het bewijs een nieuwe opmerking maakt, de controleur niet op de hoogte wordt gesteld.<p>Deze instelling wordt aanbevolen voor uw klanten op de proefdruk, zodat zij geen andere opmerkingen over de proefdruk ontvangen en alleen op de hoogte worden gesteld van antwoorden op hun eigen opmerkingen.</p><p>Hoewel revisoren met deze instelling voor e-mailwaarschuwingen geen melding krijgen van andere nieuwe opmerkingen, kunnen ze alle opmerkingen over de proefdrukken wel bekijken in de proefdrukviewer.</p><p>Zie voor meer informatie over opmerkingen <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Opmerkingen over proefdrukken weergeven en beantwoorden</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisions]</td> 
      <td>[!DNL Workfront] stuurt een e-mailbericht alleen naar de controleur wanneer iemand een beslissing neemt.<p>Dit kan nuttig zijn voor de persoon die het goedkeuringsproces beheert (zoals een projectmanager) en moet de vooruitgang op het bewijs controleren en zien welke gebruikers hun besluit hebben genomen.</p><p>Je wordt pas op de hoogte gesteld van je eigen beslissing als je een bevestigingsoptie voor e-mail selecteert wanneer je je beslissing verzendt.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Final decision]</td> 
      <td>[!DNL Workfront] stuurt een e-mail wanneer de laatste fiatteur van het bewijs zijn beslissing heeft genomen.<p>Deze waarschuwing wordt vaak gebruikt door de ontwerper, die gewoonlijk niet aan de daadwerkelijke overzichtsbespreking hoeft deel te nemen. Wanneer het definitieve besluit wordt genomen, wordt de ontwerper op de hoogte gebracht en kan dan actie ondernemen op om het even welke noodzakelijke veranderingen.</p><p>Deze waarschuwing kan ook nuttig zijn voor een afdelingsleider die slechts op de hoogte moet worden gebracht wanneer het overzichtsproces wordt gebeëindigd.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Hourly Summary]</td> 
      <td>[!DNL Workfront] Hiermee stuurt u de controleur elk uur een e-mail met een overzicht van alle opmerkingen, antwoorden en beslissingen die in het uur zijn genomen.<p>Het e-mailbericht wordt alleen verzonden wanneer er in het afgelopen uur andere activiteiten plaatsvinden dan die van uzelf. </p><p>Deze waarschuwing is een goede manier om een overzicht van het project te zien.</p><p>Een voorbeeld van een gebruiksgeval voor deze samenvatting is een senior controleur die een overzicht van het project nodig heeft, maar niet onmiddellijk op de hoogte hoeft te worden gesteld van alle activiteiten op de proefdruk.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Daily Summary]</td> 
      <td>[!DNL Workfront] verzendt één e-mail met alle commentaren, antwoorden, en besluiten die slechts op dagen worden vermeld wanneer er naast uw activiteiten is.<p>Deze waarschuwing is een goede manier om een samenvatting van het project te zien zonder overweldigd met veelvoudige updates door de dag te worden.</p><p>Een voorbeeld gebruikt geval voor deze samenvatting is een afdelingsleider die de algemene vooruitgang van het project wil controleren.</p><p>Zie voor meer informatie <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Meldingen beheren voor proefopmerkingen en -beslissingen</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL No email]</td> 
      <td>[!DNL Workfront] verzendt geen e-mailberichten.<br>Dit is nuttig voor een persoon die alleen ter referentie aan een bewijs wordt toegevoegd en niet van wijzigingen in kennis hoeft te worden gesteld.<p>Het systeemgebrek is [!UICONTROL Daily summary] (ook gezien als [!UICONTROL Not Set]). Als u of uw controleurs geen andere wijzigingen aanbrengen, hebben al uw proefdrukken deze instelling.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Wijzig een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email confirmation when proofs are ready]</td> 
      <td>Geef op of u een [!UICONTROL Proof made] e-mail wanneer u een proef creeert. Zie voor meer informatie <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">De [!UICONTROL Proof Made] email</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Format of emails sent to me] </td> 
      <td> <p>U kunt kiezen tussen e-mails met HTML-stijl en e-mails met normale tekst. </p> <p><b>OPMERKING</b></p>
      <p>De standaardinstellingen voor proefdrukken worden overschreven door de instellingen op proefdrukniveau. Als e-mailmeldingen met proefdrukken echter zijn uitgeschakeld voor de gehele account in [!UICONTROL Account] instellingen, worden er geen e-mailwaarschuwingen verzonden naar de deelnemers, zelfs als de [!UICONTROL Disabled email alert] is niet geselecteerd op proefdrukken.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Onder **[!UICONTROL Message settings]** wijzigt u een van de volgende opties:

   | Proefsjabloon | Beschrijving |
   |---|---|
   | **[!UICONTROL Proof subject template]** | Hiermee geeft u de pagina Nieuwe proefdruk, Nieuwe versie, Berichtpagina en Herinneren weer. Kan worden bewerkt voordat het wordt verzonden. |
   | **[!UICONTROL Proof message template]** | Hiermee geeft u de pagina Nieuwe proefdruk, Nieuwe versie, Berichtpagina en Herinneren weer. Kan worden bewerkt voordat het wordt verzonden. |

## E-mailwaarschuwingen voor een ontvanger wijzigen

U kunt e-mailwaarschuwingen voor een bepaalde ontvanger wijzigen in een batchactie.

1. Klikken **[!UICONTROL Contacts]** in het linkernavigatievenster.
1. Klik op de knop **[!UICONTROL More]** menu ![](assets/more-button-small.png) voor de ontvanger, dan klik **[!UICONTROL View member details]** in de vervolgkeuzelijst.

1. Open de **[!UICONTROL Shared items]** sectie.
1. Schakel het selectievakje links van elk item waarvoor u de e-mailwaarschuwing wilt wijzigen in.
1. Klikken **[!UICONTROL More]** boven de lijst met gedeelde items, klikt u op **[!UICONTROL Change email alert]** in de vervolgkeuzelijst.

1. Wijzig de e-mailwaarschuwing en klik op **[!UICONTROL Submit]**.

## Standaardwaarden voor proefdrukken voor een gebruiker configureren

Als u een [!DNL Workfront Proof] beheerder, kunt u proefdrukstandaardinstellingen instellen voor gebruikers in uw account.

1. Klikken **[!UICONTROL Settings]** > **[!UICONTROL Account settings]**.

1. Open de **[!UICONTROL Users]** tab.
1. Open de **[!UICONTROL  More]** menu ![Meer_knop_klein.png](assets/more-button-small.png) rechts van de gebruikersnaam.

1. Klikken **[!UICONTROL View users details]** in de vervolgkeuzelijst.
1. Onder **[!UICONTROL Settings]**, klikt u op **[!UICONTROL Default email alert settings]** om het uit te breiden.

1. Selecteer in de vervolgkeuzelijst rechts van de volgende twee instellingen een van de opties die in de onderstaande tabel worden beschreven:

   * **[!UICONTROL Default email alert]**: beïnvloedt elke proef die met u wordt gedeeld. Deze instelling kan worden overschreven op proefdrukniveau.
   * **[!UICONTROL Default email alert for new guest reviewers]**: Heeft gevolgen voor controleurs die voorheen niet als contactpersonen in uw account bestonden.

   >[!NOTE]
   >
   >Als u geen van de volgende opties voor een gebruiker kiest, [!DNL Workfront Proof] stuurt gebruikers dagelijks een overzicht van de activiteiten op hun proefdrukken.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL All activity]</td>
      <td>[!DNL Workfront] stuurt een e-mail naar de controleur telkens wanneer er activiteiten aan het bewijs, zoals een nieuwe commentaar, een antwoord, of een besluit zijn. <p>Dit is een goede optie voor de persoon die het proefdrukproces beheert omdat het hen toestaat om de activiteit te zien aangezien het gebeurt. </p><p>Gebruikers ontvangen geen e-mailbericht over hun eigen activiteiten.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Replies to my comments]</td>
      <td>Een e-mail wordt alleen naar de controleur verzonden als iemand uitdrukkelijk op zijn opmerking reageert (dit sluit zijn eigen reacties op zijn eigen opmerkingen uit). Dit betekent dat als iemand op het bewijs een nieuwe opmerking maakt, de controleur niet op de hoogte wordt gesteld.<p>Deze instelling wordt aanbevolen voor uw klanten op de proefdruk, zodat zij geen andere opmerkingen over de proefdruk ontvangen en alleen op de hoogte worden gesteld van antwoorden op hun eigen opmerkingen.</p><p>Hoewel revisoren met deze instelling voor e-mailwaarschuwingen geen melding krijgen van andere nieuwe opmerkingen, kunnen ze alle opmerkingen over de proefdrukken wel bekijken in de proefdrukviewer.</p><p>Zie voor meer informatie over opmerkingen <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Opmerkingen over proefdrukken weergeven en beantwoorden</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisions]</td>
      <td>[!DNL Workfront] stuurt een e-mailbericht alleen naar de controleur wanneer iemand een beslissing neemt.<p>Dit kan nuttig zijn voor de persoon die het goedkeuringsproces beheert (zoals een projectmanager) en moet de vooruitgang op het bewijs controleren en zien welke gebruikers hun besluit hebben genomen.</p><p>Je wordt pas op de hoogte gesteld van je eigen beslissing als je een bevestigingsoptie voor e-mail selecteert wanneer je je beslissing verzendt.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Final decision]</td>
      <td>[!DNL Workfront] stuurt een e-mail wanneer de laatste fiatteur van het bewijs zijn beslissing heeft genomen.<p>Deze waarschuwing wordt vaak gebruikt door de ontwerper, die gewoonlijk niet aan de daadwerkelijke overzichtsbespreking hoeft deel te nemen. Wanneer het definitieve besluit wordt genomen, wordt de ontwerper op de hoogte gebracht en kan dan actie ondernemen op om het even welke noodzakelijke veranderingen.</p><p>Deze waarschuwing kan ook nuttig zijn voor een afdelingsleider die slechts op de hoogte moet worden gebracht wanneer het overzichtsproces wordt gebeëindigd.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Hourly Summary]</td>
      <td>[!DNL Workfront] Hiermee stuurt u de controleur elk uur een e-mail met een overzicht van alle opmerkingen, antwoorden en beslissingen die in het uur zijn genomen.<p>Het e-mailbericht wordt alleen verzonden wanneer er in het afgelopen uur andere activiteiten plaatsvinden dan die van uzelf. </p><p>Deze waarschuwing is een goede manier om een overzicht van het project te zien.</p><p>Een voorbeeld van een gebruiksgeval voor deze samenvatting is een senior controleur die een overzicht van het project nodig heeft, maar niet onmiddellijk op de hoogte hoeft te worden gesteld van alle activiteiten op de proefdruk.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Daily Summary]</td>
      <td>[!DNL Workfront] verzendt één e-mail met alle commentaren, antwoorden, en besluiten die slechts op dagen worden vermeld wanneer er naast uw activiteiten is.<p>Deze waarschuwing is een goede manier om een samenvatting van het project te zien zonder overweldigd met veelvoudige updates door de dag te worden.</p><p>Een voorbeeld gebruikt geval voor deze samenvatting is een afdelingsleider die de algemene vooruitgang van het project wil controleren.</p><p>Zie voor meer informatie <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Meldingen beheren voor proefopmerkingen en -beslissingen</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL No email]</td>
      <td>[!DNL Workfront] verzendt geen e-mailberichten.<br>Dit is nuttig voor een persoon die alleen ter referentie aan een bewijs wordt toegevoegd en niet van wijzigingen in kennis hoeft te worden gesteld.<p>Het systeemgebrek is [!UICONTROL Daily summary] (ook gezien als [!UICONTROL Not Set]). Als u of uw controleurs geen andere wijzigingen aanbrengen, hebben al uw proefdrukken deze instelling.</p></td>
     </tr>
    </tbody>
   </table>

1. In de resterende **[!UICONTROL Default email alert settings]** wijzigt u een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email confirmation when proofs are ready]</td> 
      <td>Geef op of u een [!UICONTROL Proof made] e-mail wanneer u een proef creeert. Zie voor meer informatie <a href="https://support.workfront.com/hc/en-us/article">De [!UICONTROL Proof Made] E-mail.</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Format of emails sent to me] </td> 
      <td> <p>U kunt kiezen tussen e-mails met HTML-stijl en e-mails met normale tekst. </p> <p><b>OPMERKING</b></p> <p>De standaardinstellingen voor proefdrukken worden overschreven door de instellingen op proefdrukniveau. Als e-mailmeldingen met proefdrukken echter zijn uitgeschakeld voor de gehele account in [!UICONTROL Account] instellingen, worden er geen e-mailwaarschuwingen verzonden naar de deelnemers, zelfs als de [!UICONTROL Disabled email alert] is niet geselecteerd op proefdrukken.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
