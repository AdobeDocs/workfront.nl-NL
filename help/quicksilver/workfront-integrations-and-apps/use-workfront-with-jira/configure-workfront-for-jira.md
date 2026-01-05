---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Configureren  [!DNL Adobe Workfront for Jira]
description: U kunt  [!DNL Adobe Workfront for Jira]  gebruiken om uw  [!DNL Jira]  en  [!DNL Workfront]  systemen te integreren.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '2292'
ht-degree: 0%

---

# Configureren [!DNL Adobe Workfront for Jira]

<!-- Audited: 12/2023 -->


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

Met [!DNL Adobe Workfront for Jira] kunt u uw [!DNL Jira] - en [!DNL Workfront] -systemen integreren.

Nadat u de invoegtoepassing hebt geïnstalleerd, kunt u workflows definiëren waarmee automatisch [!DNL Jira] -problemen worden gemaakt wanneer [!DNL Workfront] -werkitems worden gemaakt. De items in beide toepassingen worden gekoppeld en sommige van de gegevens worden automatisch bijgewerkt in beide systemen.

Alle gebruikers in [!DNL Workfront] en [!DNL Jira] kunnen van deze integratie profiteren. Ze hebben alleen een licentie nodig voor het systeem waarin ze het meest werken, en niet voor beide systemen.

Deze invoegtoepassing is beschikbaar voor zowel de [!UICONTROL Server] - als de [!UICONTROL OnDemand] -versie (of [!UICONTROL Cloud] -versie) van [!DNL Jira] Software.

