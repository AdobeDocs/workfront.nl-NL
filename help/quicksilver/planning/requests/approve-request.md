---
title: Een aanvraag goedkeuren in Adobe Workfront-planning
description: Wanneer een gebruiker een aanvraag indient voor een aanvraagformulier dat is gekoppeld aan een goedkeuring in Adobe Workfront Planning, ontvangen fiatteurs een melding en een e-mail over de goedkeuring die in behandeling is. Ze moeten het verzoek goedkeuren voordat Workfront Planning een object maakt.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
source-git-commit: 99e26d4249162e46da1a73301e68bdf30436a81d
workflow-type: tm+mt
source-wordcount: '1116'
ht-degree: 0%

---

# Een aanvraag goedkeuren in Adobe Workfront Planning

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Wanneer een gebruiker een aanvraag indient voor een aanvraagformulier dat is gekoppeld aan een goedkeuring in Adobe Workfront Planning, ontvangen fiatteurs een melding en een e-mail over de goedkeuring die in behandeling is. Ze moeten het verzoek goedkeuren voordat Workfront Planning een object maakt.

In dit artikel wordt beschreven hoe een werkruimtebeheerder een aanvraag kan goedkeuren die is ingediend voor Workfront Planning om een record te maken.

We raden u aan ook de volgende artikelen te bekijken:

