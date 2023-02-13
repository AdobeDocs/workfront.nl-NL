---
product-area: projects
navigation-topic: manage-tasks
title: Een taak omzetten in een project
description: Wanneer een taak in een project een grotere hoeveelheid inspanning vereist om te voltooien dan u oorspronkelijk gepland, kunt u het in een project omzetten.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Een taak omzetten in een project

Wanneer een taak in een project een grotere hoeveelheid inspanning vereist om te voltooien dan u oorspronkelijk gepland, kunt u het in een project omzetten.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> <p>Bekijk of hogere toegang tot Malplaatjes, wanneer het omzetten in een project gebruikend een malplaatje</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een taak beheren</p> <p>De toestemmingen van de mening op een malplaatje, als het omzetten in een project gebruikend een malplaatje</p> <p>Nadat u het project hebt gemaakt, hebt u beheerdersmachtigingen voor het project</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Overwegingen bij het omzetten van taken in projecten

* De oorspronkelijke taak wordt verwijderd.
* Taakgoedkeuringen worden verwijderd.
* Alle subtaken, kwesties en nota&#39;s komen tot het nieuwe project.
* Documenten, documentversies en proefdrukken worden naar het nieuwe project verplaatst.
* De status en het percentage voltooide van alle subtaken en kwesties worden bewaard.
* Gedeelde gebruikers van de taak worden gedeelde gebruikers op het project.
* De begindatum van het project is ingesteld op de begindatum van de taak.
* Als de taakstatus &#39;Nieuw&#39; is, wordt de projectstatus ingesteld op &#39;Planning&#39;.
* Als de taakstatus &#39;In uitvoering&#39; is, wordt de projectstatus ingesteld op &#39;Huidig&#39;.
* Als de taakstatus &#39;Voltooid&#39; is, wordt de projectstatus ingesteld op &#39;Voltooid&#39;.

## Een taak omzetten in een project

1. Ga naar de taak die u in een project wilt omzetten.
1. Klik op de knop **Meer** pictogram ![](assets/more-icon.png)vervolgens **Omzetten in project**.
1. Kies een van de volgende opties:

   * **Nieuw project**
   * Een sjabloon in het dialoogvenster **Selecteren uit sjablonen** sectie

      ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. Klikken **Doorgaan** in het bericht dat wordt weergegeven.
1. In de **Omzetten in project** het volgende opgeven:

   * **Naam**: Geef uw project een naam. De standaardnaam is de naam van de taak.
   * (Optioneel) **Beschrijving**: Beschrijf het doel van dit project.
   * (Optioneel en voorwaardelijk) Als u een project wilt maken op basis van een sjabloon, werkt u de beschikbare velden in het dialoogvenster **Omzetten in project** in.

      Voor meer informatie over het uitgeven van gebieden op projecten, zie [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >Als u velden in het gedeelte Financiën in het vak Converteren naar project wilt bijwerken, moet u toegang tot financiële gegevens op uw toegangsniveau bewerken hebben. Als u toegang van de Mening tot Financiële Gegevens in uw toegangsniveau hebt alle financiële informatie van de malplaatjeoverdrachten aan het nieuwe project en u kunt niet het uitgeven terwijl u de kwestie omzet. Zie voor meer informatie [Toegang tot financiële gegevens verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) en [Een sjabloon delen](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (Optioneel) Toevoegen **Aangepaste Forms** aan het nieuwe project.

      >[!TIP]
      Als een aangepast formulier voor meerdere objecten dat aan de taak is gekoppeld, is geconfigureerd voor zowel taken als projecten, blijft alle informatie die in het formulier is opgeslagen, behouden wanneer u de conversie uitvoert.
      Als u een sjabloon voor de conversie gebruikt en een aangepast formulier dat aan de sjabloon is gekoppeld, een aangepast veld bevat dat ook wordt gevonden in een aangepast formulier dat aan de taak is gekoppeld, wordt de veldwaarde van de taak gebruikt voor het nieuwe project. Als het aangepaste veld echter leeg is op de taak, wordt de waarde uit de sjabloon gebruikt.

1. Klikken **Wijzigingen opslaan**.
