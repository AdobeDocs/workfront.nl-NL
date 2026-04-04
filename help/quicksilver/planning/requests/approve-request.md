---
title: Een aanvraag goedkeuren in Adobe Workfront-planning
description: Wanneer een gebruiker een aanvraag indient voor een aanvraagformulier dat is gekoppeld aan een goedkeuring in Adobe Workfront Planning, ontvangen fiatteurs een melding en een e-mail over de goedkeuring die in behandeling is. Ze moeten het verzoek goedkeuren voordat Workfront Planning een object maakt.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 0%

---

# Een aanvraag goedkeuren in Adobe Workfront Planning

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Wanneer een gebruiker een aanvraag indient voor een aanvraagformulier dat is gekoppeld aan een goedkeuring in Adobe Workfront Planning, ontvangen fiatteurs een melding en een e-mail over de goedkeuring die in behandeling is. Ze moeten het verzoek goedkeuren voordat Workfront Planning een object maakt.

In dit artikel wordt beschreven hoe een werkruimtebeheerder een aanvraag kan goedkeuren die is ingediend voor Workfront Planning om een record te maken.

We raden u aan ook de volgende artikelen te bekijken:

* [Een aanvraagformulier maken en beheren in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* [Adobe Workfront-planningsverzoeken verzenden om records te maken](/help/quicksilver/planning/requests/submit-requests.md)
* [Een goedkeuring toevoegen aan een aanvraagformulier](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## Overwegingen bij het goedkeuren van verzoeken

* Verzonden verzoeken worden in het gebied Verzoeken van Workfront weergegeven met een van de volgende aanvraagstatussen:

   * **in afwachting van overzicht**: Deze status wordt getoond wanneer geen van de fiatteurs het verzoekvoorwerp heeft geopend.
   * **In overzicht**: **In afwachting van overzicht** statusveranderingen in **In overzicht** wanneer minstens één fiatteur het verzoekvoorwerp opent. Het statuut van het verzoek blijft **in overzicht** tot alle fiatteurs het verzoek hebben goedgekeurd.
   * **Goedgekeurd**: Wanneer een fiatteur het verzoekvoorwerp goedkeurt, wordt hun individuele status **Goedgekeurd**, maar de algemene status van het verzoekvoorwerp blijft **In overzicht** tot alle fiatteurs hun besluiten hebben genomen. Wanneer alle fiatteurs een verzoek goedkeuren, wordt de verzoekstatus **Goedgekeurd**.
   * **Voltooid**: Als alle fiatteurs het verzoekvoorwerp goedkeuren, zijn statusveranderingen in **Voltooid**, of als het verzoek geen goedkeuring verwierf.
   * **Verworpen**: Als om het even welke fiatteur het verzoekvoorwerp verwerpt, wordt de status **Geweigerd**. Er wordt geen record gemaakt en er moet een nieuw verzoek worden ingediend om de record te maken.

* U kunt goedkeuringsgegevens weergeven in een record die is gemaakt door een aanvraagformulier in te dienen in de velden Goedgekeurd door en Goedgekeurd. Voor informatie, zie [&#x200B; gebieden &#x200B;](/help/quicksilver/planning/fields/create-fields.md) creëren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakketten</p></td> 
   <td> 
<p>Alle Workfront-pakketten en alle planningspakketten</p>
of
<p>Willekeurig workflowpakket en elk planningspakket</p>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Alle</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>   <p>Machtigingen beheren voor een werkruimte en recordtype </a> </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>  </td> 
  </tr>  
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een planningsverzoek goedkeuren om een record te maken

Nadat gebruikers aanvragen hebben toegevoegd aan een aanvraagformulier voor een recordtype dat is gekoppeld aan een goedkeuring, wordt het verzoek verzonden naar de fiatteurs.

De fiatteurs ontvangen de volgende meldingen over een verzoek in afwachting van hun goedkeuring:

* Een melding in de app
* Een e-mailmelding

Raadpleeg de volgende artikelen voor informatie over het goedkeuren van aanvragen van meldingen:

* [E-mailberichten voor Adobe Workfront Planning beheren](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md)
* [In-app-berichten voor Adobe Workfront-planning beheren](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md)

>[!NOTE]
>
>Het exemplaar van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden ingezien zodat de gebruikers e-mail en in-app berichten kunnen ontvangen.

U kunt verzoeken goedkeuren om verslagen van het verzoek zelf, of van Mijn goedkeurt widget in Huis tot stand te brengen.

### Goedkeuren van een planningsverzoek uit een kennisgeving of uit het gebied Verzoeken

1. Open het verzoek door een van de volgende handelingen uit te voeren:

   * Klik **&#x200B;**&#x200B;Belangrijkste menu van het Menu van de Lijnen ![&#x200B; in de upper-left hoek, dan klik &#x200B;](assets/lines-menu.png) Verzoeken **>** Gebruik nieuwe ervaring **, en klik het verzoek met het statuut van** In afwachting van Overzicht **.**

     >[!TIP]
     >
     >* Als u geen toegang hebt tot Workfront Planning, of als u geen toegang hebt tot om het even welke werkruimten te bekijken, kunt u tot een verzoek slechts toegang hebben om het goed te keuren gebruikend uw e-mail of in-app berichten.
     >* U hebt geen toegang tot planningsverzoeken vanuit de ervaring met oudere aanvragen.

   * Klik het **pictogram van het het gebiedspictogram van Meldingen** in Verenigde Shell ![&#x200B; in de hoger-juiste hoek van het scherm en klik het bericht over een verzoek in afwachting van uw goedkeuring om het verzoek te openen.](assets/notifications-area-icon-unified-shell.png)
   * Ga naar het e-mailbericht in uw e-mail die u over een verzoek in afwachting van uw goedkeuring op de hoogte brengt, dan klik **Open verzoek** om het verzoek te openen.

   De aanvraagpagina wordt geopend in de modus Alleen-lezen.

   ![&#x200B; read-only verzoekpagina in overzichtsstatus &#x200B;](assets/read-only-reqeust-page-in-review-status.png)
1. (Optioneel) Klik op het pictogram **Goedkeuringen** pictogram ![&#x200B; in de rechterbovenhoek van het verzoek om de fiatteurs weer te geven.](assets/approvals-icon.png)
1. Klik **Overzicht en keur** goed, dan kies één van het volgende:

   * **keur** goed: Dit keurt het verzoek goed. Er wordt direct een record gemaakt voor het recordtype dat aan het aanvraagformulier is gekoppeld, nadat alle fiatteurs het verzoek hebben goedgekeurd.
   * **Weigeren**: Dit verwerpt het verzoek, zelfs wanneer u de enige fiatteur bent die het verwerpt. Er wordt geen record gemaakt voor het recordtype dat aan het aanvraagformulier is gekoppeld.

   De gebruiker die het verzoek heeft ingediend, ontvangt een e-mail en een melding in een app wanneer zijn aanvraag is goedgekeurd of afgewezen.

   De status van het verzoek verandert in het volgende, afhankelijk van het goedkeuringsbesluit:

   * **Voltooid**: Het verzoek wordt goedgekeurd.
   * **Verworpen**: Het verzoek wordt verworpen.

   Het verzoek blijft op het **gebied van Verzoeken** van Workfront.

### Een verzoek goedkeuren van de widget Mijn goedkeuringen in Home

{{step1-to-home}}

1. Ga naar **Mijn goedkeurt** widget in **Huis**.

   ![&#x200B; Mijn widget goedkeurt in Huis &#x200B;](assets/my-approvals-widget-in-home.png)
1. Zoek het planningsverzoek dat u wilt goedkeuren of afwijzen.

1. (Facultatief) voeg een commentaar toe door de drop-down pijl naast **te klikken goedkeuren** of **Afwijzen**, typend in de nota, en klikkend **&#x200B;**&#x200B;toevoegt.

1. Klik op een van de volgende opties:

   * **keur** goed: Dit keurt het verzoek goed. Er wordt direct een record gemaakt voor het recordtype dat aan het aanvraagformulier is gekoppeld, nadat alle fiatteurs het verzoek hebben goedgekeurd.
   * **Weigeren**: Dit verwerpt het verzoek, zelfs wanneer u de enige fiatteur bent die het verwerpt. Er wordt geen record gemaakt voor het recordtype dat aan het aanvraagformulier is gekoppeld.

   De gebruiker die het verzoek heeft ingediend, ontvangt een e-mail en een melding in een app wanneer zijn aanvraag is goedgekeurd of afgewezen.

   De status van het verzoek verandert in het volgende, afhankelijk van het goedkeuringsbesluit:

   * **Voltooid**: Het verzoek wordt goedgekeurd.
   * **Verworpen**: Het verzoek wordt verworpen.

