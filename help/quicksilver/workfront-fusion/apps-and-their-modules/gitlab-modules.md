---
filename: gitlab-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: GitLab-modules
description: Adobe Workfront Fusion vereist naast een Adobe Workfront-licentie een Adobe Workfront Fusion-licentie.
author: Becky
feature: Workfront Fusion
exl-id: bf6c1d82-7926-4bf9-8424-e658650ee6b1
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '3549'
ht-degree: 0%

---


# [!UICONTROL GitLab] modules

Adobe Workfront Fusion vereist naast een Adobe Workfront-licentie een Adobe Workfront Fusion-licentie.

In een [!DNL Adobe Workfront Fusion] -scenario kunt u workflows automatiseren die [!UICONTROL GitLab] gebruiken en deze koppelen aan meerdere toepassingen en services van derden.

>[!NOTE]
>
>Dit artikel verwacht enige vertrouwdheid met API-documentatie en met [!DNL GitLab] functionaliteit in het algemeen.

Als u instructies bij het creëren van een scenario nodig hebt, zie [ een scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) creëren.

Voor informatie over modules, zie [ Modules in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] of hoger</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het abonnement [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Verbinden [!DNL GitLab] met [!DNL Workfront Fusion] {#connect-gitlab-to-workfront-fusion}

1. Klik in een willekeurige [!DNL Workfront Fusion] [!DNL Gitlab] -module op **[!UICONTROL Add]** naast het verbindingsveld.
1. Configureer de volgende velden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name]</td> 
      <td> <p>Voer een naam in voor de verbinding.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL GitLab] URL]</td> 
      <td>Voer de URL van de instantie [!DNL GitLab] in.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Access Token]</td> 
      <td><p>Voer uw [!UICONTROL Private Token] of [!UICONTROL Personal Access Token] in.</p><p>Voor informatie bij het bepalen van of het creëren van een persoonlijk toegangstoken in [!DNL GitLab], zie "een persoonlijk toegangstoken"in <a href="https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html"> Persoonlijke toegangstokens </a> in de [!DNL GitLab] documentatie creëren.</p></td> 
     </tr> 
    </tbody> 
   </table>


1. Klik op **[!UICONTROL Continue]**.
1. Klik op **[!UICONTROL Authorize]** om de verbinding te maken en terug te keren naar de module.

## [!DNL GitLab] modules en hun velden

Wanneer u [!DNL GitLab] modules configureert, geeft [!DNL Workfront Fusion] de onderstaande velden weer. Daarnaast kunnen aanvullende [!DNL GitLab] -velden worden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Voor meer informatie, zie [ informatie van de Kaart van één module aan een andere in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

+++**[!UICONTROL Watch build status]**

Deze onmiddellijke trekkermodule begint een scenario wanneer de status van een bouwstijl verandert.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecteer de webhaak die u voor deze trigger wilt gebruiken of voeg een nieuwe webhaak toe. </p><p>Een nieuwe webhaak toevoegen <ol><li>Klik op <b>[!UICONTROL Add]</b> naast het veld [!UICONTROL webhook] .</li><li>Voer het volgende in: <ul><li>Een naam voor de webhaak</li><li>De verbinding die u voor deze webhaak wilt gebruiken</li><li>Het project dat u wilt dat de webhaak controleert op statuswijzigingen van de build</li></ul></li><li>Klik op <b>[!UICONTROL Save]</b> om de webhaak op te slaan en terug te keren naar de module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch commit/MR/issue/snippet comments]**

Deze onmiddellijke trekkermodule begint een scenario wanneer een commentaar op begaat, fusieverzoek, kwestie, of codefragment wordt gemaakt.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecteer de webhaak die u voor deze trigger wilt gebruiken of voeg een nieuwe webhaak toe. </p><p>Een nieuwe webhaak toevoegen <ol><li>Klik op <b>[!UICONTROL Add]</b> naast het veld [!UICONTROL webhook] .</li><li>Voer het volgende in: <ul><li>Een naam voor de webhaak</li><li>De verbinding die u voor deze webhaak wilt gebruiken</li><li>Het project waarop u de webhaak wilt letten voor opmerkingen</li></ul></li><li>Klik op <b>[!UICONTROL Save]</b> om de webhaak op te slaan en terug te keren naar de module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch commits (pushes)]**

Deze onmiddellijke trekkermodule begint een scenario wanneer wordt geduwd op begaat aan een bewaarplaats. Deze module start geen scenario wanneer een tag wordt ingedrukt.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecteer de webhaak die u voor deze trigger wilt gebruiken of voeg een nieuwe webhaak toe. </p><p>Een nieuwe webhaak toevoegen <ol><li>Klik op <b>[!UICONTROL Add]</b> naast het veld [!UICONTROL webhook] .</li><li>Voer het volgende in: <ul><li>Een naam voor de webhaak</li><li>De verbinding die u voor deze webhaak wilt gebruiken</li><li>Het project waarvan u wilt dat de webhaak op toewijding let</li></ul></li><li>Klik op <b>[!UICONTROL Save]</b> om de webhaak op te slaan en terug te keren naar de module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch issue comment]**

