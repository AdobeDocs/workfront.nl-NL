---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Gekoppelde items bijwerken tussen [!DNL Jira] en [!DNL Adobe Workfront]
description: Wanneer u een koppeling [!DNL Jira] problemen [!DNL Adobe Workfront] taken of problemen, kunnen uw gebruikers items in één toepassing bijwerken en de tegenhanger van dat item wordt ook bijgewerkt voor de gebruikers die in de tweede toepassing werken.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: e01f5eaf3133fa1bdaedf4dad56e9a8175b70667
workflow-type: tm+mt
source-wordcount: '1399'
ht-degree: 0%

---

# Gekoppelde items bijwerken tussen [!DNL Jira] en [!DNL Adobe Workfront]

Wanneer u een koppeling [!DNL Jira] problemen [!DNL Adobe Workfront] taken of problemen, kunnen uw gebruikers items in één toepassing bijwerken en de tegenhanger van dat item wordt ook bijgewerkt voor de gebruikers die in de tweede toepassing werken.

Voor meer informatie over het koppelen van items tussen [!DNL Workfront] en [!DNL Jira], zie [Objecten koppelen tussen Adobe Workfront en Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Tijdens het instellen [!DNL Workfront] for [!DNL Jira], als [!DNL Jira] systeembeheerder, kunt u bepaalde gebieden van één toepassing vormen om met gebieden van verbonden punten in de andere toepassing te synchroniseren.

Meer informatie over het synchroniseren van velden tussen gekoppelde velden [!DNL Jira] en [!DNL Workfront] objecten, zie [Configureren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td><p>Nieuw: alle</p>
       <p>of</p>
       <p>Huidige: [!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td><p>Nieuw: [!UICONTROL Standard]</p>
       <p>of</p>
       <p>Huidige: [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] toegang</td> 
   <td> <p>Toegang tot systeembeheerder</p> <p>Belangrijk: wij adviseren dat u afzonderlijke rekeningen van de systeembeheerder in [!DNL Jira] en [!DNL Workfront] om aan deze integratie te wijden, eerder dan het gebruiken van bestaande degenen die aan gebruikers zouden kunnen worden vastgemaakt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder.</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

Voordat u items kunt koppelen tussen [!DNL Workfront] en [!DNL Jira], moet u:

* Installeren [!DNL Workfront for Jira].

  Voor installatie-instructies [!DNL Workfront for Jira], zie [Installeren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configureren [!DNL Workfront for Jira].

  Voor instructies over het configureren [!DNL Workfront for Jira], zie [Configureren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Items koppelen tussen [!DNL Workfront] en [!DNL Jira].

  Zie voor instructies [Items koppelen tussen [!DNL Adobe Workfront] en [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Gekoppelde items bijwerken in [!DNL Workfront]

Als u voornamelijk werkt in [!DNL Workfront]kunt u uw werkitems bijwerken in [!DNL Workfront] en hun tegenhangers in [!DNL Jira] ook bijwerken. Deze update wordt uitgevoerd door de integratie van [!DNL Workfront] for [!DNL Jira] waarvoor u geen [!DNL Jira] licentie.

Zo lang als [!DNL Workfront] beheerder heeft gevormd [!DNL Workfront for Jira] om de velden tussen gekoppelde items te synchroniseren, bepaalde velden waarin u bijwerkt [!DNL Workfront] ook bijwerken voor de gekoppelde [!DNL Jira] probleem. Voor meer informatie over het bijwerken van items in [!DNL Workfront], zie [Problemen bewerken](../../manage-work/issues/manage-issues/edit-issues.md) en [Taken bewerken](../../manage-work/tasks/manage-tasks/edit-tasks.md).

In de volgende lijst wordt aangegeven welke [!DNL Workfront] velden synchroniseren met [!DNL Jira] velden voor gekoppelde items:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Bijgewerkt [!DNL Workfront] field</strong> </th> 
   <th><strong>Gesynchroniseerd [!DNL Jira] veld/update</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Issue or Task name]</td> 
   <td> <p>[!UICONTROL Issue name]</p> <p>Er wordt een opmerking over de naamwijziging toegevoegd aan de <strong>[!DNL Workfront]</strong> tabblad van het [!DNL Jira] probleem. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Description]</td> 
   <td> <p> [!UICONTROL Issue Description]</p> <p>Er wordt een opmerking over de bijgewerkte beschrijving toegevoegd aan de <strong>[!DNL Workfront]</strong> tabblad van het [!DNL Jira] probleem.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Uploaded Documents]</p> <p>Opmerking: Documenten die zijn gekoppeld aan [!DNL Workfront] items van een externe server worden niet overgedragen naar [!DNL Jira] problemen. Alleen documenten die rechtstreeks zijn geüpload naar [!DNL Workfront] items worden ook bijgewerkt naar de gekoppelde [!DNL Jira] problemen. </p> </td> 
   <td> <p>[!UICONTROL Attachments]</p> <p>Er wordt een opmerking over de geüploade bijlagen toegevoegd aan de <strong>[!DNL Workfront]</strong> tabblad van het [!DNL Jira] probleem.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Completion Date]</td> 
   <td> <p>[!UICONTROL Due Date]</p> <p>Een opmerking over de [!UICONTROL Due Date] als gewijzigd, wordt toegevoegd aan de [!DNL Workfront] tabblad van het [!DNL Jira] probleem. </p> <p>Opmerking: u moet inschakelen <strong>[!UICONTROL Due Date]</strong> voor uw [!DNL Jira] problemen die moeten worden weergegeven in dit veld [!UICONTROL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>Aangepaste Forms- en aangepaste velden</td> 
   <td> <p> Weergeven in het dialoogvenster [!DNL Workfront] in het rechterdeelvenster van [!DNL Jira] probleem. <br>Alleen de aangepaste velden die een werkelijke waarde hebben, worden in het deelvenster weergegeven.<br></p> <p>Opmerking: secties met aangepaste formulieren worden weergegeven met het toegangsniveau van het dialoogvenster [!DNL Workfront] beheerder. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Issue or Task Priority]</td> 
   <td>Geeft in het dialoogvenster [!DNL Workfront] in het rechterdeelvenster van [!DNL Jira] probleem. <br>Het probleem wordt niet bijgewerkt <strong>[!UICONTROL Priority]</strong> veld in [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Log time] </td> 
   <td> <p>Er wordt een opmerking over de aangemelde tijd toegevoegd aan het dialoogvenster <strong>[!DNL Workfront]</strong> tabblad van het [!DNL Jira] probleem. Dit omvat de naam van de gebruiker die de tijd registreert, evenals de gebruiker voor wie de tijd wordt geregistreerd, voor het geval zij verschillend zijn. Er is geen tijd aangemeld bij het dialoogvenster <strong>[!UICONTROL Work log]</strong> tab in [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comments]</td> 
   <td> <p>De opmerking wordt toegevoegd aan de <strong>[!DNL Workfront]</strong> tabblad van het [!DNL Jira] probleem. Het wordt niet toegevoegd aan de <strong>[!UICONTROL Comments]</strong> tabblad van het [!DNL Jira] kwestie</p> <p>Opmerking: wanneer u twee bestaande items handmatig koppelt, worden de opmerkingen toegevoegd aan de [!DNL Workfront] item voordat het wordt gekoppeld aan [!DNL Jira] niet synchroniseren met de [!DNL Jira] probleem. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Gekoppelde items bijwerken in [!DNL Jira]

Als u voornamelijk werkt in [!DNL Jira]kunt u uw werkitems bijwerken in [!DNL Jira] en hun tegenhangers in [!DNL Workfront] ook bijwerken. U hoeft geen [!DNL Workfront] vergunning voor [!DNL Workfront] objecten gekoppeld aan je [!DNL Jira] problemen om de updates te ontvangen waarin u werkt [!DNL Jira].

Op voorwaarde dat uw [!DNL Workfront] beheerder heeft gevormd [!DNL Workfront] for [!DNL Jira] om de velden tussen gekoppelde items te synchroniseren, bepaalde velden waarin u bijwerkt [!DNL Jira] ook bijwerken voor de gekoppelde [!DNL Workfront] item.

In de volgende lijst wordt aangegeven welke [!DNL Jira] velden synchroniseren met [!DNL Workfront] velden voor gekoppelde items:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Bijgewerkt [!DNL Jira] Veld</strong> </th> 
   <th><strong>Gesynchroniseerd [!DNL Workfront] Veld/update</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Issue Status]</td> 
   <td> <p> [!UICONTROL Issue or Task Status]</p> <p>Status van uitgave in [!DNL Jira] synchroniseert in Workfront met de volgende statussen, of statussen die overeenkomen met de volgende statussen:</p> 
    <ul> 
     <li> <p>[!UICONTROL New] ([!UICONTROL NEW])</p> </li> 
     <li> <p>[!UICONTROL In Progress] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Closed]/[!UICONTROL Complete] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Opmerking: De [!DNL Jira] statussynchroon met de eerste [!DNL Workfront] status die overeenkomt met de desbetreffende status.</p> <p>Voor meer informatie over de status van items in [!DNL Workfront], zie <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Een status maken of bewerken</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Issue Attachments]</td> 
   <td> [!UICONTROL Issue or Task Documents]<br>Opmerking over het uploaden van een nieuw document in [!DNL Jira] wordt toegevoegd aan de [!UICONTROL Updates] tabblad van het [!DNL Workfront] probleem of taak.  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Due Date]</td> 
   <td> <p> Een opmerking over de wijziging van de [!UICONTROL Due Date] in [!DNL Jira] wordt toegevoegd aan de [!UICONTROL Updates] tabblad van het [!DNL Workfront] probleem of taak. </p> <p>Opmerking: er zijn geen datums gewijzigd op het tabblad [!DNL Workfront] probleem of taak. </p> </td> 
  </tr> 
  <tr> 
   <td> Logtijd in de [!DNL Workfront] of van het [!UICONTROL More] menu op het tabblad [!DNL Jira] kwestie<br></td> 
   <td> <p>Uren<br>Naast het toevoegen van de uren het programma geopend Jira aan verbonden [!DNL Workfront] item, wordt een opmerking over de logtijd toegevoegd aan de [!UICONTROL Updates] tabblad van het [!DNL Workfront] item.</p> <p>Voor meer informatie over het registreren van tijd bij verbonden [!DNL Jira] problemen, waaronder het bijwerken van de [!DNL Jira] gebruiker die zich aanmeldt bij de tijd [!DNL Workfront], zie <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Logtijd voor gekoppelde [!DNL Jira] en [!DNL Workfront] items</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Opmerkingen <br><br></td> 
   <td> <p>Opmerkingen worden toegevoegd aan de [!UICONTROL Updates] tabblad van het [!DNL Workfront] geeft of taakstelt <strong>[!UICONTROL Comments]</strong> in het dialoogvenster [!UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT] van de [!UICONTROL Setup] tab naar <strong>[!UICONTROL Always]</strong>.</p> <p>Voor informatie over het configureren van Workfront-instellingen in [!DNL Jira], zie <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configureren [!DNL Workfront for Jira]</a>.</p> <p>Voor informatie over opmerkingen over gekoppelde items [!DNL Jira] problemen, zie <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Opmerkingen van een gekoppelde [!DNL Jira] kwestie</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Logtijd van gekoppelde [!DNL Jira] kwesties

