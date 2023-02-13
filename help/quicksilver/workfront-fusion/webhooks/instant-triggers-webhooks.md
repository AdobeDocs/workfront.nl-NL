---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Instant triggers (webhaken) in [!DNL Adobe Workfront Fusion]
description: Veel services bieden websites voor het direct verzenden van meldingen wanneer zich een bepaalde wijziging in de service voordoet. Om deze berichten te verwerken, adviseren wij dat u onmiddellijke trekkers gebruikt. In dit artikel worden het gebruik en de functionaliteit beschreven van instant-triggers in Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: 04191419ab6079cc34576b5a7532cd1596e4b91d
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 0%

---

# Instant triggers (webhaken) in [!DNL Adobe Workfront Fusion]

Veel services bieden websites voor het direct verzenden van meldingen wanneer zich een bepaalde wijziging in de service voordoet. Om deze berichten te verwerken, adviseren wij dat u onmiddellijke trekkers gebruikt. U kunt deze gemakkelijk herkennen in [!DNL Adobe Workfront Fusion] vanwege hun tag:

![](assets/instant-350x256.png)

Als de service geen webhaken biedt, moet u opiniepeilingtriggers gebruiken om de service regelmatig te bekijken.

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] of hoger</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licentie**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## De wachtrij van een webhaak weergeven

Alle berichten van binnenkomende webhooks worden opgeslagen in de wachtrij van de website.

1. Klikken **[!UICONTROL Webhooks]** in het menu links.
1. Zoek de Webhaak waarvoor u de rij wilt bekijken.
1. Klik op de knop met een vrachtwagenpictogram en het aantal ontvangen webhaken.

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >Binnenkomende websitegegevens worden altijd in de wachtrij opgeslagen, ongeacht hoe u de optie hebt ingesteld [!UICONTROL Data] is vertrouwelijk (zie [Het deelvenster met scenario-instellingen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)). Zodra de gegevens in een scenario worden verwerkt, worden ze permanent uit het systeem verwijderd.

## Instant triggers plannen

Als uw scenario een onmiddellijke trekker bevat, kunt u het scenario plannen om onmiddellijk te lopen:

![](assets/schedule-setting-350x185.png)

In dit geval wordt uw scenario onmiddellijk uitgevoerd wanneer [!DNL Workfront Fusion] ontvangt nieuwe gegevens van de dienst. Nadat het scenario wordt uitgevoerd, wordt de totale hoeveelheid webhooks in behandeling die in de wachtrij wachten geteld en voert het scenario net zoveel cycli uit als er webhooks in behandeling zijn, waarbij één webhaak per cyclus wordt verwerkt. Zie voor meer informatie [Uitvoering van scenario&#39;s, cycli en fasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* Een cyclus is niet het zelfde als een scenario looppas. Er kunnen meerdere cycli zijn binnen 1 scenario-uitvoering.
>* Wanneer u een scenario met een onmiddellijke trekker uitvoert die onmiddellijk wordt gepland om te zijn, zijn de volgende uitzonderingen van toepassing:
   >
   >     * Het interval tussen twee uitvoeringen is niet afhankelijk van het minimuminterval volgens het prijsplan.

      >
      >       Als het scenario bijvoorbeeld eenmaal is uitgevoerd, wordt de wachtrij van de webhaak opnieuw gecontroleerd. Als er websites in behandeling zijn, wordt het scenario onmiddellijk opnieuw uitgevoerd en worden alle webhooks in behandeling opnieuw verwerkt.
   >   
   >     * De instelling Maximum aantal cyclusscenario&#39;s wordt genegeerd en ingesteld op 100. Dit betekent dat er maximaal 100 webhaken in behandeling worden verwerkt tijdens één uitvoering van het scenario (met een snelheid van 1 gebeurtenis per cyclus).
>



Als u een andere instelling voor het schema gebruikt dan [!UICONTROL Immediately], wordt het scenario uitgevoerd met de opgegeven intervallen. Aangezien verscheidene webhooks in de rij tijdens het interval kunnen worden verzameld, wordt het geadviseerd om te plaatsen [[!UICONTROL Maximum number of cycles]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) naar een hogere waarde dan standaard 1 om meer webhaken in één scenario uit te voeren:

1. Klik op de knop [!UICONTROL Scenario settings] pictogram ![](assets/gear-icon-settings.png) onder aan uw scenario.
1. In de **[!UICONTROL Scenario settings]** tekstvak dat wordt weergegeven, typt u een getal in het vak **[!UICONTROL Max number of cycles]** om op het aantal websites van de rij te wijzen die u wilt in werking stellen telkens als u het scenario uitvoert.

## Maximumtarieven

De huidige tarieflimiet is 5 webhaken per seconde. Als de limiet wordt overschreden, wordt een 429-statuscode geretourneerd.

## Verlopen van inactieve webhaken

Een webhaak die langer dan 120 uur niet aan een scenario is toegewezen, wordt verwijderd.

## WebHaaklading

[!DNL Workfront Fusion] slaat webshpayloads op voor 30 dagen. Als u meer dan 30 dagen nadat u deze hebt gemaakt toegang krijgt tot een payload van een webhaak, treedt de fout op &quot;[!UICONTROL Failed to read file from storage.]&quot;

## Foutafhandeling

Wanneer er een fout in uw scenario met een onmiddellijke trekker is, het scenario:

* Stopt onmiddellijk - wanneer het scenario wordt geplaatst om te lopen [!UICONTROL Immediately].
* Stopt na 3 mislukte pogingen (3 fouten) - wanneer het scenario wordt geplaatst om zoals gepland te lopen.

Als een fout tijdens de scenariouitvoering voorkomt, wordt webhaak terug geplaatst in de rij tijdens de het terugschroeven van prijzenfase van de instant trekker. In een dergelijke situatie kunt u het scenario oplossen en opnieuw uitvoeren. Zie voor meer informatie [Terugdraaien](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) in het artikel [Uitvoering van scenario&#39;s, cycli en fasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Als er een module van de Reactie van Webhaak in uw scenario is, wordt de fout verzonden naar de reactie Webhaak. De WebHaak reactiemodule wordt altijd als laatste uitgevoerd (in het geval waarin [!UICONTROL Auto commit] (in de Scenario-instellingen is deze optie niet ingeschakeld). Zie voor meer informatie [Reageren op webhaken](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) in het artikel [Webhaken](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Aangepaste webhaken

U kunt uw eigen webhaken maken. Zie voor meer informatie [Webhaken](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webhaak-deactivering

Webhaken worden automatisch gedeactiveerd als een van de volgende twee situaties van toepassing is:

* De webhaak is langer dan 5 dagen niet verbonden met een scenario
* De webhaak wordt alleen gebruikt in inactieve scenario&#39;s, die al meer dan 30 dagen inactief zijn.

gedeactiveerde webhaken worden automatisch verwijderd en niet geregistreerd als ze niet zijn aangesloten op scenario&#39;s en meer dan 30 dagen in de gedeactiveerde status zijn geweest.


