---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Werk verbonden punten tussen  [!DNL Jira]  en  [!DNL Adobe Workfront] bij
description: Wanneer u  [!DNL Jira]  kwesties met  [!DNL Adobe Workfront]  taken of kwesties verbindt, kunnen uw gebruikers punten in één toepassing en tegenhanger van dat punt ook bijwerken voor de gebruikers die in de tweede toepassing werken.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '1492'
ht-degree: 0%

---

# Gekoppelde items bijwerken tussen [!DNL Jira] en [!DNL Adobe Workfront]

>[!IMPORTANT]
>
>Om stabielere en scalable integratie te leveren, verschuiven wij naar een moderne, flexibele integratiebenadering gebruikend Workfront Automation and Integration (Fusion). Als deel van dit overgangsproces, zal Workfront voor de integratie van Jira niet beschikbaar na **28 Februari, 2026** zijn.
>
>We raden u aan Workfront Automation and Integration te gebruiken voor de integratiebehoeften van uw organisatie met Jira.
>
>Voor een overzicht van de Automatisering en de Integratie van Workfront, zie [ het overzicht van de Fusie van Adobe Workfront ](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Voor informatie over de specifieke mogelijkheden van de modules van de Automatisering en van de Integratie van Workfront voor Jira, zie {de modules van de Software van 0} Jira [.](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new)

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Wanneer u [!DNL Jira] -problemen koppelt aan [!DNL Adobe Workfront] -taken of -problemen, kunnen uw gebruikers items in één toepassing bijwerken en wordt de tegenhanger van dat item ook bijgewerkt voor de gebruikers die in de tweede toepassing werken.

Voor meer informatie over het verbinden van punten tussen [!DNL Workfront] en [!DNL Jira], zie [ punten van de Verbinding tussen Adobe Workfront en Jira ](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Terwijl u [!DNL Workfront] instelt voor [!DNL Jira] , kunt u als [!DNL Jira] systeembeheerder bepaalde velden in de ene toepassing configureren om te synchroniseren met velden uit gekoppelde items in de andere toepassing.

Voor meer informatie over het synchroniseren van gebieden tussen verbonden [!DNL Jira] en [!DNL Workfront] punten, zie [  [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md) vormen.

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

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat u items kunt koppelen tussen [!DNL Workfront] en [!DNL Jira] , moet u:

* Installeer [!DNL Workfront for Jira] .

  Voor instructies bij het installeren van [!DNL Workfront for Jira], zie [ installeren  [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configureer [!DNL Workfront for Jira].

  Voor instructies bij het vormen [!DNL Workfront for Jira], zie [ vormen  [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Koppel items tussen [!DNL Workfront] en [!DNL Jira] .

  Voor instructies, zie [ punten van de Verbinding tussen  [!DNL Adobe Workfront]  en  [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Gekoppelde items bijwerken in [!DNL Workfront]

Als u voornamelijk in [!DNL Workfront] werkt, kunt u uw werkitems in [!DNL Workfront] en hun tegenhangers in [!DNL Jira] ook bijwerken. Deze update vindt plaats door de integratie van [!DNL Workfront] for [!DNL Jira] , waarvoor geen [!DNL Jira] -licentie vereist is.

Zolang de [!DNL Workfront] beheerder [!DNL Workfront for Jira] heeft geconfigureerd om de velden tussen gekoppelde items te synchroniseren, worden bepaalde velden die u in [!DNL Workfront] bijwerkt ook bijgewerkt voor het gekoppelde [!DNL Jira] -probleem. Voor meer informatie over het bijwerken van punten in [!DNL Workfront], zie [ kwesties ](../../manage-work/issues/manage-issues/edit-issues.md) uitgeven en [ taken ](../../manage-work/tasks/manage-tasks/edit-tasks.md) uitgeven.

In de volgende lijst wordt aangegeven welke [!DNL Workfront] -velden worden gesynchroniseerd met [!DNL Jira] -velden op gekoppelde items:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Bijgewerkt [!DNL Workfront] gebied </strong> </th> 
   <th><strong> Gesynchroniseerd [!DNL Jira] gebied/update </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Issue or Task name]</td> 
   <td> <p>[!UICONTROL Issue name]</p> <p>Er wordt een opmerking over de naamwijziging toegevoegd aan het tabblad <strong>[!DNL Workfront]</strong> van het [!DNL Jira] -probleem. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Description]</td> 
   <td> <p> [!UICONTROL Issue Description]</p> <p>Er wordt een opmerking over de bijgewerkte beschrijving toegevoegd aan het tabblad <strong>[!DNL Workfront]</strong> van de [!DNL Jira] -uitgave.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Uploaded Documents]</p> <p>Opmerking: documenten die zijn gekoppeld aan [!DNL Workfront] -items van een externe server, worden niet overgebracht naar [!DNL Jira] -uitgaven. Alleen documenten die rechtstreeks naar [!DNL Workfront] -items zijn geüpload, worden ook bijgewerkt naar de gekoppelde [!DNL Jira] -uitgaven. </p> </td> 
   <td> <p>[!UICONTROL Attachments]</p> <p>Er wordt een opmerking over de geüploade bijlagen toegevoegd aan het tabblad <strong>[!DNL Workfront]</strong> van de uitgave [!DNL Jira] .<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Completion Date]</td> 
   <td> <p>[!UICONTROL Due Date]</p> <p>Er wordt een opmerking toegevoegd over het feit dat [!UICONTROL Due Date] is gewijzigd aan het tabblad [!DNL Workfront] van de uitgave [!DNL Jira] . </p> <p>Opmerking: u moet <strong>[!UICONTROL Due Date]</strong> inschakelen voordat uw [!DNL Jira] -problemen dit veld kunnen zien bijgewerkt in [!UICONTROL Jira] . </p> </td> 
  </tr> 
  <tr> 
   <td>Aangepaste Forms- en aangepaste velden</td> 
   <td> <p> Geef deze weer in het deelvenster [!DNL Workfront] rechts van de uitgave [!DNL Jira] . <br> slechts de Gebieden van de Douane die een daadwerkelijke waardevertoning in het paneel hebben.<br></p> <p>Opmerking: in de secties Aangepaste formulieren wordt het toegangsniveau van de [!DNL Workfront] -beheerder weergegeven. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Priority]</td> 
   <td>Wordt weergegeven in het deelvenster [!DNL Workfront] rechts van de uitgave [!DNL Jira] . <br> Het veld uitgave <strong>[!UICONTROL Priority]</strong> in [!DNL Jira] wordt niet bijgewerkt. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Log time] </td> 
   <td> <p>Er wordt een opmerking over de aangemelde tijd toegevoegd op het tabblad <strong>[!DNL Workfront]</strong> van de [!DNL Jira] -uitgave. Dit omvat de naam van de gebruiker die de tijd registreert, evenals de gebruiker voor wie de tijd wordt geregistreerd, voor het geval zij verschillend zijn. Er is geen tijd aangemeld op de tab <strong>[!UICONTROL Work log]</strong> in [!DNL Jira] .<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comments]</td> 
   <td> <p>De opmerking wordt toegevoegd aan het tabblad <strong>[!DNL Workfront]</strong> van de [!DNL Jira] -uitgave. Het wordt niet toegevoegd aan het tabblad <strong>[!UICONTROL Comments]</strong> van het [!DNL Jira] -probleem</p> <p>Opmerking: wanneer u twee bestaande items handmatig koppelt, worden de opmerkingen die aan het [!DNL Workfront] -item zijn toegevoegd voordat u het item koppelt aan [!DNL Jira] , niet gesynchroniseerd met het [!DNL Jira] -probleem. </p> <p>Jira-opmerkingen worden wel gesynchroniseerd met Workfront.</td> 
  </tr> 
 </tbody> 
</table>

## Gekoppelde items bijwerken in [!DNL Jira]

Als u voornamelijk in [!DNL Jira] werkt, kunt u uw werkitems in [!DNL Jira] en hun tegenhangers in [!DNL Workfront] ook bijwerken. U hoeft geen [!DNL Workfront] licentie te hebben voor de [!DNL Workfront] items die zijn gekoppeld aan uw [!DNL Jira] -uitgaven om de updates te ontvangen die u maakt in [!DNL Jira] .

Op voorwaarde dat de [!DNL Workfront] beheerder [!DNL Workfront] for [!DNL Jira] heeft geconfigureerd voor het synchroniseren van de velden tussen gekoppelde items, worden bepaalde velden die u bijwerkt in [!DNL Jira] ook bijgewerkt voor het gekoppelde [!DNL Workfront] -item.

In de volgende lijst wordt aangegeven welke [!DNL Jira] -velden worden gesynchroniseerd met [!DNL Workfront] -velden op gekoppelde items:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Bijgewerkt [!DNL Jira] Gebied </strong> </th> 
   <th><strong> Gesynchroniseerd [!DNL Workfront] Gebied/Update </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Issue Status]</td> 
   <td> <p> [!UICONTROL Issue or Task Status]</p> <p>De status van de kwestie in [!DNL Jira] syncs met de volgende statussen, of statussen die met de volgende statussen, in Workfront gelijkstellen:</p> 
    <ul> 
     <li> <p>[!UICONTROL New] ([!UICONTROL NEW])</p> </li> 
     <li> <p>[!UICONTROL In Progress] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Closed]/[!UICONTROL Complete] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Opmerking: de status [!DNL Jira] wordt gesynchroniseerd met de eerste [!DNL Workfront] -status die gelijk is aan de juiste status.</p> <p>Voor meer informatie over statussen van punten in [!DNL Workfront], zie <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref"> creeer of geef een status </a> uit.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Issue Attachments]</td> 
   <td> [!UICONTROL Issue or Task Documents]<br> Een opmerking over het uploaden van een nieuw document in [!DNL Jira] wordt toegevoegd aan het tabblad [!UICONTROL Updates] van de [!DNL Workfront] uitgave of taak.  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Due Date]</td> 
   <td> <p> Er wordt een opmerking over de wijziging van de [!UICONTROL Due Date] in [!DNL Jira] toegevoegd aan het tabblad [!UICONTROL Updates] van de [!DNL Workfront] -uitgave of -taak. </p> <p>Opmerking: er zijn geen datums gewijzigd voor het probleem of de taak van [!DNL Workfront] . </p> </td> 
  </tr> 
  <tr> 
   <td> Meldingstijd in het deelvenster [!DNL Workfront] rechts of in het menu [!UICONTROL More] in het venster [!DNL Jira] .<br></td> 
   <td> <p>Uren <br> naast het toevoegen van de uren het programma geopend Jira aan het verbonden [!DNL Workfront] punt, wordt een commentaar over logboektijd toegevoegd aan het [!UICONTROL Updates] lusje van het [!DNL Workfront] punt.</p> <p>Voor meer informatie over het registreren van tijd op verbonden [!DNL Jira] kwesties, met inbegrip van het bijwerken van de [!DNL Jira] gebruiker die de tijd binnen registreert [!DNL Workfront], zie <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref"> tijd van het Logboek voor Gekoppelde [!DNL Jira] en [!DNL Workfront] punten </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Opmerkingen <br><br></td> 
   <td> <p>Opmerkingen worden toegevoegd aan het tabblad [!UICONTROL Updates] van het [!DNL Workfront] -probleem of de <strong>[!UICONTROL Comments]</strong> -taak als de [!UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT] -instelling in de sectie [!UICONTROL Setup] van het tabblad <strong>[!UICONTROL Always]</strong> .</p> <p>Voor informatie over het vormen van de montages van Workfront in [!DNL Jira], zie <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md"> het Vormen [!DNL Workfront for Jira]</a>.</p> <p>Voor informatie over het becommentariëren over punten van verbonden [!DNL Jira] kwesties, zie <a href="#comment-from-a-linked-jira-issue" class="MCXref xref"> Commentaar van een verbonden [!DNL Jira] kwestie </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Logtijd van gekoppelde [!DNL Jira] uitgaven