De tijd die u voor een [!DNL Jira] item in [!DNL Jira] wordt ook overgedragen naar de gekoppelde [!DNL Workfront] item, ongeacht waar [!DNL Jira] u registreert de tijd.\
Wanneer u zich in Jira aanmeldt in het dialoogvenster [!DNL Workfront] wordt de tijd alleen opgenomen in [!DNL Workfront].\
De tijd waarin u opneemt [!DNL Workfront] heeft geen invloed op de tijd van het gekoppelde probleem in [!DNL Jira].

>[!NOTE]
>
>Als de tijd aan een [!DNL Jira] aan een [!DNL Workfront] de [!UICONTROL Hour Type] voor de tijd in [!DNL Workfront] is [!UICONTROL Task Time]. Als de tijd aan een [!DNL Jira] aan een [!DNL Workfront] de [!UICONTROL Hour Type] voor de tijd in [!DNL Workfront] is [!UICONTROL Issue Time].

Er wordt een opmerking toegevoegd aan de **[!DNL Workfront]** tab in [!DNL Jira] en aan de **[!UICONTROL Updates]** tabblad van het item in [!DNL Workfront] om registreren de tijd.\
De tijd wordt ook weergegeven in het dialoogvenster **[!UICONTROL Hours]** tabblad van het [!DNL Workfront] item.

