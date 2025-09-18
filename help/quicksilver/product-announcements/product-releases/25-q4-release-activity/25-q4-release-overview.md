---
title: Overzicht release 4de kwartaal 2025
description: Deze pagina biedt informatie over functionaliteit die is opgenomen in de release van het vierde kwartaal van 2025. Deze verbeteringen zullen naar verwachting in het hele kwartaal beschikbaar komen in de productieomgeving.
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 298473d4-7d7d-4401-80bf-899a01f570a6
source-git-commit: 30e5358549291e5d04d42ab470dccd444521ecb8
workflow-type: tm+mt
source-wordcount: '2073'
ht-degree: 2%

---

# Overzicht release 4de kwartaal 2025

Deze pagina biedt informatie over functionaliteit die is opgenomen in de release van het vierde kwartaal van 2025 die gepland is voor oktober 2025.

De verbeteringen op deze pagina zijn beschikbaar in de voorvertoningsomgeving. Deze pagina wordt bijgewerkt met aanvullende verbeteringen omdat de release van het vierde kwartaal van 2025 de geplande productie nadert.


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>Voorzien wordt dat maandelijkse en driemaandelijkse versies beschikbaar zullen zijn op de donderdag van de tweede volledige week van de maand, tenzij anders vermeld.
>
>| Maandelijkse release | Driemaandelijkse release |
>|----|----|
>| <ul><li>25.8 (14 augustus 2025)</li><li>25.9 (11 september 2025)</li><li>25.10 (16 oktober 2025)</li></ul> | <ul><li>25.10 (16 oktober 2025)</li></ul> |
>
>Merk op dat voor de definitieve versie van elk kwartaal (25.10 dit kwartaal), gebruikers op het snelle versieschema één dag vroeg (15 oktober 2025) de versie zullen ontvangen.
>
>Voor meer informatie over het snelle versieproces, zie [ toelaten of onbruikbaar maken het snelle versieproces ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Verbeteringen voor Adobe Workfront

* [Beheerdersverbeteringen](#administrator-enhancements)
* [Verbeteringen voor dashboards](#dashboards)
* [Verbeteringen voor document en proefdrukken](#document-and-proofing-enhancements)
* [Verbeteringen voor startpagina](#home-enhancements)
* [Projectverbeteringen](#project-enhancements)
* [Verbeteringen voor beheer van bronnen](#resource-management-enhancements)
* [Verbeteringen aan verzoeken](#requests-enhancements)
* [Andere verbeteringen](#other-enhancements)

### Beheerdersverbeteringen

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong> Eigenschap </strong>
        </td>
        <td><strong>Voorvertoning</strong></td>
        <td><strong>Snelle release</strong></td>
        <td><strong>Driemaandelijks</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> Nieuwe Borden Admin Mening </a><p></p>
            <p>De mening van Admin van Boards bevat een lijst van elke Raad in uw rekening die de Beheerders van het Systeem kunnen gebruiken om een snelle momentopname van de algemene details van Boards te krijgen, met inbegrip van toen zij het laatst werden bijgewerkt, hoeveel kaarten elk heeft, en meer.</p>
        </td>
        <td>vrijdag 11 september 2025</td>
        <td>donderdag 15 oktober 2025</td>
        <td>vrijdag 16 oktober 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> laat de eigenschappen van AI Beta voor uw organisatie </a> toe<p></p>
            <p>Om het voor u gemakkelijker te maken om aanstaande AI eigenschappen te zien en te beïnvloeden, hebben wij het voor u mogelijk gemaakt om Betas voor die eigenschappen voor uw organisatie toe te laten. Nu kunt u een of meer van de momenteel beschikbare AI Beta-functies inschakelen in de Systeemvoorkeuren.</p>
        </td>
        <td>vrijdag 28 augustus 2025</td>
        <td>vrijdag 11 september 2025</td>
        <td>vrijdag 16 oktober 2025</td>
    </tr>     
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> Updates aan het gebruikersprofiel van Workfront </a><p>[!BADGE Off schema]{type=Neutral}</p>
            <p>We hebben het uiterlijk van het Workfront-gebruikersprofiel bijgewerkt naar een modern ontwerp dat aansluit bij andere delen van Workfront. Deze updates zijn van toepassing op zowel een beheerder die één profiel bewerkt, als een gebruiker die meerdere profielen bewerkt of op een gebruiker die zijn of haar eigen profiel bewerkt.</p>
            <p>Er zijn enkele kleine functieverschillen ten opzichte van het huidige gebruikersprofiel, zoals:</p>
            <ul>
                <li>Sommige selectievakjes (zoals de gebruiker als actief markeren) zijn veranderd in schakelknoppen of knoppen.</li>
                <li>De optie 'Werk verzenden dat ik aan mezelf toewijs naar mijn tabblad Werken op' onder Voorkeuren is verwijderd, omdat deze naar een vervangen functie verwijst.</li>
            </ul>
        </td>
        <td>vrijdag 28 augustus 2025</td>
        <td>Geleidelijke uitrol vanaf 18 september 2025</td>
        <td>Geleidelijke uitrol vanaf 18 september 2025</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> voeg veelvoudige waardeopties van externe API aan een douanevorm toe </a><p></p>
            <p>Een nieuw veldtype, Multi-select externe zoekopdracht, is nu beschikbaar in de aangepaste formulierontwerper. Wanneer u gegevens op een extern systeem hebt opgeslagen, kunt u met dit veldtype opties laden vanuit een externe API en filteren op basis van andere veldwaarden in het aangepaste formulier. Dit is het zelfde als enig-uitgezochte externe raadpleging.</p>
            <p>Wanneer het formulier aan een object wordt toegevoegd, worden de waarden die door de API worden geretourneerd, weergegeven in een vervolgkeuzelijst en kan de gebruiker meerdere waarden selecteren.</p>
        </td>
        <td>vrijdag 31 juli 2025</td>
        <td>vrijdag 14 augustus 2025</td>
        <td>vrijdag 16 oktober 2025</td>
    </tr>     
  </tbody>
</table>

### Verbeteringen voor dashboards

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong> Eigenschap </strong>
        </td>
        <td><strong>Voorvertoning</strong></td>
        <td><strong>Snelle release</strong></td>
        <td><strong>Driemaandelijks</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-dashboards.md" class="MCXref xref" xrefformat="{para}"> Nieuwe Dashboards van het Canvas open bèta </a>
            <p>Met de nieuwe functie Canvasdashboards kunt u uw Adobe Workfront-gegevens gemakkelijk visualiseren door rapporttypen toe te voegen aan een canvas met veel flexibele layoutopties, zoals vergroten, verkleinen, slepen en neerzetten, en nog veel meer.</p>
        </td>
        <td>woensdag 26 augustus 2025</td>
        <td>woensdag 26 augustus 2025</td>
        <td>woensdag 26 augustus 2025</td>
    </tr> 
</table>

### Verbeteringen voor document en proefdrukken

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong> Eigenschap </strong>
        </td>
        <td><strong>Voorvertoning</strong></td>
        <td><strong>Snelle release</strong></td>
        <td><strong>Driemaandelijks</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-document-and-proof.md" class="MCXref xref" xrefformat="{para}"> verenigde goedkeuringen Geleidelijke Uitvoer </a><p>[!BADGE Off schema]{type=Neutral}</p>
            <p>Wij toelaten Verenigde Goedkeuringen, die vroeger als Nieuwe Goedkeuringen van het Document, in een gefaseerde uitrol worden bekend. Deze functionaliteit wordt de komende zes maanden automatisch ingeschakeld in uw Workfront-exemplaar.</p>
            <p>De verenigde goedkeuringen vervangen de goedkeuringen van het document van de Oudheid en verstrekken de nieuwe functionaliteit. 
</p>
        </td>
        <td>Geleidelijke uitrol vanaf 17 juli 2025</td>
        <td>Geleidelijke uitrol vanaf 17 juli 2025</td>
        <td>Geleidelijke uitrol vanaf 17 juli 2025</td>
    </tr> 
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-document-and-proof.md" class="MCXref xref" xrefformat="{para}"> Nieuwe Workfront AI Reviewer </a><p></p>
            <p>Opmerking: deze functie bevindt zich momenteel in bèta.</p>
            <p>De nieuwe Workfront AI Reviewer helpt de naleving van het merk van afbeeldingen te garanderen door de inhoud automatisch te controleren aan de hand van de richtlijnen voor uw merk, te beginnen met de richtlijnen voor afbeeldingen. Het verstrekt een score en actiefable terugkoppelen om het goedkeuringsproces te stroomlijnen. </p>
            <p>U kunt de AI Reviewer toevoegen aan goedkeuringssjablonen of individuele revisie- en goedkeuringsaanvragen, waardoor de productie van inhoud sneller verloopt en de merkstandaarden behouden blijven.</p>
        </td>
        <td>vrijdag 14 augustus 2025</td>
        <td>vrijdag 14 augustus 2025</td>
        <td>vrijdag 14 augustus 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-document-and-proof.md" class="MCXref xref" xrefformat="{para}"> Nieuwe het proef integratie voor Adobe Express </a><p></p>
            <p>We zijn blij dat we een nieuwe integratie tussen Adobe Express en Workfront Proof aankondigen.</p>
            <ul>
            <li>De samenwerking tussen creatieve, wettelijke, en nalevingsteams stroomlijnen om tijd te verminderen te publiceren terwijl het handhaven van toezicht</li>
            <li>Diepgaande revisies uitvoeren met markeringen voor tekeningen, annotaties en opmerkingen maken met de Workfront-proefdrukviewer</li>
            <li>Voldoen aan standaarden voor naleving door bedrijven met elektronische handtekeningen en volledige auditlogboeken</li>
            <li>Goedkeuring vereisen voor opnieuw gemengde bestanden van een Express-sjabloon</li>
            <li>Een Express-sjabloon toewijzen aan een revisie- en goedkeuringswerkstroom met meerdere stadia aan de hand van geavanceerde proefdruksjablonen</li>
            </ul>
        </td>
        <td>dinsdag 28 juli 2025</td>
        <td>dinsdag 28 juli 2025</td>
        <td>dinsdag 28 juli 2025</td>
    </tr>     
  </tbody>
</table>

### Verbeteringen voor startpagina

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong> Eigenschap </strong>
        </td>
        <td><strong>Voorvertoning</strong></td>
        <td><strong>Snelle release</strong></td>
        <td><strong>Driemaandelijks</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-home.md" class="MCXref xref" xrefformat="{para}"> Updates aan Mijn widget van Verzoeken in Huis </a><p></p>
            <p>Voor een naadloze ervaring tussen Workfront en Workfront Planning hebben we de widget Mijn verzoeken in Home opnieuw ontworpen. De nieuwe widget heeft de volgende wijzigingen:
            <ul>
                <li>Verbeterde indeling en organisatie van aanvraaggegevens</li>
                <li>Verbeterde filteropties en sorteeropties</li>
                <li>Integratie met Workfront-planning voor betere zichtbaarheid bij de toewijzing van bronnen</li>
            </ul>
            </p>
            <p>De nieuwe widget Mijn verzoeken geeft alleen die verzoeken weer die zijn gemaakt in de nieuwe ervaring die u opvraagt.</p>
        </td>
        <td>vrijdag 21 augustus 2025</td>
        <td>vrijdag 11 september 2025</td>
        <td>vrijdag 16 oktober 2025</td>
    </tr>     
  </tbody>
</table>

### Projectverbeteringen

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong> Eigenschap </strong>
        </td>
        <td><strong>Voorvertoning</strong></td>
        <td><strong>Snelle release</strong></td>
        <td><strong>Driemaandelijks</strong></td>
    </tr>
      <!--<tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}">Create project intake forms in Workfront</a>
            <p>To make it easier to create requested projects without converting from issues, we've created Project intake forms. You can configure these intake forms with specific fields, templates, and custom forms, and set approvers for project creation. Then, when a user uses this form, the project is configured to your specifications and sent for approval.</p>
        </td>
        <td>August 21, 2025</td>
        <td>September 11, 2025</td>
        <td>October 16, 2025</td>
    </tr> -->
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}"> Nieuwe bèta van de Gezondheid van het Project </a>
            <p>De nieuwe functie Projectgezondheid gebruikt de kracht van AI Assistant om u direct een beoordeling te geven van hoe uw projecten presteren en welke gebieden uw aandacht behoeven.</p>
            <p>De Medewerker van AI kan een beoordeling van de Gezondheid van het Project voor een project, een programma, en veelvoudige projecten produceren.</p>
        </td>
        <td>vrijdag 11 september 2025</td>
        <td>vrijdag 11 september 2025</td>
        <td>vrijdag 11 september 2025</td>
    </tr> 
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}"> Nieuwe uitdrukkingen die aan de formules- gebieden in de Planning en berekende douanegebieden in Workfront worden toegevoegd </a><p><p>[!BADGE Off schema]{type=Neutral}</p></p>
            <p>We hebben nieuwe expressies toegevoegd met het volgende gebruik voor formuleringsvelden in Workfront Planning en voor berekende aangepaste velden in Workfront:</p>
            <ul>
            <li>REMOVEACCENTS(tekenreeks): verwijdert diakritische tekens uit alle tekens met accent in de invoertekenreeks.</li>
            <li>REPLACEPATTERN (tekenreeks, patroon, vervangende tekenreeks): vervangt de overeenkomende waarden van het opgegeven patroon door de vervangende tekenreeks.</li>
            <li>PASCAL(string): Zet de invoertekenreeks om in PascalCase door de eerste letter van elk woord met hoofdletters te beschrijven en alle spaties te verwijderen.</li>
            </ul>
        </td>
        <td>vrijdag 7 augustus 2025</td>
        <td>vrijdag 7 augustus 2025</td>
        <td>vrijdag 7 augustus 2025</td>
    </tr> 
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-project.md" class="MCXref xref" xrefformat="{para}"> extra manier om tot Geavanceerde Toewijzingen van lijsten </a> toegang te hebben<p></p>
            <p>Een <b> Geavanceerde </b> knoop is nu beschikbaar voor taken in lijsten, die het voor u sneller maken om tot de Geavanceerde pagina van Toewijzingen toegang te hebben. Het <b> pictogram van Mensen </b> om aan Geavanceerde Taken te krijgen is ook beschikbaar op taken in lijsten.</p>
        </td>
        <td>vrijdag 7 augustus 2025</td>
        <td>vrijdag 11 september 2025</td>
        <td>vrijdag 16 oktober 2025</td>
    </tr> 
  </tbody>
  </table>

### Verbeteringen voor beheer van bronnen

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong> Eigenschap </strong>
        </td>
        <td><strong>Voorvertoning</strong></td>
        <td><strong>Snelle release</strong></td>
        <td><strong>Driemaandelijks</strong></td>
    </tr>
  <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-resource-mgmt.md" class="MCXref xref" xrefformat="{para}"> de Balancer van de Werkbelasting is nu beschikbaar op uw gebruikersprofiel </a><p></p>
            <p>Alle gebruikers kunnen nu hun eigen vraag- en capaciteitsgegevens in de werklastbalans bekijken vanuit hun profiel, ongeacht hun toegangsniveau. Wanneer u uw Workfront-gebruikersprofiel opent, wordt de werklastverdeling weergegeven in het navigatievenster aan de linkerkant.</p>
            <p>Werklastverdelingsgegevens voor een gebruiker zijn alleen-lezen. U kunt geen werk toewijzen, werk ongedaan maken of toewijzingen op gebruikersniveau aanpassen.</p>
        </td>
        <td>vrijdag 31 juli 2025</td>
        <td>vrijdag 14 augustus 2025</td>
        <td>vrijdag 16 oktober 2025</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-resource-mgmt.md" class="MCXref xref" xrefformat="{para}"> De taken van de Rol tonen in de Balancer van de Werkbelasting </a><p></p>
            <p>Bronmanagers kunnen nu taakrolltoewijzingen in Workload Balancer controleren. De taken worden getoond in het Unassigned gebied van het Werk, onder de taken of kwesties de rollen worden toegewezen aan. Alleen werkitems die aan gebruikers zijn toegewezen, worden weergegeven in het gebied Toegewezen werk. </p>
            <p>Een nieuwe instelling voor werklastverdeling, Roltoewijzingen weergeven, bepaalt of roltoewijzingen worden weergegeven. De instelling is standaard ingeschakeld.</p>
        </td>
        <td>vrijdag 31 juli 2025</td>
        <td>vrijdag 14 augustus 2025</td>
        <td>vrijdag 16 oktober 2025</td>
    </tr>     
  </tbody>
</table>

### Verbeteringen aan verzoeken

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong> Eigenschap </strong>
        </td>
        <td><strong>Voorvertoning</strong></td>
        <td><strong>Snelle release</strong></td>
        <td><strong>Driemaandelijks</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-requests.md" class="MCXref xref" xrefformat="{para}"> Nieuwe gecombineerde kolom van de Status in verenigde lijst van het Verzoek </a><p></p>
            <p>Om de verenigde verzoekervaring te vereenvoudigen, toont de kolom van de Status nu zowel de Status van het Verzoek als Status van de Goedkeuring, welke op een bepaald verzoek van toepassing is.</p>
        </td>
        <td>vrijdag 28 augustus 2025</td>
        <td>vrijdag 11 september 2025</td>
        <td>vrijdag 16 oktober 2025</td>
    </tr>     
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-requests.md" class="MCXref xref" xrefformat="{para}"> Updates om ervaring te verzoeken </a><p></p>
            <p>Om een betere gebruikerservaring te creëren wanneer het doen van verzoeken in de Planning van Workfront en Workfront, hebben wij de het vragen ervaring bijgewerkt. Nu kunt u:
            <ul>
                <li>Bekijk Workfront- en Workfront-planningsverzoeken in één lijst.</li>
                <li>Verzonden aanvragen filteren op basis van criteria die u opgeeft.</li>
                <li>Zoek naar en selecteer Workfront- verzoekrijen en de Planningsvormen van Workfront in een geconsolideerde ervaring.</li>
                <li>Kolommen in de lijst met ingediende aanvragen verbergen en opnieuw ordenen.</li>
            </ul>
            </p>
        </td>
        <td>vrijdag 21 augustus 2025</td>
        <td>vrijdag 11 september 2025</td>
        <td>vrijdag 16 oktober 2025</td>
    </tr>     
  </tbody>
</table>

### Andere verbeteringen

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong> Eigenschap </strong>
        </td>
        <td><strong>Voorvertoning</strong></td>
        <td><strong>Snelle release</strong></td>
        <td><strong>Driemaandelijks</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-other.md" class="MCXref xref" xrefformat="{para}"> Updates aan verbeterde lijsten </a><p></p>
            <p>Met onze geavanceerde lijstindeling kunt u filters en groepen gebruiken om uw werk weer te geven en beter te organiseren. Er wordt nu een blauwe-puntenindicator weergegeven boven een widget om u te laten weten wanneer een filter of groep is toegepast op een lijst in de volgende gebieden:</p>
            <ul>
                <li>Mijn verzoeken-widget</li>
                <li>Prioriteiten</li>
            </ul>
        </td>
        <td>vrijdag 28 augustus 2025</td>
        <td>vrijdag 11 september 2025</td>
        <td>vrijdag 16 oktober 2025</td>
    </tr>     
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/25-q4-release-activity/25-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}"> blik-en-voelt updates tijdens het Vierde Kwartaal 2025 versietijdframe </a></p>
                        <p>Kleine updates van het uiterlijk van verschillende onderdelen van de Adobe Workfront-toepassing worden uitgevoerd binnen de releaseperiode van het vierde kwartaal van 2025. </p>
                    </td>
                    <td><p>Gedurende het vierde kwartaal van 2025 is de releaseperiode<br /></p>
                    <td colspan="2"><p>Snelle release: minimaal 1 week na vrijgave voor voorvertoning (tenzij anders aangegeven)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

<!--
### Functionality soon to be removed from Workfront

* 
-->

## Modernisering van de interface

We werken de interface in Adobe Workfront bij om de gebruikerservaring te verbeteren en deze te verenigen met andere Adobe-toepassingen. Deze veranderingen worden vrijgegeven buiten het standaardversieschema. Voor een lijst van deze veranderingen, zie [ Modernisering van de Interface ](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

## Opmerkingen bij de release voor andere gebieden

### Workfront Fusion-verbeteringen

Nieuwe functies in Workfront Fusion zijn beschikbaar in Production op een cadence buiten de standaard releaseschema. Voor meer informatie over de recentste eigenschappen, zie [ de versieactiviteit van de Fusie van Adobe Workfront ](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity).

### Verbeteringen voor Workfront-planning

Nieuwe functies in Workfront Planning zijn beschikbaar in Production. Voor meer informatie over de recentste eigenschappen, zie [ Vierde Kwartaal 2025 versieactiviteit voor de Planning van Adobe Workfront ](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q4.md).

Er zijn geen updates voor het volgende op dit punt in de versie:

* Scenario Planner
* Proef
* Doelen

## Desktop proofing viewer-updates

### Versie 2.1.52

**de versie van de Productie voor alle klanten: 31 juli, 2025**

De Desktop Proofing Viewer is bijgewerkt naar versie 2.1.52, waarin de opgeloste problemen zijn opgelost.

De 2.1.51-update bevatte interne gereedschapsupdates die geen invloed hadden op de functionaliteit van de eindgebruiker.

Deze update geldt voor zowel Mac als Windows.

## Aankondigingen

### Nieuwe versie van Workfront voor Microsoft Teams

Als [ Microsoft overgangen aan de Nieuwe cliënt van Teams ](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability), zal de Klassieke cliënt van Teams niet meer beschikbaar na 1 Juli, 2025 zijn. Als u Microsoft Teams en geïntegreerde toepassingen zoals Workfront wilt blijven gebruiken, moeten klanten vóór deze datum overstappen naar de New Teams-client.

De bijgewerkte Workfront-integratie is nu beschikbaar en volledig compatibel met de New Teams-ervaring. In de meeste gevallen wordt Workfront automatisch weergegeven wanneer gebruikers een overgang hebben gemaakt. Als dit niet het geval is, kan de integratie handmatig worden geïnstalleerd vanaf de Microsoft Teams App Store. Om de integratie van Workfront in de Nieuwe cliënt van Teams te installeren of te verifiëren, zie [  [!DNL Adobe Workfront]  installeren voor Microsoft Teams ](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

### Workfront for Microsoft Outlook

[ Microsoft is in het proces om steun voor de online tokens van de erfenisUitwisseling ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) onbruikbaar te maken, die momenteel door de toe:voegen-binnen van Workfront Vooruitzichten voor authentificatie worden gebruikt. Deze verandering door Microsoft is al begonnen met gevolgen voor de klanten en zal tot oktober 2025 in fasen blijven doorlopen.

* **nadat Microsoft volledig deze tokens onbruikbaar maakt, zal Workfront voor de integratie van Microsoft Outlook niet meer functioneren.**

Als onderdeel van deze wijziging heeft Microsoft besloten om de manier te wijzigen waarop tokens opnieuw worden ingeschakeld. Na **Juni 30, 2025**, zullen de beheerders niet meer tokens kunnen re-toelaten zelf-slechts de Steun van Microsoft kan uitzonderingen verlenen. **Op 1 Oktober, 2025, zullen de erfenistokens voor alle huurders worden uitgezet. Er worden geen uitzonderingen toegestaan.**

### Andere Workfront-integratieovergangen

Om stabielere en scalable integratie te leveren, verschuiven wij naar een moderne, flexibele integratiebenadering gebruikend Workfront Automation and Integration (Fusion). Als deel van dit overgangsproces, zullen de volgende integraties niet beschikbaar na **28 Februari, 2026** zijn:

* Workfront for G Suite
* Workfront voor Jira
* Workfront voor Salesforce.

We raden u aan Workfront Automation and Integration te gebruiken voor de integratiebehoeften van uw organisatie met Google Workspace.
Voor een overzicht van de Automatisering en de Integratie van Workfront, zie [ het overzicht van de Fusie van Adobe Workfront ](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).

### API-versie 20

Workfront API versie 20 is uitgebracht op 4 mei 2025. Voor API versie 20 hebben we een aantal bronnen en eindpunten gewijzigd. Sommige wijzigingen ondersteunen nieuwe functionaliteit en andere maken het voor u gemakkelijker om de informatie te gebruiken die beschikbaar is via de API.

Voor informatie over wat nieuw en bijgewerkt is, zie [ wat in API versie 20 ](/help/quicksilver/wf-api/api/new-api-version-19.md) nieuw is.

Voor informatie over API versies, zie [ API versioning en steunprogramma ](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Workfront-onderhoudsupdates

Voor informatie over de onderhoudsupdates die tijdens Eerste Kwartaal 2025 versie worden gemaakt, zie {de Updates van het Onderhoud van 0} Workfront [.](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=nl-NL)

### Training-updates

Ontdek de nieuwste updates van leerprogramma&#39;s, leerpaden, video&#39;s en handleidingen voor elke Adobe Workfront-productrelease. Voor meer informatie, zie &quot;wat&quot;sectie van de [ pagina van de Leerprogramma&#39;s van Workfront ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=nl-NL) Nieuw is.
