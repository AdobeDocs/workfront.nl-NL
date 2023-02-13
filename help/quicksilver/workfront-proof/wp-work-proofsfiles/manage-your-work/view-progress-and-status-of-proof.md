---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: De voortgang en status van een proefdruk weergeven [!DNL Workfront Proof]
description: Het bewijs van voortgang geeft het werk aan dat is verricht op een bewijs vanaf het moment dat u de bewijzen aan de controleurs stuurt tot het moment dat zij een beslissing nemen over het bewijs.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 8fd85595-1403-490e-9d52-2ba5b01457b7
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1112'
ht-degree: 0%

---

# De voortgang en status van een proefdruk weergeven [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

## Proefvoortgang

Het bewijs van voortgang geeft het werk aan dat is verricht op een bewijs vanaf het moment dat u de bewijzen aan de controleurs stuurt tot het moment dat zij een beslissing nemen over het bewijs.

* [Voortgangspictogrammen](#progress-icons)
* [Voortgangsniveaus proefdrukken](#levels-of-proof-progress)

### Voortgangspictogrammen {#progress-icons}

De voortgangspictogrammen S, O, C en D worden weergegeven op de voortgangsbalk en geven de voortgang van de proefdruk aan.

![proof_edit_existing_progress.png](assets/proof-edit-existing-progress-350x78.png)

Zij geven de volgende informatie over een bewijs aan:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Pictogram Voortgang</strong> </p> </td> 
   <td> <p><strong>Beschrijving</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt="proof_progress_sent_icon.png"> </p> </td> 
   <td> <p><strong>Verzonden</strong>. Het bewijs is naar de controleurs gestuurd.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-opened-icon.png" alt="proof_progress_opened_icon.png"> </p> <p> </p> </td> 
   <td> <p><strong>Geopend</strong>. Een revisor heeft de pagina Proefgegevens geopend of de proefdruk zelf geopend in de proefdrukviewer.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-comment-icon.png" alt="proof_progress_comment_icon.png"> </p> </td> 
   <td> <p><strong>Opmerkingen</strong>. Revisoren (gebruikers die opmerkingen kunnen maken) hebben opmerkingen gemaakt over de proefdruk.</p> <p>Als er geen controleurs zijn aangewezen voor de proefdruk, wordt dit pictogram niet weergegeven.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt="proof_progress_decisions_icon.png"> </p> </td> 
   <td> <p><strong>Besluit</strong>. Een controleur heeft een besluit genomen over het bewijs.</p> <p>Als er geen fiatteurs (besluitvormers) voor de proefdruk zijn aangewezen, wordt dit pictogram niet weergegeven. </p> </td> 
  </tr> 
 </tbody> 
</table>

Deze pictogrammen kunnen in de volgende kleuren worden weergegeven om bepaalde informatie over de voortgang van het bewijs aan te geven:

* **Groen**. Voltooid.
* **Wit**. Niet voltooid.
* **Oranje**. Niet voltooid en deadline is minder dan 24 uur.
* **Rood**. Niet volledig en na de deadline.

### Voortgangsniveaus proefdrukken {#levels-of-proof-progress}

Workfront Proof gebruikt de voortgangspictogrammen om de voortgang van een proefdruk op elk van de volgende niveaus bij te houden:

* Voor elke controleur, op basis van de activiteit van die persoon op het bewijs.
* Voor elk stadium, gebaseerd op de vooruitgang de recensent op het stadium die het meest achterop in het proefdrukproces is. Zie voor meer informatie [Overzicht van geautomatiseerde werkstroomfasen](../../../review-and-approve-work/proofing/proofing-overview/stages.md).
* Voor de proefdruk, op basis van de voortgang van het werkgebied (groep van controleurs), dat het meest achterloopt in het proefdrukproces.

Een voorbeeld van hoe [!DNL Workfront Proof] bepaalt de voortgang met behulp van de revisor of het stadium dat het meest achterloopt. Stel dat drie revisoren een beslissing moeten nemen op basis van een bewijs. Als twee van hen hun besluit hebben genomen, maar de derde niet, dan blijkt de voortgangsbalk voor het bewijs niet groen uit het feit dat de D nog niet is afgehandeld.

Als de [!UICONTROL Primary Decision Maker] de instelling wordt gekozen op basis van een bewijs en de primaire besluitvormer legt een besluit voor, de D in de voortgangsbalk van het bewijs wordt groen voor alle controleurs omdat geen andere besluiten vereist zijn.

Als de [!UICONTROL Only One Decision Required] De instelling wordt geselecteerd op basis van een bewijs en een revisor geeft een beslissing. De D in de voortgangsbalk van het bewijs wordt groen voor alle revisoren omdat er geen andere beslissingen hoeven te worden genomen.

## Proefstatus

De status van de proefdruk geeft de status aan van de beslissingen die voor de proefdruk vereist zijn.

![proof_edit_existing_status.png](assets/proof-edit-existing-status-350x78.png)\
De standaardstatusopties zijn:

* In behandeling
* Goedgekeurd
* Goedgekeurd met wijzigingen
* Wijzigingen vereist
* Niet relevant

Als er aangepaste beslissingen in uw account zijn geconfigureerd, weerspiegelen de statusopties uw aangepaste beslissingsinstellingen.

De status van het bewijs wordt aangestuurd door de &quot;worst case&quot;-deelnemer. Stel dat er bijvoorbeeld drie beslissingen zijn over het bewijs: twee hebben de status van **Geaccepteerd** en één heeft de status van **Geweigerd**. Het &quot;worst case&quot;-besluit van de afwijzing van de overregulering van de overige besluiten en de algemene status van het bewijs worden weergegeven als **Geweigerd**.

## Voortgang en status weergeven {#viewing-progress-and-status}

U kunt de voortgang en status van proefdrukken, fasen en revisoren in elk werkgebied bekijken.

* [Proefoverzicht](#proof-summary)
* [Menu Werkgebiedhandelingen](#stage-actions-menu)
* [In de [!UICONTROL Summary] kunt u ook de menu&#39;s met revisieacties openen, op voorwaarde dat u bewerkingsrechten hebt voor de proefdruk. Zie Proefprofielen voor proefdrukmachtigingen in Workfront Proef en Proefdrukrollen beheren in Workfront Proof voor meer informatie. De [!UICONTROL Reviewer actions] (1) wordt weergegeven wanneer u de muisaanwijzer op de details van de Revisor plaatst en u in staat stelt:](#in-the-summary-section-you-can-also-access-the-reviewer-actions-menus-provided-you-have-edit-rights-on-the-proof-for-more-information-see-proof-permissions-profiles-in-workfront-proof-and-manage-proof-roles-in-workfront-proof-the-reviewer-actions-menu-1-appears-when-you-hover-over-the-reviewer-s-details-and-allows-you-to)
* [Menu Proefacties](#proof-actions-menu)

### Proefoverzicht {#proof-summary}

Elke proef in de omslag heeft een uitbreidbare samenvatting die u snel de details van de proef kunt bekijken en uitgeven.

Het overzicht uitvouwen of samenvouwen:

1. Klik op de pijl links van de proefdruk in het dashboard of in een lijstweergave.

![Summary_expandable.png](assets/summary-expandable-350x68.png)

De samenvatting bevat het volgende:

* Workflow (2)
* Versie (3)
* Map (4)
* Staat (5)\
   ![summary_2.png](assets/summary-2-350x160.png)

In het overzicht kunt u de volgende gegevens van uw proefdruk weergeven en bewerken:

* Voortgang van proefdrukken (1)
* Voortgang van elke fase (2)
* Termijn voor het werkgebied (3)
* Details revisor:

   * Aantal opmerkingen en antwoorden van elke controleur (4)
   * Voortgang van elke controleur (5)
   * Beslissing (als een besluit een elektronische handtekening heeft, wordt naast de beslissing die dit aangeeft een pictogram weergegeven.) (6)
   * Rol op het bewijs (7)
   * Instellingen voor e-mailwaarschuwingen (8)

>[!NOTE]
>
>Uw mogelijkheid om de proefdrukgegevens te bewerken, hangt af van uw rechten op de proefdrukweergave (zie [Profielen met proefmachtigingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) en [Proefrollen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![summary_details_3.png](assets/summary-details-3-350x160.png)

### [!UICONTROL Stage Actions] Menu  {#stage-actions-menu}

Elk stadium van uw werkstroom heeft een afzonderlijk menu, dat u toestaat om bulkacties met betrekking tot de recensenten in dat stadium uit te voeren.

De [!UICONTROL Stage actions] wordt weergegeven wanneer u de cursor boven de sectie Werkgebied houdt (1) en u

* [!UICONTROL Message all] (2)
* [!UICONTROL Share] (3)
* [!UICONTROL Delete stage] (4)

>[!NOTE]
>
>De beschikbaarheid van deze opties hangt af van uw rechten op de proefdruk (zie [Profielen met proefmachtigingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) en [Proefrollen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![Stage_actions_menu.png](assets/stage-actions-menu-350x161.png)

In de sectie Overzicht kunt u ook de menu&#39;s voor revisieacties openen, op voorwaarde dat u bewerkingsrechten hebt voor de proefdruk. Zie voor meer informatie [Profielen met proefmachtigingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) en [Proefrollen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md). Het menu Acties van Revisor (1) wordt weergegeven wanneer u de muisaanwijzer boven de details van de Revisor houdt. U kunt dan het volgende doen:

* Een bericht naar de controleur sturen (2)
* Details van revisor bewerken (3)- Hiermee kunt u de weergavenaam, de proefdrukrol en de e-mailwaarschuwing voor die revisor bewerken
* Van hen de eigenaar van het bewijs maken (4)
* Van hen de primaire besluitvormer maken (5)
* Uit het bewijs halen (6)

>[!NOTE]
>
>De zichtbaarheid van deze opties hangt af van uw rechten op de proefdruk (zie [Profielen met proefmachtigingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) en [Proefrollen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![Revisor_acties_menu.png](assets/reviewer-actions-menu-350x135.png)

### Menu Proefacties {#proof-actions-menu}

Elke proef heeft ook een menu (1) dat u toestaat om de hieronder acties uit te voeren:

* U hebt toegang tot de pagina Proefgegevens (2)
* Het bewijs delen met andere personen (3)
* Een bericht verzenden aan revisoren (4)
* Een nieuwe versie van de proefdruk maken (5)
* Bewijs kopiëren (6)
* Het oorspronkelijke bestand downloaden (7)
* Proofingkoppelingen delen (8)
* Opmerkingen afdrukken (9)
* Een Excel-overzicht van de proefdruk aanvragen (10)
* De proefdruk vergrendelen (11)
* De proefdruk verwijderen (12)

![Proef_actions_menu_1_.png](assets/proof-actions-menu--1--350x158.png)

>[!NOTE]
>
>De beschikbaarheid van deze opties hangt af van uw rechten op de proefdruk (zie [Profielen met proefmachtigingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) en [Proefrollen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

Voor informatie over de voortgang en status van de proefdrukken binnen [!DNL Workfront], zie [Voortgang en status weergeven](#viewing-progress-and-status).

Ga voor informatie over de voortgang en status van de weergave in de Desktop Proofing Viewer naar [Een workflow controleren in de conceptviewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-workflow.md).
