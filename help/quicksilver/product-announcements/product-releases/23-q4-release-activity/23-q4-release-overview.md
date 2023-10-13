---
title: Overzicht release 4de kwartaal 2023
description: Overzicht release 4de kwartaal 2023
author: Becky
feature: Product Announcements
exl-id: 6c14bd61-60b1-49aa-84bd-d494a226d70e
source-git-commit: 1b247102f3d413e779106577a8b4a9c2c39b20da
workflow-type: tm+mt
source-wordcount: '2528'
ht-degree: 0%

---

# Overzicht release 4de kwartaal 2023

Deze pagina bevat informatie over de functionaliteit die is opgenomen in de release van het vierde kwartaal van 2023. Deze verbeteringen zullen naar verwachting beschikbaar komen in de productieomgeving voor alle klanten met de release 23.10 op 26 en 27 oktober 2023.

<!--
These enhancements will be included in the following releases:

>|Monthly release|Quarterly release|
>|----|----|
>|<ul><li>23.8 (August 31, 2023)</li><li>23.9 (September 28, 2023)</li><li>23.10 (October 26, 2023)</li></ul>| <ul><li>23.10 (Week of October 26, 2023)</li></ul>|
-->

Het webinar uit de release van 23.10 was op 5 oktober 2023. U kunt [register voor webinar om hier een opname op aanvraag te bekijken](https://webinars.on24.com/adobe_workfront/whatsnewin2310?partnerref=releasenotes).

<span class="preview">Functies die buiten de cyclus vallen (kenmerken die vóór de releasedatum van het vierde kwartaal van 2023 in productie zijn), worden geel gemarkeerd.</span>

>[!IMPORTANT]
>
>De release van 23.3 bevatte de optie om uw organisatie te verplaatsen naar maandelijkse releases. Daarom wijzigt Workfront het nummeringsschema van releaseversies om rekening te houden met zowel maandelijks als driemaandelijks releasetracks.
>
>* Als u op de **snelle release (maandelijks)** track, de release na 23.3 is **23,8**, op 31 augustus 2023.
> * Als u op de **kwartaal** vrijgavespoor, de release na 23.3 is **23,10**, in de week van 26 oktober 2023.
> 
> De driemaandelijkse versies zullen functionaliteit van drie maandelijkse versies omvatten. De driemaandelijkse versie van 23.10 bevat bijvoorbeeld functies die worden vrijgegeven in de maandelijkse versies 23.8, 23.9 en 23.10.
>
>Maandelijkse en driemaandelijkse versies zullen naar verwachting beschikbaar zijn op de laatste donderdag van de maand.
>
>| Maandelijkse release | Driemaandelijkse release |
>|----|----|
>| <ul><li>23.8 (31 augustus 2023)</li><li>23.9 (28 september 2023)</li><li>23.10 (26 oktober 2023)</li></ul> | <ul><li>23.10 uur (week 26 oktober 2023)</li></ul> |
>| <ul><li>Geen release (november 2023)</li><li>Geen vrijgave (december 2023)</li><li>24.1 (januari 2024)</li></ul> | <ul><li>24.1 (januari 2024)</li></ul> |
>
>Zie voor meer informatie over het snelle releaseproces [Het proces voor snelle release in- of uitschakelen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Verbeteringen voor Adobe Workfront

* [Beheerdersverbeteringen](#administrator-enhancements)
* [Verbeteringen voor borden](#boards-enhancements)
* [Verbeteringen voor financieel beheer](#financial-management-enhancements)
* [Verbeteringen voor startpagina](#home-enhancements)
* [Verbeteringen voor integratie](#integration-enhancements)
* [Projectverbeteringen](#project-enhancements)
* [Andere verbeteringen](#other-enhancements)

### Beheerdersverbeteringen

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Functie</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Releasedatums</span>
                        </p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Berekende velden op aangepaste formulieren kunnen nu de joker $$USER gebruiken</a></p>
                        <p>Het jokerteken $$USER is nu beschikbaar in berekende aangepaste velden en externe opzoekvelden op de nieuwe formulierontwerper.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 5 oktober 2023</p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met 23,10 release</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Waardeopties van een externe API toevoegen aan een aangepast formulier</a></p>
                        <p>[!BADGE in productie voor Snelle Versie ]{type=Positive}</p>
                        <p>een nieuw veldtype, <strong>Externe zoekopdracht</strong>, is nu beschikbaar op de aangepaste formulierontwerper. Wanneer u gegevens op een extern systeem hebt opgeslagen, kunt u met dit veldtype opties laden vanuit een externe API en filteren op basis van andere veldwaarden in het aangepaste formulier.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 14 september 2023</p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met de release van 23,9</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Verbeteringen voor borden

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Functie</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Releasedatums</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Subtaken zijn nu beschikbaar op Adobe Workfront-borden</a><span style="color: #ff0000;"> Nieuw in Voorvertoning.</span></p><p>Wanneer u een aangesloten kaart aan een raad voor een taak van Workfront toevoegt, worden om het even welke bestaande subtaken ingevoerd op de kaart. Wanneer u een subtaak maakt op een aangesloten kaart, wordt bovendien een subtaak toegevoegd aan de Workfront-taak.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 12 oktober 2023</p>
                            </li>
                            <li>
                                <p>Productie voor de vroege toegang tot de kamers:</p>
                            </li>
                            <li>
                                <p>Productie voor snelle afgifte: n.v.t.</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Verbeteringen voor gebruikerstoewijzingen op borden en kaarten</a></p><p>[!BADGE in productie ]{type=Informative}</p><p>Er zijn nu verbeteringen beschikbaar die flexibiliteit bieden bij het toevoegen van gebruikers aan borden en kaarten in Adobe Workfront Boards.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 21 augustus 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Productie voor alle afnemers: 24 augustus 2023</span>
                            </li> 
                       </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Documenten toevoegen aan verbonden kaarten</a></p><p>U kunt nu documenten op verbonden kaarten aan Adobe Workfront Boards toevoegen. Alle documenten die u op de kaart toevoegt, worden beschikbaar op het tabblad Documenten van de verbonden taak of uitgave. Dezelfde bestandstypen worden in beide gebieden ondersteund.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 21 augustus 2023</p>
                            </li>
                            <li>
                                <p>Productie voor raden van bestuur: 24 augustus 2023</p>
                            </li>
                            <li>
                                <p>Productie voor snelle afgifte: n.v.t.</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Documenten die als alleen-weergeven beschikbaar zijn op verbonden kaarten</a></p><p>Voor verbonden kaarten op Adobe Workfront Boards kunt u nu documenten zoals afbeeldingen en PDF bekijken. U kunt een voorvertoning van een document weergeven in de browser of het document downloaden naar de computer. </p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 3 augustus 2023</p>
                            </li>
                            <li>
                                <p>Productie voor raden van bestuur: 10 augustus 2023</p>
                            </li>
                            <li>
                                <p>Productie voor snelle afgifte: n.v.t.</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">De mening van de raad van een project nu beschikbaar voor kwesties</a></p><p>U kunt nu een Board-weergave openen van een lijst met projectkwesties. Met het Kanban-bord kunt u de voortgang van de problemen op een meer visuele manier volgen dan ze in de lijst weer te geven. </p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 3 augustus 2023</p>
                            </li>
                            <li>
                                <p>Productie voor de vroege toegang tot de kamers:</p>
                            </li>
                             <li>
                                <p>Productie voor snelle afgifte: n.v.t.</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>    
           </tbody>
        </table>

### Verbeteringen voor financieel beheer

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Functie</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Releasedatums</span>
                        </p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">Daadwerkelijke kosten en factureringstarieven</a></p>
                        <p>De effectieve datum van kosten en factureringstarieven zijn nu beschikbaar voor het bedrijf, de gebruiker, en de baanobjecten van de rol in Workfront. Wanneer de datum daadwerkelijke tarieven op een project worden toegepast, en de uren het programma worden geopend projecttaken, worden de kosten en de opbrengst berekend gebruikend de gespecificeerde tarieven voor elke tijdspanne.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 29 juni 2023</p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met 23,10 release</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Verbeteringen voor startpagina

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Functie</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Releasedatums</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">De widget Nieuwe borden voor Nieuwe startpagina</a> <span style="color: #ff0000;"> Nieuw in Voorvertoning.</span></p>
                        <p>In een belangrijke nieuwe aanvulling op de opties voor werkbeheer die beschikbaar zijn in New Home, kunt u nu een board weergeven op uw homepage!</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 12 oktober 2023</p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met 23,10 release</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nieuwe standaardlandingspagina van contribuant: Nieuwe startpagina</a> <span style="color: #ff0000;"> Nieuw in Voorvertoning.</span> </p>
                        <p>Nieuwe startpagina is nu de standaardbestemmingspagina voor contributoraccounts. Deze nieuwe standaardstartpagina bevat een aantal widgets die specifiek zijn geselecteerd om medewerkers in staat te stellen hun werk direct te beheren.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 12 oktober 2023</p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met 23,10 release</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Wijzigingen voor werkregistratie in Nieuwe startpagina </a> </p>
                        <p>[!BADGE in productie voor Snelle Versie ]{type=Positive}</p>
                        <p>Op basis van gebruikersfeedback hebben we het tijdbereikfilter en de overzichtsbalk voor de hele pagina verwijderd, waarin taken werden beschreven die moesten worden uitgevoerd en voltooid. De widgets van het project, van de Taak, en van de Kwestie elk hebben ingebouwde het filtreren eigenschappen die u toestaan om hun werkingsgebied op een individuele basis aan te passen.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 13 september 2023<br /></p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met de release van 23,9</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nieuwe snelle toegangsknoppen voor widgets Project, Taak en Probleem bijhouden</a> </p>
                        <p>[!BADGE in productie voor Snelle Versie ]{type=Positive}</p>
                        <p>Uw mogelijkheden om het werk rechtstreeks vanuit New Home te beheren, zijn uitgebreid en er zijn nieuwe sneltoegangsknoppen toegevoegd aan de widgets Project, Taak en Probleem bijhouden.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 13 september 2023<br /></p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met de release van 23,9</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Nieuwe filteropties voor Nieuwe startpagina</a> </p>
                        <p>[!BADGE in productie voor Snelle Versie ]{type=Positive}</p>
                        <p>Er zijn nu nieuwe filteropties beschikbaar voor de widget Mijn werk in Nieuwe startpagina. U kunt onder andere filters voor objecttypen (taken, problemen en verzoeken) en statussen (niet gereed, klaar om te starten, te werken en te voltooien) kiezen.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 17 augustus 2023<br /></p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met de release van 23.8</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Ondersteuning voor aangepaste terminologie voor New Home</a> </p><p>[!BADGE in productie ]{type=Informative}</p>
                        <p>Om beter aan de unieke behoeften van organisaties te voldoen, gebruikt Nieuw Huis nu douaneterminologie voor voorwerpen zoals die in de lay-outmalplaatjes van een instantie worden bepaald. Als "Project"-objecten bijvoorbeeld in uw Workfront-instantie als "Campagnes" zijn gelabeld, wordt de widget Mijn projecten in plaats daarvan weergegeven als Mijn campagnes in Nieuw startpunt.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 17 augustus 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Productie voor alle afnemers: 31 augustus 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">De knop Nieuwe startpagina wordt verwijderd voor accounts waarvoor Nieuwe startpagina is uitgeschakeld</a> </p>
                        <p>[!BADGE in productie voor Snelle Versie ]{type=Positive}</p>
                        <p>De knop Nieuwe startpagina proberen is niet meer beschikbaar voor accounts waarvoor Nieuwe startpagina is uitgeschakeld. Het nieuwe Huis moet door de systeembeheerder opnieuw worden toegelaten alvorens individuele gebruikers de knoop kunnen gebruiken om Nieuwe Huis te proberen.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 17 augustus 2023<br /></p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met de release van 23.8</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">Wijzigen in standaardwidget Nieuwe startpagina</a> </p>
                        <p>[!BADGE in productie voor Snelle Versie ]{type=Positive}</p>
                        <p>De widget Aan/uit, waarvoor toestemming nodig is om taken te maken, is nu alleen aanwezig in de standaardwidget die is ingesteld voor gebruikers met de licentietypen Standaard, Overzicht of Werkwerk. Bovendien is de widget automatisch verwijderd van de homepages van gebruikers met alle andere licentietypen.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 17 augustus 2023<br /></p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: 17 augustus 2023</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: 17 augustus 2023</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Verbeteringen voor integratie

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Functie</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Releasedatums</span>
                        </p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Verbeteringen op gebied van ervaring bij het verzenden van documenten naar SharePoint (GraphAPI)</a></p><p>[!BADGE in productie ]{type=Informative}</p><p>We hebben een aantal wijzigingen aangebracht om het gemakkelijker te maken om mappen te zoeken wanneer u documenten naar uw SharePoint-mappen (GraphAPI) verzendt</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 24 augustus 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Productie voor alle afnemers: 31 augustus 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Upgrades voor slepen en neerzetten voor documentintegratie</a></p><p>[!BADGE in productie ]{type=Informative}</p><p>Er zijn verbeteringen aangebracht om de duidelijkheid te verbeteren en gebruikersfouten te verwijderen bij het slepen en neerzetten van een bestand in een gekoppelde map.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 24 augustus 2023<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Productie voor alle afnemers: 31 augustus 2023</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Projectverbeteringen

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Functie</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Releasedatums</span>
                        </p>
                    </td>
                 </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Goedkeuring van nieuwe documenten</a> <span style="color: #ff0000;"> Nieuw in Voorvertoning.</span></p>
                        <p>In deze versie is het goedkeuringsproces gestroomlijnd voor zowel het maken van goedkeuringen als het goedkeuren/reviseren van documenten, naast nieuwe functionaliteit.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 12 oktober 2023<br /></p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met 23,10 release</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                        <p><span style="color: #ff0000;">Deze functie maakt deel uit van een gefaseerde release en is momenteel alleen beschikbaar voor specifieke klanten.</span></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Bijgewerkt ontwerp wanneer het toevoegen van een nieuwe kwestie aan een project</a> </p>
                        <p>[!BADGE in productie voor Snelle Versie ]{type=Positive}</p>
                        <p>Deze update is aangekondigd met de release 23.3.</p>
                        <p>We hebben het vak Nieuwe uitgave bijgewerkt, dat wordt weergegeven wanneer u een nieuwe uitgave naar een project verzendt. Nu, past de interface het Nieuwe verzoekvakje aan dat toont wanneer het voorleggen van een nieuw verzoek aan een verzoekrij.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 26 juli 2023<br /></p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met de release van 23.8</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Dynamische herberekening van berekende velden op formulieren</a></p>
                        <p>[!BADGE in productie voor Snelle Versie ]{type=Positive}</p>
                        <p>Berekende velden op een formulier dat aan een object is gekoppeld, worden nu dynamisch opnieuw berekend in real-time wanneer afhankelijke waarden van een formulier op de pagina worden gewijzigd. Zo kunt u de bijgewerkte resultaten bekijken zonder het formulier op te slaan.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 17 augustus 2023<br /></p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met de release van 23.8</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Geplande uren instellen voor terugkerende taken van onderliggende items met het type Eenvoudige duur zonder toewijzingen</a></p>
                        <p>[!BADGE in productie voor Snelle Versie ]{type=Positive}</p>
                        <p>We hebben een wijziging aangebracht in de manier waarop geplande uren worden toegewezen aan terugkerende taken zonder toewijzingen en met een eenvoudige tijdsduur. Nu, wanneer u Geplande Uren op een nieuwe terugkomende taak met een Eenvoudig Type van Duur en geen taken plaatst, worden de uren ook toegewezen aan de individuele herhalingen. Vóór deze wijziging werden de uren niet opgeslagen voor afzonderlijke herhalingen toen de bovenliggende taken niet werden toegewezen.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 17 augustus 2023<br /></p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met de release van 23.8</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Andere verbeteringen

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Functie</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Releasedatums</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Bijgewerkte e-mailsjablonen</a> <span style="color: #ff0000;"> Nieuw in Voorvertoning.</span></p>
                        <p>Als het begin van een nieuw initiatief om onze e-mails met gebeurtenismeldingen bij te werken, hebben we twee van de meest gebruikte programma's bijgewerkt: documentgoedkeuring en het delen van objecten.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 12 oktober 2023</p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met 23,10 release</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Wijzigingen in hoofdmenu van Contribute</a> <span style="color: #ff0000;"> Nieuw in Voorvertoning.</span></p>
                        <p>Om contribuanten beter te informeren over de functies die beschikbaar zijn met een betaald Workfront-licentietype, kunnen ze nu alle beschikbare opties in het hoofdmenu zien.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 12 oktober 2023</p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met 23,10 release</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md" class="MCXref xref" xrefformat="{para}">Nieuwe bètaverbeteringen voor opmerkingervaring</a> </p>
                        <p>[!BADGE in productie voor Snelle Versie ]{type=Positive}</p>
                        <p>De verbeteringen aan de sectie van Updates worden ter beschikking gesteld binnen het Vierde Kwartaal 2023 versietijdskader voor het becommentariëren ervarings bèta. Deze verbeteringen zullen in de Productomgeving voor alle klanten beschikbaar worden gesteld met de vierde release van 2023 (oktober 2023).</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: gedurende de releaseperiode van het vierde kwartaal van 2023<br /></p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: vanaf de 23,8-release</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release (tenzij anders gespecificeerd)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-release-activity.md" class="MCXref xref" xrefformat="{para}">Nieuwe bètaverbeteringen voor canvasdashboards</a> </p>
                        <p>[!BADGE in productie voor Snelle Versie ]{type=Positive}</p>
                        <p>De verbeteringen aan de dashboards van het Canvas worden ter beschikking gesteld binnen het vierde Kwartaal 2023 releasetijdschema als deel van aan de gang zijnde bèta. Deze verbeteringen zullen in de Productomgeving voor alle klanten beschikbaar worden gesteld met de vierde release van 2023 (oktober 2023).</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: gedurende de releaseperiode van het vierde kwartaal van 2023<br /></p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: vanaf de 23,8-release</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 23.10 release (tenzij anders gespecificeerd)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">Updates weergeven en weergeven tijdens het vierde kwartaal van 2023</a></p><p>Kleine updates van de look and feel van verschillende onderdelen van de Adobe Workfront-toepassing worden uitgevoerd binnen het vierde kwartaal van 2023. Bekijk de afzonderlijke releaseopmerkingen voor specifieke releasedatums.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: gedurende de releaseperiode van het vierde kwartaal van 2023</p>
                            </li>
                            <li>
                                <p><span class="preview">Productieversie: bekijk de opmerkingen bij de release voor specifieke datums</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

## Aankondigingen

### Workfront Fusion-verbeteringen

Nieuwe functies in Workfront Fusion zijn beschikbaar in Production op een cadence buiten het 4e kwartaal van 2023 releaseschema. Voor meer informatie over de nieuwste functies raadpleegt u [Adobe Workfront Fusion-releaseactiviteit](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Verbeteringen in Workfront Scenario Planner

Er zijn op dit punt in de release geen Scenario Planner-updates. Dit gebied wordt bijgewerkt wanneer er updates beschikbaar zijn.

### Verbeteringen in Workfront Proof

Er zijn momenteel geen Workfront Proof-updates beschikbaar. Dit gebied wordt bijgewerkt wanneer er updates beschikbaar zijn.

### Verbeteringen voor Workfront-doelen

Er zijn op dit moment geen updates voor Workfront Goals beschikbaar in de release. Dit gebied wordt bijgewerkt wanneer er updates beschikbaar zijn.

### API-versie 17

API-versie 17 is uitgebracht op 12 oktober 2023. Voor API versie 17 hebben we een aantal bronnen en eindpunten gewijzigd. Sommige wijzigingen ondersteunen nieuwe functionaliteit en andere maken het voor u gemakkelijker om de informatie te gebruiken die beschikbaar is via de API.

Voor informatie over nieuwe en bijgewerkte functies raadpleegt u [Nieuwe functies in API-versie 17](/help/quicksilver/wf-api/api/new-api-version-17.md).

Zie voor informatie over API-versies [API-versieschema en ondersteuningsschema](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Workfront-onderhoudsupdates

Voor informatie over de onderhoudsupdates die tijdens de versie 22.3 zijn gemaakt, raadpleegt u [Workfront-onderhoudsupdates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Training-updates

Ontdek de nieuwste updates van leerprogramma&#39;s, leerpaden, video&#39;s en handleidingen voor elke Adobe Workfront-productrelease. Raadpleeg voor meer informatie de sectie &quot;Nieuwe functies&quot; van het dialoogvenster [Workfront Tutorials pagina](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).

### Functionaliteit die binnenkort uit Workfront wordt verwijderd

De volgende functionaliteit wordt binnenkort verwijderd uit Workfront:

#### Verouderde proefversie van de mobiele app Proof met 23.10

De Proof mobile-app wordt officieel vervangen door de release 23.10. De algemene mobiele Workfront-app voor mobiele apparaten is verbeterd met nieuwe proefdrukfunctionaliteit (zie de releaseopmerking onder Workfront Mobile-verbeteringen voor meer informatie) en gebruikers wordt aangeraden deze zo snel mogelijk te gebruiken voor proefdrukken.

Voor de mobiele Workfront-app is een Workfront-aanmelding vereist. Externe gebruikers en gasten kunnen de proefdrukapp blijven gebruiken voor proefdrukken. Deze wordt echter niet meer ondersteund en is niet meer beschikbaar vanaf 23.10.

#### Workstreams verwijderd voor accounts die deze niet gebruiken

Voor accounts die nog nooit een workstream in Adobe Workfront Boards hebben gemaakt, is het Workstreams-gebied vanaf 11 oktober 2023 van het dashboard van Boards verwijderd. Accounts die wel werkstromen gebruiken, hebben nog steeds toegang tot deze accounts. De verbeterde schermfunctionaliteit zal in toekomstige versies worden behandeld.

<!-- HTML you might need

New table

### add product area name

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Feature</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Release dates</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="ADD LINK" class="MCXref xref" xrefformat="{para}">Title</a><span style="color: #ff0000;"> New in Preview!</span></p>
                        <p>Body</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release:<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Production release: </span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

New row for table 

<tr>
  <td>
    <a href="ADD%20LINK">Title</a> New in Preview!
    <p>Body</p>
  </td>
  <td>
    <p><strong>Available on these dates:</strong></p>
    <ul>
      <li>
        <p>Preview release:</p>
      </li>
      <li>
        <p>Production release:</p>
      </li>
    </ul>
  </td>
</tr>


New in preview, prod, and coming soon text

<span style="color: #ff0000;"> New in Preview!</span>
<span style="color: #ff0000;"> New in Production!</span>
<span style="color: #ff0000;"> Coming soon!</span>

Badge for available in Fast Release

[!BADGE In production for Fast Release ]{type=Positive}
[!BADGE In production ]{type=Informative}



Test for boards early access stuff

Production release for early opt-in: March 2, 2023 This feature is available in Production only through the early feature opt-in for Workfront Boards.

Production release for all customers: With the 23.2 release

-->
