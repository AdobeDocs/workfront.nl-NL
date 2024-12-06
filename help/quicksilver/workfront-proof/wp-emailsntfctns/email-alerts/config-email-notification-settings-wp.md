---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: Instellingen voor e-mailmeldingen configureren in  [!DNL Workfront Proof]
description: Via e-mailberichten die door Workfront Proof zijn gegenereerd, worden medewerkers op de hoogte gebracht van recente activiteiten op proefdrukken, zoals opmerkingen, antwoorden of besluiten.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: 12f1443d69bb9306af29e4ab295f701089cdfb88
workflow-type: tm+mt
source-wordcount: '1876'
ht-degree: 0%

---

# Instellingen voor e-mailmeldingen configureren in [!DNL Workfront Proof]

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [ het Bewijzen ](../../../review-and-approve-work/proofing/proofing.md).

Via e-mailmeldingen worden medewerkers op de hoogte gebracht van recente activiteiten op proefdrukken, zoals opmerkingen, antwoorden of besluiten.

U kunt e-mailmeldingen instellen voor revisoren in de volgende gebieden:

E-mailmeldingen voor revisoren kunnen worden ingesteld op de pagina Nieuwe proefdruk [!UICONTROL New version] en worden beheerd in de sectie [!UICONTROL Workflow] van de pagina [!UICONTROL Proof details] . Voor meer informatie, zie [ Proefdrukken binnen produceren  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* De pagina Nieuwe proefdruk
* De pagina [!UICONTROL New version]
* De sectie [!UICONTROL Workflow] van de pagina [!UICONTROL Proof details] .

Voor meer informatie, zie [ Proefdrukken binnen produceren  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)


* [ produceer Proofs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [ produceer Proofs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [ beheert de Details van het Bewijs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).


Elke gebruiker kan ook zijn eigen instellingen voor e-mailwaarschuwingen instellen die automatisch worden toegepast wanneer een proefdruk met hen wordt gedeeld als de medewerkers hun voorkeuren hebben of als accountbeheerders hun aanbeveling over de frequentie van waarschuwingen hebben. Dit kan als proefgebrek op de pagina&#39;s van gebruikersdetails worden geplaatst.

Elke gebruiker kan ook zijn eigen instellingen voor e-mailwaarschuwingen instellen die automatisch worden toegepast wanneer een proefdruk met hem wordt gedeeld. <!--If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a proof default on the users details pages.-->

>[!NOTE]
>
>Deze instellingen worden voorgesteld wanneer gebruikers de proefdrukken maken en deze deelnemers toevoegen. Dit zijn echter alleen suggesties, zodat ze op elk moment tijdens het herzieningsproces kunnen worden aangepast en de wijzigingen van toepassing zijn op alle activiteiten die na de wijziging worden verricht. De standaardinstellingen voor proefdrukken worden overschreven door de instellingen op proefdrukniveau.

Gebruikers met [!UICONTROL Administrator] - of [!UICONTROL Billing Administrator] -profielen kunnen de standaardwaarden voor proefdrukken ook instellen voor andere gebruikers in hun account vanuit de accountinstellingen.

Voor informatie over profielen, zie {de Profielen van de Toestemmingen van 0} Bewijs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).[

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
<tr> 
   <td role="rowheader">Product</td> 
   <td>Workfront Proof standalone</td> 
  </tr> 
</table>

+++

## Standaardwaarden voor proefdrukken configureren in persoonlijke instellingen ([!DNL Workfront Proof] alleen gebruikers)

U kunt proefdrukinstellingen configureren voor proefdrukken die u maakt.

<!--For information about proof settings the [!DNL Workfront] administrator or [!DNL Workfront Proof] administrator can configure, see .-->

1. Klik op de profielfoto in de rechterbovenhoek en klik vervolgens op **[!UICONTROL Personal settings]** .

1. Klik op de tab **[!UICONTROL Proofing defaults]** .
1. Klik op **[!UICONTROL Default email notification settings]** om het uit te vouwen.
1. Selecteer in de vervolgkeuzelijst rechts van de volgende twee instellingen een van de opties die in de onderstaande tabel worden beschreven.

   * **[!UICONTROL Default email alert]**: beïnvloedt elke proef die met u wordt gedeeld. Deze instelling kan worden overschreven op proefdrukniveau.
   * **[!UICONTROL Default email alert for new guest reviewers]**: heeft invloed op controleurs die voorheen niet als contactpersonen in uw account bestonden.

   >[!NOTE]
   >
   >Als u geen van de volgende opties kiest, verzendt [!DNL Workfront Proof] u dagelijks een overzicht van de activiteiten op uw proefdrukken.

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
      <td>Een e-mail wordt alleen naar de controleur verzonden als iemand uitdrukkelijk op zijn opmerking reageert (dit sluit zijn eigen reacties op zijn eigen opmerkingen uit). Dit betekent dat als iemand op het bewijs een nieuwe opmerking maakt, de controleur niet op de hoogte wordt gesteld.<p>Deze instelling wordt aanbevolen voor uw klanten op de proefdruk, zodat zij geen andere opmerkingen over de proefdruk ontvangen en alleen op de hoogte worden gesteld van antwoorden op hun eigen opmerkingen.</p><p>Hoewel revisoren met deze instelling voor e-mailwaarschuwingen geen melding krijgen van andere nieuwe opmerkingen, kunnen ze alle opmerkingen over de proefdrukken wel bekijken in de proefdrukviewer.</p><p>Voor informatie over commentaren, zie <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref"> Mening en antwoord aan proefdrukcommentaren </a>.</p></td> 
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
      <td>[!DNL Workfront] verzendt één e-mail met alle commentaren, antwoorden, en besluiten die slechts op dagen worden vermeld wanneer er naast uw activiteiten is.<p>Deze waarschuwing is een goede manier om een samenvatting van het project te zien zonder overweldigd met veelvoudige updates door de dag te worden.</p><p>Een voorbeeld gebruikt geval voor deze samenvatting is een afdelingsleider die de algemene vooruitgang van het project wil controleren.</p><p>Voor meer informatie, zie <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref"> berichten voor proefdrukcommentaren en besluiten </a> leiden.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL No email]</td> 
      <td>[!DNL Workfront] verzendt geen e-mailberichten.<br> dit is nuttig voor een persoon die aan een proef slechts voor verwijzingsdoeleinden wordt toegevoegd en te hoeven niet van om het even welke veranderingen worden op de hoogte gebracht.<p>De standaardwaarde van het systeem is [!UICONTROL Daily summary] (ook gezien als [!UICONTROL Not Set]). Als u of uw controleurs geen andere wijzigingen aanbrengen, hebben al uw proefdrukken deze instelling.</p></td> 
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
      <td>Geef op of u een [!UICONTROL Proof made] -e-mail wilt ontvangen wanneer u een proefdruk maakt. Voor meer informatie, zie <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref"> E-mail [!UICONTROL Proof Made] </a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Format of emails sent to me] </td> 
      <td> <p>U kunt kiezen tussen e-mails met HTML-stijl en e-mails met normale tekst. </p> <p><b>OPMERKING</b></p>
      <p>De standaardinstellingen voor proefdrukken worden overschreven door de instellingen op proefdrukniveau. Als de instellingen voor [!UICONTROL Account] echter de optie E-mailmeldingen met een proefdruk voor de gehele account uitschakelen, worden er geen e-mailwaarschuwingen verzonden naar de deelnemers, zelfs als de [!UICONTROL Disabled email alert] niet is geselecteerd op proefdrukken.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Wijzig onder **[!UICONTROL Message settings]** een of meer van de volgende instellingen:

   | Proefsjabloon | Beschrijving |
   |---|---|
   | **[!UICONTROL Proof subject template]** | Hiermee geeft u de pagina Nieuwe proefdruk, Nieuwe versie, Berichtpagina en Herinneren weer. Kan worden bewerkt voordat het wordt verzonden. |
   | **[!UICONTROL Proof message template]** | Hiermee geeft u de pagina Nieuwe proefdruk, Nieuwe versie, Berichtpagina en Herinneren weer. Kan worden bewerkt voordat het wordt verzonden. |

## E-mailwaarschuwingen voor een ontvanger wijzigen

U kunt e-mailwaarschuwingen voor een bepaalde ontvanger wijzigen in een batchactie.

1. Klik op **[!UICONTROL Contacts]** in het navigatievenster aan de linkerkant.
1. Klik op het **[!UICONTROL More]** menu ![](assets/more-button-small.png) voor de ontvanger en klik vervolgens op **[!UICONTROL View member details]** in het vervolgkeuzemenu.

1. Open de sectie **[!UICONTROL Shared items]** .
1. Schakel het selectievakje links van elk item waarvoor u de e-mailwaarschuwing wilt wijzigen in.
1. Klik op **[!UICONTROL More]** boven de lijst met gedeelde items en klik vervolgens op **[!UICONTROL Change email alert]** in het vervolgkeuzemenu.

1. Wijzig de e-mailwaarschuwing en klik op **[!UICONTROL Submit]** .

## Standaardwaarden voor proefdrukken voor een gebruiker configureren

Als u een [!DNL Workfront Proof] beheerder bent, kunt u proefdrukstandaardinstellingen instellen voor gebruikers in uw account.

1. Klik op **[!UICONTROL Account settings]** boven aan het scherm.

1. Open de tab **[!UICONTROL Users]** .
1. Open het **[!UICONTROL  More]** menu ![ More_button_small.png ](assets/more-button-small.png) aan het recht van de naam van de gebruiker.

1. Klik op **[!UICONTROL View users details]** in de vervolgkeuzelijst.
1. Klik onder **[!UICONTROL Settings]** op **[!UICONTROL Default email alert settings]** om het uit te vouwen.

1. Selecteer in de vervolgkeuzelijst rechts van de volgende twee instellingen een van de opties die in de onderstaande tabel worden beschreven:

   * **[!UICONTROL Default email alert]**: beïnvloedt elke proef die met u wordt gedeeld. Deze instelling kan worden overschreven op proefdrukniveau.
   * **[!UICONTROL Default email alert for new guest reviewers]**: heeft invloed op controleurs die voorheen niet als contactpersonen in uw account bestonden.

   >[!NOTE]
   >
   >Als u geen van de volgende opties voor een gebruiker kiest, stuurt [!DNL Workfront Proof] gebruikers een dagelijks overzicht van de activiteiten op hun proefdrukken.

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
      <td>Een e-mail wordt alleen naar de controleur verzonden als iemand uitdrukkelijk op zijn opmerking reageert (dit sluit zijn eigen reacties op zijn eigen opmerkingen uit). Dit betekent dat als iemand op het bewijs een nieuwe opmerking maakt, de controleur niet op de hoogte wordt gesteld.<p>Deze instelling wordt aanbevolen voor uw klanten op de proefdruk, zodat zij geen andere opmerkingen over de proefdruk ontvangen en alleen op de hoogte worden gesteld van antwoorden op hun eigen opmerkingen.</p><p>Hoewel revisoren met deze instelling voor e-mailwaarschuwingen geen melding krijgen van andere nieuwe opmerkingen, kunnen ze alle opmerkingen over de proefdrukken wel bekijken in de proefdrukviewer.</p><p>Voor informatie over commentaren, zie <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref"> Mening en antwoord aan proefdrukcommentaren </a>.</p></td>
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
      <td>[!DNL Workfront] verzendt één e-mail met alle commentaren, antwoorden, en besluiten die slechts op dagen worden vermeld wanneer er naast uw activiteiten is.<p>Deze waarschuwing is een goede manier om een samenvatting van het project te zien zonder overweldigd met veelvoudige updates door de dag te worden.</p><p>Een voorbeeld gebruikt geval voor deze samenvatting is een afdelingsleider die de algemene vooruitgang van het project wil controleren.</p><p>Voor meer informatie, zie <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref"> berichten voor proefdrukcommentaren en besluiten </a> leiden.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL No email]</td>
      <td>[!DNL Workfront] verzendt geen e-mailberichten.<br> dit is nuttig voor een persoon die aan een proef slechts voor verwijzingsdoeleinden wordt toegevoegd en te hoeven niet van om het even welke veranderingen worden op de hoogte gebracht.<p>De standaardwaarde van het systeem is [!UICONTROL Daily summary] (ook gezien als [!UICONTROL Not Set]). Als u of uw controleurs geen andere wijzigingen aanbrengen, hebben al uw proefdrukken deze instelling.</p></td>
     </tr>
    </tbody>
   </table>

1. Wijzig in de resterende **[!UICONTROL Default email alert settings]** een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email confirmation when proofs are ready]</td> 
      <td>Geef op of u een [!UICONTROL Proof made] -e-mail wilt ontvangen wanneer u een proefdruk maakt. Voor meer informatie, zie <a href="https://support.workfront.com/hc/en-us/article"> E-mail [!UICONTROL Proof Made].</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Format of emails sent to me] </td> 
      <td> <p>U kunt kiezen tussen e-mails met HTML-stijl en e-mails met normale tekst. </p> <p><b>OPMERKING</b></p> <p>De standaardinstellingen voor proefdrukken worden overschreven door de instellingen op proefdrukniveau. Als de instellingen voor [!UICONTROL Account] echter de optie E-mailmeldingen met een proefdruk voor de gehele account uitschakelen, worden er geen e-mailwaarschuwingen verzonden naar de deelnemers, zelfs als de [!UICONTROL Disabled email alert] niet is geselecteerd op proefdrukken.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
