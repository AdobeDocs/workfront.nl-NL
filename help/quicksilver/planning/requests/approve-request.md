---
title: Een aanvraag goedkeuren in Adobe Workfront-planning
description: Wanneer een gebruiker een aanvraag indient voor een aanvraagformulier dat is gekoppeld aan een goedkeuring in Adobe Workfront Planning, ontvangen fiatteurs een melding en een e-mail over de goedkeuring die in behandeling is. Ze moeten het verzoek goedkeuren voordat Workfront Planning een object maakt.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 0%

---

# Een aanvraag goedkeuren in Adobe Workfront Planning

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [&#x200B; snelle versies voor uw organisatie &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

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

* <span class="preview"> u kunt goedkeuringsinformatie over een verslag tonen dat door een verzoekvorm in Goedgekeurd door en Goedgekeurde datumgebieden wordt gecreeerd voor te leggen. Voor informatie, zie [&#x200B; gebieden &#x200B;](/help/quicksilver/planning/fields/create-fields.md) creëren.</span>

## Toegangsvereisten

+++ Vouw uit om de vereisten voor toegang weer te geven.

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Producten</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront-abonnement*</p></td>
   <td>
<p>Een van de volgende Workfront-plannen:</p>
<ul><li>Selecteren</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-planningspakket*</p></td>
   <td>
<p>Alle </p>  
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningsplan is opgenomen. </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-platform</p></td>
   <td>
<p>Het geval van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden genegeerd om tot de Planning van Workfront te kunnen toegang hebben.</p>
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td>
   <td>
   <p>Standaard</p>
   <p>Workfront Planning is niet beschikbaar voor oudere Workfront-licenties</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td>
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objectmachtigingen</p></td>
   <td>
   <ul>
   <li><p>Machtigingen beheren in een werkruimte en recordtype </p></li>
    <li><p>Systeembeheerders kunnen werkruimten beheren die ze niet hebben gemaakt. </p></li>
    </ul>
   <p>Voor informatie over het delen van machtigingen voor Workfront Planning-objecten raadpleegt u  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md"> Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront </a> 
  </td>
  </tr>
 </tbody>
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Een verzoek tot het maken van een record goedkeuren

Nadat gebruikers aanvragen hebben toegevoegd aan een aanvraagformulier voor een recordtype dat is gekoppeld aan een goedkeuring, wordt het verzoek verzonden naar de fiatteurs.

De fiatteurs ontvangen de volgende meldingen over een verzoek in afwachting van hun goedkeuring:

* Een melding in de app
* Een e-mailmelding

>[!NOTE]
>
>Het exemplaar van Workfront van uw organisatie moet aan de Verenigde Ervaring van Adobe worden ingezien zodat de gebruikers e-mail en in-app berichten kunnen ontvangen.

Een verzoek goedkeuren:

1. Voer een van de volgende handelingen uit:

   * Als u toegang tot de Planning van Workfront hebt en minstens één werkruimte kunt bekijken, klik **het Belangrijkste menu van het Menu** Dots ![&#x200B; in de hoger-juiste hoek van het scherm, of &#x200B;](assets/dots-menu.png) Belangrijkste Menu **&#x200B;**&#x200B;het belangrijkste menu van Lijnen ![&#x200B; in de upper-left hoek, als beschikbaar, dan klik &#x200B;](assets/lines-menu.png) Verzoeken **>** > **2&rbrace; Planning**, en klik het verzoek met het statuut van **In afwachting van overzicht** of **in overzicht**.**&#x200B;**

     >[!TIP]
     >
     >Als u geen toegang hebt tot Workfront Planning, of als u geen toegang hebt tot om het even welke werkruimten te bekijken, kunt u tot een verzoek slechts toegang hebben om het goed te keuren gebruikend uw e-mail of in-app berichten.

   * Klik het **pictogram van het het gebiedspictogram van Meldingen** in Verenigde Shell ![&#x200B; in de hoger-juiste hoek van het scherm en klik het bericht over een verzoek in afwachting van uw goedkeuring om het verzoek te openen.](assets/notifications-area-icon-unified-shell.png)
   * Ga naar het e-mailbericht in uw e-mail die u over een verzoek in afwachting van uw goedkeuring op de hoogte brengt, dan klik **Open verzoek** om het verzoek te openen. <!--add the name of the button here, from the email-->

   De aanvraagpagina wordt geopend in de modus Alleen-lezen.

   ![&#x200B; read-only verzoekpagina in overzichtsstatus &#x200B;](assets/read-only-reqeust-page-in-review-status.png)

1. (Optioneel) Klik op het pictogram **Goedkeuringen** pictogram ![&#x200B; in de rechterbovenhoek van het verzoek om de fiatteurs weer te geven.](assets/approvals-icon.png)
1. Klik **Overzicht en keur** goed, dan kies één van het volgende:

   * **keur** goed: Dit keurt het verzoek goed. Er wordt direct een record gemaakt voor het recordtype dat aan het aanvraagformulier is gekoppeld, nadat alle fiatteurs het verzoek hebben goedgekeurd.
   * **Weigeren**: Dit verwerpt het verzoek, zelfs wanneer u de enige fiatteur bent die het verwerpt. Er wordt geen record gemaakt voor het recordtype dat aan het aanvraagformulier is gekoppeld.

   De gebruiker die het verzoek heeft ingediend, ontvangt een e-mail en in een app-melding wanneer zijn aanvraag is goedgekeurd of afgewezen.

   De status van het verzoek verandert in het volgende, afhankelijk van het goedkeuringsbesluit:

   * **Voltooid**: Het verzoek wordt goedgekeurd.
   * **Verworpen**: Het verzoek wordt verworpen.

   Het verzoek blijft op het lusje van de Planning van de Verzendende sectie in het gebied van Verzoeken van Workfront.
