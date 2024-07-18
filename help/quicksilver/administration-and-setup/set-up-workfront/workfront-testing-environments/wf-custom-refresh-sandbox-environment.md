---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Het  [!DNL Adobe Workfront]  milieu van de Douane verfrist Sandbox
description: De aangepaste sandbox Vernieuwen is een omgeving waarin u gegevens uit uw productieomgeving kunt testen en gebruiken. Het is ook ideaal voor het uitvoeren van trainingen en het bepalen van instelfunctionaliteit.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1594'
ht-degree: 0%

---

# De [!DNL Adobe Workfront] aangepaste Sandbox-omgeving voor vernieuwen

De aangepaste sandbox Vernieuwen is een omgeving waarin u gegevens uit uw productieomgeving kunt testen en gebruiken. Het is ook ideaal voor het uitvoeren van trainingen en het bepalen van instelfunctionaliteit.

>[!NOTE]
>
>Dit is anders dan de voorvertoningssandbox, die ook een testomgeving is waarin uw [!DNL Workfront] -productieomgeving wordt gerepliceerd.
>
>* Nieuwe functies worden geïntroduceerd in de voorvertoningssandbox voordat deze beschikbaar worden in Productie.
>* Nieuwe functies worden niet geïntroduceerd in de aangepaste sandbox Vernieuwen voordat deze beschikbaar worden in Productie.
>
>  Er zijn ook extra kosten voor het ophalen van de aangepaste vernieuwingssandbox die niet vereist zijn voor de voorvertoningssandbox.
>
>  Voor meer informatie over de zandbak van de Voorproef, zie [ het  [!DNL Adobe Workfront]  Milieu van de Voorproef Sandbox ](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).


## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] plan</td> 
   <td> <p>[!UICONTROL Business] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] licentie</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>U moet een [!DNL Workfront] beheerder zijn. Voor informatie over [!DNL Workfront] beheerders, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> een gebruiker volledige administratieve toegang verlenen </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ondersteuningspakket</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred] of [!UICONTROL Enterprise]</p> <p>Het standaard ondersteuningspakket heeft geen toegang tot de aangepaste sandbox Vernieuwen, maar heeft wel toegang tot de voorvertoningssandbox.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## De aangepaste vernieuwingssandbox vernieuwen

De sandbox Aangepast vernieuwen bevat de werkelijke productiegegevens. Deze worden pas vernieuwd als u dit wilt doen. U kunt vernieuwen op elk gewenst moment plannen, zo vaak als eenmaal per week.

