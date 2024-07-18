---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Opties voor goedkeuringsbeslissingen configureren in  [!DNL Workfront Proof]
description: U kunt de opties van het goedkeuringsbesluit voor alle proeven vormen die door  [!DNL Workfront Proof]  worden gecreeerd gebruikers in uw organisatie.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 9e1c2a4e-0641-4334-8ff9-dbb203ccbc82
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Opties voor goedkeuringsbeslissingen configureren in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [ het Bewijzen ](../../../review-and-approve-work/proofing/proofing.md).

Als [!DNL Workfront Proof] beheerder die een Uitgezochte of de uitgave van de Premie plan gebruikt, kunt u de opties van het goedkeuringsbesluit op de volgende manieren voor alle proeven vormen die door [!DNL Workfront Proof] gebruikers in uw organisatie worden gecreeerd:

* De naam van de beslissing wijzigen
* De volgorde van de beslissingen in de proefdrukviewer wijzigen
* Beslissen welke besluiten moeten worden weergegeven

In dit artikel wordt het volgende uitgelegd:

## Instellingen voor besluit configureren

1. Klik op **[!UICONTROL Account Settings]**.
1. Open de tab **[!UICONTROL Decisions]** .
1. Breng een van de volgende wijzigingen aan:

   * Als u een beslissing wilt verbergen, klikt u op **[!UICONTROL Hide]** rechts van de beslissing die u niet nodig hebt.
   * Als u de naam van een beslissing wilt wijzigen, klikt u op de naam van de beslissing, bewerkt u de beslissing en klikt u buiten het vak (of drukt u op Enter). [!DNL Workfront Proof] werkt de naam van de beslissing bij op alle bestaande proefdrukken in uw systeem.

     >[!IMPORTANT]
     >
     >Behoud de logica voor een besluit wanneer u het anders noemt. De standaardbeslissing &#39;Afgewezen&#39; kan bijvoorbeeld worden gewijzigd in &#39;Nieuwe versie vereist&#39;, maar niet in &#39;Verzenden naar printers&#39;.

     Als u wilt terugkeren naar de standaardinstellingen van [!DNL Workfront Proof] , kunt u op Standaardinstellingen herstellen klikken.

>[!NOTE]
>
>* De logica achter de besluiten wordt gebruikt om de algemene status van een proefwerkschema te berekenen als er veelvoudige besluiten van diverse niveaus zijn.
>* De besluiten &quot;Goedgekeurd&quot;en &quot;Goedgekeurd met veranderingen&quot;brengen de volgende fase in automatische werkschema&#39;s teweeg.
>* Als u de naam van een beslissing wijzigt en u de logica wilt verifiëren, klikt u op **[!UICONTROL Activity]** in het navigatievenster aan de linkerkant en controleert u het activiteitenlogboek, waar de oorspronkelijke beslissingen tussen haakjes worden weergegeven.
>
>  ![ 2016-12-20_1921.png ](assets/2016-12-20-1921-350x132.png)>

## Redenen voor besluiten

Beslissingsredenen zijn een goede manier om aanvullende informatie over besluiten over een bewijs vast te leggen.

1. Klik op **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]** .

1. Open de tab **[!UICONTROL Decisions]** .
Standaard zijn er redenen voor alle besluitvormers op uw proefdrukken, maar u kunt dat beperken tot primaire besluitvormers.
Afhankelijk van uw vereisten kunt u meerdere redenen selecteren of één keuzelijst maken. U kunt ook redenen verplicht stellen, wat betekent dat revisoren een reden moeten kiezen voordat ze hun beslissing op een bewijs kunnen bewaren.
   ![ Redons_setup.png ](assets/reasons-setup-350x121.png)

1. Klik in de sectie **[!UICONTROL Reasons]** op **[!UICONTROL New reason]** .
   ![ New_reason.png ](assets/new-reason-350x135.png)

1. Typ een titel in het vak onder **[!UICONTROL Reason]** om de redenen.
1. Selecteer **[!UICONTROL Include text box]** als u een tekstvak wilt opnemen.
1. Klik op **[!UICONTROL Save]**.
   ![ reasons_setup_2.png ](assets/reasons-setup-2-350x146.png)
De belangrijkste stap is het selecteren van de beslissingen die de redenen moeten weergeven. Als je dat vergeet, zullen de redenen niet op je proefdrukken worden vermeld.

1. Schakel de vakken in de kolom **[!UICONTROL Display reasons]** in de lijst met beslissingen boven aan de pagina in. U kunt een of meer beslissingen selecteren om uw redenen.
   ![ reasons_-_decisions_selection.png ](assets/reasons---decision-selection-350x150.png)

## Post-beslissingsbericht maken

U kunt een bericht voor een postbeslissing maken om weer te geven nadat een controleur zijn beslissing over de bewijsmiddelen heeft opgeslagen.

1. Klik op **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]** .

1. Open de tab **[!UICONTROL Decisions]** .
1. Klik in de sectie **[!UICONTROL Post decision message]** op **[!UICONTROL Edit]** aan het einde van de rij **[!UICONTROL Message]** .
U kunt ook beslissen of u wilt dat het bericht aan alle besluitvormers wordt getoond of dat u het tot de Primaire besluitvormer wilt beperken.
   ![ post_Decision_message_set_up.png ](assets/post-decision-message-set-up-350x125.png)

1. Geef in de kolom **[!UICONTROL Display message]** de beslissingen op waarop dit bericht moet worden weergegeven.
Als u niet minstens één beslissing selecteert, wordt het bericht niet weergegeven op uw proefdrukken. Controleer minstens één vakje in deze kolom.
   ![ post_Decision_message_set_up_2.png ](assets/post-decision-message-set-up-2-350x151.png)