Deze instant triggermodule start een scenario wanneer er een opmerking over een probleem wordt gemaakt.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecteer de webhaak die u voor deze trigger wilt gebruiken of voeg een nieuwe webhaak toe. </p><p>Een nieuwe webhaak toevoegen <ol><li>Klik op <b>[!UICONTROL Add]</b> naast het veld [!UICONTROL webhook] .</li><li>Voer het volgende in: <ul><li>Een naam voor de webhaak</li><li>De verbinding die u voor deze webhaak wilt gebruiken</li><li>Het project dat u wilt dat de webhaak controleert op opmerkingen over de uitgave</li></ul></li><li>Klik op <b>[!UICONTROL Save]</b> om de webhaak op te slaan en terug te keren naar de module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch issues]**

Deze [!UICONTROL instant trigger] -module start een scenario wanneer een uitgave wordt gemaakt of wanneer een bestaande uitgave wordt bijgewerkt, gesloten of opnieuw geopend.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecteer de webhaak die u voor deze trigger wilt gebruiken of voeg een nieuwe webhaak toe. </p><p>Een nieuwe webhaak toevoegen <ol><li>Klik op <b>[!UICONTROL Add]</b> naast het veld [!UICONTROL webhook] .</li><li>Voer het volgende in: <ul><li>Een naam voor de webhaak</li><li>De verbinding die u voor deze webhaak wilt gebruiken</li><li>Het project dat u wilt dat de webhaak voor problemen oplet</li></ul></li><li>Klik op <b>[!UICONTROL Save]</b> om de webhaak op te slaan en terug te keren naar de module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch merge requests]**

Deze instant trekkermodule begint een scenario wanneer één van het volgende voorkomt:

* Er wordt een nieuwe aanvraag voor samenvoegen gemaakt
* Een bestaand samenvoegverzoek wordt bijgewerkt, samengevoegd of gesloten
* Vastleggen is toegevoegd in de bronvertakking


<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecteer de webhaak die u voor deze trigger wilt gebruiken of voeg een nieuwe webhaak toe. </p><p>Een nieuwe webhaak toevoegen <ol><li>Klik op <b>[!UICONTROL Add]</b> naast het veld [!UICONTROL webhook] .</li><li>Voer het volgende in: <ul><li>Een naam voor de webhaak</li><li>De verbinding die u voor deze webhaak wilt gebruiken</li><li>Het project dat u wilt dat de webhaak voor fusieverzoeken let</li></ul></li><li>Klik op <b>[!UICONTROL Save]</b> om de webhaak op te slaan en terug te keren naar de module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch merge request comments]**

Deze onmiddellijke trekkermodule begint een scenario wanneer een commentaar op een fusieverzoek wordt gemaakt.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecteer de webhaak die u voor deze trigger wilt gebruiken of voeg een nieuwe webhaak toe. </p><p>Een nieuwe webhaak toevoegen <ol><li>Klik op <b>[!UICONTROL Add]</b> naast het veld [!UICONTROL webhook] .</li><li>Voer het volgende in: <ul><li>Een naam voor de webhaak</li><li>De verbinding die u voor deze webhaak wilt gebruiken</li><li>Het project dat u wilt dat de webhaak voor de commentaren van het fusieverzoek let</li></ul></li><li>Klik op <b>[!UICONTROL Save]</b> om de webhaak op te slaan en terug te keren naar de module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch pipeline status]**

Deze onmiddellijke trekkermodule begint een scenario wanneer de status van een pijpleiding verandert.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecteer de webhaak die u voor deze trigger wilt gebruiken of voeg een nieuwe webhaak toe. </p><p>Een nieuwe webhaak toevoegen <ol><li>Klik op <b>[!UICONTROL Add]</b> naast het veld [!UICONTROL webhook] .</li><li>Voer het volgende in: <ul><li>Een naam voor de webhaak</li><li>De verbinding die u voor deze webhaak wilt gebruiken</li><li>Het project dat u wilt dat webhaak op de veranderingen van de pijpleidingsstatus letten</li></ul></li><li>Klik op <b>[!UICONTROL Save]</b> om de webhaak op te slaan en terug te keren naar de module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch projects]**

Deze geplande trekkermodule begint een scenario wanneer een nieuw project wordt toegevoegd, waarvan de voor authentiek verklaarde gebruiker een lid is.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Voor instructies over het aansluiten van uw [!DNL GitLab] rekening aan [!DNL Workfront] Fusion, zie <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref"> [!DNL GitLab] verbinden met [!DNL Workfront] Fusion </a> in dit artikel.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Max. resultaten</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt letten.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch repository branches]**

