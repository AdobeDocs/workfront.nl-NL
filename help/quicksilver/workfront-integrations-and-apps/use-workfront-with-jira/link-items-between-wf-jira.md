---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: De punten van de verbinding tussen  [!DNL Adobe Workfront]  en  [!DNL Jira]
description: U kunt  [!DNL Jira]  kwesties aan  [!DNL Adobe Workfront]  taken of kwesties of automatisch of manueel verbinden.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '1126'
ht-degree: 0%

---

# Items koppelen tussen [!DNL Adobe Workfront] en [!DNL Jira]

U kunt [!DNL Jira] -uitgaven automatisch of handmatig koppelen aan [!DNL Adobe Workfront] -taken of -problemen.

Er kan slechts één item in [!DNL Workfront] worden gekoppeld aan één item in [!DNL Jira] . U kunt een [!DNL Workfront] -item nooit koppelen aan meerdere [!DNL Jira] -problemen of een [!DNL Jira] -probleem aan meerdere [!DNL Workfront] -items.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan] </a>*</td> 
   <td> <p>[!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref"> Adobe [!DNL Workfront] overzicht van vergunningen </a>*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegang tot Jira</td> 
   <td> <p>Toegang tot systeembeheerder</p> <p><b>BELANGRIJK</b>

Wij adviseren dat u afzonderlijke rekeningen van de systeembeheerder in [!DNL Jira] en [!DNL Workfront] creeert om aan deze integratie te wijden, eerder dan het gebruiken van bestaande die aan gebruikers zouden kunnen worden vastgemaakt.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder zijn. Voor informatie over [!DNL Workfront] beheerders, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> een gebruiker volledige administratieve toegang verlenen </a>.</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de [!DNL Workfront] -beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een [!DNL Workfront] beheerder uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw [!DNL Workfront] beheerder.

## Vereisten

Voordat u items kunt koppelen tussen [!DNL Workfront] en [!DNL Jira] , moet u

* Installeren [!DNL Workfront] voor [!DNL Jira]

  Voor instructies bij het installeren van Workfront voor Jira, zie [ Adobe Workfront voor Jira installeren ](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* [!DNL Workfront] voor Jira configureren

  Voor instructies bij het vormen van Workfront voor Jira, zie [ Adobe Workfront voor Jira ](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) vormen.

## [!DNL Workfront] -items automatisch koppelen aan [!DNL Jira] -problemen

Als [!DNL Workfront] beheerder kunt u triggers definiëren die automatisch een probleem kunnen maken in [!DNL Jira] telkens wanneer aan bepaalde voorwaarden wordt voldaan voor een taak of een probleem in [!DNL Workfront] . De Workfront- en [!DNL Jira] -items worden gekoppeld.

Nadat u de configuratie van [!DNL Workfront] voor Jira hebt voltooid, wordt wanneer een item in [!DNL Workfront] wordt gemaakt of bijgewerkt zodat dit overeenkomt met uw triggers, automatisch een nieuw item gemaakt in [!DNL Jira] .\
Workfront-gebruikers die Workfront-items maken en bijwerken, hebben geen [!DNL Jira] -licentie nodig om het maken van items in [!DNL Jira] te activeren.

Voor meer informatie over het bepalen van trekkers voor het creëren van kwesties Jira automatisch, zie [  [!DNL Adobe Workfront]  voor Jira ](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) vormen.

>[!NOTE]
>
>U kunt [!DNL Jira] items automatisch maken door een sjabloon aan een project te koppelen. Als de sjabloon taken bevat met toewijzingen die voldoen aan de triggers van [!DNL Jira] , genereren de nieuwe taken nieuwe [!DNL Jira] -problemen.

Het automatisch koppelen van een [!DNL Workfront] -uitgave aan een [!DNL Jira] -uitgave is hetzelfde als het automatisch koppelen van een [!DNL Workfront] -taak aan een [!DNL Jira] -uitgave.

Als u een [!DNL Workfront] -taak automatisch wilt koppelen aan een [!DNL Jira] -probleem:

1. Zorg ervoor dat de systeembeheerder van [!DNL Jira] triggers heeft geconfigureerd voor het automatisch maken van [!DNL Jira] -problemen wanneer [!DNL Workfront] -items worden toegewezen. Meld u vervolgens aan bij [!DNL Workfront] met een toegangsniveau waarmee u een taak kunt maken.

   Voor meer informatie over toegang tot taken, zie [ Toegang van de Verlening tot taken ](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

1. Ga naar een project en selecteer **[!UICONTROL Tasks]** ![](assets/tasks-icon-in-left-panel-14x14.png) in het linkerdeelvenster.

1. Klikken **[!UICONTROL New Task]**

   of

   Selecteer een bestaande taak, dan klik **uitgeven**.

1. Geef de velden op die beschikbaar zijn voor de taak of werk deze bij.
1. Klik op **[!UICONTROL Assignments]** en wijs de taak toe aan een gebruiker, rol of team die is opgegeven als trigger bij de [!DNL Jira] -integratie.

1. Klik **sparen Veranderingen**.

   In Workfront wordt een nieuwe taak gemaakt.

   In het gedeelte **[!UICONTROL Updates]** van de nieuwe taak ziet u een opmerking die aangeeft dat er ook een nieuwe uitgave is gemaakt in [!DNL Jira] .

1. (Optioneel) Klik op de koppeling naar de Jira-kwestie om deze in Jira te openen.

   of

   Klik op de koppeling **[!UICONTROL Go to Jira]** in het **[!UICONTROL Integrations]** -gebied van de **[!UICONTROL Details]** -sectie of in de taak- of uitgaveheader om het [!DNL Jira] -probleem te openen.

   Uw systeem- of groepsbeheerder moet het veld [!UICONTROL Integrations] toevoegen aan uw lay-outsjabloon om dit in de taak- of uitgiftekop weer te geven. Voor informatie, zie [ objecten kopballen aanpassen gebruikend een lay-outmalplaatje ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Elke [!DNL Jira] -gebruiker kan direct beginnen te werken aan automatisch van [!DNL Workfront] gemaakte items. De updates van deze items worden overgebracht naar [!DNL Workfront] zonder dat hiervoor een licentie voor [!DNL Workfront] is vereist.

   Alleen de velden die u als [!DNL Workfront] beheerder tijdens de installatie van de [!DNL Workfront] invoegtoepassing hebt geconfigureerd, worden bijgewerkt.

   Voor meer informatie over het synchroniseren van gebieden tussen Workfront en Jira, zie [ Workfront voor Jira ](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira) sectie in [ vormen Adobe Workfront voor Jira ](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >Het probleem [!DNL Jira] wordt niet toegewezen aan iemand in [!DNL Jira] wanneer het automatisch wordt gemaakt vanuit Workfront.

## [!DNL Jira] -problemen handmatig koppelen aan [!DNL Workfront] -items

Nadat items in [!DNL Jira] en [!DNL Workfront] zijn gemaakt, onafhankelijk van elkaar, kunt u een [!DNL Jira] -uitgave handmatig koppelen aan een bestaande [!DNL Workfront] -taak of -uitgave.\
U kunt een [!DNL Workfront] item van [!DNL Workfront] niet handmatig koppelen aan een bestaand [!DNL Jira] item.

>[!NOTE]
>
>Als het [!DNL Jira] -probleem zich niet voordoet in een project dat niet is geïdentificeerd als een trigger in de [!DNL Workfront] -integratie, kunt u het niet handmatig koppelen aan een Workfront-item wanneer u de integratie met [!DNL Jira] On-Premise gebruikt.\
>Voor meer informatie over vestiging trekkers voor Workfront aan het werkschema van Jira, zie [ automatisch de punten van Workfront met de kwesties van Jira verbinden ](#automatically-link-workfront-items-to-jira-issues).

Wanneer [!DNL Workfront] - en [!DNL Jira] -items aan elkaar zijn gekoppeld, kunnen bepaalde velden van het ene item automatisch worden bijgewerkt.\
Voor meer informatie over het bijwerken van verbonden punten, zie [ Gekoppelde punten tussen Jira en Adobe Workfront ](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md) bijwerken.

[!DNL Jira] -uitgaven handmatig koppelen aan [!DNL Workfront] -items:

1. (Voorwaardelijk) Meld u aan bij [!DNL Workfront] en zoek een probleem of een taak die u wilt koppelen aan [!DNL Jira] -probleem.
1. (Voorwaardelijk) van de adresbar van het punt, kopieer **URL** van het punt in Workfront.

   of

   Kopieer vanuit het gebied [!UICONTROL Details] de **[!UICONTROL Reference Number]** van het item in Workfront.

   >[!NOTE]
   >
   >U moet een [!DNL Workfront] -licentie hebben om u aan te melden bij [!DNL Workfront] . Anders moet een [!DNL Workfront] -gebruiker deze informatie aan u verstrekken.

1. Navigeer in [!DNL Jira] naar een uitgave die u handmatig wilt koppelen aan het [!DNL Workfront] -item.
1. In het [!DNL Workfront] juiste paneel, kleef **URL** of **[!UICONTROL Reference Number]** van het [!DNL Workfront] punt dat u aan het wilt verbinden.

1. Klik op **[!UICONTROL Link]**.

   De twee items worden gekoppeld en het deelvenster [!DNL Workfront] rechts wordt gevuld met informatie uit het [!DNL Workfront] -item.

   De volgende [!DNL Workfront] -velden zijn standaard zichtbaar in [!DNL Jira] in het deelvenster [!DNL Workfront] rechts:

   * The **[!UICONTROL Name]** of the item: You can access the [!DNL Workfront] item by click the name in the panel.
   * **[!UICONTROL Project Name]**
   * De **[!UICONTROL Status]** van het item
   * De **[!UICONTROL Priority]** van het item
   * De datum waarop deze werd gemaakt in [!DNL Workfront]
   * De **[!UICONTROL Planned Hours]** van het item
   * De lus **[!UICONTROL Reference Number]** : u kunt het [!DNL Workfront] -item openen door op de knop [!UICONTROL Reference Number] in het deelvenster te klikken.

Voor meer informatie over het toelaten van extra gebieden om in het juiste paneel te tonen, zie [ gebiedssynchronisatie tussen  [!DNL Jira]  en  [!DNL Workfront]  Punten ](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization) sectie in [ vormen  [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). Een opmerking van de [!DNL Workfront] -beheerder die aan de integratie is gekoppeld, wordt op het tabblad **[!DNL Workfront]** van de [!DNL Jira] -uitgave geplaatst om te bevestigen dat een nieuw [!DNL Jira] -item is gemaakt. De opmerking bevat een koppeling naar de [!DNL Jira] -kwestie.

## Items ontkoppelen tussen [!DNL Jira] en [!DNL Workfront]

Gekoppelde items tussen [!DNL Jira] en [!DNL Workfront] kunnen handmatig worden ontkoppeld vanuit [!DNL Jira] .\
U kunt een [!DNL Workfront] -item niet ontkoppelen van de [!DNL Jira] tegenhanger in [!DNL Workfront] .

U hebt de volgende toegang nodig om handmatig gekoppeld item te ontkoppelen:

* U bent de gebruiker die de items handmatig heeft gekoppeld
* U bent de [!DNL Jira] systeembeheerder

Alleen een [!DNL Workfront] -beheerder kan items ontkoppelen die automatisch zijn gekoppeld.

Een [!DNL Jira] -uitgave loskoppelen van een [!DNL Workfront] -item:

1. Navigeer in [!DNL Jira] naar een probleem dat is gekoppeld aan een [!DNL Workfront] -taak of -probleem.
1. Ga naar het rechterdeelvenster van [!DNL Workfront] , klik op het pictogram **[!UICONTROL Unlink]** en klik vervolgens op **[!UICONTROL Unlink]** .

   De eerder gekoppelde [!DNL Jira] - en [!DNL Workfront] -items worden nu ontkoppeld. Alle velden, opmerkingen of documenten die in de toekomst afzonderlijk op de velden kunnen worden bijgewerkt, worden niet bijgewerkt op de vorige versie in de andere toepassing.
