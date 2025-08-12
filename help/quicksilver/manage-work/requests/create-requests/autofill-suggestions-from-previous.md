---
title: Een verzoek uit vorige gegevens automatisch invullen
content-type: reference
description: Met AI kunt u aanvraagvelden automatisch invullen met gegevens uit vorige aanvragen.
author: Becky
feature: Get Started with Workfront
exl-id: a0cd1fbf-d3c6-454c-a85a-ceca4b1e8a7b
source-git-commit: fd42ac97be05df9499ea3214642099738ccc69b1
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---

# Een verzoek uit vorige gegevens automatisch invullen

>[!NOTE]
>
>* Deze functionaliteit zal als open bèta op het volgende programma beschikbaar zijn:
>
>   * Maandbericht: 11 september 2025
>   * Kwartaalversie: 16 oktober 2025

Met AI kunt u aanvraagvelden automatisch invullen op basis van eerdere aanvragen. U kunt deze suggesties goedkeuren of verwerpen alvorens het verzoek in te dienen.

Met Automatisch vullen worden geen velden overschreven die u al hebt ingevuld.

Gebruikers ontvangen geen suggesties voor gegevens waartoe zij anders geen toegang hebben.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Nieuw: Medewerker of hoger</p>
   of
   <p>Huidig: Verzoek of hoger</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot problemen bewerken</p>  </td> 
  </tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td><p>Toegang tot het toevoegen van verzoeken aan een aanvraagwachtrij</p> <p>De toestemmingen van de mening of hoger op het bestaande verzoek</p> <p>Voor informatie bij vestiging ziet een verzoekrij, <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref"> een Rij van het Verzoek </a> creëren. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Suggesties ophalen bij het invullen van het formulier

Als u het formulier automatisch invult, kunt u aangeven welke veldwaarden u wilt gebruiken. Als u waarden invoert in de aanvraagvelden, vergelijkt Workfront deze waarden met eerdere aanvragen. Als de ingevoerde waarde in eerdere verzoeken in een vergelijkbare context nauw samenvalt met andere veldwaarden, stelt Workfront deze waarden voor.

Als een kliniek bijvoorbeeld altijd dezelfde factureringscode gebruikt, suggereert Workfront dat factureringscode in het juiste veld wordt gebruikt wanneer de naam van de kliniek wordt ingevoerd.

Op eerdere verzoeken gebaseerde suggesties gebruiken:

1. Maak een aanvraag.

   Voor instructies, zie [ verzoeken ](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md) creëren en voorleggen.

1. Velden invullen.

   Terwijl u velden invult, kunnen in andere velden suggesties worden weergegeven.

1. Voor elke gebiedssuggestie, keurt de uitgezochte **** goed of **verwerpt** voor dat gebied.

   ![ Accepteer of verwerp suggestie ](assets/accept-reject-suggestion.png)

   of

   Selecteer **goedkeuren allen** of **verwerping allen** bij de bovenkant van de pagina om alle suggesties goed te keuren of te verwerpen.

   >[!NOTE]
   >
   >Eventuele suggesties die niet zijn gecontroleerd, worden automatisch geaccepteerd wanneer u het verzoek indient.