Zie [!DNL Jira] [!DNL Workfront for Jira] op de website [[!DNL Workfront for Jira] voor een lijst met &#x200B;](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) versies die [!DNL Atlassian Marketplace] momenteel ondersteunt.

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

## Vereisten

Voordat u [!DNL Workfront for Jira] kunt configureren, moet u:

* Installeer [!DNL Workfront for Jira] .
Voor instructies bij het installeren van [!DNL Workfront for Jira], zie [&#x200B; installeren  [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Configureren [!DNL Workfront for Jira]

Door [!DNL Workfront for Jira] te configureren, kunt u:

* Definieer triggers die [!DNL Jira] -items maken wanneer [!DNL Workfront] -items worden gemaakt.
* Geef op welke velden moeten worden gesynchroniseerd tussen items die zijn gekoppeld tussen [!DNL Jira] en [!DNL Workfront] .

>[!NOTE]
>
>* Nadat u [!DNL Workfront for Jira] hebt geconfigureerd in uw [!DNL Jira] -omgeving, zien alle [!DNL Jira] -gebruikers een [!DNL Workfront] rechterdeelvenster op alle [!DNL Jira] -items. Het deelvenster bevat informatie over de items die kunnen worden gekoppeld vanuit [!DNL Workfront] of geeft op dat er geen [!DNL Workfront] -items zijn gekoppeld aan [!DNL Jira] -items.
>* Wanneer u de [!DNL Jira Server] -installatie gebruikt, wordt alleen het Workfront-deelvenster weergegeven voor de problemen die worden geassocieerd met projecten die zijn geïdentificeerd als triggers voor de Workfront-integratie. Voor meer informatie over vestiging trekkers voor het [!DNL Workfront to Jira] werkschema, zie [&#x200B; trekkers voor het automatisch verbinden van punten tussen  [!DNL Jira]  en  [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront) vormen.
>

Om [!DNL Workfront for Jira] te configureren:

1. Meld u aan bij [!DNL Jira] als [!DNL Jira] -beheerder.
1. Klik op **[!UICONTROL Settings]** in het hoofdmenu [!DNL Jira] .
1. Klik op **[!UICONTROL Add-ons]** en vervolgens op **[!UICONTROL Manage add-ons]** .

1. Vouw de invoegtoepassing **[!DNL Workfront]** uit.
1. Klik op **[!UICONTROL Configure]**.
1. Volg de aanwijzingen om u aan te melden bij [!DNL Workfront] .

   >[!NOTE]
   >
   >De gebruiker moet een geldige `apiKey` in [!UICONTROL Workfront] hebben om een verbinding tot stand te brengen.

   U moet zich aanmelden bij [!DNL Workfront] als [!DNL Workfront] -beheerder om de configuratie voort te zetten.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] maakt verbinding met [!DNL Jira] via OAuth 2.0, een standaard die door de meeste webgebaseerde integraties wordt gebruikt voor de verificatie en autorisatie van gebruikers.
   >* Wanneer u wordt ertoe aangezet om het domein van uw [!DNL Workfront] rekening in te gaan, typ het gebruikend dit formaat: *yourCompany&#39;sDomain.my.workfront.com*. Het domein van uw bedrijf is gewoonlijk de naam van uw bedrijf.
   >* Verbeterde verificatie is pas beschikbaar als een [!DNL Workfront] -beheerder deze heeft ingeschakeld voor deze integratie.

1. Selecteer in Jira het tabblad **[!UICONTROL Triggers]** om het automatisch maken van [!DNL Jira] items te configureren als er nieuwe [!DNL Workfront] -items worden gemaakt.

   Voor meer informatie over vestiging trekkers voor Workfront aan [!DNL Jira] werkschema, zie [&#x200B; trekkers voor automatisch het verbinden van punten tussen  [!DNL Jira]  en  [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront) vormen.

1. Selecteer het tabblad **[!UICONTROL Setup]** om de synchronisatie van velden tussen gekoppelde [!DNL Jira] - en [!DNL Workfront] -items te configureren.

   Voor meer informatie over vestiging de synchronisatie van gebieden tussen [!DNL Jira] en [!DNL Workfront], zie [&#x200B; gebiedssynchronisatie tussen  [!DNL Jira]  en  [!DNL Workfront]  Punten &#x200B;](#configure-field-synchronization-between-jira-and-workfront-items) vormen.

   >[!NOTE]
   >
   >Nadat u de triggers en de synchronisatie van velden tussen de twee toepassingen hebt gedefinieerd, kan elke [!DNL Workfront] -gebruiker die taken of problemen kan maken, mogelijk een item maken in [!DNL Jira] . De gebruiker kan een item maken als de criteria voor het item dat hij of zij maakt, overeenkomen met de triggers in [!DNL Jira] , zelfs als de gebruiker geen [!DNL Jira] -licentie heeft. Bovendien kan elke gebruiker van [!DNL Jira] direct aan het [!DNL Jira] -item beginnen te werken en zijn de updates ervan zichtbaar in [!DNL Workfront] zonder een [!DNL Workfront] -licentie. Alle updates in [!DNL Workfront] zijn ook zichtbaar op de [!DNL Jira] -items.

1. (Optioneel) Selecteer het tabblad **[!UICONTROL Activity Log]** om eventuele fouten te controleren die tijdens de integratie zijn opgetreden.

   Voor meer informatie over [!UICONTROL Activity Log], zie [&#x200B; Mening  [!DNL Jira] [!UICONTROL Activity Log]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## triggers configureren voor het automatisch koppelen van items tussen [!DNL Jira] en [!DNL Workfront]

Als systeembeheerder van [!DNL Jira] kunt u triggers definiëren die automatisch problemen veroorzaken in [!DNL Jira] wanneer een item in [!DNL Workfront] aan bepaalde criteria voldoet.

>[!NOTE]
>
>Het kan tot 10 minuten duren voordat de integratie nieuwe problemen oplevert in [!DNL Jira] .

Houd rekening met het volgende wanneer u het maken van [!DNL Jira] -items activeert terwijl [!DNL Workfront] -items worden gemaakt:

* De integratie verloopt in één richting: u kunt alleen items die u maakt in [!DNL Workfront], activeren en automatisch maken in [!DNL Jira] . U kunt items die u maakt in [!DNL Jira] niet automatisch laten activeren in [!DNL Workfront] .
* Er is geen limiet voor het aantal triggers dat u kunt gebruiken.
* Als een item dat u maakt in [!DNL Workfront] overeenkomt met meerdere triggers, wordt er slechts één item gemaakt in [!DNL Jira] . Het item wordt gemaakt in [!DNL Jira] op basis van de eerste trigger (in de volgorde waarin deze zijn gedefinieerd in [!DNL Jira] ). Alle andere triggers worden genegeerd.
* Er kan slechts één item in [!DNL Workfront] worden gekoppeld aan één item in Jira. U kunt één [!DNL Workfront] -item nooit koppelen aan meerdere [!DNL Jira] -problemen of één [!DNL Jira] -uitgave aan meerdere [!DNL Workfront] -items.

triggers configureren voor het automatisch maken van items in [!DNL Jira] :

1. Meld u aan bij [!DNL Jira] als systeembeheerder.
1. Klik op **[!UICONTROL Settings]** in het hoofdmenu [!DNL Jira] .
1. Klik op **[!UICONTROL Add-ons]** en vervolgens op **[!UICONTROL Manage add-ons]** .
1. Vouw de invoegtoepassing **[!DNL Workfront]** uit.
1. Klik op **[!UICONTROL Configure]**.
1. Meld u aan bij [!DNL Workfront] als systeembeheerder.

   Het tabblad **[!UICONTROL Triggers]** is standaard geselecteerd in Jira.

1. Klik op **[!UICONTROL Add trigger]** om een nieuwe trigger toe te voegen.
1. Geef in het veld **[!UICONTROL Workfront team/user/role]** de naam van een [!DNL Workfront] -team, -gebruiker of -taakrol op en klik om deze te selecteren wanneer deze in de lijst wordt weergegeven.

   >[!NOTE]
   >
   >U kunt geen veelvoudige trekkers voor het zelfde team, de gebruiker, of de rol hebben.

   Wanneer iemand een taak of een uitgave maakt en deze aan een van deze entiteiten toewijst, wordt automatisch een uitgave gemaakt in [!DNL [!DNL Jira]].

1. Typ in het veld **[!UICONTROL [!DNL Jira] project]** de naam van een [!DNL Jira] -project en klik om het te selecteren wanneer het in de lijst wordt weergegeven.

   Wanneer de [!DNL Jira] -uitgave wordt gemaakt, wordt deze geplaatst in het project dat u hier hebt gekozen.

1. Selecteer een **I[!UICONTROL ssue type]** van het drop-down menu.

   Dit geeft het type uitgave aan dat wordt gemaakt in [!DNL Jira] wanneer aan de voorwaarden van deze trigger wordt voldaan, op basis van uw instellingen voor dat specifieke project in [!DNL Jira] .

1. Klik op **[!UICONTROL Save]**.

   Met deze configuratie wordt telkens wanneer een [!DNL Workfront] -gebruiker een item maakt dat overeenkomt met de opgegeven triggers, een nieuwe uitgave gemaakt in [!DNL Jira] .

## Veldsynchronisatie configureren tussen [!DNL Jira] en [!DNL Workfront] Items

Als beheerder [!DNL Jira] kunt u bepalen welke velden automatisch moeten worden gesynchroniseerd voor items die zijn gekoppeld tussen [!DNL Workfront] en Jira. Bepaalde velden kunnen worden gesynchroniseerd van het item [!DNL Workfront] naar het item [!DNL Jira] en andere velden kunnen worden gesynchroniseerd van Jira naar Workfront.

Om te bepalen welke gebieden automatisch op punten zouden moeten synchroniseren die tussen de twee toepassingen worden verbonden:

1. Meld u aan bij [!DNL Jira] als Jira-beheerder.
1. Klik op **[!UICONTROL Settings]** in het hoofdmenu [!DNL Jira] .
1. Klik op **[!UICONTROL Add-ons]** en vervolgens op **[!UICONTROL Manage add-ons]** .
1. Vouw de invoegtoepassing **[!DNL Workfront]** uit.
1. Klik op **[!UICONTROL Configure]**.
1. Meld u aan bij [!DNL Workfront] als Workfront-beheerder.
1. Klik in Jira op de tab **[!UICONTROL Setup]** .
1. Selecteer in de sectie **[!UICONTROL Synchronize from Workfront to Jira]** de velden die u wilt bijwerken in [!DNL Jira] wanneer deze worden bijgewerkt in Workfront.

   1. Selecteer een van de volgende frequenties waarmee de velden worden gesynchroniseerd:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL On Creation]</td>
              <td>De velden die u opgeeft, worden gesynchroniseerd tussen de gekoppelde Workfront- en [!DNL Jira] -items wanneer het item in Workfront wordt gemaakt.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>De velden die u opgeeft, worden gesynchroniseerd tussen de gekoppelde Workfront- en [!DNL Jira]-items wanneer de velden worden bijgewerkt in Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Never]</td>
              <td>De velden die u opgeeft, worden nooit gesynchroniseerd tussen de gekoppelde [!DNL Workfront] - en [!DNL Jira] -items. Er zijn geen aanwijzingen in [!DNL Jira] dat het veld is bijgewerkt in [!DNL Workfront] . </td>
          </tr>
      </table>

   1. Selecteer een van de volgende opties om de velden van [!DNL Workfront] tot en met [!DNL Jira] te synchroniseren:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>De naam van een taak of een uitgave in [!DNL Workfront] wordt de naam van de uitgave waaraan deze is gekoppeld in [!DNL Jira] .</p><p>Opmerking: wanneer nieuwe items automatisch in [!DNL Jira] worden gemaakt, wordt de [!DNL Workfront] naam altijd bijgewerkt op het [!DNL Jira] -item, ongeacht of dit veld hier is ingeschakeld of niet. Wanneer een [!DNL Jira] punt manueel met een [!DNL Workfront] punt wordt verbonden, werkt de Naam van het [!DNL Workfront] punt slechts in [!DNL Jira] bij wanneer u aan <strong> selecteert altijd </strong> dit gebied synchroniseert. Voor meer informatie over het verbinden van punten manueel of automatisch, zie <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref"> punten tussen [!DNL Adobe Workfront] en [!DNL Jira]</a> verbinden.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Description]</td>
         <td>De beschrijving van een taak of een probleem in [!DNL Workfront] wordt de beschrijving van de uitgave waaraan deze is gekoppeld in [!DNL Jira] .</td>
        </tr>
        <tr>
         <td role="rowheader">Documenten</td>
         <td><p>Documenten die zijn gekoppeld aan een taak of een uitgave in [!DNL Workfront] , worden ook gekoppeld aan de uitgave waaraan deze is gekoppeld in Jira. De nieuwe documentversies van [!DNL Workfront] worden toegevoegd als afzonderlijke documenten aan Jira en met <i> _v&lt;version number&gt; </i> toegevoegd om op de genummerde versie in Workfront te wijzen. </p><p>Bijvoorbeeld, als de naam van een document in [!DNL Workfront] <strong> HoofdAdvertentie </strong> is, en u een nieuwe versie aan het binnen [!DNL Workfront] toevoegt, wordt de nieuwe versie overgebracht naar [!DNL Jira] als nieuw document met de naam <strong> HoofdAd_v2 </strong>.</p><p>Belangrijk: <p>Houd rekening met het volgende wanneer u documenten synchroniseert:</p>
           <ul>
            <li><p>Documenten groter dan 5 MB worden niet gesynchroniseerd. Als een documentsynchronisatie mislukt omdat het document te groot is, wordt een fout in het activiteitenlogboek geregistreerd. </p><p>Voor meer informatie over het activiteitenlogboek, zie <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref"> Mening het Logboek van de Activiteit van Jira </a>.</p></li>
            <li><p>Documenten die zijn gekoppeld aan taken en uitgaven van externe servers worden niet overgebracht naar de [!DNL Jira] -items. Alleen documenten die rechtstreeks op de taak of de uitgave in [!DNL Workfront] zijn geüpload, worden overgebracht naar de gekoppelde uitgave in [!DNL Jira] .</p></li>
            <li><p>Als u een proefdruk wilt maken op basis van een document, moet u de proefdruk genereren in [!DNL Workfront] . </p><p>Voor meer informatie bij het produceren van een proef, zie <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref"> een proef voor een bestaand document </a> in <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref"> creëren een proef voor een document </a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Planned Completion Date]</td>
         <td><p>De [!UICONTROL Planned Completion Date] van een taak of een uitgave in [!DNL Workfront] wordt de [!UICONTROL Due Date] van de uitgave waaraan deze is gekoppeld in [!DNL Jira] .</p><p>Opmerking: zorg ervoor dat u <strong>[!UICONTROL Due Date]</strong> bij [!DNL Jira] -problemen weergeeft, zodat deze waarde wordt gesynchroniseerd.</p></td>
        </tr>
       </tbody>
      </table>

1. Selecteer in de sectie **[!UICONTROL Synchronize from [!DNL Jira] to [!DNL Workfront]]** de velden die u wilt bijwerken in [!DNL Workfront] wanneer deze worden bijgewerkt in [!DNL Jira] .

   1. Selecteer een van de volgende frequenties waarmee de velden worden gesynchroniseerd:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>De velden die u opgeeft, worden altijd gesynchroniseerd tussen de gekoppelde [!DNL Workfront] - en [!DNL Jira] -items wanneer de velden worden bijgewerkt in [!DNL Jira] . </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Never]</td>
         <td><p>De velden die u opgeeft, worden nooit gesynchroniseerd tussen de gekoppelde [!DNL Workfront] - en [!DNL Jira] -items. Er zijn geen aanwijzingen in [!DNL Workfront] dat het veld is bijgewerkt in [!DNL Jira] . </p><p>Opmerking: als u Nooit selecteert, kunnen [!DNL Workfront] -velden nog steeds handmatig worden bijgewerkt vanuit [!DNL Jira] in het linkerdeelvenster [!DNL Workfront] van het [!DNL Jira] -probleem. Deze updates worden alleen weergegeven voor [!DNL Workfront] items in [!DNL Jira] en [!DNL Workfront] en niet voor [!DNL Jira] -items.</p></td>
        </tr>
       </tbody>
      </table>

   1. Selecteer deze optie om de volgende velden van [!DNL Jira] tot en met [!DNL Workfront] te synchroniseren:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>De [!UICONTROL Status] van een uitgave in [!DNL Jira] wordt de [!UICONTROL Status] van de taak of uitgave waaraan deze is gekoppeld in [!DNL Workfront] .<br> voor meer informatie over [!DNL Workfront] statussen, zie <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref"> een status </a> creëren of uitgeven.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Assignee]</td>
         <td><p>De [!UICONTROL Assignee] van een uitgave in [!DNL Jira] wordt de [!UICONTROL Assignee] van de taak of uitgave waaraan deze is gekoppeld in [!DNL Workfront] .</p><p>Belangrijk: Wanneer u een punt in [!DNL Jira] aan een gebruiker toewijst die geen [!DNL Workfront] rekening heeft, leidt de integratie tot een nieuwe actieve gebruiker in [!DNL Workfront] slechts wanneer <strong> automatisch tot een gebruiker in [!DNL Workfront] leidt als de [!DNL Jira] gebruiker geen [!DNL Workfront] rekening </strong> aan <strong>[!UICONTROL Always]</strong> heeft. Deze gebruiker neemt geen [!DNL Workfront] -licentie in. Actieve gebruikers kunnen worden toegewezen aan tijdelijke items in [!DNL Workfront] , maar ze kunnen niet worden opgenomen in updates. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Attachments]</td>
         <td>Bijlagen van een probleem in [!DNL Jira] worden ook toegevoegd aan de taak of het probleem waaraan het is gekoppeld in [!DNL Workfront] . </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comments]</td>
         <td><p>Een opmerking over een [!DNL Jira] -uitgave wordt ook gepost op het gekoppelde [!DNL Workfront] -item in het [!UICONTROL Updates] -gebied. Een opmerking die in het [!UICONTROL Updates] -gebied is geplaatst voor een [!DNL Workfront] taak of Issues syncs naar de native commentaarstream van [!DNL Jira] voor de gekoppelde uitgave. </p><p>Deze is standaard ingesteld op <strong>[!UICONTROL Always]</strong> . Als u <strong>[!UICONTROL Never]</strong> hier selecteert, kunt u nog steeds handmatig opmerkingen op een gekoppeld item posten in [!DNL Workfront] of in [!DNL Jira] .</p></td>
        </tr>
       </tbody>
      </table>

