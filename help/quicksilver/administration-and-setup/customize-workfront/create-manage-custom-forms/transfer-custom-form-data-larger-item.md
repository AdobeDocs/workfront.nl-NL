---
title: Aangepaste formuliergegevens overbrengen bij de conversie van een object
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Wanneer het werk dat in een het werkpunt wordt bepaald te groot wordt, kunt u het in een groter het werkpunt omzetten.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Aangepaste formuliergegevens overbrengen bij de conversie van een object

Afhankelijk van de bedrijfsbehoeften van uw organisatie, zou het werk dat in een taak of een kwestie wordt bepaald te groot kunnen worden om het binnen de taak of de kwestie te beheren. In dit geval kunt u ze omzetten in een groter werkitem:

* U kunt uitgaven in taken of in projecten omzetten
* U kunt taken omzetten in projecten

Als u aangepaste formuliergegevens van een uitgave wilt overbrengen naar een taak of project, moet u de twee taken in dit artikel in de onderstaande volgorde uitvoeren.

Zie voor meer informatie [Overzicht van conversie van problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md) of [Overzicht van conversie van problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-abonnement*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> <p>Ga voor informatie over hoe Workfront-beheerders deze toegang verlenen naar <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, type licentie of configuraties op toegangsniveau u hebt.

## Eerste: Het aangepaste formulier kopiëren {#first-copy-the-custom-form}

Eerst moet u ervoor zorgen dat u aangepaste formuliergegevens behoudt voor een taak of uitgave die u wilt converteren. Omdat de aangepaste formuliergegevens exact moeten overeenkomen met het geconverteerde item, is het aan te raden het formulier te dupliceren, zodat u het aan het nieuwe object kunt koppelen.

>[!TIP]
>
>Een andere manier om aangepaste formuliergegevens in deze situatie te behouden, is door het grotere objecttype toe te voegen aan het aangepaste formulier. Zie de sectie [Een aangepast formulier bewerken starten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) in het artikel [Een aangepast formulier maken of bewerken](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Aangepaste Forms**.
1. Selecteer het aangepaste formulier voor taken of uitgaven en klik op **Kopiëren**.
1. In de **Aangepast formulier** geeft u een naam op voor het nieuwe formulier.

1. Van de **Formuliertype** selecteert u het type object waarvoor u het nieuwe aangepaste formulier wilt maken

   **Voorbeeld:** Selecteer Project als u de aangepaste formuliergegevens naar een project wilt overbrengen.

1. Klikken **Formulier kopiëren**.

   Dit gekopieerde aangepaste formulier kan nu worden gekoppeld aan een taak of project.

1. Doorgaan naar [Tweede: De uitgave of taak converteren en de aangepaste formuliergegevens overdragen](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Tweede: De uitgave of taak converteren en de aangepaste formuliergegevens overdragen {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Kopieer het aangepaste formulier naar de uitgave of taak die u converteert, zoals wordt uitgelegd in de sectie [Eerste: Het aangepaste formulier kopiëren](#first-copy-the-custom-form) in dit artikel.
1. Converteer het probleem of de taak met de opdracht **Aangepaste Forms** in het vak dat wordt weergegeven, selecteert u het aangepaste formulier dat u hebt gekopieerd. Zie de volgende artikelen voor instructies:

   * [Een uitgave converteren naar een project in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Een uitgave converteren naar een taak in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Een taak omzetten in een project](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. In de **Omzetten in (objecttype)** in het dialoogvenster dat wordt weergegeven, klikt u op de knop **Forms toevoegen** en selecteert u het formulier dat u in de vorige sectie hebt gekopieerd.

   De informatie die wordt vastgelegd in de aangepaste velden van de uitgave wordt nu overgebracht naar het aangepaste formulier op de taak.