>[!NOTE]
>
>* U kunt niet plannen verfrist zich voor de huidige dag. Als vandaag bijvoorbeeld 1 juni is, is 2 juni de vroegste dag waarop u kunt plannen om te vernieuwen.
>* De geplande vernieuwing vindt ergens in de nacht plaats, op basis van de cluster van de gebruiker (clusters in de VS ververversen &#39;s nachts in de VS). De specifieke tijd is onvoorspelbaar toe te schrijven aan andere klanten in de rij en hoeveel gegevens worden verfrist. Als de rij vele grote klanten heeft, verfrist zich kan niet tot later die dag, of de volgende dag lopen.
>* Uw aangepaste vernieuwingssandbox heeft altijd dezelfde productfuncties als uw productieomgeving. Wanneer u de aangepaste vernieuwingssandbox vernieuwt, blijft de branding echter alleen behouden voor de achtergrondkleur van het aanmeldingsscherm. De standaardwaarden voor het aanmeldingsscherm en de navigatiebalklogo&#39;s zijn ingesteld op [!DNL Workfront] en brandingafbeeldingen die u vóór het vernieuwen hebt gewijzigd, worden niet weergegeven.
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## De aangepaste vernieuwingssandbox openen vanuit de productieomgeving {#access-the-custom-refresh-sandbox-from-your-production-environment}

Als [!DNL Workfront] beheerder kunt u tot uw Douane toegang hebben vernieuwt Sandbox van uw productiemilieu.

>[!NOTE]
>
>Als uw account zich op Cluster 4 (EMEA-cluster) bevindt, hebt u vanuit de productieomgeving geen toegang tot uw aangepaste vernieuwingssandbox. Voor meer informatie over hoe u tot uw Douane kunt toegang hebben verfrist Sandbox wanneer u een rekening op Cluster 4 hebt, zie [ tot de Douane verfrissen Sandbox voor Rekeningen op Cluster 4 (EMEA Rekeningen) ](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [ toegang tot de Douane verfrist Sandbox voor Rekeningen op Cluster 4 (EMEA Rekeningen) ](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

Ga als volgt te werk om uw aangepaste vernieuwingssandbox te openen:

1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in [!DNL Adobe Workfront] en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png) .

1. Klik **[!UICONTROL System]** > **[!UICONTROL Preferences]**.

1. Klik in de sectie **[!UICONTROL Test Environment]** op **[!UICONTROL Sandbox 1]** of **[!UICONTROL Sandbox 2]** .

   Met het ondersteuningspakket geeft u op of u toegang hebt tot een of twee aangepaste vernieuwingssandboxen.

1. Meld u aan met uw aanmeldingsgegevens voor Aangepast vernieuwen in sandbox.

   Uw referenties voor Aangepaste sandbox vernieuwen zijn gelijk aan de gegevens voor uw productie, tenzij u uw productiereferenties hebt gewijzigd sinds u de aangepaste sandbox Vernieuwen voor het laatst hebt vernieuwd. De logins worden alleen gesynchroniseerd wanneer het vernieuwen plaatsvindt. Ze worden niet automatisch gesynchroniseerd.

   In de sandbox Aangepast vernieuwen ziet u zowel de versie als de datum die voor het laatst is vernieuwd in de banner boven aan het scherm. Alle informatie van productie is beschikbaar en klaar om met te werken nadat verfrissen voltooit.

## Via een URL toegang krijgen tot de sandbox Aangepast vernieuwen {#access-the-custom-refresh-sandbox-using-a-url}

Elke gebruiker heeft via een URL toegang tot de sandbox Aangepast vernieuwen.

* [Ga tot de Aangepaste Refresh Sandbox voor rekeningen op Clusters 1, 2, 3, en 5 toegang hebben](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [Toegang tot de Aangepaste vernieuwingssandbox voor accounts in cluster 4 (EMEA-accounts)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### Ga tot de Aangepaste Refresh Sandbox voor rekeningen op Clusters 1, 2, 3, en 5 toegang hebben {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

Afhankelijk van uw ondersteuningspakket hebt u toegang tot een of twee aangepaste vernieuwingssandboxen.

Via een URL toegang krijgen tot uw aangepaste sandbox Vernieuwen:

1. Navigeer naar deze URL als u slechts één aangepaste vernieuwingssandbox hebt:

   https://companyname.sb01.workfront.com (oude URL :https: /cr1.attasksandbox.com/.)

   Of als u twee aangepaste vernieuwingssandboxen hebt, in aanvulling op de bovenstaande URL&#39;s, kunt u ook naar de volgende URL gaan om toegang te krijgen tot uw tweede aangepaste vernieuwingssandbox:

   https://companyname.sb02.workfront.com (oude URL :https: /cr2.attasksandbox.com/)

1. Meld u in het aanmeldingsscherm aan met uw aanmeldingsgegevens voor Aangepast vernieuwen in sandbox.
1. Uw referenties voor Aangepaste sandbox vernieuwen zijn gelijk aan de gegevens voor uw productie, tenzij u uw productiereferenties hebt gewijzigd sinds de aangepaste sandbox voor het vernieuwen van uw product voor het laatst is vernieuwd. De logins worden alleen gesynchroniseerd wanneer het vernieuwen plaatsvindt. Ze worden niet automatisch gesynchroniseerd.

### Toegang tot de Aangepaste vernieuwingssandbox voor accounts in cluster 4 (EMEA-accounts) {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

Als uw [!DNL Workfront] -account zich in Cluster 4 (EMEA-cluster) bevindt, hebt u alleen via een URL toegang tot uw aangepaste sandbox Vernieuwen. Neem contact op met ons Customer Support-team om te weten te komen in welk cluster uw account staat.

Afhankelijk van uw ondersteuningspakket hebt u toegang tot een of twee aangepaste vernieuwingssandboxen.

Via een URL toegang krijgen tot uw aangepaste sandbox Vernieuwen:

1. Navigeer naar deze URL als u slechts één aangepaste vernieuwingssandbox hebt:

   https://companyname.sb01.workfront.com (oude URL :https://cr3.attasksandbox.com)

   of

   Ga naar een van deze URL&#39;s als u twee aangepaste vernieuwingssandboxen hebt:

   https://companyname.sb01.workfront.com (oude URL :https://cr3.attasksandbox.com)

   https://companyname.sb02.workfront.com (oude URL :https://cr4.attasksandbox.com)

1. Meld u in het aanmeldingsscherm aan met uw aanmeldingsgegevens voor Aangepast vernieuwen in sandbox.

   Uw referenties voor Aangepaste sandbox vernieuwen zijn gelijk aan de gegevens voor uw productie, tenzij u uw productiereferenties hebt gewijzigd sinds de aangepaste sandbox voor het vernieuwen van uw product voor het laatst is vernieuwd. De logins worden alleen gesynchroniseerd wanneer het vernieuwen plaatsvindt. Ze worden niet automatisch gesynchroniseerd.

## Plan vernieuwen van uw aangepaste vernieuwingssandbox

>[!IMPORTANT]
>
>De duur van vernieuwen is afhankelijk van de grootte van de gegevens die worden vernieuwd. Tijdens het vernieuwingsproces is het van essentieel belang dat uw aangepaste sandboxomgeving op geen enkele manier wordt gebruikt (inclusief API-aanroepen en -integratie), omdat anders de sandbox niet goed kan worden vernieuwd. [!DNL Workfront] schakelt de aangepaste sandboxomgeving voor vernieuwen uit voordat deze begint, maar u moet alle actieve sessies beëindigen om ervoor te zorgen dat de sandbox vernieuwd wordt.

Nadat u de aangepaste vernieuwingssandbox hebt gepland, kunt u deze annuleren door boven aan de pagina op [!UICONTROL Cancel] te klikken. U kunt de sjabloon ook later opnieuw plannen.

>[!NOTE]
>
>U kunt automatische sandboxvernieuwingen niet plannen.

Om een verfrissing van uw Klant te plannen vernieuwt Sandbox:

1. Meld u aan bij uw aangepaste vernieuwingssandbox.
1. Klik op **[!UICONTROL Schedule]** in de banner boven aan het scherm en selecteer een datum in de kalender.
1. Selecteer een datum waarop u wilt vernieuwen en klik op **[!UICONTROL Schedule Refresh]** .

## Overschakelen naar productie vanuit de aangepaste vernieuwingssandbox

1. Meld u aan bij uw aangepaste vernieuwingssandbox.

   Voor meer informatie over de toegang tot van uw Douane verfrist Sandbox, zie [ Toegang tot Aangepast vernieuwt Sandbox van uw milieu van de Productie ](#access-the-custom-refresh-sandbox-from-your-production-environment) of [ toegang tot Aangepast vernieuwt Sandbox gebruikend URL ](#access-the-custom-refresh-sandbox-using-a-url).

1. Klik op **[!UICONTROL Go To Production]** in de banner boven aan het scherm.

   Vergeet niet dat het werk dat in de sandbox wordt gedaan niet zichtbaar is in de [!UICONTROL production] -omgeving, omdat de gegevensoverdracht eenrichtingsverkeer is, van productie naar de aangepaste vernieuwingssandbox en niet andersom.

## E-mails ontvangen vanuit de Aangepaste sandbox Vernieuwen

[!DNL Workfront] schakelt alle e-mailcommunicatie uit vanuit de aangepaste Sandbox-omgeving voor vernieuwen. Als u e-mailmeldingen wilt ontvangen vanuit de aangepaste Sandbox-omgeving voor vernieuwen, moet u deze functionaliteit inschakelen in uw gebruikersinstellingen. Voor meer informatie over het toelaten van e-mailberichten in de Douane verfrist het milieu van Sandbox, zie [ levering van e-mails van het milieu van de zandbak van de Voorproef ](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md) toelaten.

>[!NOTE]
>
>Leverings- en pushberichten van rapporten op de mobiele app zijn altijd uitgeschakeld voor de aangepaste Sandbox-omgeving voor vernieuwen. U kunt noch de beheerder van [!DNL Workfront] de levering van rapporten of pushmeldingen voor de mobiele app inschakelen wanneer u toegang krijgt tot de aangepaste Sandbox-omgeving voor vernieuwen.\
>Voor meer informatie over rapportleveringen voor het productiemilieu, zie [ het leveringsoverzicht van het Rapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).Voor meer informatie over dupberichten op mobiele app voor het productiemilieu, zie de sectie in.

## Eén aanmelding configureren in de sandbox Aangepast vernieuwen

Als u uw Douane wilt vormen vernieuwt Sandbox om met Één Enige Sign-On oplossing te werken, kunt u dit doen door het los van uw milieu van de Productie te vormen. De configuratie SSO in Aangepast vernieuwt Sandbox is onafhankelijk van uw configuratie SSO in de omgeving van de Productie.\
Wanneer u uw Douane vernieuwt Sandbox, wordt de informatie SSO niet gekopieerd van uw milieu van de Productie om de Douane te overschrijven vernieuwt Sandbox configuratie.

De stappen voor het vormen van enig teken-binnen in de Douane verfrissen Sandbox zijn gelijkaardig aan die voor het vormen van het in het milieu van de Productie.\
Voor meer informatie over het vormen [!DNL Workfront] met SSO, zie [ Overzicht van enige teken-op in Adobe Workfront ](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>Dit is niet beschikbaar als de [!DNL Workfront] -instantie van uw organisatie is ingeschakeld met Adobe IMS. Zie uw netwerk of beheerder van IT als u meer informatie nodig hebt.

## Beoogd gebruik en beschikbaarheid

* [!DNL Workfront] Aangepaste Sandbox-omgevingen voor vernieuwen zijn niet bedoeld voor prestatie- of laadtests. Gebruik in plaats daarvan deze omgevingen om de functionaliteit van functies te valideren met de bestaande workflows van uw organisatie.

* [!DNL Workfront] Aangepaste Sandbox-omgevingen voor vernieuwen zijn altijd beschikbaar. Elke storing in een aangepaste Sandbox-omgeving voor het vernieuwen van Workfront tijdens normale kantooruren is een eerste prioriteit onmiddellijk nadat eventuele productiekwesties zijn opgelost. Elke storing in een aangepaste sandbox van Workfront Vernieuwen tijdens weekends (zaterdag en zondag) wordt opgelost, zodat de omgeving op maandag voor kantooruren wordt gebruikt.

* Proofing is niet beschikbaar in de aangepaste Sandbox-omgeving voor vernieuwen.
