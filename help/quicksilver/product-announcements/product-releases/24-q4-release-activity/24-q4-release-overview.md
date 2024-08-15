---
title: Overzicht release 4de kwartaal 2024
description: Deze pagina biedt informatie over functionaliteit die is opgenomen in de release van het vierde kwartaal van 2024. Deze verbeteringen zullen naar verwachting in het hele kwartaal beschikbaar komen in de productieomgeving.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6cc67488-1ba9-4455-9152-366aaabf0939
source-git-commit: 5138321543175cac3e51cc21c8309cbefd8bc1e8
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 0%

---

# Overzicht release 4de kwartaal 2024

Deze pagina biedt informatie over functionaliteit die is opgenomen in de release van het vierde kwartaal van 2024. Deze verbeteringen zullen naar verwachting in het hele kwartaal beschikbaar komen in de productieomgeving.

<span class="preview"> off-cycle eigenschappen (die die aan Productie voorafgaand aan het Vierde Kwartaal 2024 versiedatum vrijgeven) worden benadrukt in geel.</span>

>[!IMPORTANT]
>
>De release van 23.3 bevatte de optie om uw organisatie te verplaatsen naar maandelijkse releases. Daarom heeft Workfront het nummeringsschema van releaseversies gewijzigd om rekening te houden met zowel het maandelijks- als driemaandelijkse releasespoor. Het eerste getal geeft het jaar aan en het tweede getal geeft de maand van de release aan. Voorbeeld: De release voor april 2024 luidt als 24.4.
>
>Voorzien wordt dat maandelijkse en driemaandelijkse versies beschikbaar zullen zijn op de donderdag van de tweede volledige week van de maand, tenzij anders vermeld.
>
>| Maandelijkse release | Driemaandelijkse release |
>|----|----|
>| <ul><li>24.8 (augustus 2024)</li><li>24.9 (september 2024)</li><li>24.10 (oktober 2024)</li></ul> | <ul><li>24.10 (oktober 2024)</li></ul> |
>
>Merk op dat voor de definitieve versie van elk kwartaal (24.10 dit kwartaal), gebruikers op het snelle versieschema één dag vroeg de versie zullen ontvangen.
>
>Voor meer informatie over het snelle versieproces, zie [ toelaten of onbruikbaar maken het snelle versieproces ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Verbeteringen voor Adobe Workfront

* [ de verhogingen van de Beheerder ]
* [Projectverbeteringen](#project-enhancements)
* [Verbeteringen voor integratie](#integration-enhancements)
* [Andere verbeteringen](#other-enhancements)

### Beheerdersverbeteringen

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold"> Eigenschap </span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold"> de data van de Versie </span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}"> de knoop van de Lay-out op de ontwerper van de douanevorm staat twee of drie kolommen </a> toe</p>
                        <p>Met de knop Indeling in de aangepaste formulierontwerper kunt u kiezen uit een werkgebied met twee of drie kolommen. De oorspronkelijke formulierontwerper gebruikt drie kolommen en de veldinstellingen worden uiterst rechts weergegeven. Als u twee kolommen selecteert, worden de veldinstellingen in de linkerkolom naast de veldbibliotheek weergegeven.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 12 augustus 2024</p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met de release van 24.9 (september 2024)</p>
                            </li>
                            <li>
                                <p>Productieversie voor alle klanten: TBD</p>
                            </li>
                        </ul>
                        <p><i>Deze functie maakt deel uit van een gefaseerde release en zal in september beschikbaar zijn voor een beperkt aantal klanten.</i></p>
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
                        <p><span class="bold"> Eigenschap </span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold"> de data van de Versie </span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}"> meer relevante die taken aan het Nieuwe werkschema van de Taak worden toegevoegd </a></p>
                        [!BADGE in productie voor Snelle Versie ]{type=Positive}
                        <p>Wij hebben de zelfde functionaliteit voor relevantere slimme taken aan het gebied van Taken in het Nieuwe vakje van de Taak toegevoegd wanneer het toevoegen van een taak aan een project en in een lijst van de projecttaak.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 13 februari 2024</p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met 24,5 release (16 mei 2024)</p>
                            </li>
                            <li>
                                <p>Productieversie voor alle klanten: met de release van 24.10 (oktober 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}"> relevantere slimme taken </a></p>
                        [!BADGE in productie ]{type=Informative}
                        <p>We hebben het algoritme gewijzigd dat Workfront gebruikt om slimme toewijzingen voor taken te berekenen en voor te stellen. Het nieuwe algoritme is van toepassing op de volgende gebieden in Workfront waar u een taak toewijst: taaklijsten, het gebied van Toewijzingen in de taakkopbal, Huis, en het Summiere paneel.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 21 december 2023</p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met 24,5 release (16 mei 2024)</p>
                            </li>
                            <li>
                                <p>Productieversie voor alle klanten: met de release van 24.10 (oktober 2024)</p>
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
                        <p><span class="bold"> Eigenschap </span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold"> de data van de Versie </span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}"> Verbeteringen van de de integratielogin van Vooruitzichten </a></p>
                        <p>De login ervaring voor de integratie van Vooruitzichten is gestroomlijnd zodat alle klanten de zelfde knoop zien aan login aan Workfront al dan niet zij IMS-Toegelaten zijn. De volgende aanmeldstappen verschillen voor IMS- en niet-IMS-instanties, maar de eerste pagina is voor alle gebruikers hetzelfde.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 6 augustus 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Productieversie voor alle afnemers: 6 augustus 2024</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}"> blik-en-voelt updates tijdens het Vierde Kwartaal 2024 timeframe </a></p>
                        <p>Kleine updates van de look and feel van verschillende onderdelen van de Adobe Workfront-toepassing worden uitgevoerd binnen het vierde kwartaal van 2024. Bekijk de afzonderlijke releaseopmerkingen voor specifieke releasedatums.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: gedurende de releaseperiode van het vierde kwartaal van 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Productieversie: bekijk de opmerkingen bij de release voor specifieke datums</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}"> de Medewerker van de Adobe AI beschikbaar in Workfront </a></p>
                        <p>Om het voor u gemakkelijker te maken om uw werk te voltooien, hebben wij de Medewerker van AI van Adobe aan Workfront toegevoegd. AI Assistant kan u helpen door:</p>
                        <ul>
                            <li>Het samenvatten van het werkpunten en documenten, toestaand u om een algemeen inzicht in taken, projecten, en activa snel te bereiken.</li>
                            <li>Het verstrekken van informatie van de documentatie van het Experience League, het brengen van instructies en verwijzingsmateriaal in Workfront, terwijl het verbinden aan meer diepgaande documentatie.</li>
                            <li>Formules maken en verfijnen voor berekende aangepaste formuliervelden, formules genereren op basis van tekstaanwijzingen of fouten zoeken in bestaande formules.</li>
                            </ul>
                            <p>Uw Workfront-beheerder kan AI Assistant voor uw organisatie in- of uitschakelen. De AI-assistent is beschikbaar voor instanties met de plannen Selecteren, Primair en Ultimate.</p>
                        </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 28 augustus 2024</p>
                            </li>
                            <li>
                                <p class="preview">Productieversie: 28 augustus 2024</p>
                            </li>
                        </ul>
                    </td>
                </tr>                            
           </tbody>
        </table>

## Aankondigingen

### Workfront Fusion-verbeteringen

Nieuwe functies in Workfront Fusion zijn beschikbaar in Production op een cadence buiten het 4e kwartaal van 2024 releaseschema. Voor meer informatie over de recentste eigenschappen, zie [ de versieactiviteit van de Fusie van Adobe Workfront ](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Verbeteringen in Workfront Scenario Planner

Er zijn op dit punt in de release geen Scenario Planner-updates. Dit gebied wordt bijgewerkt wanneer er updates beschikbaar zijn.

### Verbeteringen voor Workfront Proof

Er zijn op dit moment geen Workfront Proof-updates beschikbaar. Dit gebied wordt bijgewerkt wanneer er updates beschikbaar zijn.

### Verbeteringen voor Workfront-doelen

Er zijn op dit moment geen updates voor Workfront Goals beschikbaar in de release. Dit gebied wordt bijgewerkt wanneer er updates beschikbaar zijn.

### API-versie 18

Voor API versie 18 hebben we een aantal bronnen en eindpunten gewijzigd. Sommige wijzigingen ondersteunen nieuwe functionaliteit en andere maken het voor u gemakkelijker om de informatie te gebruiken die beschikbaar is via de API.

Voor informatie over wat nieuw en bijgewerkt is, zie [ wat in API versie 18 ](/help/quicksilver/wf-api/api/new-api-version-18.md) nieuw is.

Voor informatie over API versies, zie [ API versioning en steunprogramma ](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Workfront-onderhoudsupdates

Voor informatie over de onderhoudsupdates die tijdens de Vierde Versie van het Kwartaal 2024 worden gemaakt, zie [ Updates van het Onderhoud van Workfront ](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### Training-updates

Ontdek de nieuwste updates van leerprogramma&#39;s, leerpaden, video&#39;s en handleidingen voor elke Adobe Workfront-productrelease. Voor meer informatie, zie &quot;wat&quot;sectie van de [ pagina van de Tutorials van Workfront ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html) Nieuw is.

### Functionaliteit die binnenkort uit Workfront wordt verwijderd

De volgende functionaliteit wordt binnenkort verwijderd uit Workfront:

#### Veroudering van de oudere Home-ervaring met 24.10

Met de release van 24.10 zullen we de oude Home-ervaringen officieel verouderd hebben. Gebruikers wordt aangeraden om nieuwe introducties te gebruiken. Deze worden dan nog steeds uitgebreid met extra functies voordat de site wordt vervangen. Meer informatie over de overgang, inclusief wat gebruikers en beheerders kunnen doen om zich voor te bereiden, is beschikbaar.
