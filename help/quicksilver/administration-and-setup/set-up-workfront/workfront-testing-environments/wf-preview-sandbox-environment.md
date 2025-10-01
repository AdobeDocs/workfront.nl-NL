---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Het  [!DNL Adobe Workfront]  Milieu van de zandbak van de Voorproef
description: De voorvertoningssandbox is een testomgeving die fungeert als replica van uw live omgeving. Het wordt elk weekend vernieuwd door Workfront. Gegevens die op vrijdag aan uw live omgeving zijn toegevoegd, worden op de volgende maandag in de voorvertoningssandbox weergegeven. Alle ondersteuningspakketten hebben toegang tot deze sandbox.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: 8df1889997937b2a4238862eb2f86aeda84ed104
workflow-type: tm+mt
source-wordcount: '1285'
ht-degree: 0%

---

# De [!DNL Adobe Workfront] Sandbox-voorvertoningsomgeving

<!-- Audited: 12/2023 -->

Er zijn twee testomgevingen voor [!DNL Workfront] die replica&#39;s zijn van uw [!DNL Workfront] -productieomgeving:

* De voorvertoningssandbox

  De voorvertoningssandbox is een testomgeving die fungeert als replica van uw live omgeving en die elk weekend wordt vernieuwd door [!DNL Workfront] . Gegevens die op vrijdag aan uw live omgeving zijn toegevoegd, worden op de volgende maandag in de voorvertoningssandbox weergegeven.

  Alle ondersteuningspakketten hebben toegang tot de voorvertoningssandbox.

