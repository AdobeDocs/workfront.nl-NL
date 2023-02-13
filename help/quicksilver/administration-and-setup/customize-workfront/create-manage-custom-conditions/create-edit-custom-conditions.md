---
title: Een aangepaste voorwaarde maken of bewerken
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Als Adobe Workfront-beheerder kunt u een aangepaste voorwaarde maken of bewerken voor projecten, taken en uitgaven die aansluiten op de behoeften van uw organisatie.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5c950862-4358-4aab-997b-223972662150
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Een aangepaste voorwaarde maken of bewerken

Als Adobe Workfront-beheerder kunt u een aangepaste voorwaarde maken of bewerken voor projecten, taken en uitgaven die aansluiten op de behoeften van uw organisatie.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Een aangepaste voorwaarde maken of bewerken

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Projectvoorkeuren** > **Voorwaarden**.

1. Klik op de tab van het objecttype (**Project**, **Taak**, of **Probleem**) die u aan de voorwaarde wilt koppelen.

1. Als u een nieuwe voorwaarde wilt maken, klikt u op **Een nieuwe voorwaarde toevoegen**.

   of

   Als u een bestaande voorwaarde wilt bewerken, houdt u de muisaanwijzer boven de voorwaarde die u wilt bewerken en klikt u op de knop **Bewerken** pictogram helemaal rechts.

   ![](assets/custom-condition-edit-nwe.jpg)

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
      <p>Voor informatie over standaardvoorwaarden, zie <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Een aangepaste voorwaarde instellen als standaard voor projecten</a> en <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md" class="MCXref xref">Een aangepaste voorwaarde instellen als standaard voor taken en problemen</a>.</p>
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

1. (Optioneel) Slepen ![](assets/move-icon---dots.png) alle voorwaarden naar een nieuwe positie om de lijst opnieuw te ordenen.

   Dit verandert de orde waarin de voorwaarden in projecten, taken en kwesties tonen:

   * Wanneer een gebruiker een project bewerkt

      ![](assets/change-condition-edit-project.png)

   * Wanneer een gebruiker de voorwaarde voor een taak of kwestie op het lusje van Updates verandert:

      ![](assets/change-condition-update-comment.png)

   * Wanneer een gebruiker de voorwaarde voor een taak of kwestie in een lijstmening wijzigt:

      ![](assets/change-conditions-list-dropdown-only.png)

1. Klikken **Opslaan**.

U kunt uw douanevoorwaarde als standaardvoorwaarde voor projecten of voor taken en kwesties plaatsen. Zie voor meer informatie [Een aangepaste voorwaarde instellen als standaard voor projecten](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md) en [Een aangepaste voorwaarde instellen als standaard voor taken en problemen](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Zie voor meer informatie over aangepaste voorwaarden [Aangepaste voorwaarden](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
