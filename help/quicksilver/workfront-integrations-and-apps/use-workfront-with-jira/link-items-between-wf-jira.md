---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: De punten van de verbinding tussen  [!DNL Adobe Workfront]  en  [!DNL Jira]
description: U kunt  [!DNL Jira]  kwesties aan  [!DNL Adobe Workfront]  taken of kwesties of automatisch of manueel verbinden.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 0%

---

# Items koppelen tussen [!DNL Adobe Workfront] en [!DNL Jira]

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>Om stabielere en scalable integratie te leveren, verschuiven wij naar een moderne, flexibele integratiebenadering gebruikend Workfront Automation and Integration (Fusion). Als deel van dit overgangsproces, zal Workfront voor de integratie van Jira niet beschikbaar na **28 Februari, 2026** zijn.
>
>We raden u aan Workfront Automation and Integration te gebruiken voor de integratiebehoeften van uw organisatie met Jira.
>
>Voor een overzicht van de Automatisering en de Integratie van Workfront, zie [&#x200B; het overzicht van de Fusie van Adobe Workfront &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Voor informatie over de specifieke mogelijkheden van de modules van de Automatisering en van de Integratie van Workfront voor Jira, zie {de modules van de Software van 0} Jira [.](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new)

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

U kunt [!DNL Jira] -uitgaven automatisch of handmatig koppelen aan [!DNL Adobe Workfront] -taken of -problemen.

Er kan slechts één item in [!DNL Workfront] worden gekoppeld aan één item in [!DNL Jira] . U kunt een [!DNL Workfront] -item nooit koppelen aan meerdere [!DNL Jira] -problemen of een [!DNL Jira] -probleem aan meerdere [!DNL Workfront] -items.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td><p>Alle</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard </p>
       <p>Plan </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Toegang tot Jira</td> 
   <td> <p>Toegang tot systeembeheerder</p> <p>Belangrijk: wij adviseren dat u afzonderlijke rekeningen van de systeembeheerder in Jira en Workfront creeert om aan deze integratie te wijden, eerder dan het gebruiken van bestaande die aan gebruikers zouden kunnen worden vastgemaakt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Installeren [!DNL Workfront] voor [!DNL Jira]

[!DNL Workfront] voor [!DNL Jira] OnDemand installeren is hetzelfde als op een [!DNL Jira] Server-instantie installeren.

U moet een [!DNL Jira] -beheerder zijn om de [!DNL Workfront] add-on te installeren.

Als u geen [!DNL Jira] beheerder bent, kunt u naar de [!DNL Workfront] add-on bladeren en vragen of deze kan worden geïnstalleerd. Uw verzoek wordt naar de [!DNL Jira] -beheerder verzonden voor goedkeuring en installatie.

Voor meer informatie over het verzoeken van om toe:voegen-op om op uw [!DNL Jira] toepassing te worden geïnstalleerd, zie [&#x200B; het Leiden gebruikersverzoeken om toe:voegen-ons.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Ga als volgt te werk om [!DNL Workfront for Jira] te installeren:

1. Meld u aan bij [!DNL Jira] als [!DNL Jira] -beheerder.
1. Vind **[!DNL Workfront for Jira]** toe:voegen-op in [[!DNL Atlassian Marketplace] &#x200B;](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview).

1. Klik op **[!UICONTROL Get it now]** om de toepassing te installeren.

   Nadat de installatie is voltooid, kunt u zich aanmelden bij [!DNL Workfront] vanuit [!DNL Jira] en uw integratie configureren.

   Voor meer informatie, zie [&#x200B; Adobe Workfront voor Jira &#x200B;](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) vormen.

## Vereisten

Voordat u items kunt koppelen tussen [!DNL Workfront] en [!DNL Jira] , moet u het volgende doen:

* Installeer [!DNL Workfront] voor [!DNL Jira] .

  Voor instructies, zie [&#x200B; installeer Adobe Workfront voor Jira &#x200B;](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* [!DNL Workfront] voor Jira configureren.

  Voor instructies, zie [&#x200B; Adobe Workfront voor Jira &#x200B;](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) vormen.

## [!DNL Workfront] -items automatisch koppelen aan [!DNL Jira] -problemen

Als [!DNL Workfront] -beheerder kunt u triggers definiëren die automatisch een probleem in [!DNL Jira] maken wanneer aan bepaalde voorwaarden wordt voldaan voor een taak of een probleem in [!DNL Workfront] . De Workfront- en [!DNL Jira] -items worden gekoppeld.

Nadat u de configuratie van [!DNL Workfront] voor Jira hebt voltooid, wordt wanneer een item in [!DNL Workfront] wordt gemaakt of bijgewerkt zodat dit overeenkomt met uw triggers, automatisch een nieuw item gemaakt in [!DNL Jira] .

Workfront-gebruikers die Workfront-items maken en bijwerken, hebben geen [!DNL Jira] -licentie nodig om het maken van items in [!DNL Jira] te activeren.

Voor meer informatie, zie [&#x200B;  [!DNL Adobe Workfront]  voor Jira &#x200B;](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) vormen.

>[!NOTE]
>
>U kunt [!DNL Jira] items automatisch maken door een sjabloon aan een project te koppelen. Als de sjabloon taken bevat met toewijzingen die voldoen aan de triggers van [!DNL Jira] , genereren de nieuwe taken nieuwe [!DNL Jira] -problemen.

Het automatisch koppelen van een [!DNL Workfront] -uitgave aan een [!DNL Jira] -uitgave is hetzelfde als het automatisch koppelen van een [!DNL Workfront] -taak aan een [!DNL Jira] -uitgave.

Als u een [!DNL Workfront] -taak automatisch wilt koppelen aan een [!DNL Jira] -probleem:

1. Zorg ervoor dat de systeembeheerder van [!DNL Jira] triggers heeft geconfigureerd voor het automatisch maken van [!DNL Jira] -problemen wanneer [!DNL Workfront] -items worden toegewezen. Meld u vervolgens aan bij [!DNL Workfront] met een toegangsniveau waarmee u een taak kunt maken.

   Voor meer informatie over toegang tot taken, zie [&#x200B; Toegang van de Verlening tot taken &#x200B;](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

{{step1-to-projects}}

1. Voor de **pagina van Projecten**, selecteer een project.

1. Selecteer **[!UICONTROL Tasks]** in het deelvenster aan de linkerkant van het project.

1. Klik **+ Nieuwe Taak**.

   >[!NOTE]
   >
   >Om een bestaand punt van Workfront met een kwestie van Jira te verbinden, uitgezocht **&#x200B;**&#x200B;van het punt **meer** ![&#x200B; &#x200B;](assets/more-icon.png) menu van het pictogram Meer &lbrace;uitgeven.

1. Geef de velden op die beschikbaar zijn voor de taak of werk deze bij.
1. Zoek en selecteer in het veld **[!UICONTROL Assignments]** de gebruiker, rol of het team dat als trigger voor de [!DNL Jira] -integratie is opgegeven.

1. Klik **creëren Taak**. De taak wordt gecreeerd in Workfront, en een nieuwe commentaar verschijnt in het 1&rbrace; lusje van de Updates van de taak **&lbrace;om erop te wijzen dat een nieuwe kwestie ook in** is gecreeerd.[!DNL Jira]

1. (Optioneel) Klik in het gedeelte **[!UICONTROL Integrations]** van de **[!UICONTROL Details]** -sectie van de taak- of uitgiftekop op de koppeling **[!UICONTROL Go to Jira]** om het probleem te openen in Jira.

   Uw systeem- of groepsbeheerder moet het veld [!UICONTROL Integrations] toevoegen aan uw lay-outsjabloon om dit in de taak- of uitgiftekop weer te geven. Voor informatie, zie [&#x200B; objecten kopballen aanpassen gebruikend een lay-outmalplaatje &#x200B;](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Elke [!DNL Jira] -gebruiker kan direct beginnen te werken aan automatisch van [!DNL Workfront] gemaakte items. De updates van deze items worden overgebracht naar [!DNL Workfront] zonder dat hiervoor een licentie voor [!DNL Workfront] is vereist.

   Alleen de velden die u als [!DNL Workfront] beheerder tijdens de installatie van de [!DNL Workfront] invoegtoepassing hebt geconfigureerd, worden bijgewerkt.

   Voor meer informatie over het synchroniseren van gebieden tussen Workfront en Jira, zie Configure Workfront voor de sectie van Jira in [&#x200B; Adobe Workfront voor Jira &#x200B;](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) vormen.

   >[!NOTE]
   >
   >Het [!DNL Jira] -probleem wordt niet toegewezen aan iemand in [!DNL Jira] wanneer het automatisch wordt gemaakt vanuit Workfront.

## [!DNL Jira] -problemen handmatig koppelen aan [!DNL Workfront] -items

Nadat items in [!DNL Jira] en [!DNL Workfront] onafhankelijk van elkaar zijn gemaakt, kunt u een [!DNL Jira] -uitgave handmatig koppelen aan een bestaande [!DNL Workfront] -taak of -uitgave.

U kunt een [!DNL Workfront] item van [!DNL Workfront] niet handmatig koppelen aan een bestaand [!DNL Jira] item.

>[!NOTE]
>
>Als het [!DNL Jira] -probleem zich niet voordoet in een project dat niet is geïdentificeerd als een trigger in de [!DNL Workfront] -integratie, kunt u het niet handmatig koppelen aan een Workfront-item wanneer u de integratie met [!DNL Jira] On-Premise gebruikt.\
>Voor meer informatie over vestiging trekkers voor Workfront aan het werkschema van Jira, zie [&#x200B; automatisch de punten van Workfront met de kwesties van Jira verbinden &#x200B;](#automatically-link-workfront-items-to-jira-issues).

Wanneer [!DNL Workfront] - en [!DNL Jira] -items aan elkaar zijn gekoppeld, kunnen bepaalde velden van het ene item automatisch worden bijgewerkt.\
Voor meer informatie over het bijwerken van verbonden punten, zie [&#x200B; Gekoppelde punten tussen Jira en Adobe Workfront &#x200B;](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md) bijwerken.

[!DNL Jira] -uitgaven handmatig koppelen aan [!DNL Workfront] -items:

1. (Voorwaardelijk) Meld u aan bij [!DNL Workfront] en zoek een probleem of een taak die u wilt koppelen aan een [!DNL Jira] -probleem.
1. (Voorwaardelijk) in de **Basisinformatie** sectie in de **Details van de Taak** of **Details van de Uitgave** lusje, kopieer **[!UICONTROL Reference Number]** van het punt in Workfront.

   of

   Van de adresbar van het punt, kopieer **URL** van het punt in Workfront.

   >[!IMPORTANT]
   >
   >Als uw organisatie aan de Adobe Verenigde Ervaring is bezet, moet u het **Aantal van de Verwijzing** gebruiken voor het verbinden van de punten van Workfront met Jira. (De optie URL is beschikbaar, maar er wordt een fout geretourneerd als u deze optie gebruikt.) Voor informatie over de Verenigde Ervaring, zie [&#x200B; Adobe Verenigde Ervaring voor Workfront &#x200B;](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
   >
   >Voor organisaties die zich niet op de Adobe Verenigde Ervaring bevinden, wordt het niet aanbevolen om de optie URL te gebruiken omdat URLs kan veranderen.

   >[!NOTE]
   >
   >U moet een [!DNL Workfront] -licentie hebben om u aan te melden bij [!DNL Workfront] . Anders moet een [!DNL Workfront] -gebruiker deze informatie aan u verstrekken.

1. Navigeer in [!DNL Jira] naar een uitgave die u handmatig wilt koppelen aan het [!DNL Workfront] -item.
1. In het [!DNL Workfront] juiste paneel, kleef **[!UICONTROL Reference Number]** of **URL** van het [!DNL Workfront] punt dat u het aan wilt verbinden.

1. Klik op **[!UICONTROL Link]**. De twee items worden gekoppeld en het deelvenster [!DNL Workfront] rechts wordt gevuld met informatie uit het [!DNL Workfront] -item.

   Standaard zijn de volgende [!DNL Workfront] -velden zichtbaar in [!DNL Jira] in het rechterdeelvenster van [!DNL Workfront] :

   * De **[!UICONTROL Name]** van het item. U kunt het [!DNL Workfront] -item openen door op de naam in het deelvenster te klikken.
   * De **[!UICONTROL Project Name]** .
   * De **[!UICONTROL Status]** van het item.
   * De **[!UICONTROL Priority]** van het item.
   * De datum waarop deze is gemaakt in [!DNL Workfront] .
   * De **[!UICONTROL Planned Hours]** van het item.
   * De **[!UICONTROL Reference Number]** . U kunt tot het [!DNL Workfront] punt toegang hebben door het **Aantal van de Verwijzing** in het paneel te klikken.

   Voor meer informatie over het toelaten van extra gebieden om in het juiste paneel te tonen, zie de Configure gebiedssynchronisatie tussen [!DNL Jira] en [!DNL Workfront] sectie van Punten in [&#x200B; vormen  [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). Een opmerking van de [!DNL Workfront] -beheerder die aan de integratie is gekoppeld, wordt op het tabblad **[!DNL Workfront]** van de [!DNL Jira] -uitgave geplaatst om te bevestigen dat een nieuw [!DNL Jira] -item is gemaakt. De opmerking bevat een koppeling naar de [!DNL Jira] -kwestie.

## Items ontkoppelen tussen [!DNL Jira] en [!DNL Workfront]

Gekoppelde items tussen [!DNL Jira] en [!DNL Workfront] kunnen handmatig worden ontkoppeld in [!DNL Jira] . U kunt een [!DNL Workfront] -item niet ontkoppelen van de [!DNL Jira] tegenhanger in [!DNL Workfront] .

U hebt de volgende toegang nodig om handmatig gekoppeld item te ontkoppelen:

* U bent de gebruiker die de items handmatig heeft gekoppeld.
* U bent de [!DNL Jira] systeembeheerder.

>[!NOTE]
>
>Alleen een [!DNL Workfront] -beheerder kan items ontkoppelen die automatisch zijn gekoppeld.

Een [!DNL Jira] -uitgave loskoppelen van een [!DNL Workfront] -item:

1. Log in bij Jira.
1. Navigeer naar het probleem dat is gekoppeld aan een [!DNL Workfront] -taak of -uitgave.
1. Ga naar het **Workfront** juiste paneel.
1. Klik op het pictogram **[!UICONTROL Unlink]** en klik vervolgens op **[!UICONTROL Unlink]** . De eerder gekoppelde [!DNL Jira] - en [!DNL Workfront] -items worden ontkoppeld.

   Een van de velden, opmerkingen of documenten die in de toekomst worden bijgewerkt, wordt niet bijgewerkt op de vorige versie in de andere toepassing.