* [Een aanvraagformulier maken en beheren in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* [Adobe Workfront-planningsverzoeken verzenden om records te maken](/help/quicksilver/planning/requests/submit-requests.md)
* [Een goedkeuring toevoegen aan een aanvraagformulier](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## Overwegingen bij het goedkeuren van verzoeken

* De ingediende verzoeken worden getoond op het lusje van de Planning van de Voorgelegde sectie in het gebied van Verzoeken van Workfront met één van de volgende verzoekstatussen:

   * **in afwachting van overzicht**: Deze status wordt getoond wanneer geen van de fiatteurs het verzoekvoorwerp heeft geopend.
   * **In overzicht**: **In afwachting van overzicht** statusveranderingen in **In overzicht** wanneer minstens één fiatteur het verzoekvoorwerp opent. Het statuut van het verzoek blijft **in overzicht** tot alle fiatteurs het verzoek hebben goedgekeurd.
   * **Goedgekeurd**: Wanneer een fiatteur het verzoekvoorwerp goedkeurt, wordt hun individuele status **Goedgekeurd**, maar de algemene status van het verzoekvoorwerp blijft **In overzicht** tot alle fiatteurs hun besluiten hebben genomen. Wanneer alle fiatteurs een verzoek goedkeuren, wordt de verzoekstatus **Goedgekeurd**.
   * **Voltooid**: Als alle fiatteurs het verzoekvoorwerp goedkeuren, zijn statusveranderingen in **Voltooid**, of als het verzoek geen goedkeuring verwierf.
   * **Verworpen**: Als om het even welke fiatteur het verzoekvoorwerp verwerpt, wordt de status **Geweigerd**. Er wordt geen record gemaakt en er moet een nieuw verzoek worden ingediend om de record te maken.

* U kunt goedkeuringsgegevens weergeven in een record die is gemaakt door een aanvraagformulier in te dienen in de velden Goedgekeurd door en Goedgekeurd. Voor informatie, zie [ gebieden ](/help/quicksilver/planning/fields/create-fields.md) creëren.

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

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een verzoek tot het maken van een record goedkeuren

Nadat gebruikers aanvragen hebben toegevoegd aan een aanvraagformulier voor een recordtype dat is gekoppeld aan een goedkeuring, wordt het verzoek verzonden naar de fiatteurs.

De fiatteurs ontvangen de volgende meldingen over een verzoek in afwachting van hun goedkeuring:

* Een melding in de app
* Een e-mailmelding

>[!NOTE]
>
>Het exemplaar van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden ingezien zodat de gebruikers e-mail en in-app berichten kunnen ontvangen.

U kunt verzoeken goedkeuren om verslagen van het verzoek zelf tot stand te brengen, <span class="preview"> of van Mijn widget goedkeurt in Huis.</span>

* [Een verzoek van het bedrijf in Workfront Planning goedkeuren](#approve-a-request-from-the-request-in-workfront-planning)
* [Een verzoek goedkeuren van de widget Mijn goedkeuringen in Home](#approve-a-request-from-the-my-approvals-widget-in-home)

### Een verzoek van het bedrijf in Workfront Planning goedkeuren

1. (Voorwaardelijk) Als u de ervaring voor het aanvragen van oudere bestanden in Workfront gebruikt, kunt u het verzoek op een van de volgende manieren openen:

   * Als u toegang tot de Planning van Workfront hebt en minstens één werkruimte kunt bekijken, klik **het Belangrijkste menu van het Menu** Dots ![ in de hoger-juiste hoek van het scherm, of ](assets/dots-menu.png) Belangrijkste Menu **** het belangrijkste menu van Lijnen ![ in de upper-left hoek, als beschikbaar, dan klik ](assets/lines-menu.png) Verzoeken **>** > **2} Planning**, en klik het verzoek met het statuut van **In afwachting van overzicht** of **in overzicht**.****

     >[!TIP]
     >
     >Als u geen toegang hebt tot Workfront Planning, of als u geen toegang hebt tot om het even welke werkruimten te bekijken, kunt u tot een verzoek slechts toegang hebben om het goed te keuren gebruikend uw e-mail of in-app berichten.

   * Klik het **pictogram van het het gebiedspictogram van Meldingen** in Verenigde Shell ![ in de hoger-juiste hoek van het scherm en klik het bericht over een verzoek in afwachting van uw goedkeuring om het verzoek te openen.](assets/notifications-area-icon-unified-shell.png)
   * Ga naar het e-mailbericht in uw e-mail die u over een verzoek in afwachting van uw goedkeuring op de hoogte brengt, dan klik **Open verzoek** om het verzoek te openen. <!--add the name of the button here, from the email-->

   De aanvraagpagina wordt geopend in de modus Alleen-lezen.

   ![ read-only verzoekpagina in overzichtsstatus ](assets/read-only-reqeust-page-in-review-status.png)
1. Als u nieuwe het vragen ervaring in Workfront gebruikt, klik **het HoofdMenu** Dots belangrijkste menu ![ in de hoger-juiste hoek van het scherm, of het ](assets/dots-menu.png) Belangrijkste Menu **** Belangrijkste menu van Lijnen ![ in de upper-left hoek, als beschikbaar, dan klik ](assets/lines-menu.png) Verzoeken **, en klik het verzoek dat u met de status van** in afwachting van overzicht wilt goedkeuren **of** In overzicht **.**
1. (Optioneel) Klik op het pictogram **Goedkeuringen** pictogram ![ in de rechterbovenhoek van het verzoek om de fiatteurs weer te geven.](assets/approvals-icon.png)
1. Klik **Overzicht en keur** goed, dan kies één van het volgende:

   * **keur** goed: Dit keurt het verzoek goed. Er wordt direct een record gemaakt voor het recordtype dat aan het aanvraagformulier is gekoppeld, nadat alle fiatteurs het verzoek hebben goedgekeurd.
   * **Weigeren**: Dit verwerpt het verzoek, zelfs wanneer u de enige fiatteur bent die het verwerpt. Er wordt geen record gemaakt voor het recordtype dat aan het aanvraagformulier is gekoppeld.

   De gebruiker die het verzoek heeft ingediend, ontvangt een e-mail en in een app-melding wanneer zijn aanvraag is goedgekeurd of afgewezen.

   De status van het verzoek verandert in het volgende, afhankelijk van het goedkeuringsbesluit:

   * **Voltooid**: Het verzoek wordt goedgekeurd.
   * **Verworpen**: Het verzoek wordt verworpen.

   Het verzoek blijft op het lusje van de Planning van de Verzendende sectie in het gebied van Verzoeken van Workfront.

<div class="preview">

### Een verzoek goedkeuren van de widget Mijn goedkeuringen in Home

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Home]**.

   of

   Klik het [!UICONTROL Home] pictogram van het pictogram van het pictogram ![ Huis ](/help/_includes/assets/home-icon-30x29.png) in de upper-left hoek van Adobe Workfront, dan bepaal de plaats van Mijn Bevestiging widget.

1. Zoek het object dat u wilt goedkeuren of afwijzen.

1. (Optioneel) Voeg een opmerking toe door op de vervolgkeuzepijl naast Goedkeuren of Afwijzen te klikken, de notitie te typen en op Toevoegen te klikken.

1. Kies een van de volgende opties:

   * **keur** goed: Dit keurt het verzoek goed. Er wordt direct een record gemaakt voor het recordtype dat aan het aanvraagformulier is gekoppeld, nadat alle fiatteurs het verzoek hebben goedgekeurd.
   * **Weigeren**: Dit verwerpt het verzoek, zelfs wanneer u de enige fiatteur bent die het verwerpt. Er wordt geen record gemaakt voor het recordtype dat aan het aanvraagformulier is gekoppeld.

   De gebruiker die het verzoek heeft ingediend, ontvangt een e-mail en in een app-melding wanneer zijn aanvraag is goedgekeurd of afgewezen.

   De status van het verzoek verandert in het volgende, afhankelijk van het goedkeuringsbesluit:

   * **Voltooid**: Het verzoek wordt goedgekeurd.
   * **Verworpen**: Het verzoek wordt verworpen.

</div>
