---
product-area: projects
navigation-topic: manage-issues
title: Uitgiftestatussen automatisch bijwerken in afwachting van feedback naar Bezig
description: Wanneer de primaire contactpersoon van een uitgave een update van de uitgave uitvoert door een veld (inclusief een aangepast veld) bij te werken of een opmerking toe te voegen, wordt de status van de uitgave automatisch bijgewerkt naar In uitvoering.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: 948cd81908df3174eb985d1c65533077d3ef5d49
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Uitgiftestatussen automatisch bijwerken in afwachting van feedback naar Bezig

Wanneer de primaire contactpersoon van een uitgave een update van de uitgave uitvoert door een veld (inclusief een aangepast veld) bij te werken of een opmerking toe te voegen, wordt de status van de uitgave automatisch bijgewerkt naar In uitvoering.

Deze automatische statuswijziging is alleen mogelijk als:

* De kwestie moet door een verzoekrij zijn ingegaan.

  Voor informatie over het creëren van verzoekrijen, zie [Aanvraagwachtrijen maken en beheren](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) sectie. Voor informatie over het creëren van verzoeken, zie [Adobe Workfront-aanvragen maken en verzenden](../../../manage-work/requests/create-requests/create-submit-requests.md).

* De Details van de Rij in de verzoekrij moeten deze montages hebben:
   * **Wanneer iemand een verzoek indient, automatisch** is ingesteld op **Contribute Access**
   * **Status wijzigen** is geselecteerd onder Geavanceerde instellingen

  ![Wachtrijdetails geven Contribute toegang en Wijzigingsstatus is geselecteerd.](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  Wanneer vestiging een verzoekrij, kunt u de toegang primaire contacten aan de kwesties bepalen die zij voorleggen.
  >
  >Wanneer u de instelling Status wijzigen uitschakelt bij het instellen van de aanvraagwachtrij, moet u niet vergeten dat systeembeheerders altijd toegang hebben om de status van problemen te wijzigen, zelfs als de optie Status wijzigen is uitgeschakeld in de instellingen voor de wachtrij van aanvragen.

  Voor meer informatie over de Details van de Rij, zie [Een aanvraagwachtrij maken](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* Het probleem moet in wachtende status zijn.
* Voor problemen op systeemniveau moet er een Awachtback-status (AWF) beschikbaar zijn.

  Voor meer informatie over statussen op systeemniveau raadpleegt u [Een status maken of bewerken](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