1. Selecteer in de sectie **[!UICONTROL OTHER]** welke extra velden moeten worden bijgewerkt tussen gekoppelde items.

   1. Selecteer een optie om te bepalen of de velden die u opgeeft **[!UICONTROL Always]** of **[!UICONTROL Never]** bijwerken in [!DNL Jira] of [!DNL Workfront] wanneer ze worden gewijzigd.

   1. Selecteer een van de volgende velden en updates:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Aangepaste gegevens in het rechterdeelvenster in [!DNL Jira]]</td>
         <td><p>Hiermee geeft u de [!DNL Workfront] aangepaste gegevens van een item weer in het deelvenster [!DNL Workfront] rechts.</p><p>Opmerking: secties Aangepaste formulieren worden weergegeven in het rechterdeelvenster van [!DNL Workfront] en hebben toegang tot het toegangsniveau van de [!DNL Workfront] System Administrator.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Prioriteit in het rechterdeelvenster in [!DNL Jira]]</td>
         <td>Geeft de [!DNL Workfront] Prioriteit van een item weer in het deelvenster [!DNL Workfront] rechts.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Add an update in the [!DNL Workfront] Tabblad Updates over wijzigingen in Vervaldatum in [!DNL Jira]]</td>
         <td>Voegt een opmerking toe op het tabblad [!UICONTROL Update] van het [!DNL Workfront] -item wanneer de [!UICONTROL Due Date] verandert in een gekoppeld [!DNL Jira] -item.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Automatically create a user in [!DNL Workfront] als de [!DNL Jira] -gebruiker geen [!DNL Workfront] -account heeft]</td>
         <td><p>De volgende scenario's bestaan:</p>
          <ul>
           <li>Wanneer u <strong>[!UICONTROL Always]</strong> selecteert, schakelt u de integratie in om een nieuwe Workfront-gebruiker te maken telkens wanneer een [!DNL Jira] gebruiker zonder een [!DNL Workfront] -account de volgende handelingen uitvoert op een gekoppelde [!DNL Jira] -uitgave:
            <ul>
             <li>Wordt toegewezen aan een [!DNL Jira] -uitgave</li>
             <li><p>Hiermee wordt tijd geregistreerd voor een [!DNL Jira] -probleem</p><p>Deze nieuwe gebruiker neemt geen [!DNL Workfront] -licentie in. De standaardinstelling is Altijd. Aan de naam van de gebruiker die op deze manier in [!DNL Workfront] is gemaakt, is "[!UICONTROL Jira]" toegevoegd.</p></li>
            </ul></li>
           <li>Wanneer u <strong>[!UICONTROL Never]</strong> selecteert, gebeuren de volgende dingen:
            <ul>
             <li>U kunt geen [!DNL Jira] toewijzingen zien voor de [!DNL Workfront] -items. In dit geval worden alleen toewijzingen die in [!DNL Workfront] zijn gemaakt, weergegeven op de [!DNL Workfront] -items.</li>
             <li>De tijd die door een gebruiker zonder een [!DNL Jira] -account is aangemeld bij een gekoppelde [!DNL Workfront] -uitgave, wordt niet automatisch overgedragen naar het gekoppelde [!DNL Workfront] -item. U kunt de tijd nog steeds vastleggen op het [!DNL Workfront] -item in het rechterdeelvenster van het [!DNL Jira] -probleem.</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Klik op **[!UICONTROL Save]**.

   Nu, telkens wanneer een gebruiker om het even welke gebieden bijwerkt die in deze configuratie op een punt in of [!DNL Jira] of [!DNL Workfront] worden gespecificeerd, wordt het verbonden punt in de andere toepassing ook bijgewerkt.

