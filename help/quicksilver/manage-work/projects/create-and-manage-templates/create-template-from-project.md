---
product-area: templates
navigation-topic: templates-navigation-topic
title: Sjabloon maken van project
description: U kunt sjablonen maken wanneer u een bestaand project opslaat als een sjabloon.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 923deab4-205b-4312-9ec4-4471fd6cea26
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Sjabloon maken van project

<!--Audited: 10/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: Keep this article in the Creating and Managing Templates area with the detailed information that this contains. Since this is an article about creating TEMPLATES, this needs to be detailed under Templates; there is a similar article with almost the same title in Managing projects that points to this one - since this functionality is in the UI under Projects, this article must have a presence in that areas as well. Keep both, but make this one the only editable one (iterative))</p>
-->

U kunt sjablonen maken wanneer u een bestaand project opslaat als een sjabloon.

Nadat u een bestaand project als malplaatje opslaat, kunt u het nieuwe malplaatje gebruiken om nieuwe projecten tot stand te brengen. Dit vereenvoudigt en versnelt het proces van de projectverwezenlijking.

>[!NOTE]
>
>Wanneer het bewaren van een project als malplaatje, slaan de daadwerkelijke data van de taken en van het project niet voor het malplaatje op.
>
>Een malplaatje en zijn taken hebben geen daadwerkelijke data, maar eerder een aanwijzing van welke dag (van wanneer het toekomstige project zou kunnen beginnen) een taak zou kunnen beginnen en op welke dag de taak zou kunnen moeten voltooien. Wanneer het gebruiken van malplaatjes om de toekomstige projecten tot stand te brengen, zullen de projecten daadwerkelijke data ontvangen. Voor informatie, zie [ een project ](../create-projects/create-project.md) creëren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot sjablonen bewerken</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening of hoger aan een project </p> <p>Nadat u de sjabloon hebt gemaakt, hebt u beheermachtigingen voor de sjabloon nodig</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project </p> <p>You obtain Manage permissions to the template after you create it</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Sjabloon maken van project

1. Ga naar het project dat u als malplaatje wilt bewaren.
1. Klik **Meer** menu ![ Meer pictogram ](assets/more-icon.png), dan **sparen als Malplaatje**.
1. Geef de volgende informatie voor de sjabloon op:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Sjabloonnaam</td> 
      <td>Geef een naam voor de sjabloon op.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td>Geef een beschrijving voor de sjabloon.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Is actief</td> 
      <td> <p>Selecteer een van de volgende opties:</p> 
       <ul> 
        <li> <p><strong> ja </strong>: Andere gebruikers kunnen het malplaatje vinden en het aan projecten vastmaken.</p> </li> 
        <li><strong> Nr </strong>: Andere gebruikers kunnen niet het malplaatje vinden en kunnen het niet aan projecten vastmaken.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **Forms van de Douane** in het linkerpaneel.
1. Klik **voeg douaneformulier** gebied toe en of begin het typen van de naam van een projectdouane voor, of selecteer één van de lijst.

   Als er al aangepaste formulieren zijn gekoppeld aan het project, worden alle gegevens in de bestaande velden van die aangepaste formulieren weergegeven op de formulieren.

   U kunt maximaal 10 aangepaste formulieren in één sjabloon opnemen.

1. Houd de muisaanwijzer boven de naam van een formulier en klik om het te slepen en neer te zetten op een nieuwe plaats.

   ![ sparen project als malplaatjebovenkant van de doos ](assets/save-project-as-template-top-of-the-form.png)

1. Klik **Opties** in het linkerpaneel, dan selecteer de gebieden of de punten u aan het malplaatje wilt overbrengen.

   Alle items zijn standaard ingeschakeld. Niet-geselecteerde items worden niet naar de sjabloon overgebracht.

   ![ sparen als malplaatjeopties ](assets/save-project-as-template-options-area.png)

1. Klik **uitsluiten** in het linkerpaneel, dan om het even welke taken selecteren die u van het project wilt uitsluiten.

   ![ sparen als malplaatje sluit uit ](assets/save-project-as-template-exclude-area.png)

1. Klik **Einde en sparen Malplaatje.**

   De sjabloon wordt nu weergegeven in de lijst met beschikbare sjablonen. De gebruikers kunnen of het nieuwe malplaatje aan een bestaand project vastmaken of het gebruiken om een project tot stand te brengen.


