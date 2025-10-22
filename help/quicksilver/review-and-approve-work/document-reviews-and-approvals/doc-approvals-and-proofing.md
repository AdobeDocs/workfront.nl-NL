---
product-area: documents
navigation-topic: approvals
title: Verenigde goedkeuringen en proefdrukken samen gebruiken
description: U kunt Verenigde Goedkeuringen met proef gebruiken.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# Verenigde goedkeuringen en proefdrukken samen gebruiken

De verenigde goedkeuringen in Workfront introduceren een nieuwe reeks eigenschappen om u te helpen documenten herzien en goedkeuren. U kunt een Unified Approval-workflow gebruiken met de bestaande proefdrukviewer om opmerkingen en markeringen toe te voegen aan documenten die worden gecontroleerd.

Er zijn sommige zeer belangrijke verschillen in het werkschema wanneer het gebruiken van Verenigde Goedkeuringen en het proef samen:

* Deelnemers worden weergegeven in de samenvatting van het document, niet in de proefdrukworkflow

* De gegevens in de documentlijst die zijn verzonden, geopend, Opmerking, Besluit (SOCD), houden verband met de proefdrukken en weerspiegelen niet de beslissingsstatus van het document.

## Een document uploaden en een proefdruk maken

1. Ga naar het project, de taak, of de kwestie waar u een nieuw document wilt toevoegen.
1. Klik het **lusje van Documenten**, dan klik **voeg Nieuw** drop-down menu toe.
of
Sleep het document naar de documentlijst.

   >[!NOTE]
   >
   >Als u **hebt produceren automatisch proeven wanneer het uploaden van documenten** toegelaten in uw gebruikersprofiel, leidt het systeem automatisch tot een eenvoudige proef.

1. Beweeg over het document, dan klik **creeer de verbinding van het Bewijs** die onder de documentnaam verschijnt, en selecteer **Eenvoudige Bewijs**. U moet een eenvoudige proefdruk maken omdat u de proefdrukworkflow niet gebruikt voor goedkeuringen.

Gebruikers die als deelnemers zijn toegewezen, kunnen de proefdrukviewer gebruiken om opmerkingen en markeringen aan het document toe te voegen. Ga verder met de volgende sectie om te leren hoe u deelnemers voor revisies kunt toevoegen.

## Documentoverzicht openen en deelnemers toewijzen

U kunt revisoren, fiatteurs of een combinatie van beide toewijzen:

* **de Controleurs** kunnen commentaren toevoegen en activa opsommen. Als ze klaar zijn, kunnen ze de revisie als voltooid markeren. Het is niet nodig de revisie als voltooid te markeren om het document verder te laten gaan in het goedkeuringsproces.
* **Approvers** kunnen commentaren toevoegen en activa opsommen. Zij moeten een besluit nemen om het goedkeuringsproces vooruit te helpen.

Om deelnemers toe te wijzen:

1. Selecteer het document dat u hebt geüpload en open de samenvatting van het document.
   ![ Open documentsamenvatting ](assets/open-doc-summary.png)

1. De rol neer aan de sectie van Goedkeuringen, dan klikt **toevoegt**.

1. (Optioneel) Kies een bestaande goedkeuringssjabloon. Gebruikers met een standaardlicentie kunnen acceptatiesjablonen maken die u kunt gebruiken vanuit het gedeelte Instellen. Voor meer informatie, zie [ een Malplaatje van de Goedkeuring voor activa en documenten ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) creëren.

1. (Optioneel) Stel een deadline in voor de goedkeuring. Gebruikers en teams worden 72 uur per e-mail op de hoogte gesteld en 24 uur vóór de opgegeven deadline.

1. Als u een fiatteur wilt toevoegen, klikt u op de knop fiatteur en typt u een gebruiker- of teamnaam.

1. Als u een revisor wilt toevoegen, klikt u op de knop Revisor en typt u de naam van een gebruiker of team.

   ![ voegt fiatteurs ](assets/add-approvers.png) toe

1. Zodra u alle recensenten en fiatteurs hebt toegevoegd, klik **voorleggen Verzoek**. Deelnemers worden via e-mail op de hoogte gesteld.

## Maak zo nodig een nieuwe versie

Als u nog een revisie- en goedkeuringsronde nodig hebt, kunt u een nieuwe proefversie maken en de vorige deelnemers, nieuwe deelnemers of een combinatie van beide toevoegen. In het overzicht van het document kunt u informatie over eerdere versies en deelnemers weergeven.

Een nieuwe versie toevoegen:

1. Sleep het nieuwe bestand naar het vorige document in Workfront. Hiermee wordt automatisch een nieuwe versie gemaakt.

1. Zodra het document eindigt uploadend, selecteer het document, dan klik **creeer bewijs** > **Eenvoudige proef**.

1. Selecteer het document opnieuw en open het document Summary.
   ![ Open documentsamenvatting ](assets/open-doc-summary.png)

1. De rol neer aan de sectie van Goedkeuringen, dan klikt **toevoegt**.

1. (Optioneel) Kies een bestaande goedkeuringssjabloon. Gebruikers met een standaardlicentie kunnen acceptatiesjablonen maken die u kunt gebruiken vanuit het gedeelte Instellen. Voor meer informatie, zie [ een Malplaatje van de Goedkeuring voor activa en documenten ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) creëren.

1. (Optioneel) Stel een deadline in voor de goedkeuring. Gebruikers en teams worden 72 uur per e-mail op de hoogte gesteld en 24 uur vóór de opgegeven deadline.

1. Als u een fiatteur wilt toevoegen, klikt u op de knop fiatteur en typt u een gebruiker- of teamnaam of kiest u een fiatteur uit de vorige versie.

1. Als u een revisor wilt toevoegen, klikt u op de knop Revisor en typt u een gebruiker- of teamnaam. Kies vervolgens een revisor uit de vorige versie.

   ![ voegt fiatteurs ](assets/add-approvers.png) toe

1. Zodra u alle recensenten en fiatteurs hebt toegevoegd, klik **voorleggen Verzoek**. Deelnemers worden via e-mail op de hoogte gesteld.

<!-- add info about reusing previous participants once released -->


## Het bewijs beoordelen en een beslissing nemen

Het document wordt pas naar een goedgekeurde status verplaatst als alle toegewezen fiatteurs &quot;Goedgekeurd&quot; hebben gekozen.

Een document controleren en goedkeuren:

1. Ga naar uw overzicht e-mailbericht, en klik aan **gaan** herzien.

1. Zodra u in Workfront bent, klik **gaan aan proef**.

1. Bekijk de inhoud en voeg eventuele opmerkingen of markeringen toe. Voor meer informatie over hoe te om de het proeven kijker te gebruiken, zie [ proefdrukken van het Overzicht binnen Adobe Workfront: artikelindex ](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Kies een van de volgende beslissingen:

   * **keur** goed: Het document vereist geen veranderingen en is klaar voor gebruik.
   * **keur met veranderingen** goed: Het document vereist veranderingen en is klaar voor gebruik zodra zij worden gemaakt. Aanvullende goedkeuring is niet vereist.
   * **het werk van behoeften**: Het document vereist veranderingen en is niet klaar voor gebruik. Nadat de opgegeven wijzigingen zijn aangebracht, moet het document worden geüpload als een nieuwe versie en door een andere goedkeuringsronde worden geleid. Voor meer informatie bij het uploaden van een nieuwe versie, zie [ een nieuwe versie creëren zoals nodig ](#create-a-new-version-as-needed) in dit artikel.

Nadat u een beslissing hebt genomen, wordt de eigenaar van het document via e-mail op de hoogte gesteld.

