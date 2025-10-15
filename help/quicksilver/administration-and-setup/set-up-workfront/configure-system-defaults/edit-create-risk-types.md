---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Risicotypen bewerken en maken
description: U kunt risico's aan een project in de planningsfase toevoegen om potentiële obstakels te identificeren alvorens om het even welk werk goed te keuren. Risico's zijn mogelijke gebeurtenissen die een tijdige voltooiing van het project of binnen de begroting kunnen verhinderen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Risicotypen bewerken en maken

<!--Audited: 03/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Adobe Workfront heeft een aantal standaardrisicopatypen die u in de planningsfase aan projecten kunt koppelen om potentiële obstakels te identificeren alvorens om het even welk werk goed te keuren.

Risico&#39;s zijn mogelijke gebeurtenissen die een tijdige voltooiing van het project of binnen de begroting kunnen verhinderen.

Naast de standaardrisicstypen kunt u ook een nieuw type risico toevoegen om aan de behoeften van uw organisatie te voldoen.

U kunt risicstypes met projectrisico&#39;s associëren om te identificeren welk soort risico een project zou kunnen ontmoeten.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licentie</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Risicotypes

De types van risico zijn etiketten u voor uw risico&#39;s kunt gebruiken om hen voor rapporteringsdoeleinden te categoriseren.

Als a [!DNL Workfront] beheerder, kunt u [!UICONTROL Risk Types] in het [!UICONTROL **3} gebied van de Opstelling {tot stand brengen.**]

Nadat u de typen risico&#39;s hebt ingesteld, zijn deze allemaal voor uw systeem beschikbaar.

Alle eigenaars van projecten kunnen dezelfde soorten risico&#39;s gebruiken voor hun projecten.

## Risicotypen bewerken en maken

Sommige risicstypen bevinden zich standaard al in [!DNL Workfront] .


U kunt het volgende doen om het aantal risicstypen in uw Workfront-instantie te verbeteren:

* [Bestaande risicopatypen bewerken](#edit-existing-risk-types)
* [Risicotypen maken](#create-risk-types)

### Bestaande risicopatypen bewerken {#edit-existing-risk-types}

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Risk Types]**.
1. Selecteer het risicatype dat u wilt bewerken.
1. Klik het **[!UICONTROL Edit]** pictogram ![ uitgeven pictogram ](assets/edit-icon.png).

   Het [!UICONTROL **geeft het Type van Risico**] vakje uit opent.

   ![ geef risicomatype doos ](assets/edit-risk-type-box.png) uit

   >[!TIP]
   >
   >U kunt de informatie over het risicatype inline bewerken wanneer u dubbelklikt op de naam of beschrijving van een risicatype in een lijst met risicstypen.

1. (Optioneel) Wijzig de naam en de beschrijving van het type risico.

   De velden **[!UICONTROL Name]** en **[!UICONTROL Description]** mogen maximaal 50 tekens bevatten.

1. Klik op **[!UICONTROL Save Changes].**

1. (Facultatief) om een risicatype te schrappen, het in de lijst te selecteren, dan het [!UICONTROL **pictogram van de Schrapping**] ![ te klikken pictogram van de Schrapping ](assets/delete.png), dan ja te klikken [!UICONTROL **, het**] te schrappen. Het risicomatype wordt verwijderd en kan niet worden hersteld.

1. (Facultatief) om een lijst van risicstypes uit te voeren, klik het [!UICONTROL **pictogram van de Uitvoer**] pictogram van de Uitvoer ![. ](assets/export-icon.png) U kunt naar de volgende bestandstypen exporteren:

   * PDF
   * Excel
   * Excel (xlsx)
   * Door tabs gescheiden

   >[!TIP]
   >
   >   U kunt eerst een beperkt aantal soorten risico selecteren en deze vervolgens voor een kleinere lijst exporteren.

### Risicotypen maken {#create-risk-types}

Naast de standaardtypen kunt u ook soorten risico&#39;s maken.

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Risk Types]**.

1. Klik **[!UICONTROL New Risk Type]** om de [!UICONTROL **Nieuwe doos van het Type van Risico**] te openen

   of

   Klik [!UICONTROL **toevoegen Meer Types van Risico**] in de laag-linkerhoek van de lijst van het risicatype om inline risicstypes toe te voegen.

   Het **Nieuwe vakje van het Type van Risico** opent.

   ![ Nieuwe doos van het risicatype ](assets/new-risk-type-box.png)

1. Voeg een **[!UICONTROL Name]** (vereist) en een **[!UICONTROL Description]** (facultatief) voor het risicatype toe.

   De velden **[!UICONTROL Name]** en **[!UICONTROL Description]** mogen maximaal 50 tekens bevatten.

1. Klik op **[!UICONTROL Create Risk Type]**,

   Of als u in-line bewerking hebt gebruikt om uw risicatype toe te voegen, klikt u op **[!UICONTROL Enter]** wanneer u klaar bent.

   >[!TIP]
   >
   >Zie de sectie [[!UICONTROL Edit existing] risicstypen ](#edit-existing-risk-types) in dit artikel voor informatie over het bewerken van een type aangepast risico.

## Risico&#39;s koppelen aan soorten risico&#39;s in projecten

U kunt risicstypes gebruiken om risico&#39;s te etiketteren die aan uw projecten worden toegevoegd.

Voor meer informatie over hoe te om risico&#39;s aan projecten toe te voegen, zie [ risico&#39;s op projecten ](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md) creëren en uitgeven.
