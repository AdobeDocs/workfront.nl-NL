---
title: Een aangepaste voorwaarde maken of bewerken
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Als Adobe Workfront-beheerder kunt u een aangepaste voorwaarde maken of bewerken voor projecten, taken en uitgaven die aansluiten op de behoeften van uw organisatie.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5c950862-4358-4aab-997b-223972662150
source-git-commit: b7f59552e5b66a3b2db765a49abdb2f49b1a51ec
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Een aangepaste voorwaarde maken of bewerken

Als Adobe Workfront-beheerder kunt u een aangepaste voorwaarde maken of bewerken voor projecten, taken en uitgaven die aansluiten op de behoeften van uw organisatie.

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
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een aangepaste voorwaarde maken of bewerken

{{step-1-to-setup}}

1. Klik **Voorkeur van het Project** > **Voorwaarden**.

1. Klik het lusje van het objecten type (**Project**, **Taak**, of **Uitgave**) dat u met de voorwaarde wilt associëren.

1. Om een nieuwe voorwaarde tot stand te brengen, klik **voeg een nieuwe voorwaarde** toe.

   of

   Om een bestaande voorwaarde uit te geven, **geeft** naast de voorwaardennaam uit.

   ![ geef douanetoewijzing ](assets/custom-conditions-0825.png) uit

1. Configureer uw aangepaste voorwaarde met behulp van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Naam voorwaarde</td> 
      <td>(Vereist) Typ een beschrijvende naam voor de voorwaarde.</td> 
     </tr> 
     <tr> 
      <td>Beschrijving</td> 
      <td>(Optioneel) Typ een beschrijving van het doel van de voorwaarde voor de gebruikers.</td> 
     </tr> 
     <tr> 
      <td>Kleur</td> 
      <td>(Optioneel) Klik op het kleurpictogram en kies de kleur die u voor de voorwaarde wilt gebruiken wanneer deze wordt weergegeven in projecten, taken of problemen. U kunt ook een hexadecimaal getal typen.</td> 
     </tr> 
     <tr> 
      <td>Vergelijkt met </td> 
      <td><p>(Vereist, alleen voor projecten) Klik op de optie in de vervolgkeuzelijst die de functie van de nieuwe voorwaarde het best beschrijft. Bijvoorbeeld, voor een voorwaarde genoemd het Volgen goed, zou u op Doel klikken. Dit bepaalt hoe uw standaardvoorwaarden werken. Elke voorwaarde die u maakt, moet overeenkomen met een van de opties in het keuzemenu.</p>
      <p>Voor informatie over standaardvoorwaarden, zie <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref"> Plaats een douanetoewijzing als gebrek voor projecten </a> en <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md" class="MCXref xref"> plaats een douanetoewijzing als gebrek voor taken en kwesties </a>.</p>
      <p>Deze optie kan niet worden gewijzigd nadat u de voorwaarde hebt gemaakt.</p></td> 
     </tr> 
     <tr> 
      <td>Sleutel</td> 
      <td><p>(Vereist) Typ voor een projectvoorwaarde een alfanumerieke afkorting die gebruikers kunnen herkennen. Typ voor een taak- of uitgiftevoorwaarde een numerieke code van twee cijfers tussen 01 en 99. </p>
      <p>Deze sleutel, die wordt gebruikt in de API en kan worden gebruikt voor rapportagedoeleinden, moet uniek zijn voor elk object.</p>
      <p>U kunt de sleutel voor een voorwaarde niet wijzigen nadat u de voorwaarde hebt opgeslagen. </p></td> 
     </tr> 
     <tr> 
      <td>Voorwaarde verbergen</td> 
      <td><p>(Optioneel) Deze optie is beschikbaar voor aangepaste voorwaarden die u niet langer wilt gebruiken, maar die u om historische redenen wilt behouden. </p>
      <p>Als u een aangepaste voorwaarde verbergt die is gebruikt voor werkitems, wordt deze op die werkitems weergegeven nadat u deze hebt verborgen. </p></td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >U kunt de terminologie en de kleuren van voorwaarden standaardiseren voor alle drie de objecttypen. Om dit te doen, kopieer de voorwaardenNaam en de hexadecimale code van de Kleur van één lusje (Project, Taak, Kwestie) aan de overeenkomstige voorwaarde op de andere twee lusjes.

1. (Facultatief) sleep ![ pictogram van de Beweging ](assets/move-icon---dots.png) om het even welke voorwaarde aan een nieuwe positie om de lijst opnieuw in orde te brengen.

   Dit verandert de orde waarin de voorwaarden in projecten, taken en kwesties tonen:

   * Wanneer een gebruiker een project bewerkt

     ![ voorwaarde van de Verandering wanneer het uitgeven van project ](assets/change-condition-edit-project-0825.png)

   * Wanneer een gebruiker de voorwaarde voor een taak of kwestie in een lijstmening wijzigt:

     ![ voorwaarde van de Verandering in lijst ](assets/change-conditions-list-dropdown-0925.png)

     >[!NOTE]
     >
     >In de standaardmening van de Voorwaarde, is het **1} gebied van de Voorwaarde een type van gebied dat niet inline kan worden uitgegeven.** Wanneer u het **gebied van de Voorwaarde** aan een mening afzonderlijk toevoegt, is het editable. Voor informatie over gealigneerde het uitgeven, zie [ gealigneerd punten in een lijst in Adobe Workfront ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md) uitgeven.

1. Klik **sparen**.

U kunt uw douanevoorwaarde als standaardvoorwaarde voor projecten of voor taken en kwesties plaatsen. Voor meer informatie, zie [ Plaats een douanetoewijzing als gebrek voor projecten ](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md) en [ plaats een douanetoewijzing als gebrek voor taken en kwesties ](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Voor meer informatie over douanevoorwaarden, zie [ de voorwaarden van de Douane ](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).


<!-- THIS WAS ORIGINALLY BETWEEN THE OTHER TWO BULLETS.
   * When a user is changing the condition for a task or issue on the Updates tab:

     ![Change condition when updating comment](assets/change-condition-update-comment.png)
   -->
