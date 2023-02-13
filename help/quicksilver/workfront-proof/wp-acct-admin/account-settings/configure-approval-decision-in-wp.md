---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Opties voor goedkeuringsbeslissingen configureren in [!DNL Workfront Proof]
description: Als [!DNL Workfront Proof] beheerder die een Uitgezochte of de uitgave van de Premie plan gebruikt, kunt u opties van het goedkeuringsbesluit op de volgende manieren voor alle proeven vormen die door worden gecreeerd [!DNL Workfront Proof] gebruikers in uw organisatie - BEWERK ME.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 9e1c2a4e-0641-4334-8ff9-dbb203ccbc82
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# Opties voor goedkeuringsbeslissingen configureren in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Als [!DNL Workfront Proof] beheerder die een Uitgezochte of de uitgave van de Premie plan gebruikt, kunt u opties van het goedkeuringsbesluit op de volgende manieren voor alle proeven vormen die door worden gecreeerd [!DNL Workfront Proof] gebruikers in uw organisatie:

* De naam van de beslissing wijzigen
* De volgorde van de beslissingen in de proefdrukviewer wijzigen
* Beslissen welke besluiten moeten worden weergegeven

In dit artikel wordt het volgende uitgelegd:

## Instellingen voor besluit configureren

1. Klik op **[!UICONTROL Account Settings]**.
1. Open de **[!UICONTROL Decisions]** tab.
1. Breng een van de volgende wijzigingen aan:

   * Als u een beslissing wilt verbergen, klikt u op **[!UICONTROL Hide]** rechts van de beslissing die u niet nodig hebt.
   * Als u de naam van een beslissing wilt wijzigen, klikt u op de naam van de beslissing, bewerkt u de beslissing en klikt u buiten het vak (of drukt u op Enter). [!DNL Workfront Proof] werkt de naam van het besluit op alle bestaande proefdrukken in uw systeem bij.

      >[!IMPORTANT]
      >
      >Behoud de logica voor een besluit wanneer u het anders noemt. De standaardbeslissing &#39;Afgewezen&#39; kan bijvoorbeeld worden gewijzigd in &#39;Nieuwe versie vereist&#39;, maar niet in &#39;Verzenden naar printers&#39;.

      Als je terug wilt gaan naar de [!DNL Workfront Proof] standaardinstellingen, kunt u op Standaardinstellingen herstellen klikken.

>[!NOTE]
>
>* De logica achter de besluiten wordt gebruikt om de algemene status van een proefwerkschema te berekenen als er veelvoudige besluiten van diverse niveaus zijn.
>* De besluiten &quot;Goedgekeurd&quot;en &quot;Goedgekeurd met veranderingen&quot;brengen de volgende fase in automatische werkschema&#39;s teweeg.
>* Als u de naam van een beslissing wijzigt en u de logica wilt controleren, klikt u op **[!UICONTROL Activity]** in het linkernavigatievenster en controleer uw activiteitenlogboek waar de oorspronkelijke besluiten tussen haakjes worden weergegeven.
>
>  ![2016-12-20_1921.png](assets/2016-12-20-1921-350x132.png)>

## Redenen voor besluiten

Beslissingsredenen zijn een goede manier om aanvullende informatie over besluiten over een bewijs vast te leggen.

1. Klik op **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]**.

1. Open de **[!UICONTROL Decisions]** tab.
Standaard zijn er redenen voor alle besluitvormers op uw proefdrukken, maar u kunt dat beperken tot primaire besluitvormers.
Afhankelijk van uw vereisten kunt u meerdere redenen selecteren of één keuzelijst maken. U kunt ook redenen verplicht stellen, wat betekent dat revisoren een reden moeten kiezen voordat ze hun beslissing op een bewijs kunnen bewaren.
   ![Redenen_instellen.png](assets/reasons-setup-350x121.png)

1. In de **[!UICONTROL Reasons]** sectie, klikt u op **[!UICONTROL New reason]**.
   ![New_reason.png](assets/new-reason-350x135.png)

1. Typ een titel voor de sectie Redenen in het vak onder **[!UICONTROL Reason]**.
1. Als u een tekstvak wilt opnemen, selecteert u **[!UICONTROL Include text box]**.
1. Klik op **[!UICONTROL Save]**.
   ![reasons_setup_2.png](assets/reasons-setup-2-350x146.png)
De belangrijkste stap is het selecteren van de beslissingen die de redenen moeten weergeven. Als je dat vergeet, zullen de redenen niet op je proefdrukken worden vermeld.

1. Schakel de selectievakjes in het dialoogvenster **[!UICONTROL Display reasons]** in de lijst met beslissingen boven aan de pagina. U kunt een of meer beslissingen selecteren om uw redenen.
   ![reason_besluit_selection.png](assets/reasons---decision-selection-350x150.png)

## Berichten na een beslissing maken

U kunt een bericht voor een postbeslissing maken om weer te geven nadat een controleur zijn beslissing over de bewijsmiddelen heeft opgeslagen.

1. Klik op **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]**.

1. Open de **[!UICONTROL Decisions]** tab.
1. In de **[!UICONTROL Post decision message]** sectie, klikt u op **[!UICONTROL Edit]** aan het einde van de **[!UICONTROL Message]** rij.
U kunt ook beslissen of u wilt dat het bericht aan alle besluitvormers wordt getoond of dat u het tot de Primaire besluitvormer wilt beperken.
   ![post_Decision_message_set_up.png](assets/post-decision-message-set-up-350x125.png)

1. In de **[!UICONTROL Display message]** kolom, specificeer de besluiten dit bericht zou moeten worden getoond.
Als u niet minstens één beslissing selecteert, wordt het bericht niet weergegeven op uw proefdrukken. Controleer minstens één vakje in deze kolom.
   ![post_Decision_message_set_up_2.png](assets/post-decision-message-set-up-2-350x151.png)
