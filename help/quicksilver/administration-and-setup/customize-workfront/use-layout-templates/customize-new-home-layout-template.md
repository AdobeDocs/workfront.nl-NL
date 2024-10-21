---
title: Nieuwe startpagina aanpassen met een lay-outsjabloon
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Met een lay-outsjabloon kunt u configureren wat gebruikers zien wanneer ze nieuwe startpagina openen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: 1426f806b72d740712eba5e337c8424f8af6c9dc
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 0%

---

# Nieuwe startpagina aanpassen met een lay-outsjabloon

Met een lay-outsjabloon kunt u configureren wat gebruikers zien wanneer ze nieuwe startpagina voor het eerst openen.

U kunt configureren:

* Welke widgets standaard in de werkruimte worden weergegeven
* Welke achtergrond is geselecteerd
* Specifieke widgetinstellingen, waaronder de filters en groepen die beschikbaar zijn voor de widgets Mijn projecten, Mijn taken en Mijn problemen, en de standaardwaarden

>[!IMPORTANT]
>
>Eindgebruikers kunnen hun achtergrond en widgets opnieuw ordenen op de pagina wijzigen nadat het Lay-outsjabloon is toegepast. Ze kunnen geen widgets verwijderen die door een Workfront-beheerder zijn opgenomen.
> <br>
>Beheerders kunnen nieuwe widgets toevoegen aan gebruikers. Als een eindgebruiker echter zijn widgetvolgorde of achtergrondselectie al heeft aangepast, worden deze specifieke aanpassingen niet gewijzigd.



Voor informatie over nieuw Huis, zie [ begonnen worden met Huis ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

Voor informatie over het creëren van lay-outmalplaatjes, zie [ lay-outmalplaatjes ](../use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.

Voor informatie over lay-outmalplaatjes voor groepen, zie [ tot stand brengen en wijzigen de lay-outmalplaatjes van een groep ](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nadat u een lay-outmalplaatje hebt gevormd, moet u het aan gebruikers voor veranderingen toewijzen u aanbracht om aan anderen zichtbaar te zijn. Voor informatie over het toewijzen van een lay-outmalplaatje aan gebruikers, zie [ gebruikers aan een lay-outmalplaatje ](../use-layout-templates/assign-users-to-layout-template.md) toewijzen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td><p>Nieuw: Standaard</p>
  <p> Huidig: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Om deze stappen op systeemniveau uit te voeren, hebt u het toegangsniveau van de Beheerder van het Systeem nodig.
Om hen voor een groep uit te voeren, moet u een manager van die groep zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Nieuwe startpagina aanpassen met een lay-outsjabloon

Nieuwe startpagina aanpassen met een lay-outsjabloon:

1. Begin werkend aan een lay-outmalplaatje, zoals die in [ wordt beschreven creeer en beheer lay-outmalplaatjes ](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Klik de benedenpijl ![](assets/dropdown-arrow.png) onder **aanpassen welke gebruikers** zien, dan **Workspace van het Huis** klikken.

1. In de lusjes die aan het recht verschijnen, klik of **Ontwerp &amp; lay-out** om widgets en de achtergrond te kiezen en te schikken, of **montages van Widget** om montages voor individuele widgets zoals beschikbare filters en groepen te beheren.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ontwerp en lay-out</td> 
      <td>
      <p>Selecteer welke widgets in de werkruimten van de gebruikers aanwezig zullen zijn, hun positie, en kies een achtergrond. Hoewel gebruikers de geselecteerde widgets niet kunnen verwijderen, kunnen ze deze wel verplaatsen, de grootte ervan wijzigen en extra widgets toevoegen.</p>
      <p>Dit lusje functioneert hoofdzakelijk als kleine nieuwe werkruimte van het Huis; als dusdanig, kan het volgens de stappen worden aangepast die in <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md" class="MCXref xref"> worden beschreven toevoegen, uitgeven, of verwijder widgets in Huis </a>. Selecteer widgets en rangschik de werkruimte zoals u deze voor gebruikers wilt weergeven.</p>
      <p>Om de achtergrond te veranderen, volg de stappen onder <b> aanpassing van de Achtergrond </b> in <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref"> begonnen worden met Huis </a>.</p>
      <p>

>[!NOTE]
>
>Alleen het verplaatsen of vergroten of verkleinen van widgets in de Lay-outsjabloon leidt ertoe dat de nieuwe startpagina&#39;s van gebruikers hun lay-out niet bijwerken. Als u echter een widget toevoegt of verwijdert, wordt de pagina&#39;s van de gebruiker bijgewerkt.

</p>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Widget-instellingen</td> 
      <td>
      <p>Wijzig de instellingen voor afzonderlijke widgets. Momenteel worden slechts drie widgets ondersteund:</p>
      <ul>
        <li>Mijn projecten</li>
        <li>Mijn taken</li>
        <li>Mijn problemen</li>
      </ul>
      <p>Nadat u de widget hebt geselecteerd die u wilt bewerken, worden de beschikbare opties rechts weergegeven. Deze opties omvatten <b> Filters </b>, <b> Kolommen </b>, en <b> Groepen </b>. U kunt:</p>
      <ul>
      <li><p><b>Selecteer en bestel filters, kolommen of groepen die beschikbaar zijn voor gebruikers:</b></p>
      <p>Schakel het vakje naast alle opties in de lijst in die gebruikers mogen gebruiken. Deze opties gelden niet voor het deelvenster Samenvatting. U moet dat gebied configureren op het tabblad Samenvatting in het Lay-outsjabloon. Niet-geselecteerde opties worden niet weergegeven voor gebruikers. Met de opties voor slepen en neerzetten in de lijst kunt u een volgorde instellen.</li></p>
      <p>

>[!IMPORTANT]
>
>Gebruikers moeten ten minste toegang tot weergaven maken hebben om de configuratie van de beheerderskolom correct toe te passen op hun nieuwe startpagina&#39;s.

</p>
      <li><p><b>Stel een standaardfilter of -groep in voor de widget:</b></p>
      <p>Houd de muis boven een optie en er verschijnt een knop waarmee u die optie als de standaardinstelling voor gebruikers kunt instellen. De huidige standaardinstelling heeft rechts een blauwe standaardbadge.</li></p>
      <li><p><b>Voeg een bestaand filter, een bestaande kolom of een bestaande groep toe aan de lijst met beschikbare opties:</b></p>
      <p>Klik op de knop met het plusteken onder aan elke lijst om een optie aan die lijst toe te voegen. Merk op dat alleen bestaande filters, velden (voor kolommen) of groepen op deze manier kunnen worden toegevoegd.</p></li>
      </ul>
      <p>

>[!NOTE]
>
>Als u een standaardfilter of groep voor een specifieke widget instelt met een lay-outsjabloon, wordt dit mogelijk niet onmiddellijk van kracht vanwege bestaande gebruikersvoorkeuren. Als u het nieuwe filter of de nieuwe groep direct wilt toepassen, moet u of de gebruiker zijn gebruikersvoorkeuren mogelijk opnieuw instellen door &#39;/resetUser&#39; toe te voegen aan het einde van de URL.

</p>
  </td> 
  </tr>
  </tbody> 
  </table>

1. Blijf het lay-outmalplaatje aanpassen.

   of

   Als u wordt gebeëindigd aanpassend, klik **sparen** in de bodem-linkerhoek.

>[!IMPORTANT]
>
>U moet de nieuwe startpagina vernieuwen om aanpassingen in de lay-outsjabloon te kunnen zien.