* [Logtijd voor gekoppelde [!DNL Jira] en [!DNL Workfront] items](#log-time-for-linked-jira-and-workfront-items)
* [Logtijd van [!DNL Jira] een [!DNL Workfront] item](#log-time-from-jira-to-a-workfront-item)

### Logtijd voor gekoppelde [!DNL Jira] en [!DNL Workfront] items

U kunt de tijd vanaf een [!DNL Jira] aan een [!DNL Workfront] en de tijd wordt zowel op het [!DNL Jira] en de [!DNL Workfront] item.

>[!IMPORTANT]
>
>Als de gebruiker zich aanmeldt [!DNL Jira] bestaat niet in [!DNL Workfront], maakt de integratie een nieuwe actieve gebruiker in Workfront als de **[!UICONTROL Automatically create a user in [!DNL Workfront]&#x200B;if the [!DNL Jira] user does not have a* [!DNL Workfront]&#x200B;account]** is ingesteld op **[!UICONTROL Always]**. Deze gebruiker neemt geen [!DNL Workfront] licentie. U kunt actieve gebruikers toewijzen aan werkitems in [!DNL Workfront], maar u kunt ze niet opnemen in updates. Voor informatie over het configureren van het automatisch maken van [!DNL Workfront] gebruikers van [!DNL Jira], zie [Configureren [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

Aan logboektijd voor een punt binnen [!DNL Jira] en deze zowel in [!DNL Jira] en [!DNL Workfront]:

1. Aanmelden [!DNL Jira].
1. Ga naar de [!DNL Jira] in verband met de [!DNL Workfront] item.
1. Breid uit **[!UICONTROL More]** menu en klik op **[!UICONTROL Log work]**.

1. In de **[!UICONTROL Time Spent]** , geeft u aan hoeveel tijd u aan deze kwestie hebt besteed. U moet de tijd opgeven met de volgende tijdsperiodes:

   * [!UICONTROL Weeks] b)
   * [!UICONTROL Days] d)
   * [!UICONTROL Hours] h)

