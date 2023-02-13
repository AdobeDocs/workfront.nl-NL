---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: proof-notifications-and-reminders
title: Nieuwe proefe-mail
description: Dit artikel werkt beter voor PiW.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d879b1c6-e862-4653-aa93-90ad92170951
source-git-commit: 0c40e2b4e691d63832842736eaf09eeb67127498
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Nieuwe proefe-mail

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

<!--
<p style="color: #000000;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Make this article work better for PiW.</p>
-->

Wanneer u een nieuwe proefdruk of een nieuwe versie van een proefdruk maakt, nieuwe personen toevoegt aan een proefdruk of een workflow toevoegt aan een proefdruk, kunt u besluiten of u de controleurs een e-mail wilt sturen, zoals in de volgende artikelen wordt uitgelegd:

* [Een geavanceerde proefdruk maken met een geautomatiseerde workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Proefdrukken genereren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

Het e-mailbericht dat uw ontvangers ontvangen, wordt het [!UICONTROL New Proof] e-mail. Alleen de maker van de proef en gebruikers die revisoren mogen toevoegen aan een proefdruk, kunnen dit e-mailbericht besturen. Ontvangers kunnen deze functie niet uitschakelen.

Het e-mailadres voor nieuwe proefdrukken bevat:

* Uw persoonlijke bericht (als u ervoor kiest om er een op te nemen)
* Als u altijd hetzelfde aangepaste bericht naar de controleurs verzendt, is het wellicht verstandig het bericht op te slaan in uw [!UICONTROL Personal settings] onder de [!UICONTROL Proofing defaults] tab. Zie voor meer informatie.
* Persoonlijke link naar het bewijs
* **[!UICONTROL View details]** koppeling die u naar de gekoppelde koppeling brengt [!DNL Workfront] object (zoals een project, taak of uitgave)
* Miniatuur van de proefdrukafbeelding
* De volgende bewijsgegevens:

   * Proefnaam
   * Versienummer

      Zie voor meer informatie.

   * Lijst van de controleurs en hun vorderingen op de proefstukken
   * Een koppeling om de proefdruk met iemand anders te delen

      Zo kunt u de proef-URL en/of de downloadkoppeling delen voor het oorspronkelijke bestand. Hierdoor kunt u niet expliciet revisoren aan de proefdruk toevoegen, u deelt alleen de URL van de openbare proefdruk en de ontvanger krijgt alleen-lezen toegang tot de proefdruk.

      Zie [Een proef delen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) voor meer informatie .

      Als u niet wilt dat deze koppeling wordt weergegeven in de e-mail van de ontvanger, kunt u de optie [!UICONTROL Public Sharing] instellingen op de proefdruk

      (Oorspronkelijke bestand downloaden en Openbare URL). Zie [Proofinggegevens beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) voor meer informatie .

## Het activiteitenlog

Een [!UICONTROL New Proof] e-mail naar een revisor is aangemeld bij de [!UICONTROL Activity] deel van [!UICONTROL Proof details] pagina. Zie  [Beheren[!UICONTROL  Proof Details] in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) voor meer informatie . U kunt controleren of de [!UICONTROL New Proof] E-mail is ingeschakeld op het moment dat u een proefdruk maakt.

![New_Verison_email_-_activity_log.png](assets/new-verison-email---acitivity-log-350x44.png)

>[!NOTE]
>
>* Indien de maker of eigenaar van het bewijs [!UICONTROL Proof Made] e-mails die standaard zijn uitgeschakeld (in hun persoonlijke instellingen), ontvangen geen [!UICONTROL Proof made] of [!UICONTROL New proof] e-mailberichten, zelfs als de [!UICONTROL Notify people by email] wordt ingeschakeld op de pagina Nieuwe proefdruk. Zie voor meer informatie.
>* Als de e-mailmeldingen standaard zijn uitgeschakeld in het dialoogvenster [!UICONTROL Account settings] de maker/eigenaar van het bewijs geen [!UICONTROL Proof made] of [!UICONTROL New proof] e-mails, zelfs als dit is ingeschakeld in de persoonlijke instellingen en de [!UICONTROL Notify] personen via e-mail worden ingeschakeld op de pagina Nieuwe proefdruk. Voor meer informatie, [De [!UICONTROL Proof Made] email](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) en zie.
>




## De optie [!UICONTROL New Proof] e-mail en omvat een aangepast bericht

U kunt opgeven of u een e-mailwaarschuwing wilt verzenden naar de controleurs op een proefdruk wanneer u deze maakt of wanneer u er iemand aan toevoegt.

* [Wanneer u een proefdruk maakt](#when-you-create-a-proof)
* [Wanneer u een revisor aan een proefdruk toevoegt](#when-you-add-a-reviewer-to-a-proof)

### Wanneer u een proefdruk maakt {#when-you-create-a-proof}

Wanneer u een nieuwe proefdruk maakt in het dialoogvenster [!UICONTROL New proof] pagina, onder de **[!UICONTROL Share]** kunt u kiezen of u e-mailwaarschuwingen wilt verzenden:

* Hier kunt u beslissen of u wilt [!UICONTROL Notify people by email] (1) Als u deze optie uitschakelt, ontvangen geen van de revisoren een e-mail om hen te laten weten dat de proefdruk gereed is voor revisie.
* U kunt ook een aangepast bericht opnemen in het e-mailbericht (2).
* Als u besluit uw eigen aangepaste bericht toe te voegen, kunt u een aangepaste onderwerpregel (3) en een bericht in de tekst van de e-mail (4) plaatsen.
* Als u het aangepaste bericht wilt verwijderen, klikt u gewoon op de koppeling (5).

   >[!NOTE]
   >
   >Als u altijd hetzelfde aangepaste bericht naar de controleurs verzendt, is het wellicht een goed idee om het bericht op te slaan in uw persoonlijke instellingen onder de [!UICONTROL Proofing defaults] tab. Zie voor meer informatie.

![New_Proof_page_1.png](assets/new-proof-page-1-350x186.png)

![New_Proof_page_2.png](assets/new-proof-page-2-350x283.png)

### Wanneer u een revisor aan een proefdruk toevoegt {#when-you-add-a-reviewer-to-a-proof}

U kunt aangeven of een nieuwe controleur die aan een bestaande proefdruk is toegevoegd, op de hoogte wordt gesteld van de proefdruk (vergelijkbaar met bovenstaande).

* Voeg eerst nieuwe revisoren toe door op de knop **[!UICONTROL Share this Version]** op de knop **[!UICONTROL Proof details]** pagina (1).

![Proef_Details_pagina_1.png](assets/proof-details-page-1-350x118.png)

* Er wordt een vak weergegeven waarin u nieuwe revisoren kunt toevoegen. Vervolgens kunt u bepalen of u een e-mailbericht wilt ontvangen (2) en een aangepast bericht aan de e-mail wilt toevoegen (3).

![Proef_Details_page_2.png](assets/proof-details-page-2-350x174.png)

* Als u ervoor kiest een aangepast bericht toe te voegen, wordt het vak groter en kunt u een aangepaste onderwerpregel (4) en aangepaste tekst in de hoofdtekst van de e-mail (5) plaatsen. U kunt het aangepaste bericht ook verwijderen door op de koppeling (6) te klikken.

![Proef_Details_page_3.png](assets/proof-details-page-3-350x258.png)