* De aangepaste vernieuwingssandbox

  De aangepaste vernieuwingssandbox is een aparte testomgeving die u handmatig kunt vernieuwen. Er zijn extra kosten voor het ophalen van de aangepaste vernieuwingssandbox. Voor meer informatie over dit milieu, zie [&#x200B; de  [!DNL Adobe Workfront]  Douane verfrist het milieu van Sandbox &#x200B;](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>[!UICONTROL Standard] Ondersteuningspakket </strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Plus] , [!UICONTROL Preferred] en [!UICONTROL Enterprise] Ondersteuningspakketten </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>Voorvertoning sandbox</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>Aangepaste vernieuwingssandbox</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## Voorvertoning sandbox

De voorvertoningssandbox fungeert als een omgeving waarin gebruikers in uw organisatie veilig gegevens kunnen testen en met gegevens uit de productieomgeving kunnen werken zonder dat dit van invloed is op de productieomgeving.

De voorvertoningssandbox bevat uw werkelijke productiegegevens. Deze worden echter elk weekend vernieuwd, zodat de gegevens maximaal een week achter de productieomgeving kunnen liggen. De punten die sinds laatste worden gecreeerd verfrissen tijd zijn in het milieu van de Sandbox van de Voorproef tot het volgende verfrist zich.

De gegevensstromen uni-directioneel, van Productie aan Voorproef, en niet in omgekeerde. De voorvertoningsomgeving wordt altijd door [!DNL Workfront] elk weekend vernieuwd.

Met de voorvertoningssandbox kunnen in [!DNL Workfront] ook nieuwe functies worden geïmplementeerd in een veilige omgeving voordat deze klaar zijn om te worden geïmplementeerd op Productie. U kunt de nieuwe functies testen en [!DNL Workfront] feedback geven over de functionaliteit ervan door de voorvertoningssandbox te openen. Daarom is de code van de Voorvertoning-sandbox altijd voor de productiecode, hoewel uw gegevens wekelijks worden vernieuwd.

De voorvertoningsomgeving is ideaal voor het uitvoeren van trainingen, het testen van nieuwe functies en het bepalen van de installatiefunctionaliteit.

>[!NOTE]
>
>Wanneer u de zandbak van de Voorproef toegang hebt, zie de blauwe banner bij de bovenkant van het scherm. De banner kan niet worden verwijderd terwijl u in deze omgeving werkt.
>
>De naam van de omgeving die u opent (Voorvertoning) en de releaseversie van de code worden weergegeven op de banner. Klik op **[!UICONTROL See what's new]** voor meer informatie over die release.
>
>![&#x200B; banner van de Voorproef &#x200B;](assets/preview-banner-nwe-350x161.png)

## De voorvertoningssandbox openen

Als [!DNL Workfront] -beheerder hebt u standaard toegang tot de [!UICONTROL Preview] Sandbox-omgeving. Als u geen toegang hebt tot de [!UICONTROL Preview] Sandbox-omgeving zoals beschreven in deze sectie, neemt u contact op met uw [!DNL Workfront] -beheerder of ons Customer Support-team.


### De voorvertoningssandbox openen via de interface van [!DNL Workfront] {#accessing-the-preview-sandbox-from-the-workfront-interface}

Als [!DNL Workfront] beheerder hebt u via de [!DNL Workfront] -interface toegang tot de voorvertoningssandbox.

De voorvertoningssandbox openen:

{{step-1-to-setup}}

1. Klik op **[!UICONTROL System]** > **[!UICONTROL Preferences]** .

1. Klik in de sectie **[!UICONTROL Test Environments]** op **[!UICONTROL Sandbox Preview]** .

1. Meld u aan met uw voorvertoningsreferenties.

   Deze moeten hetzelfde zijn als de gegevens van uw productie, tenzij u deze hebt gewijzigd in Productie nadat de voorvertoning is vernieuwd. De logins worden alleen gesynchroniseerd wanneer het vernieuwen plaatsvindt. Ze worden niet automatisch gesynchroniseerd.

### De voorvertoningssandbox openen met een URL {#accessing-the-preview-sandbox-using-a-url}

Via een URL hebt u toegang tot de voorvertoningssandbox.

#### Toegang tot de voorvertoningssandbox voor accounts in cluster 1,2,3 en 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

De URL voor de voorvertoningssandbox is: `https://companyname.preview.workfront.com/` .

>[!NOTE]
>
>Als er bladwijzers zijn gekoppeld aan de oude URL voor de voorvertoningssandbox, moet u deze wijziging noteren en de URL in uw bladwijzers bijwerken.

U kunt als volgt via een URL aanmelden bij de voorvertoningssandbox:

1. Navigeer naar deze URL: `https://companyname.preview.workfront.com/` .

   Als u een EMEA-klant bent en uw account zich op Cluster 4 bevindt, raadpleegt u de sectie Toegang tot de voorbeeldsandbox voor accounts in cluster 4 (EMEA-accounts) hieronder.

1. Meld u aan met uw voorvertoningsreferenties.

   >[!TIP]
   >
   >De voorvertoningsgegevens moeten hetzelfde zijn als de gegevens voor de productie, tenzij u deze in Productie hebt gewijzigd nadat de voorvertoning is vernieuwd. De logins worden alleen gesynchroniseerd wanneer het vernieuwen plaatsvindt. Ze worden niet automatisch gesynchroniseerd.


#### Toegang tot de voorbeeldsandbox voor accounts in cluster 4 (EMEA-accounts) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

U kunt als volgt via een URL aanmelden bij de voorvertoningssandbox:

1. Navigeer naar deze URL: `https://companyname.preview.workfront.com/` .

   U kunt tot de Sandbox van de Voorproef ook toegang hebben door [&#x200B; https://cl04.preview.workfront.com/login &#x200B;](https://cl04.preview.workfront.com/login) te gaan.

1. Meld u aan met uw voorvertoningsreferenties.

   De voorvertoningsgegevens moeten hetzelfde zijn als de gegevens voor de productie, tenzij u deze in Productie hebt gewijzigd nadat de voorvertoning is vernieuwd. De logins worden alleen gesynchroniseerd wanneer het vernieuwen plaatsvindt. Ze worden niet automatisch gesynchroniseerd.

## E-mails ontvangen vanuit de voorvertoningssandbox

Workfront schakelt alle e-mailcommunicatie uit vanuit de omgeving van de voorvertoningssandbox. Als u e-mailmeldingen wilt ontvangen vanuit de omgeving van de voorvertoningssandbox, moet u deze functionaliteit inschakelen in uw gebruikersinstellingen. Voor meer informatie over het toelaten van e-mailberichten in het milieu van de Sandbox van de Voorproef, zie [&#x200B; levering van e-mails van het milieu van de zandbak van de Voorproef &#x200B;](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md) toelaten.

>[!NOTE]
>
>Leverings- en pushberichten van rapporten op de mobiele app zijn altijd uitgeschakeld voor de voorvertoningssandbox-omgeving. De beheerder van [!DNL Workfront] kan het verzenden van rapporten of pushmeldingen voor de mobiele app niet inschakelen wanneer u de omgeving van de voorvertoningssandbox opent.
>
>Voor meer informatie over rapportleveringen voor het productiemilieu, zie [&#x200B; de leveringsoverzicht van het Rapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## Eenmalige aanmelding (SSO)

Als u SSO gebruikt, werkt u samen met ons klantenondersteuningsteam om ervoor te zorgen dat dit op de juiste wijze is geconfigureerd, zodat u uw SSO-gegevens kunt gebruiken om u aan te melden bij de sandbox van [!UICONTROL Preview] . Neem contact op met uw normale ondersteuningscontactpersoon of [!DNL Workfront] beheerder als uw initiële aanmelding mislukt.

Voor meer informatie over Enige Sign-On, zie [&#x200B; Overzicht van enige sign-on in Adobe Workfront &#x200B;](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Single Sign-On configureren in de voorvertoningssandbox

>[!IMPORTANT]
>
>De op deze pagina beschreven procedure is alleen van toepassing op organisaties die nog niet zijn aangemeld bij de [!DNL Adobe Admin Console] . Als uw organisatie is aangemeld bij de [!DNL Adobe Admin Console] , is geen actie nodig.
>
>Voor een lijst van procedures die verschillen gebaseerd op of uw organisatie aan [!DNL Adobe Admin Console] is genegeerd, zie [&#x200B; Op platform-gebaseerde beleidsverschillen ([!UICONTROL Adobe Workfront]/ [!UICONTROL Adobe Business Platform]) &#x200B;](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


Als u uw zandbak van de Voorproef wilt vormen om met Één Enige Sign-On oplossing te werken, kunt u dit doen door het los van uw milieu van de Productie te vormen. De configuratie SSO in de zandbak van de Voorproef is onafhankelijk van uw configuratie SSO in het milieu van de Productie.

Wanneer uw zandbak van de Voorproef (elk weekend) verfrist, wordt de informatie SSO niet gekopieerd van uw milieu van de Productie om de configuratie van de Sandbox van de Voorproef te beschrijven.

De stappen voor het vormen van enig teken-binnen in de zandbak van de Voorproef zijn gelijkaardig aan die voor het vormen van het in het milieu van de Productie.

Voor meer informatie over het vormen [!DNL Workfront] met SSO, zie [&#x200B; Overzicht van enige teken-op in Adobe Workfront &#x200B;](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Automatische herberekening van projecttijdlijnen

Het opnieuw berekenen van chronologie staat managers toe om te zien hoe de krachten buiten het project de chronologie van het project beïnvloeden. De tijdlijn van een project verwijst naar de geplande en geplande data voor het project.

Als Workfront-beheerder kunt u configureren wanneer Workfront de projecttijdlijnen automatisch opnieuw berekent. Workfront kan projectchronologie of elke nacht opnieuw berekenen of wanneer het projectwerkingsgebied verandert, of allebei.

Voor informatie, zie [&#x200B; chronologieherberekeningen voor projecten &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md) vormen.

Voor de omgeving van de Voorproef, wordt de niight herberekening onbruikbaar gemaakt, en de projectchronologie worden niet automatisch opnieuw berekend. U moet de projectchronologie voor het milieu van de Voorproef manueel opnieuw berekenen. Voor informatie, zie [&#x200B; projectchronologie &#x200B;](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md) opnieuw berekenen.


## Voorbeeld van prestaties en beschikbaarheid van omgeving

* [!DNL Workfront] Voorvertoningsomgevingen zijn niet bedoeld voor het testen van prestaties of belasting. Gebruik in plaats daarvan deze omgevingen om de functionaliteit van functies te valideren met de bestaande workflows van uw organisatie.

* Workflows waarbij documenten betrokken zijn, moeten zich richten op het proces en niet op het testen van het laden. Grote bestanden worden niet ondersteund in Sandbox-omgevingen.

* [!DNL Workfront] Voorvertoningsomgevingen zijn altijd beschikbaar.

* Elke storing in een [!DNL Workfront] -voorvertoningsomgeving tijdens normale kantooruren is een eerste prioriteit onmiddellijk nadat eventuele productieproblemen zijn opgelost.

* Elke storing in een [!DNL Workfront] Voorvertoningsomgeving tijdens weekends (zaterdagen en zondag) wordt opgelost, zodat de omgeving op maandag voor kantooruren wordt uitgevoerd.

* Proofing is niet beschikbaar in voorvertoningsomgevingen.
