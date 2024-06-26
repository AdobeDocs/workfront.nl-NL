---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Slimme toewijzingen maken
description: U kunt slimme toewijzingen gebruiken om te bepalen wie de beste gebruiker het werk moet voltooien. De slimme taken zijn suggesties voor gebruikers, rollen, of teams die Adobe Workfront aan u voorstelt wanneer u het werkpunten aan middelen toewijst die op een algoritme worden gebaseerd dat het meest aangewezen middel voor de baan bepaalt. Zie Overzicht slimme toewijzingen voor informatie over slimme toewijzingen.
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 02a47566acd0fff151656fe2c5b59a6679748b15
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Slimme toewijzingen maken

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">De gemarkeerde informatie op deze pagina verwijst naar functionaliteit die nog niet algemeen beschikbaar is. Deze functie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten of in de productieomgeving voor klanten die snelle releases hebben ingeschakeld.</span>

<span class="preview">Voor informatie over snelle versies raadpleegt u [Snelle releases voor uw organisatie in- of uitschakelen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Voor informatie over de huidige versie raadpleegt u [Overzicht release derde kwartaal 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

U kunt slimme toewijzingen gebruiken om te bepalen wie de beste gebruiker het werk moet voltooien.

De slimme taken zijn suggesties voor gebruikers, rollen, of teams die Adobe Workfront aan u voorstelt wanneer u het werkpunten aan middelen toewijst. Workfront baseert zijn suggesties op een algoritme dat de meest aangewezen bron voor de baan bepaalt.

<span class="preview">Er zijn twee aparte algoritmen in Workfront die slimme toewijzingen berekenen die verschillend werken voor taken en voor problemen. </span>

Zie voor meer informatie over de criteria die worden gebruikt bij het bepalen van slimme toewijzingen [Overzicht van slimme toewijzingen](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuw: Standaard</p>
      of
      <p>Huidig: Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken en problemen bewerken</p> <p>Toegang tot projecten weergeven of vergroten</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute of hoger met de mogelijkheid om taken en uitgaven toe te wijzen</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt. Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Slimme toewijzingen maken

Slimme toewijzingen zijn beschikbaar op de meeste locaties waar u toewijzingen kunt maken in Workfront.

1. Ga naar de volgende gebieden en klik op **Toewijzingen** of **Deze toewijzen aan** veld:

   * Een taak- of uitgiftenlijst of rapport
   * Een taak- of uitgiftekoptekst
   * Het deelvenster Overzicht van taken of uitgaven
   * <span class="preview">Een nieuwe Taak of het Nieuwe vakje van de Uitgave, aangezien u een nieuwe taak of een kwestie aan een project toevoegt</span>
   * Het veld Toewijzingen voor een item dat wordt vermeld in het gebied Home
   * Een taak of probleem in het werklastevenwicht

1. Plaats de cursor in het veld Toewijzingen en wacht twee seconden.

   <div class="preview">
   Een of meer van de volgende secties met suggesties voor slimme toewijzingen worden weergegeven:

   * **Voorgestelde toewijzingen**: wordt weergegeven voor taken. <!--remove the note when we go to production with smarter assignments-->

     >[!TIP]
     >
     >   De lijstkoptekst wordt weergegeven **Hier volgen enkele aanbevelingen** in plaats van **Voorgestelde toewijzingen** in de productieomgeving.
     >
   * **Gebruikers en teams**: Hier worden taken en problemen weergegeven.
   * **Functies**: Geeft niet voor taken en problemen.
   * **Functies voor kaarttaken beoordelen**: wordt weergegeven voor taken. Zie voor meer informatie [Creditcards beheren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).<!--check later with Lisa to see if this also came to issues?! - and always keep this in yellow-->
   </div>

   <span class="preview">![](assets/smart-assignments-task-header-nwe-350x302.png)</span>


   Voor taken worden de slimme toewijzingen weergegeven in de volgende secties, afhankelijk van de fase van de berekening van het algoritme waarin de toewijzingen zijn geïdentificeerd:

   * **Voorgestelde toewijzingen**: Toewijzingen die zijn geïdentificeerd in de eerste fase van de algoritmeberekening van de slimme toewijzing van de taak. <span class="preview">Deze sectie is niet beschikbaar voor problemen.</span>
   * <span class="preview">**Gebruikers en teams**, **Functies**, of **Functies voor kaarttaken beoordelen**: Toewijzingen die zijn geïdentificeerd in de tweede fase van de algoritmeberekening van de slim-toewijzing van de taak. <!--no longer valid: This section is not available for issues. --></span> <!--replace this with the new UI: "Other assignments"-->

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   Zie voor meer informatie [Overzicht van slimme toewijzingen](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Selecteer de gebruiker in de lijst met aanbevelingen door op de gewenste naam te klikken.

1. (Optioneel) Klik op **Toewijzen aan mij** om het werkitem aan uzelf toe te wijzen.

   >[!TIP]
   >
   >Als er geen suggesties zijn, wordt de lijst met suggesties niet geopend.

1. (Optioneel) Als u een van de aanbevolen gebruikers in de lijst met slimme toewijzingen niet wilt gebruiken, typt u de naam van de gewenste bron en selecteert u de naam wanneer deze in de lijst wordt weergegeven.
1. Klikken **Enter** om de toewijzing te maken.

   De geselecteerde gebruiker wordt toegewezen aan de taak of uitgave.