De tijd die u opneemt voor een [!DNL Jira] item in [!DNL Jira] , wordt ook overgebracht naar het gekoppelde [!DNL Workfront] item, ongeacht de locatie in [!DNL Jira] waar u de tijd registreert.\
Wanneer u zich aanmeldt in Jira in het deelvenster [!DNL Workfront] , wordt de tijd alleen in [!DNL Workfront] opgenomen.\
De tijd die u in [!DNL Workfront] opneemt, heeft geen invloed op de tijd van de gekoppelde uitgave in [!DNL Jira] .

>[!NOTE]
>
>Als de tijd wordt toegevoegd aan een [!DNL Jira] -item dat is gekoppeld aan een [!DNL Workfront] -taak, is de [!UICONTROL Hour Type] voor de tijd in [!DNL Workfront] gelijk aan [!UICONTROL Task Time] . Als de tijd wordt toegevoegd aan een [!DNL Jira] -item dat is gekoppeld aan een [!DNL Workfront] -uitgave, is de [!UICONTROL Hour Type] voor de tijd in [!DNL Workfront] [!UICONTROL Issue Time] .

Er wordt een opmerking toegevoegd aan de tab **[!DNL Workfront]** in [!DNL Jira] en aan de tab **[!UICONTROL Updates]** van het item in [!DNL Workfront] om de logboekregistratie van de tijd op te nemen.\
De tijd wordt ook weergegeven op het tabblad **[!UICONTROL Hours]** van het [!DNL Workfront] -item.

