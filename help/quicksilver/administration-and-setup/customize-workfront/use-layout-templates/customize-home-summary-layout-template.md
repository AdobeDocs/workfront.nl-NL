---
title: Het deelvenster Samenvatting aanpassen met een lay-outsjabloon
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: U kunt een Malplaatje van de Lay-out gebruiken om te vormen wat de gebruikers zien wanneer zij een taak of een kwestie in het Overzicht klikken. Elke configuratie die u uitvoert met de onderstaande stappen, is van invloed op het deelvenster Samenvatting. Deze aanpassingen zijn niet van toepassing op het deelvenster Documentoverzicht.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: 43cf88c533b80324266f0660648c6a1ab13ca8fc
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 0%

---

# Het deelvenster Samenvatting aanpassen met een lay-outsjabloon


U kunt een Malplaatje van de Lay-out gebruiken om te vormen wat de gebruikers zien wanneer zij een taak of een kwestie in het Overzicht klikken. Elke configuratie die u uitvoert met de onderstaande stappen, is van invloed op het deelvenster Samenvatting. Deze aanpassingen zijn niet van toepassing op het deelvenster Documentoverzicht.

U kunt configureren:

* Welke velden worden weergegeven voor een taak of uitgave in het gebied Details en in welke volgorde
* Of updates, geregistreerde tijd, bijgevoegde documenten, en tijdstempels voor een geselecteerde taak of kwestie tonen

U kunt de gebieden ook aanpassen die de gebruikers in het gebied van het Huis zien wanneer de gebruikers een projectgoedkeuring, documentgoedkeuring, of de goedkeuring van de documentversie klikken die aan hen wordt toegewezen.

Voor informatie over het Summiere paneel, zie [ Overzicht ](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

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

## Het deelvenster Samenvatting aanpassen met een lay-outsjabloon

1. Begin werkend aan een lay-outmalplaatje, zoals die in [ wordt beschreven creeer en beheer lay-outmalplaatjes ](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Klik de benedenpijl ![](assets/dropdown-arrow.png) onder **aanpassen welke gebruikers** zien, dan klik **Samenvattend paneel**.

1. In de lijst op de linkerzijde, klik het objecten type (**Taken**, **Kwesties**, **Projecten**, **Documenten**, of **Versies van het Document**) dat u in het Summiere paneel wilt aanpassen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Taken</td> 
      <td><p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Problemen</td> 
      <td><p>In een lijst met problemen beïnvloedt deze instelling het deelvenster Samenvatting dat aan de rechterkant van de pagina wordt weergegeven wanneer een gebruiker een probleem selecteert en vervolgens op het pictogram Samenvatting openen <img src="assets/summary-panel-icon.png"> klikt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projecten</td> 
      <td><p>In Huis, wanneer een gebruiker een projectgoedkeuring klikt die aan hen wordt toegewezen, beïnvloedt uw configuratie voor dit het plaatsen het gebied rechts van de goedkeuring.</p>
      <p>BELANGRIJK: dit is een verouderde functie. Wijzigingen die u aanbrengt in dit gebied, zijn gerelateerd aan een functie die Workfront heeft verwijderd. Deze optie wordt uit Workfront verwijderd met een latere onderhoudsupdate.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenten</td> 
      <td><p>Wanneer een gebruiker in Home op een aan hem toegewezen documentgoedkeuring klikt, is de configuratie voor deze instelling van invloed op het gebied rechts van de goedkeuring.</p>
      <p>BELANGRIJK: dit is een verouderde functie. Wijzigingen die u aanbrengt in dit gebied, zijn gerelateerd aan een functie die Workfront heeft verwijderd. Deze optie wordt uit Workfront verwijderd met een latere onderhoudsupdate.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentversies</td> 
      <td><p>Wanneer een gebruiker in Home op een goedkeuring klikt die aan hem is toegewezen voor een bepaalde versie van een document, is de configuratie voor deze instelling van invloed op het gebied rechts van de goedkeuring.</p>
      <p>BELANGRIJK: dit is een verouderde functie. Wijzigingen die u aanbrengt in dit gebied, zijn gerelateerd aan een functie die Workfront heeft verwijderd. Deze optie wordt uit Workfront verwijderd met een latere onderhoudsupdate.</p>
      </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Als een taak niet toegewezen is, zal de gebruiker die aan het lay-outmalplaatje wordt toegewezen niet de gebiedsaanpassingen in de Samenvatting zien.

1. (Voorwaardelijk) als u Taken of Kwesties in de vorige stap klikte, selecteer de categorie van taak of kwestie die u wilt aanpassen.

   ![](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (Voorwaardelijk) als de **Vastgestelde primaire actieknoop** drop-down menu verschijnt (als u **Taken** of **Kwesties** in de lijst op de linkerzijde) selecteert, klik de primaire actie (**Gedaan** of **Status**) die u beschikbaar voor gebruikers in het Samenvattende paneel wilt wanneer zij een taak of een kwestie bekijken.

   ![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. Voeg ![](assets/add-item-plus-in-circle-blue.png) of verberg ![](assets/close-or-hide---x.png) gebieden voor het geselecteerde objecten type toe.

   ![](assets/lt-home-add-hide-fields-adobe-branding.png)

1. Herhaal stap 3-6 om het deelvenster Samenvatting aan te passen voor andere objecttypen.
1. Klik **Globale montages**, dichtbij de lagere linkerhoek, dan toelaten of onbruikbaar maken om het even welke volgende opties met betrekking tot de voorwerpen van Adobe Workfront in de Samenvatting:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Updates tonen voor werk</td> 
      <td>Hiermee geeft u updates weer voor een geselecteerde taak of uitgave in het deelvenster Samenvatting. Dit omvat zowel systeemupdates als updates die door een gebruiker zijn gemaakt. De gebruikers kunnen systeemupdates nog uit filtreren, zoals die in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref"> worden beschreven toelaten of systeemupdates </a> in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref"> werk van de Update </a> onbruikbaar maken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Logtijd van arbeid</td> 
      <td>Hiermee geeft u de optie Logtijd weer tegen het werk als een taak of uitgave is geselecteerd, zodat gebruikers zich rechtstreeks vanuit het gebied Home en Summary kunnen aanmelden bij werkitems.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documenten weergeven die zijn gekoppeld aan werk</td> 
      <td>Hiermee geeft u een gebied Documenten in het deelvenster Samenvatting weer wanneer een taak of uitgave is geselecteerd en alle documenten worden weergegeven die aan de taak of uitgave zijn gekoppeld. Gebruikers kunnen op documenten klikken om deze weer te geven in een voorvertoningsvenster.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tijdstempel verbergen</td> 
      <td>Hiermee verbergt u tijdstempels voor de volgende datumvelden in het deelvenster Samenvatting:
       <ul>
        <li>Geplande afsluitdatum</li>
        <li>Vastlegdatum</li>
        <li>Verzenddatum</li>
       </ul></td> 
     </tr> 
    </tbody> 
   </table>

1. Blijf het lay-outmalplaatje aanpassen.

   of

   Als u wordt gebeëindigd aanpassend, klik **sparen**.

Voor meer informatie over lay-outmalplaatjes, zie [ lay-outmalplaatjes ](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.