1. Voeg informatie aan je tijdgegevens toe, zoals een **[!UICONTROL Work Description]** en klik vervolgens op **[!UICONTROL Log]**.\
   De tijd wordt toegevoegd aan de **[!UICONTROL Work log]** tabblad van het [!DNL Jira] en de [!DNL Workfront] item dat eraan gekoppeld is.\
   De werkbeschrijving van de tijdvermelding wordt opgenomen als een opmerking bij het uur-item in [!DNL Workfront].

### Logtijd van [!DNL Jira] een [!DNL Workfront] item

U kunt de tijd alleen aan de gekoppelde [!DNL Workfront] item van [!DNL Jira] uitgave zonder deze keer op te nemen aan [!DNL Jira] probleem.

1. Aanmelden [!DNL Jira].
1. Navigeren naar een [!DNL Jira] kwestie die verband houdt met een [!DNL Workfront] item.

   De details van de [!DNL Workfront] item moet worden weergegeven in het [!DNL Workfront] in het rechterdeelvenster van de uitgave.

1. Klik op de knop **[!UICONTROL Log Time]** pictogram.

1. Geef de hoeveelheid op van **[!UICONTROL Hours]** en **[!UICONTROL Minutes]** u wilt u voor de kwestie registreren.

1. Klik op **[!UICONTROL Log Time]**.

   De tijd wordt toegevoegd aan de [!DNL Workfront] item.

   Deze tijd wordt niet toegevoegd aan de [!UICONTROL Work Log] tabblad van het [!DNL Jira] probleem.

## Opmerkingen van een gekoppelde [!DNL Jira] kwestie {#comment-from-a-linked-jira-issue}

Wanneer u een opmerking maakt over een [!DNL Jira] item van [!DNL Workfront] rechterdeelvenster in [!DNL Jira]wordt de opmerking ook toegevoegd aan de [!UICONTROL Updates] tabblad van het gekoppelde item in Workfront.

Als u opmerkingen wilt maken van [!DNL Jira] een [!DNL Workfront] item:

1. Aanmelden [!DNL Jira].
1. Navigeren naar een [!DNL Jira] kwestie die verband houdt met een [!DNL Workfront] item.

   De details van de [!DNL Workfront] item moet worden weergegeven in het [!DNL Workfront] in het rechterdeelvenster van de uitgave.

1. Klik op de knop **[!UICONTROL Comments]** in het deelvenster [!DNL Workfront] of op het **[!UICONTROL Comments]** tab.

1. Typ een opmerking en klik vervolgens op **[!UICONTROL Send]**.

   De opmerking wordt toegevoegd aan het volgende:

   * De **[!DNL Workfront]** tabblad van het [!DNL Jira] probleem.
   * De **[!UICONTROL Comments]** tabblad van het [!DNL Jira] probleem.
   * De **[!UICONTROL Updates]** tabblad van het gekoppelde item in Workfront.
