---
product-previous: workfront-proof
product-area: documents
navigation-topic: share-proofs-and-files
title: Proefrollen beheren in [!DNL Workfront Proof]
description: De rollen van het bewijs laten u toe om toestemmingen aan gebruikers te verlenen die door het toestemmingsprofiel worden beperkt dat op hun gebruikersprofiel wordt gevormd. (Zie Proefprofielen voor machtigingen in voor meer informatie over machtigingsprofielen [!DNL Workfront Proof].)
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b371cc20-4226-49ce-96c6-9815b2e84713
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1324'
ht-degree: 0%

---

# Proefrollen beheren in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

De rollen van het bewijs laten u toe om toestemmingen aan gebruikers te verlenen die door het toestemmingsprofiel worden beperkt dat op hun gebruikersprofiel wordt gevormd. (Zie voor meer informatie over machtigingsprofielen [Profielen met proefmachtigingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).)

Proefrollen verschillen van accountprofielen. Uw accountprofiel heeft betrekking op het algemene machtigingsniveau in uw account en heeft invloed op de rechten die u hebt op alle proefdrukken in uw account, ook op de rechten die niet expliciet met u zijn gedeeld.

Zie voor meer informatie [Profielen met proefmachtigingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Proefrollen

De volgende proefdrukrollen worden aan gebruikers toegekend voor een afzonderlijke proefdruk op het moment dat de gebruiker wordt verzocht de proefdruk te beoordelen:

* [Alleen-lezen](#read-only)
* [Revisor](#reviewer)
* [Fiatteur](#approver)
* [Revisor en fiatteur](#reviewer-approver)
* [Auteur](#author)
* [Moderator](#moderator)

De proefdrukrol bepaalt welke acties een recensent met betrekking tot die specifieke proef kan ondernemen.

Als u bijvoorbeeld Revisor bent, wordt u gevraagd de proefdruk te controleren door markeringen en opmerkingen toe te voegen. Als u Revisor &amp; fiatteur bent, wordt u gevraagd om de bewijsvoering te beoordelen en ook een beslissing te nemen.

Bepaalde proefdrukrollen geven een revisor bewerkingsrechten op de proefdruk (zelfs als zijn accountprofiel dat niet doet) en bieden deze een aantal extra functies, zoals het toevoegen van handelingen voor opmerkingen, het maken van nieuwe versies en het toevoegen van meer controleurs aan de proefdruk.

Raadpleeg de volgende artikelen voor meer informatie:

* [Handelingen gebruiken voor opmerkingen bij proefdrukken](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)
* [Een proef delen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)

### Alleen-lezen

{#read-only}

![schoner.png](assets/cleaner.png) Kan een proefdruk weergeven

![no.png](assets/no.png) Kan geen markeringen toevoegen

![no.png](assets/no.png) Kan geen opmerkingen toevoegen

![no.png](assets/no.png) Kan geen beslissing nemen

![no.png](assets/no.png) Kan opmerkingen van anderen niet verwijderen

![no.png](assets/no.png) Heeft geen bewerkingsrechten op de proefdruk

>[!NOTE]
>
>Als een map wordt gedeeld met een gebruiker van [!DNL Workfront Proof], krijgen ze automatisch alleen-lezen rechten voor alle bestaande en vervolgens toegevoegde items in de map.

Zie voor meer informatie [Mappen delen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

### Revisor {#reviewer}

![schoner.png](assets/cleaner.png) Kan een proefdruk weergeven

![schoner.png](assets/cleaner.png) Kan markeringen toevoegen

![schoner.png](assets/cleaner.png) Kan opmerkingen toevoegen

![[!DNL cleaner].png](assets/cleaner.png) Kan eigen opmerkingen bewerken als er geen reacties zijn

![no.png](assets/no.png) Kan geen beslissing nemen

![no.png](assets/no.png) Kan opmerkingen van anderen niet bewerken of verwijderen

![no.png](assets/no.png) Heeft geen bewerkingsrechten op de proefdruk

### Fiatteur {#approver}

![schoner.png](assets/cleaner.png) Kan een proefdruk weergeven

![schoner.png](assets/cleaner.png) Kan een beslissing nemen

![no.png](assets/no.png) Kan geen markeringen toevoegen

![no.png](assets/no.png) Kan geen opmerkingen toevoegen

![no.png](assets/no.png) Kan opmerkingen van anderen niet bewerken of verwijderen

![no.png](assets/no.png) Heeft geen bewerkingsrechten op de proefdruk

### Revisor en fiatteur {#reviewer-approver}

![schoner.png](assets/cleaner.png) Kan een proefdruk weergeven

![schoner.png](assets/cleaner.png) Kan markeringen toevoegen

![schoner.png](assets/cleaner.png) Kan opmerkingen toevoegen

![[!DNL cleaner].png](assets/cleaner.png) Kan eigen opmerkingen bewerken als er geen reacties zijn

![schoner.png](assets/cleaner.png) Kan een beslissing nemen

![no.png](assets/no.png) Kan opmerkingen van anderen niet bewerken of verwijderen

![no.png](assets/no.png) Heeft geen bewerkingsrechten op de proefdruk

### Auteur {#author}

![schoner.png](assets/cleaner.png) Kan markeringen toevoegen

![schoner.png](assets/cleaner.png) Kan opmerkingen toevoegen

![[!DNL cleaner].png](assets/cleaner.png) Kan eigen opmerkingen bewerken als er geen reacties zijn

![schoner.png](assets/cleaner.png) Kan een beslissing nemen

![schoner.png](assets/cleaner.png) Kan nieuwe versies verzenden

![schoner.png](assets/cleaner.png) Kan een kopie van de proefdruk maken

![schoner.png](assets/cleaner.png) Kan de proefdruk delen met anderen

![schoner.png](assets/cleaner.png) Kan handelingen toepassen op opmerkingen

![schoner.png](assets/cleaner.png) Kan opmerkingen oplossen

![no.png](assets/no.png) Kan opmerkingen van anderen niet bewerken of verwijderen

>[!NOTE]
>
>Deze rol kan alleen worden toegewezen aan gebruikers van [!DNL Workfront Proof]

### Moderator {#moderator}

![schoner.png](assets/cleaner.png) Kan markeringen toevoegen

![schoner.png](assets/cleaner.png) Kan opmerkingen toevoegen

![[!DNL cleaner].png](assets/cleaner.png) Kan eigen opmerkingen bewerken als er geen reacties zijn

![schoner.png](assets/cleaner.png) Kan een beslissing nemen

![schoner.png](assets/cleaner.png) Kan nieuwe versies verzenden

![schoner.png](assets/cleaner.png) Kan nieuwe revisoren toevoegen

![schoner.png](assets/cleaner.png) Kan handelingen toepassen op opmerkingen

![schoner.png](assets/cleaner.png) Kan opmerkingen oplossen

![schoner.png](assets/cleaner.png) Kan opmerkingen en antwoorden op de proefdruk (gemaakt door henzelf of anderen) verwijderen

* Als u de eerste opmerking in een opmerkingsthread verwijdert, wordt de hele thread verwijderd.
* Als u reacties in de commentaarthread verwijdert, wordt alleen dat antwoord verwijderd.

![no.png](assets/no.png) Kan opmerkingen van anderen niet bewerken

Deze rol stelt de persoon in staat de bewijsopmerkingen te beheren en te matigen, zodat hij alleen relevante opmerkingen over het bewijs kan bewaren en niet-relevante opmerkingen kan verwijderen.

>[!NOTE]
>
>Deze rol kan alleen worden toegewezen aan gebruikers van [!DNL Workfront Proof].

## Proefdrukrollen toewijzen

U kunt proefdrukrollen toewijzen bij het maken van nieuwe proefdrukken, het maken van nieuwe versies van bestaande proefdrukken of op bestaande proefdrukken.

* [Nieuwe proefdrukken](#new-proofs)
* [Nieuwe versies](#new-versions)
* [Bestaande proefdrukken](#existing-proofs)

### Nieuwe proefdrukken {#new-proofs}

Proefdrukrollen kunnen worden toegewezen aan revisoren op de [!UICONTROL New proof] pagina tijdens het maken van proefdrukken (1).

![Proef_rollen_-_New_Proof_page.png](assets/proof-roles---new-proof-page-350x184.png)

### Nieuwe versies {#new-versions}

Als u een nieuwe versie van een proefdruk maakt, worden de controleurs van de vorige versie automatisch weergegeven (met dezelfde rol als de vorige versie).

U kunt de proefdrukrollen die zijn toegepast op controleurs bewerken bij het maken van de nieuwe versie (1).

![Proef_rollen_-_New_Version_page.png](assets/proof-roles---new-version-page-350x164.png)

### Bestaande proefdrukken {#existing-proofs}

Als u de rol van een persoon op een bestaande proefdruk wilt wijzigen, kunt u dat doen op de knop [!UICONTROL Proof details] pagina door inlinebewerking van hun rol in de werkstroomsectie (1):

![Proef_Roles_-_Proof_Details_page_2.png](assets/proof-roles---proof-details-page-2-350x131.png)

## Rollen controleren in de Proefweergave

U kunt de rol van een revisor rechtstreeks vanuit de Proefweergave (1) controleren en deze (2) bewerken.

![Proef_rollen_-_Proof_Viewer.png](assets/proof-roles---proof-viewer-350x300.png)

## Standaardproefdrukrollen

U kunt de standaardproefdrukrol instellen op de knop [!DNL Proofing Defaults] in uw persoonlijke instellingen. Dit betekent dat wanneer u aan een proef wordt toegevoegd, uw standaardproefdrukrol automatisch zal worden bevolkt. Deze rol kan op proefdrukniveau worden gewijzigd door een gebruiker met bewerkingsrechten op een proefdrukbewijs.

>[!NOTE]
>
>Alleen gebruikers met beheerdersprofielen of factureringsprofielen kunnen de standaardwaarden voor proefdrukken wijzigen voor andere gebruikers in hun account.

Zie voor meer informatie [Persoonlijke instellingen in [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/personal-settings.md).

## Maker en eigenaar

Maker en eigenaar hebben volledige bewerkingsrechten op de proefdruk.

* [Maker](#creators)
* [Eigenaars](#owners)

### Maker {#creators}

De maker van het bewijs is de persoon die het bewijs in eerste instantie uploadt. De maker van de proefdruk wordt automatisch weergegeven in de lijst met personen voor de proefdruk (in de standaardrol).

Op de [!UICONTROL New proof] op de pagina kunt u een andere proefdrukrol toewijzen aan de maker van de proefdruk (anders dan de standaardrol).

De maker van de proefdruk kan niet worden gewijzigd of uit een proefdruk worden verwijderd.

### Eigenaars {#owners}

Standaard is de maker ook de eigenaar van het bewijs; de maker kan echter iemand anders de eigenaar van de proef maken bij het maken van de proef (op de [!UICONTROL New proof] pagina).

De eigenaar wijzigen op de pagina Nieuwe proefdruk:

1. Klik op de wijzigingskoppeling die naast de naam van de maker wordt weergegeven.
1. Selecteer de nieuwe eigenaar in het keuzemenu. (2)

![Proef_rollen_-_new_proof_page_change_owner_2.png](assets/proof-roles---new-proof-page-change-owner-2-350x185.png)

Zodra het bewijs is gecreeerd, is het nog mogelijk om de eigenaar te veranderen. Iedereen met bewerkingsrechten op de proefdruk kan de proefdrukeigenaar via de [!UICONTROL Proof details] pagina (zie hieronder).

De mogelijkheid om de eigenaar van een proefdruk te wijzigen is vooral handig vanuit het oogpunt van workflowbeheer. Hierdoor kan de persoon die verantwoordelijk is voor het project de eigendom van proefdrukken overnemen, zodat hij bewerkingsrechten krijgt op proefdrukken en deze in de [!UICONTROL My proofs] weergeven.

De eigenaar van het bewijs wijzigen via de [!UICONTROL Proof details] pagina:

* Klik op het menu Handelingen naast de naam van de persoon die u wilt maken.
* Selecteren [!UICONTROL Make owner] in het keuzemenu.
* U kunt ook in de [!UICONTROL Owner] naast de proefdrukafbeelding en kies in het vervolgkeuzemenu de nieuwe eigenaar.

Zodra dit wordt gedaan, zal het woord &quot;Eigenaar&quot;naast de naam van die persoon worden getoond.

>[!NOTE]
>
>Alleen een gebruiker van dezelfde account of een partneraccount kan de eigenaar van een bewijs worden. Een gebruiker in een partnerrekening kan tot eigenaar van een bewijs slechts worden gemaakt wanneer:
>
>* Er is een bestaande partnerverhouding opstelling tussen de rekeningen. Zie voor meer informatie [Partneraccounts in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/partner-accounts/partner-accounts.md).
>* Er zijn geen aangepaste velden op de [!UICONTROL New proof] pagina.
>* De proefdruk is niet toegewezen aan een map.
>* Er zijn geen codes toegepast op de proefdruk.
>




Bewijs tijdelijk delegeren binnen [!DNL Workfront Proof], zie [Aanwijzing van eigenaars van tijdelijke bewijzen in [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).