Deze geplande triggermodule start een scenario wanneer een nieuwe vertakking wordt toegevoegd aan een opslagplaats.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Voor instructies over het aansluiten van uw [!DNL GitLab] rekening aan [!DNL Workfront] Fusion, zie <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref"> [!DNL GitLab] verbinden met [!DNL Workfront] Fusion </a> in dit artikel.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Max. resultaten</td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt letten.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch repository tags]**

Deze instant trigger-module start een scenario wanneer een tag wordt gemaakt of verwijderd in een repository.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecteer de webhaak die u voor deze trigger wilt gebruiken of voeg een nieuwe webhaak toe. </p><p>Een nieuwe webhaak toevoegen <ol><li>Klik op <b>[!UICONTROL Add]</b> naast het veld [!UICONTROL webhook] .</li><li>Voer het volgende in: <ul><li>Een naam voor de webhaak</li><li>De verbinding die u voor deze webhaak wilt gebruiken</li><li>Het project dat u wilt dat de webhaak controleert op tags</li></ul></li><li>Klik op <b>[!UICONTROL Save]</b> om de webhaak op te slaan en terug te keren naar de module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch snippet comments]**

Deze instant trigger-module start een scenario wanneer er een nieuwe opmerking wordt gemaakt over een fragment.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecteer de webhaak die u voor deze trigger wilt gebruiken of voeg een nieuwe webhaak toe. </p><p>Een nieuwe webhaak toevoegen <ol><li>Klik op <b>[!UICONTROL Add]</b> naast het veld [!UICONTROL webhook] .</li><li>Voer het volgende in: <ul><li>Een naam voor de webhaak</li><li>De verbinding die u voor deze webhaak wilt gebruiken</li><li>Het project waarop u de webhaak wilt letten voor opmerkingen</li></ul></li><li>Klik op <b>[!UICONTROL Save]</b> om de webhaak op te slaan en terug te keren naar de module. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Watch todos]**

Deze geplande trekkermodule begint een scenario wanneer nieuw wordt toegevoegd. Wanneer geen filter wordt toegepast, wordt de trigger uitgevoerd wanneer een nieuw in behandeling zijnde taak wordt toegevoegd.

Voor informatie over gebieden, zie [ een lijst krijgen van te doen ](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL Watch wiki page]**

Deze onmiddellijke trekkermodule begint een scenario wanneer een wikipagina wordt gecreeerd of uitgegeven.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Selecteer de webhaak die u voor deze trigger wilt gebruiken of voeg een nieuwe webhaak toe. </p><p>Een nieuwe webhaak toevoegen <ol><li>Klik op <b>[!UICONTROL Add]</b> naast het veld [!UICONTROL webhook] .</li><li>Voer het volgende in: <ul><li>Een naam voor de webhaak</li><li>De verbinding die u voor deze webhaak wilt gebruiken</li><li>Het project dat u wilt dat de webhaak op wikiepagina's letten</li></ul></li><li>Klik op <b>[!UICONTROL Save]</b> om de webhaak op te slaan en terug te keren naar de module. </td> 
   </tr> 
   </tbody> 
</table>

+++

### Handelingen

+++**[!UICONTROL Accept merge request]**

Deze actiemodule voegt ingediende wijzigingen samen met het opgegeven samenvoegverzoek.

Voor informatie over gebieden, zie [ samenvoegverzoek ](https://docs.gitlab.com/ee/api/merge_requests.html#accept-mr) in de [!DNL GitLab] documentatie goedkeuren.

+++

+++**[!UICONTROL Cancel a build]**

Deze actiemodule annuleert één enkele bouwstijl van een project.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Voor instructies over het aansluiten van uw [!DNL GitLab] rekening aan [!DNL Workfront] Fusion, zie <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref"> [!DNL GitLab] verbinden met [!DNL Workfront] Fusion </a> in dit artikel.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p>Selecteer of wijs het project toe dat de bouwstijl bevat u wilt annuleren.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Build ID]</td> 
   <td>Selecteer of wijs de bouwstijl toe die u wilt annuleren.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Merge commit message]</td> 
   <td> Voer een bericht voor het samenvoegen in of wijs dit toe.
    </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Should remove source branch]</td> 
   <td>Selecteer of u de bronvertakking wilt verwijderen wanneer de samenvoeging is voltooid.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Merge when build succeeds]</td> 
   <td>Selecteer of de aanvraag voor het samenvoegen moet worden samengevoegd zodra de build is voltooid.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL SHA]</td> 
   <td>Indien aanwezig, dan moet dit SHA de HEAD van de brontak aanpassen. Als deze niet overeenkomt, mislukt het samenvoegen.</td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Cancel a pipeline's builds]**

Deze actiemodule annuleert de bouwstijlen voor één enkele pijpleiding.