## Problemen oplossen

### Items kunnen niet in [!DNL Jira] worden gemaakt vanwege triggervelden gemarkeerd als &quot; [!UICONTROL Couldn't be found]&quot;

#### Probleem

Wanneer een fout optreedt met de [!DNL Workfront for Jira] -toepassing, schakelt [!DNL Workfront] de triggers uit om verdere complicaties te voorkomen. Wanneer die trekkers gehandicapt zijn, tonen zij als &quot;[!UICONTROL Couldn't be found]&quot;.

#### Oplossing

Zoek de fout die de triggers heeft uitgeschakeld. U kunt de fout vinden in [!DNL Workfront for Jira] [!UICONTROL Activity Log] .

De gemeenschappelijkste oorzaak van dit gedrag is de fout &quot;[!UICONTROL Field 'duedate' cannot be set. It is not on the appropriate screen, or unknown.]&quot;

Deze fout houdt in dat u [!UICONTROL Planned Completion Date] van [!DNL Workfront] tot [!DNL Jira] probeert te synchroniseren. Hiervoor moet u ervoor zorgen dat uw [!DNL Jira] -objecten een veld hebben met de naam &quot;[!UICONTROL Due Date]&quot;. Als ze dit veld niet hebben, kan [!DNL Workfront] de geplande afsluitdatum niet synchroniseren vanaf [!DNL Workfront] en worden de triggers uitgeschakeld.

Voer een van de volgende handelingen uit om deze fout op te lossen:

* Vraag de [!DNL Jira] -beheerder om de betrokken [!DNL Jira] -objecten bij te werken om er zeker van te zijn dat ze een datumveld hebben dat is ingesteld op de datum waarop ze zijn toegepast.
* Schakel de synchronisatie uit van de geplande afsluitdatum van [!DNL Workfront] op de Workfront [!UICONTROL Setup] -pagina.
