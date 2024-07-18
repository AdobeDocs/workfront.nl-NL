---
product-area: resource-management
navigation-topic: resource-planning
title: De gebruikersweergave van de bronnenplanner delen met een koppeling
description: Adobe Workfront kan een unieke URL genereren voor de gebruikersweergave van de bronnenplanner die u als externe pagina kunt insluiten in een dashboard, of deze afzonderlijk openen in een nieuw browsertabblad. Dit is nuttig wanneer het delen van de informatie van de Planner van het Middel met gebruikers die geen directe toegang tot het gebied van de Middel zouden kunnen hebben.
author: Alina
feature: Resource Management
exl-id: feb2ec26-f1a6-4581-9e1d-be948a2170c3
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# De gebruikersweergave van de bronnenplanner delen met een koppeling

Adobe Workfront kan een unieke URL genereren voor de gebruikersweergave van de bronnenplanner die u als externe pagina kunt insluiten in een dashboard, of deze afzonderlijk openen in een nieuw browsertabblad. Dit is nuttig wanneer het delen van de informatie van de Planner van het Middel met gebruikers die geen directe toegang tot het gebied van de Middel zouden kunnen hebben.

![](assets/rp-user-view-with-link-highlight-350x49.png)

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Pro en hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>De mening of hogere toegang tot het Beheer van het Middel, Projecten, en Gebruikers</p> <p>Toegang tot financiële gegevens bekijken om kosteninformatie weer te geven </p> <p><b> NOTA </b> als u nog geen toegang hebt, vraag uw beheerder van Workfront als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De mening of hogere toestemmingen aan de projecten u in de Planner van het Middel wilt tonen</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.


Overweeg het volgende wanneer het produceren van unieke URL voor de Mening van de Gebruiker van de Planner van het Middel:

* U kunt alleen een unieke URL ophalen voor de weergave Gebruiker. De optie om URL te produceren bestaat niet in de Mening van het Project of van de Rol.
* U kunt de URL delen met andere gebruikers, waaronder gebruikers met een licentie voor Werk en Revisie.\
  Ze moeten toegang hebben tot andere gebruikers om de informatie in de bronnenplanner te kunnen bekijken via de URL die u met hen deelt.
* De volgende informatie wordt opgeslagen wanneer u de URL deelt met andere gebruikers:

   * Het type tijdsperiodes (week, maand, kwartaal).
   * De filters die u toepast.
   * Het type weergave (uren of FTE).

U kunt als volgt een unieke URL opvragen in de weergave Gebruiker van de functie voor het plaatsen van bronnen en deze delen met andere gebruikers:

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront.

1. Klik **Middelen**.
1. In, uitgezochte **Mening door Gebruiker**.
1. (Optioneel) Selecteer de tijdlijn waarbinnen u de informatie wilt weergeven in de functie Bronnen. Selecteer een van de volgende opties:

   * Week
   * Maand
   * Kwart

1. (Facultatief) selecteer of u de informatie door **FTE** of **Uren** wilt bekijken.\
   ![ RP_hours_or_fte_in_user_view.png ](assets/rp-hours-or-fte-in-user-view.png)

1. (Optioneel) Pas filters toe op de functie Bronnen.\
   Voor informatie over het toepassen van filters, zie [ informatie van de Filter in de Planner van het Middel ](../../resource-mgmt/resource-planning/filter-resource-planner.md).

1. Klik het **hyperlink** pictogram.\
   ![ RP_Storm_generate_URL_with_copy_URL_link.png ](assets/rp-storm-generate-url-with-copy-url-link-350x182.png)

1. Klik **Exemplaar URL**.\
   Hiermee wordt de unieke URL van de bronnenplanner in de gebruikersweergave naar het klembord gekopieerd.

1. (Optioneel) Voer een van de volgende handelingen uit:  

   * Plak de URL in een andere toepassing om deze naar een andere gebruiker te verzenden.\
     De gebruiker moet aan Workfront worden aangemeld om de Planner van het Middel in de mening van de Gebruiker te bekijken.
   * Open een nieuw browsertabblad of een nieuw browservenster en plak de gekopieerde koppeling en klik vervolgens op Enter op het toetsenbord om de Resource Planner in een nieuw tabblad of venster te openen.
   * Ga als volgt te werk:

     <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     (NOTE:&nbsp;turn this into a numbered list)   
     </MadCap:conditionalText>   
     -->

      1. Ga naar **Meldend**> **Dashboards**> **Nieuw Dashboard**> **voeg Externe Pagina toe.**

      1. Plak de verbinding u aan uw klembord op het **** gebied URL kopieerde.
      1. Klik **sparen**, dan **sparen + Sluiten**.\
         Hierdoor wordt de URL ingesloten in het dashboard en wordt de gebruikersweergave van de functie voor het plaatsen van bronnen weergegeven in een afzonderlijk dashboard.

1. (Optioneel) Als u de URL in een dashboard hebt ingesloten, kunt u deze aan een lay-outsjabloon toevoegen of delen met andere gebruikers die mogelijk geen toegang hebben tot het gebied Bronbeheer.\
   Voor informatie over het toevoegen van dashboards aan een lay-outmalplaatje, zie [ lay-outmalplaatjes ](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.\
   Voor informatie over het delen van dashboards, zie [ een dashboard ](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) delen.\
   Wanneer het bekijken van gedeelde URL, kunnen de gebruikers de informatie met de montages zien die u oorspronkelijk op de Planner van het Middel toepaste. Ze moeten zijn aangemeld bij Workfront om de gedeelde URL weer te geven.\
   ![ user_view_dashoard_from_unique_url.png ](assets/user-view-dashoard-from-unique-url-350x85.png)