Voor informatie over gebieden, zie [ de banen van een pijpleiding ](https://docs.gitlab.com/ee/api/pipelines.html#cancel-a-pipelines-jobs) in de [!DNL GitLab] documentatie annuleren.

+++

+++**[!UICONTROL Cancel merge when pipeline succeeds]**

Als een fusieverzoek wordt geplaatst om samen te voegen wanneer een pijpleiding slaagt, annuleert deze actiemodule die actie.

Voor informatie over gebieden, zie [ samenvoegen annuleren wanneer de pijpleiding ](https://docs.gitlab.com/ee/api/merge_requests.html) in de [!DNL GitLab] documentatie slaagt.

+++

+++**[!UICONTROL Cherry pick a commit]**

Deze actiemodule zoekt naar betrokkenheid bij een bepaalde vertakking.

Voor informatie over gebieden, zie [ Kers plukken a zich ](https://docs.gitlab.com/ee/api/commits.html#cherry-pick-a-commit) in de [!DNL GitLab] documentatie begaan.

+++

+++**[!UICONTROL Create a new label]**

Deze actiemodule leidt tot een nieuw etiket voor de bepaalde bewaarplaats.

Voor informatie over gebieden, zie [ een nieuw etiket ](https://docs.gitlab.com/ee/api/labels.html#create-a-new-label) in de [!DNL GitLab] documentatie creëren.

+++

+++**[!UICONTROL Create a new pipeline]**

Deze actiemodule leidt tot een nieuwe pijpleiding voor het bepaalde project.

Voor informatie over gebieden, zie [ een nieuwe pijpleiding ](https://docs.gitlab.com/ee/api/pipelines.html#create-a-new-pipeline) in de [!DNL GitLab] documentatie creëren.

+++

+++**[!UICONTROL Create a new release]**

Met deze actiemodule voegt u releaseopmerkingen toe aan de bestaande it-tag.

Voor informatie over gebieden, zie [ een versie ](https://docs.gitlab.com/ee/api/releases/#create-a-release) in de [!DNL GitLab] documentatie creëren.

+++

+++**[!UICONTROL Create a new tag]**

Deze actiemodule maakt een nieuwe tag in de opslagplaats die naar de opgegeven ref verwijst.

Voor informatie over gebieden, zie [ een nieuwe markering ](https://docs.gitlab.com/ee/api/tags.html#create-a-new-tag) in de [!DNL GitLab] documentatie creëren.

+++

+++**[!UICONTROL Create a todo]**

Deze actiemodule maakt een taak voor de huidige gebruiker met betrekking tot de geselecteerde uitgave. De huidige gebruiker is de gebruiker die door de geloofsbrieven op de verbinding wordt geïdentificeerd die voor deze module wordt gebruikt.

Voor informatie over gebieden, zie [ a creëren om ](https://docs.gitlab.com/ee/api/issues.html#create-a-todo) in de [!DNL GitLab] documentatie te doen.

+++

+++**[!UICONTROL Create a todo on a merge request]**

Deze actiemodule leidt tot een taak voor de huidige gebruiker op het geselecteerde fusieverzoek. De huidige gebruiker is de gebruiker die door de geloofsbrieven op de verbinding wordt geïdentificeerd die voor deze module wordt gebruikt.

Voor informatie over gebieden, zie [ a tot stand brengen ](https://docs.gitlab.com/ee/api/merge_requests.html#create-a-todo) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL Create merge request]**

Deze actiemodule leidt tot een nieuw fusieverzoek op een project.

Voor informatie over gebieden, zie [ Samenvoegingsverzoek ](https://docs.gitlab.com/ee/api/merge_requests.html#create-mr) in de [!DNL GitLab] documentatie creëren.

+++

+++**[!UICONTROL Create new file in repository]**

Deze actiemodule maakt een nieuw bestand in de geselecteerde opslagplaats.

Voor informatie over gebieden, zie [ nieuw dossier in bewaarplaats ](https://docs.gitlab.com/ee/api/repository_files.html#create-new-file-in-repository) in de [!DNL GitLab] documentatie creëren.

+++

+++**[!UICONTROL Create new issue note]**

Deze actiemodule leidt tot een probleemnota voor één enkele projectkwestie.

Voor informatie over gebieden, zie [ nieuwe uitgevende nota ](https://docs.gitlab.com/ee/api/notes.html#create-new-issue-note) in de [!DNL GitLab] documentatie creëren.

+++

+++**[!UICONTROL Create new merge request note]**

Deze actiemodule leidt nota voor één enkel fusieverzoek.

Voor informatie over gebieden, zie [ nieuwe nota van het fusieverzoek ](https://docs.gitlab.com/ee/api/notes.html#create-new-merge-request-note) in de [!DNL GitLab] documentatie creëren.

+++

+++**[!UICONTROL Create a new milestone]**

Deze actiemodule leidt tot een nieuwe mijlpaal voor een project.

Voor informatie over gebieden, zie [ nieuwe mijlpaal ](https://docs.gitlab.com/ee/api/milestones.html#create-new-milestone) in de [!DNL GitLab] documentatie creëren.

+++

+++**[!UICONTROL Create new snippet note]**

Deze actiemodule maakt een nieuwe notitie voor één fragment. Fragmentnotities zijn opmerkingen die gebruikers naar een fragment kunnen posten.

Voor informatie over gebieden, zie [ nieuwe fragmentnota ](https://docs.gitlab.com/ee/api/notes.html#create-new-snippet-note) in de [!DNL GitLab] documentatie creëren.

+++

+++**[!UICONTROL Create repository branch]**

Deze actiemodule leidt tot één enkele bewaarplaats tak.

Voor informatie over gebieden, zie [ tot de vertakking van de bewaarplaats ](https://docs.gitlab.com/ee/api/branches.html#create-repository-branch) in de [!DNL GitLab] documentatie leiden.

+++

+++**[!UICONTROL Create build variable]**

Deze actiemodule leidt tot een nieuwe bouwstijlvariabele.

Voor informatie over gebieden, zie [ veranderlijke ](https://docs.gitlab.com/ee/api/project_level_variables.html#create-variable) tot stand brengen in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL Delete a merge request]**

Deze actiemodule is alleen voor beheerders en projecteigenaars. Het verwijdert het fusieverzoek in kwestie

Voor informatie over gebieden, zie [ een fusieverzoek ](https://docs.gitlab.com/ee/api/merge_requests.html#delete-a-merge-request) in de [!DNL GitLab] documentatie schrappen.

+++

+++**[!UICONTROL Delete existing file in repository]**

Deze actiemodule verwijdert een bestaand bestand uit de opslagplaats.

Voor informatie over gebieden, zie [ Bestaande dossier in bewaarplaats ](https://docs.gitlab.com/ee/api/repository_files.html#delete-existing-file-in-repository) in de [!DNL GitLab] documentatie schrappen.

+++

+++**[!UICONTROL Delete repository branch]**

Deze actiemodule verwijdert een vertakking uit de opslagplaats.

Voor informatie over gebieden, zie [ vertakking van de bewaarplaats van de Schrapping ](https://docs.gitlab.com/ee/api/branches.html#delete-repository-branch) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL Edit issue]**

Deze actiemodule werkt een bestaand projectprobleem bij. Deze aanroep wordt ook gebruikt om een probleem als gesloten te markeren.

Voor informatie over gebieden, zie [ uitgeven kwestie ](https://docs.gitlab.com/ee/api/issues.html#edit-issue) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL Edit Milestone]**
Deze actiemodule werkt een bestaande projectmijlpaal bij.

Voor informatie over gebieden, zie [ mijlpaal ](https://docs.gitlab.com/ee/api/milestones.html#edit-milestone) in de [!DNL GitLab] documentatie uitgeven.

+++

+++**[!UICONTROL Erase a build]**

Deze actiemodule wist een bouwstijl van een project (verwijdert baanartefacten en baanlogboek).

Voor informatie over gebieden, zie [ een baan ](https://docs.gitlab.com/ee/api/jobs.html#erase-a-job) in de [!DNL GitLab] documentatie wissen.

+++

+++**[!UICONTROL Get a list of todos]**

Deze onderzoeksmodule wint een lijst van te doen punten terug.

Voor informatie over gebieden, zie [ een lijst krijgen van te doen ](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL Get a single build]**

Deze actiemodule wint één enkele baan van een project terug.

Voor informatie over gebieden, zie [ één enkele baan ](https://docs.gitlab.com/ee/api/jobs.html#get-a-single-job) in de [!DNL GitLab] documentatie krijgen.

+++

+++**[!UICONTROL Get a single repository tag]**

Deze actiemodule haalt een specifieke opslagplaats op die wordt bepaald door de naam ervan.

Voor informatie over gebieden, zie [ één enkele bewaarplaatstag ](https://docs.gitlab.com/ee/api/tags.html#get-a-single-repository-tag) in de [!DNL GitLab] documentatie krijgen.

+++

+++**[!UICONTROL Get a specific deployment]**

Deze actiemodule wint een specifieke plaatsing terug.

Voor informatie over gebieden, zie [ een specifieke plaatsing ](https://docs.gitlab.com/ee/api/deployments.html#get-a-specific-deployment) in de [!DNL GitLab] documentatie krijgen.

+++

+++**[!UICONTROL Get all issues assigned to a single milestone]**

Deze onderzoeksmodule wint alle kwesties terug die aan één enkele projectmijlpaal worden toegewezen.

Voor informatie over gebieden, zie [ alle kwesties krijgen die aan één enkele mijlpaal ](https://docs.gitlab.com/ee/api/milestones.html#get-all-issues-assigned-to-a-single-milestone) in de [!DNL GitLab] documentatie worden toegewezen.

+++

+++**[!UICONTROL Get file from repository]**

Deze actiemodule haalt informatie op over een bestand in de repository, zoals naam, grootte of inhoud.

Voor informatie over gebieden, zie [ krijgen dossier van bewaarplaats ](https://docs.gitlab.com/ee/api/repository_files.html#get-file-from-repository) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL Get project users]**

Deze onderzoeksmodule wint de gebruikers van het project terug.

Voor informatie over gebieden, zie [ projectgebruikers ](https://docs.gitlab.com/ee/api/projects.html#get-project-users) in de [!DNL GitLab] documentatie krijgen.

+++

+++**[!UICONTROL Get a single issue]**

Deze actiemodule wint probleemdetails op.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Om een nieuwe verbinding tot stand te brengen, zie <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] aan Workfront Fusion] </a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td> <p>Selecteer het project dat de kwestie bevat u details over wilt terugwinnen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Issue ID]</td> 
   <td> <p>Ga of kaart de naam van de kwestie in u details over wilt terugwinnen.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Get single issue note]**

Deze actiemodule wint één enkele nota voor een specifieke projectkwestie terug.

Voor informatie over gebieden, zie [ één enkele puntennota ](https://docs.gitlab.com/ee/api/notes.html#get-single-issue-note) in de [!DNL GitLab] documentatie krijgen.

+++

+++**[!UICONTROL Get single merge request]**

Deze actiemodule wint informatie over één enkel fusieverzoek terug.

Voor informatie over gebieden, zie [ één enkel fusieverzoek ](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr) in de [!DNL GitLab] documentatie krijgen.

+++

+++**[!UICONTROL Get single merge request changes]**

Deze zoekmodule haalt informatie op over de samenvoegaanvraag, inclusief de bestanden en wijzigingen.

Voor informatie over gebieden, zie [ krijgt enige veranderingen van het fusieverzoek ](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-changes) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL Get single merge request commits]**

Deze actiemodule wint een lijst van de gehechtheid van het fusieverzoek terug.

Voor informatie over gebieden, zie [ krijgt enige fusieverzoek begaat ](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-commits) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL Get single merge request note]**

Deze actiemodule keert één enkele nota voor een bepaald fusieverzoek terug.

Voor informatie over gebieden, zie [ één enkele nota van het fusieverzoek ](https://docs.gitlab.com/ee/api/notes.html#get-single-merge-request-note) in de [!DNL GitLab] documentatie krijgen.

+++

+++**[!UICONTROL Get a Milestone]**

Deze actiemodule wint mijlpaal details terug.

Voor informatie over gebieden, zie [ enige mijlpaal ](https://docs.gitlab.com/ee/api/milestones.html#get-single-milestone) in de [!DNL GitLab] documentatie krijgen.

+++

+++**[!UICONTROL Get single project]**

Deze actiemodule wint projectdetails terug.

Voor informatie over gebieden, zie [ één enkel project ](https://docs.gitlab.com/ee/api/projects.html#get-single-project) in de [!DNL GitLab] documentatie krijgen.

+++

+++**[!UICONTROL Get single repository branch]**

Deze actiemodule haalt de gegevens van de opslagplaats op.

Voor informatie over gebieden, zie [ enige bewaarplaats vertakking ](https://docs.gitlab.com/ee/api/branches.html#get-single-repository-branch) in de [!DNL GitLab] documentatie krijgen.

+++

+++**[!UICONTROL Get snippet note]**

Deze module wint één enkele nota voor een bepaald fragment terug.

Voor informatie over gebieden, zie [ één enkele fragmentnota ](https://docs.gitlab.com/ee/api/notes.html#get-single-snippet-note) in de [!DNL GitLab] documentatie krijgen.

+++

+++**[!UICONTROL Get the comments of a commit]**

Deze onderzoeksmodule wint commentaren van terug van begaat in een project.

Voor informatie over gebieden, zie [ de commentaren van begaat ](https://docs.gitlab.com/ee/api/commits.html#get-the-comments-of-a-commit) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL Get the diff of a commit]**

Deze actiemodule krijgt diff van begaat in een project.

Voor informatie over gebieden, zie [ diff van krijgen ](https://docs.gitlab.com/ee/api/commits.html#get-the-diff-of-a-commit) in de [!DNL GitLab] documentatie begaan.

+++

+++**[!UICONTROL Keep artifacts]**

Voorkomt dat artefacten worden verwijderd wanneer de vervaldatum wordt ingesteld.

Voor informatie over gebieden, zie [ artefacten ](https://docs.gitlab.com/ee/api/job_artifacts.html#keep-artifacts) in de [!DNL GitLab] documentatie houden.

+++

+++**[!UICONTROL List all merge request notes]**

Deze zoekmodule haalt een lijst op met alle notities voor één samenvoegaanvraag.

Voor informatie over gebieden, zie [ van de Lijst alle nota&#39;s van het fusieverzoek ](https://docs.gitlab.com/ee/api/notes.html#list-all-merge-request-notes) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL List all snippet notes]**

Deze module krijgt een lijst van alle nota&#39;s voor één enkel fragment. Fragmentnotities zijn opmerkingen die gebruikers naar een fragment kunnen posten.

Zie [? ](https://docs.gitlab.com/ee/api/notes.html#list-all-snippet-notes) in de [!DNL GitLab] documentatie voor informatie over velden.

+++

+++**[!UICONTROL List commit builds]**

Deze onderzoeksmodule keert een lijst van bouwstijlen voor specifiek terug begaat in een project.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Om een nieuwe verbinding tot stand te brengen, zie <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] aan Workfront Fusion] </a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p>Selecteer het project dat het begaat bevat dat u wilt een lijst maken bouwt voor.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scope]</td> 
   <td> Als u de zoekopdracht wilt beperken tot het samenstellen met een specifieke status, selecteert u de status. Als u dit veld leeg laat, worden alle builds van de commit geretourneerd.  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL List issues]**

Deze zoekmodule retourneert alle uitgaven volgens de opgegeven filterinstellingen.

Voor informatie over gebieden, zie [ kwesties van de Lijst ](https://docs.gitlab.com/ee/api/issues.html#list-issues) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL List Issues That Close on Merge]**

Deze zoekmodule haalt alle problemen op die zouden worden gesloten door de opgegeven samenvoegaanvraag samen te voegen.

Voor informatie over gebieden, zie [ de kwesties van de Lijst die op fusie ](https://docs.gitlab.com/ee/api/merge_requests.html#list-issues-that-will-close-on-merge) in de [!DNL GitLab] documentatie zullen sluiten.

+++

+++**[!UICONTROL List Labels]**

Deze onderzoeksmodule wint alle etiketten in het project terug.

Voor informatie over gebieden, zie [ de etiketten van de Lijst ](https://docs.gitlab.com/ee/api/labels.html#list-labels) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL List merge requests]**

Deze zoekmodule haalt alle samenvoegverzoeken op basis van de filterinstellingen op.

Voor informatie over gebieden, zie [ de fusieverzoeken van de Lijst ](https://docs.gitlab.com/ee/api/merge_requests.html#list-merge-requests) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL List Owned Projects]**

Deze onderzoeksmodule wint projecten terug waar de voor authentiek verklaarde gebruiker als eigenaar wordt geplaatst.

Voor informatie over gebieden, zie [ gebruikersprojecten van de Lijst ](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL List project builds]**

Deze onderzoeksmodule wint een lijst van bouwstijlen in een project terug.

Voor informatie over gebieden, zie [ het projectbanen van de Lijst ](https://docs.gitlab.com/ee/api/jobs.html#list-project-jobs) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL List project deployments]**

Deze onderzoeksmodule wint een lijst van plaatsingen in een project terug.

Voor informatie over gebieden, zie [ het projectplaatsingen van de Lijst ](https://docs.gitlab.com/ee/api/deployments.html#list-project-deployments) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL List project issue notes]**

Deze zoekmodule haalt een lijst op met alle notities voor één enkele uitgave.

Voor informatie over gebieden, zie [ de nota&#39;s van de projectkwestie van de Lijst ](https://docs.gitlab.com/ee/api/notes.html#list-project-issue-notes) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL List project issues]**

Deze onderzoeksmodule keert alle kwesties in een gespecificeerd project terug.

Voor informatie over gebieden, zie [ de projectkwesties van de Lijst ](https://docs.gitlab.com/ee/api/issues.html#list-project-issues) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL List project milestones]**

Deze onderzoeksmodule wint alle mijlpalen in het project terug.

Voor informatie over gebieden, zie [ het projectmijlpalen van de Lijst ](https://docs.gitlab.com/ee/api/milestones.html#list-project-milestones) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL List project pipelines]**

Deze onderzoeksmodule wint alle pijpleidingen voor het project terug.

Voor informatie over gebieden, zie [ het projectpijpleidingen van de Lijst ](https://docs.gitlab.com/ee/api/pipelines.html#list-project-pipelines) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL List project repository tags]**

Deze zoekmodule haalt een lijst op met opslagplaatstags uit een project, gesorteerd op naam in omgekeerde alfabetische volgorde.

Voor informatie over gebieden, zie {de markeringen van de het projectbewaarplaats van de 0} Lijst ](https://docs.gitlab.com/ee/api/tags.html#list-project-repository-tags) in de [!DNL GitLab] documentatie.[

+++

+++**[!UICONTROL List project variables]**

Deze onderzoeksmodule wint een lijst van de variabelen van een project terug.

Voor informatie over gebieden, zie [ het projectvariabelen van de Lijst ](https://docs.gitlab.com/ee/api/project_level_variables.html#list-project-variables) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL List projects]**

Deze onderzoeksmodule wint alle projecten terug waarvan de voor authentiek verklaarde gebruiker een lid is.

Voor informatie over gebieden, zie [ een lijst maken van alle projecten ](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL List repository branches]**

Deze module zoekt naar vertakkingen in de opslagplaats op de zoekterm.

Voor informatie over gebieden, zie [ de vertakkingen van de bewaarplaats van de Lijst ](https://docs.gitlab.com/ee/api/branches.html#list-repository-branches) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL List repository commits]**

Deze onderzoeksmodule wint een lijst van bewaarplaatsverplichtingen in een project terug.

Voor informatie over gebieden, zie [ de bewaarplaats van de Lijst begaat ](https://docs.gitlab.com/ee/api/commits.html#list-repository-commits) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL List repository contributors]**

Deze zoekmodule haalt een lijst met contribuanten in de repository op.

Voor informatie over gebieden, zie [ Medewerkers ](https://docs.gitlab.com/ee/api/repositories.html#contributors) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL List repository tree]**

Deze zoekmodule haalt een lijst op met bestanden en mappen in de opslagplaats in een project.

Voor informatie over gebieden, zie [ de opbergboom van de Lijst ](https://docs.gitlab.com/ee/api/repositories.html#list-repository-tree) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL Mark a todo as done]**

Deze handelingsmodule markeert één enkel in afwachting om punt te doen dat door zijn identiteitskaart voor de huidige gebruiker zoals gedaan wordt gegeven.

Voor informatie over gebieden, zie [ Teken a om punt te doen zoals gedaan ](https://docs.gitlab.com/ee/api/todos.html#mark-a-todo-as-done) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL Modify existing issue note]**

Wijzigt een bestaande notitie van een uitgave.

Voor informatie over gebieden, zie [ bestaande voorwaardennota ](https://docs.gitlab.com/ee/api/notes.html#modify-existing-issue-note) in de [!DNL GitLab] documentatie wijzigen.

+++

+++**[!UICONTROL Modify existing merge request note]**

Hiermee wordt de bestaande notitie van een samenvoegaanvraag gewijzigd.

Voor informatie over gebieden, zie [ bestaande nota van het fusieverzoek ](https://docs.gitlab.com/ee/api/notes.html#modify-existing-merge-request-note) in de [!DNL GitLab] documentatie wijzigen.

+++

+++**[!UICONTROL Modify existing snippet note]**

Deze actiemodule wijzigt een bestaande notitie van een fragment.

Voor informatie over gebieden, zie [ bestaande fragmentnota wijzigen ](https://docs.gitlab.com/ee/api/notes.html#modify-existing-snippet-note) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL New issue]**

Deze actiemodule leidt tot een nieuwe projectkwestie.

Voor informatie over gebieden, zie [ Nieuwe kwestie ](https://www.integromat.com/en/help/app/gitlab) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL Play a build]**

Deze actiemodule activeert een handmatige handeling om een taak te starten.

Voor informatie over gebieden, zie [ Spel een baan ](https://docs.gitlab.com/ee/api/jobs.html#play-a-job) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL Post comment to commit]**

Deze actiemodule voegt een opmerking toe aan een commit.

Voor informatie over gebieden, zie [ commentaarpost ](https://docs.gitlab.com/ee/api/commits.html#post-comment-to-commit) in de [!DNL GitLab] documentatie begaan.

+++

+++**[!UICONTROL Remove variable]**

Deze actiemodule verwijdert de variabele van een project.

Voor informatie over gebieden, zie [ veranderlijke ](https://docs.gitlab.com/ee/api/project_level_variables.html#remove-variable) in de [!DNL GitLab] documentatie verwijderen.

+++

+++**[!UICONTROL Retry a build]**

Deze actiemodule probeert één enkele bouwstijl in begaat opnieuw.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Om een nieuwe verbinding tot stand te brengen, zie <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] aan Workfront Fusion] </a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p>Selecteer het project dat de bouwstijl bevat u wilt opnieuw proberen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Build ID]</td> 
   <td> Selecteer de build die u opnieuw wilt proberen. </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Retry Failed Jobs in a Pipeline]**

Deze actiemodule probeert ontbroken bouwt in een pijpleiding opnieuw.

Voor informatie over gebieden, zie [ banen in een pijpleiding ](https://docs.gitlab.com/ee/api/pipelines.html#retry-jobs-in-a-pipeline) in de [!DNL GitLab] documentatie opnieuw proberen.

+++

+++**[!UICONTROL Get a Variable]**

Deze module wint details van de specifieke variabele van een project terug.

Voor informatie over gebieden, zie [ veranderlijke details ](https://docs.gitlab.com/ee/api/project_level_variables.html#show-variable-details) in de [!DNL GitLab] documentatie tonen.

+++

+++**[!UICONTROL Update a release]**

Deze actiemodule werkt een versie bij.

Voor informatie over gebieden, zie [ een versie ](https://docs.gitlab.com/ee/api/releases/#update-a-release) in de [!DNL GitLab] documentatie bijwerken.

+++

+++**[!UICONTROL Update merge request]**

Deze actiemodule werkt een bestaande samenvoegaanvraag bij. U kunt de doelvertakking, de titel veranderen, of zelfs MR sluiten.

Voor informatie over gebieden, zie [ de fusieverzoek van de Update ](https://docs.gitlab.com/ee/api/merge_requests.html#update-mr) in de [!DNL GitLab] documentatie.

+++

+++**[!UICONTROL Update a Variable]**

Deze actiemodule werkt de variabele van een project bij.

Voor informatie over gebieden, zie [ veranderlijke Update ](https://docs.gitlab.com/ee/api/project_level_variables.html#update-variable) in de [!DNL GitLab] documentatie.

+++