* [ tijd van het Logboek voor Gekoppelde  [!DNL Jira]  en  [!DNL Workfront]  punten ](#log-time-for-linked-jira-and-workfront-items)
* [De tijd van het logboek van  [!DNL Jira]  aan a [!DNL Workfront]  punt](#log-time-from-jira-to-a-workfront-item)

### Logtijd voor gekoppelde [!DNL Jira] en [!DNL Workfront] items

U kunt tijd vastleggen vanuit een [!DNL Jira] -uitgave die is gekoppeld aan een [!DNL Workfront] -item en de tijd wordt zowel op de [!DNL Jira] -uitgave als op het [!DNL Workfront] -item vastgelegd.

>[!IMPORTANT]
>
>Als de gebruiker die zich aanmeldt op de tijd in [!DNL Jira] , niet bestaat in [!DNL Workfront] , wordt door de integratie een nieuwe actieve gebruiker in Workfront gemaakt als **[!UICONTROL Automatically create a user in [!DNL Workfront]&#x200B;if the [!DNL Jira] user does not have a* [!DNL Workfront]&#x200B;account]* * is ingesteld op **[!UICONTROL Always]** . Deze gebruiker neemt geen [!DNL Workfront] -licentie in. U kunt actieve gebruikers toewijzen aan werkitems in [!DNL Workfront] , maar u kunt deze gebruikers niet opnemen in updates. Voor informatie over het vormen van de automatische verwezenlijking van [!DNL Workfront] gebruikers van [!DNL Jira], zie [ het Vormen  [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

U kunt als volgt de tijd voor een item in [!DNL Jira] vastleggen en deze zowel in [!DNL Jira] als [!DNL Workfront] laten opnemen:

1. Meld u aan bij [!DNL Jira] .
1. Ga naar het [!DNL Jira] -probleem dat aan het [!DNL Workfront] -item is gekoppeld.
1. Vouw het menu **[!UICONTROL More]** uit en klik op **[!UICONTROL Log work]** .

1. Geef in het veld **[!UICONTROL Time Spent]** de hoeveelheid tijd op die u aan dit probleem hebt besteed. U moet de tijd opgeven met de volgende tijdsperiodes:

   * [!UICONTROL Weeks] (w)
   * [!UICONTROL Days] (d)
   * [!UICONTROL Hours] (h)

1. Voeg informatie toe aan uw tijdinvoer, inclusief een **[!UICONTROL Work Description]** en klik vervolgens op **[!UICONTROL Log]** .\
   De tijd wordt toegevoegd aan het tabblad **[!UICONTROL Work log]** van het [!DNL Jira] -item en aan het [!DNL Workfront] -item dat eraan is gekoppeld.\
   De werkbeschrijving van de tijdinvoer wordt opgenomen als een opmerking bij het uuritem in [!DNL Workfront] .

### Logtijd van [!DNL Jira] naar een [!DNL Workfront] -item

U kunt de tijd van het gekoppelde [!DNL Workfront] -item vanuit het [!DNL Jira] -probleem gewoon vastleggen zonder deze keer naar het [!DNL Jira] -probleem op te nemen.

1. Meld u aan bij [!DNL Jira] .
1. Navigeer naar een [!DNL Jira] -uitgave die is gekoppeld aan een [!DNL Workfront] -item.

   De details van het [!DNL Workfront] -item moeten worden weergegeven in het rechterdeelvenster van de uitgave van [!DNL Workfront] .

1. Klik op het pictogram **[!UICONTROL Log Time]** .

1. Geef op hoeveel **[!UICONTROL Hours]** en **[!UICONTROL Minutes]** u wilt aanmelden voor de uitgave.

1. Klik op **[!UICONTROL Log Time]**.

   De tijd wordt toegevoegd aan het item [!DNL Workfront] .

   Deze keer wordt niet toegevoegd aan het tabblad [!UICONTROL Work Log] van het [!DNL Jira] -probleem.

## Opmerking van een gekoppelde [!DNL Jira] uitgave {#comment-from-a-linked-jira-issue}

Wanneer u in het [!DNL Jira] rechterdeelvenster [!DNL Workfront] een opmerking maakt over een [!DNL Jira] -item, wordt de opmerking ook toegevoegd aan het tabblad [!UICONTROL Updates] van het gekoppelde item in Workfront.

Opmerkingen van [!DNL Jira] naar een [!DNL Workfront] -item:

1. Meld u aan bij [!DNL Jira] .
1. Navigeer naar een [!DNL Jira] -uitgave die is gekoppeld aan een [!DNL Workfront] -item.

   De details van het [!DNL Workfront] -item moeten worden weergegeven in het rechterdeelvenster van de uitgave van [!DNL Workfront] .

1. Klik op het pictogram **[!UICONTROL Comments]** in het deelvenster [!DNL Workfront] of op de tab **[!UICONTROL Comments]** .

1. Typ een opmerking en klik op **[!UICONTROL Send]** .

   De opmerking wordt toegevoegd aan het volgende:

   * Het tabblad **[!DNL Workfront]** van het [!DNL Jira] -probleem.
   * Het tabblad **[!UICONTROL Comments]** van het [!DNL Jira] -probleem.
   * Het tabblad **[!UICONTROL Updates]** van het gekoppelde item in Workfront.
