---
title: Overzicht release derde kwartaal 2024
description: Deze pagina bevat informatie over de functionaliteit die is opgenomen in de release van het derde kwartaal van 2024. Deze verbeteringen zullen naar verwachting in het hele kwartaal beschikbaar komen in de productieomgeving.
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
source-git-commit: 76b44f3d5ff7d7747da801a051a457157e08ea4a
workflow-type: tm+mt
source-wordcount: '1849'
ht-degree: 0%

---

# Overzicht release derde kwartaal 2024

Deze pagina bevat informatie over de functionaliteit die is opgenomen in de release van het derde kwartaal van 2024. Deze verbeteringen zullen naar verwachting in het hele kwartaal beschikbaar komen in de productieomgeving.

Het levende 24.7 versiewebinar werd geannuleerd, maar u kunt nog [ op een videodemonstratie van 24.7 eigenschappen hier ](https://video.tv.adobe.com/v/3430532/%20) letten.

<span class="preview"> off-cycle eigenschappen (die die aan Productie voorafgaand aan het Derde Kwartaal 2024 versiedatum vrijgeven) worden benadrukt in geel.</span>

>[!IMPORTANT]
>
>De release van 23.3 bevatte de optie om uw organisatie te verplaatsen naar maandelijkse releases. Daarom heeft Workfront het nummeringsschema van releaseversies gewijzigd om rekening te houden met zowel het maandelijks- als driemaandelijkse releasespoor. Het eerste getal geeft het jaar aan en het tweede getal geeft de maand van de release aan. Voorbeeld: De release voor april 2024 luidt als 24.4.
>
>Voorzien wordt dat maandelijkse en driemaandelijkse versies beschikbaar zullen zijn op de donderdag van de tweede volledige week van de maand, tenzij anders vermeld.
>
>| Maandelijkse release | Driemaandelijkse release |
>|----|----|
>| <ul><li>24.5 (16 mei 2024)</li><li>24.6 (13 juni 2024)</li><li>24.7 (18 juli 2024)</li></ul> | <ul><li>24.7 (18 juli 2024)</li></ul> |
>
>Voor meer informatie over het snelle versieproces, zie [ toelaten of onbruikbaar maken het snelle versieproces ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Verbeteringen voor Adobe Workfront

* [Beheerdersverbeteringen](#administrator-enhancements)
* [Verbeteringen op het gebied van financieel beheer](#financial-management-enhancements)
* [Verbeteringen voor integratie](#integration-enhancements)
* [Projectverbeteringen](#project-enhancements)
* [Verbeteringen voor proefdrukken](#proofing-enhancements)
* [Verbeteringen voor hulpbronnenbeheer](#resource-management-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> Bedrijfs regels zijn nu beschikbaar </a></p>
                        [!BADGE in productie ]{type=Informative}
                        <p>Beheerders kunnen nu bedrijfsregels toevoegen in het gedeelte Setup van Workfront.</p>
                        <p>Met een bedrijfsregel kunt u validatie toepassen op Workfront-objecten en voorkomen dat gebruikers een object maken, bewerken of verwijderen als aan bepaalde voorwaarden is voldaan. De regels worden opgebouwd met een formule die vergelijkbaar is met berekende velden in aangepaste formulieren.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 4 juli 2024</p>
                            </li>
                            <li>
                                <p>Productieversie voor alle klanten: met de release van 24,7 (18 juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> de vormontwerper van de Douane algemeen beschikbaar in Adobe Workfront </a></p>
                        [!BADGE in productie ]{type=Informative}
                        <p>Met de versie 24.7 is de formulierontwerper over het algemeen beschikbaar en wordt deze de standaardeigenschap voor het maken en bewerken van aangepaste formulieren in Adobe Workfront. Wanneer u een nieuw aangepast formulier maakt of een bestaand formulier opent, wordt de werkruimte in canvasstijl van de formulierontwerper weergegeven.</p>
                        <p>Na deze release kunt u niet meer terugkeren naar de oude formulierbuilder.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 19 juni 2024</p>
                            </li>
                            <li>
                                <p>Productieversie voor alle klanten: met de release van 24,7 (18 juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> de voorwerpen van de beweging tussen de milieu's van Workfront met milieubevordering </a></p>
                        [!BADGE in productie ]{type=Informative}
                        <p>Met de functie voor milieubescherming kunt u objecten verplaatsen van de ene Workfront-omgeving naar de andere, zoals van een sandboxomgeving naar een productieomgeving. U kunt voorwerpen vormen en testen zonder enig risico voor de gegevens en de verslagen van uw organisatie. U kunt die voorwerpen aan productie dan bewegen zonder het moeten hen aanpassen, besparend tijd en inspanning.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Productieversie voor alle klanten: met de release van 24.6 (13 juni 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> Aangepaste vormen en douanegebieden van het Aandeel in de ontwerper van de douanevorm </a></p>
                        [!BADGE in productie ]{type=Informative}
                        <p>U kunt nu zowel aangepaste formulieren als aangepaste velden delen in de nieuwe formulierontwerper. Hierdoor kan er beter worden samengewerkt tussen gebruikers op aangepaste formulieren.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 6 juni 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Productieversie voor alle afnemers: 13 juni</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> voeg een nieuw douanegebied van het gebied van Gebieden </a> toe</p>
                        [!BADGE in productie ]{type=Informative}
                        <p>U kunt nu een nieuw aangepast veld of een nieuwe widget rechtstreeks vanuit het gebied Velden in Workfront toevoegen zonder dat u een aangepast formulier hoeft te openen om het veld te maken. Zo kunt u snel opnieuw bruikbare aangepaste velden maken.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 6 juni 2024</p>
                            </li>
                            <li>
                                <p>Productieversie voor alle klanten: met de release van 24,7 (18 juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md"> Multi-uitgezochte drop-down gebiedstype beschikbaar op de vormontwerper </a></p>
                        [!BADGE in productie ]{type=Informative}
                        <p>We hebben het veld Multi-Select Dropdown toegevoegd aan de aangepaste formulierontwerper om het eenvoudiger te maken vervolgkeuzelijsten te definiëren. Met dit veldtype kunnen gebruikers meerdere opties in een vervolgkeuzelijst kiezen.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 4 juni 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Productie voor alle afnemers: 4 juni 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Verbeteringen op het gebied van financieel beheer

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}"> Billable en niet-factureerbare uitgavengebieden beschikbaar voor projecten en taken </a></p>
                        [!BADGE in productie ]{type=Informative}
                        <p>Om u gemakkelijker te helpen uitgaventypes bekijken, zijn de uitgaven in factureerbare en niet factureerbare uitgaven op projecten en taken gescheiden. U kunt de volgende velden toevoegen aan weergaven en rapporten:</p>
                        <ul>
                            <li><p>Geplande aanpasbare kosten</p></li>
                            <li><p>Geplande niet-aanpasbare kosten</p></li>
                            <li><p>Werkelijke niet-aanpasbare kosten</p></li>
                            <li><p>Werkelijke niet-aanpasbare kosten</p></li>
                        </ul>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 10 mei 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Productie voor alle afnemers: 10 mei 2024</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}"> Workfront voor Experience Manager Assets en de verbeteringen van Assets Essentials </a></p>
                        [!BADGE in productie ]{type=Informative}
                        <p>We hebben de volgende verbeteringen aangebracht voor de integratie van Workfront voor Experience Manager Assets en Assets Essentials:</p>
                        <ul>
                            <li><p>De integratie ondersteunt nu GCP als cloudserviceprovider. AWS en Azure werden eerder ondersteund.</p></li>
                            <li><p>De formaatlimiet voor bestanden die via de integratie naar de Experience Manager worden verzonden, is verhoogd tot 30 GB. Eerder was de limiet 5 GB.</p></li>
                        </ul>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 27 juni 2024</p>
                            </li>
                            <li>
                                <p>Productie voor alle klanten: met de 24,7-release (18 juli 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}"> geef de taak uit en geef de Datum en de Voorwaarde van Vastleggen van de kopbal of de sectie van Details </a> uit</p>
                        [!BADGE in productie ]{type=Informative}
                        <p>Om het voor u gemakkelijker te maken om taken en kwesties bij te werken, hebben wij nu de gebieden van de Datum en van de Voorwaarde van de Vastlegging toegevoegd als opties om aan taak toe te voegen en kopballen en de sectie van Details in een lay-outmalplaatje uit te geven. Gebruikers kunnen deze velden nu bijwerken vanuit de koptekst- of detailsectie van een pagina wanneer ze zijn toegewezen aan de gewijzigde lay-outsjabloon.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 30 mei 2024</p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met de release van 24.6 (13 juni 2024)</p>
                            </li>
                            <li>
                                <p>Productieversie voor alle klanten: met de release van 24,7 (18 juli 2024)</p>
                            </li>
                        </ul>
                        <p><span class="preview">Deze functie is tijdelijk verwijderd uit Productie voor klanten die zich niet volgens de snelle releaseschema bevinden.</span></p>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}"> meer relevante die taken aan het Nieuwe werkschema van de Taak worden toegevoegd </a></p>
                        [!BADGE in productie ]{type=Informative}
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
                                <p>Productieversie voor alle klanten: met de release van 24,7 (18 juli 2024)</p>
                            </li>
                        </ul>
                        <p><span class="preview"> Deze eigenschap is tijdelijk verwijderd uit Productie voor klanten die niet op het snelle versieschema zijn.</span>&lt;/
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}"> relevantere slimme taken </a></p>
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
                                <p>Productieversie voor alle klanten: met de release van 24,7 (18 juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
           </tbody>
        </table>

### Verbeteringen voor proefdrukken

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}"> de updates van de Veiligheid voor de Desktop het Proofing Kijker </a></p>
                        [!BADGE in productie ]{type=Informative}
                        <p>De beveiligingsupdate Workfront Proof Desktop Proofing Viewer 2.1.35 biedt oplossingen voor beveiligingsproblemen voor kwetsbaarheden die zijn geïdentificeerd in eerdere releases.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 4 juli 2024</p>
                            </li>
                            <li>
                                <p><span class="preview">Productie voor alle afnemers: 4 juli 2024</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>             
           </tbody>
        </table>

### Verbeteringen voor hulpbronnenbeheer

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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-resource-mgmt-enhancements.md"> Tijd van nu terug die in de Balancer van de Werkbelasting </a> wordt weerspiegeld</p>
                        [!BADGE in productie ]{type=Informative}
                        <p>Om het werk naadloos aan te passen wanneer de primaire toegewezen persoon aan een taak tijd weg heeft gepland, wijst de Balancer van de Werkbelasting nu uren aan zowel de primaire als secundaire gebruikers opnieuw toe wanneer de projectchronologie wordt herberekend.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 6 juni 2024</p>
                            </li>
                            <li>
                                <p>Productieversie voor alle klanten: met de release van 24,7 (18 juli 2024)</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}"> Verandering van de steun in productGidsen </a></p>
                        <p>In de komende weken implementeren we een technologische wijziging voor onze gidsen in producten. Terwijl we hebben geprobeerd de impact van deze overgang te minimaliseren, kunnen sommige gebruikers gidsen tegenkomen die zij eerder hebben gezien.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Productie voor alle klanten: incrementeel tot medio augustus 2024</p>
                            </li>
                         </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}"> Adobe Verenigde Ervaring nu beschikbaar voor meer organisaties van Workfront </a></p>
                        [!BADGE in productie ]{type=Informative}
                        <p>Om organisaties toegang tot de voordelen van de Adobe Verenigde Ervaring toe te staan, zijn wij begonnen het ter beschikking te stellen aan bestaande klanten van Workfront. </p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 20 juni 2024</p>
                            </li>
                            <li>
                                <p>Productie voor opgegeven klanten: met de release van 24.7 (18 juli 2024)</p>
                            </li>
                         </ul>
                         <span style="color: #ff0000;"> de Adobe verenigde Shell wordt ter beschikking gesteld in een gefaseerde uitrol. De extra organisaties zullen aan de Adobe Verenigde Shell met de 24.10 en 25.1 versies worden genegeerd. </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}"> knoop van de Hulp die van de belangrijkste navigatiebar wordt verwijderd </a></p>
                        [!BADGE in productie ]{type=Informative}
                        <p>Om de ervaring voor gebruikers te verenigen niet op Verenigde Shell, is de knoop van de Hulp op de belangrijkste navigatiebar verwijderd. Deze knoop, die niet voor gebruikers op Verenigde Shell aanwezig is, verbonden aan de documentatie van Workfront en met een gelijkaardige knoop van de Hulp beschikbaar voor alle gebruikers in het Belangrijkste Menu overtollig was.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 6 juni 2024</p>
                            </li>
                            <li>
                                <p>Productieversie voor alle klanten: met de release van 24,7 (18 juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}"> Verbeterde ervaring UI voor gebruikers met beperkte objecten toegang </a></p>
                        [!BADGE in productie ]{type=Informative}
                        <p>Wanneer een gebruiker geen toegang heeft tot een object, ziet de gebruiker "Geen toegang" op een willekeurige locatie waar de naam van dat object wordt weergegeven in Workfront. Deze verbeterde ervaring geldt ook voor de Workfront API.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: 27 maart 2024</p>
                            </li>
                            <li>
                                <p>Productie voor snelle release: met 24,5 release (16 mei 2024)</p>
                            </li>
                            <li>
                                <p>Productie voor driemaandelijkse release: met 24,7 release (18 juli 2024)</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}"> blik-en-voelt updates tijdens Derde Kwartaal 2024 timeframe </a></p>
                        <p>Kleine updates van het uiterlijk van verschillende onderdelen van de Adobe Workfront-toepassing worden uitgevoerd binnen het derde kwartaal van 2024. Bekijk de afzonderlijke releaseopmerkingen voor specifieke releasedatums.</p>
                    </td>
                    <td><p><b>Beschikbaar op deze data:</b></p>
                        <ul>
                            <li>
                                <p>Voorvertoningsrelease: gedurende de volledige releaseperiode van het derde kwartaal van 2024</p>
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

De nieuwe eigenschappen in Workfront Fusion zijn beschikbaar in Productie bij een kadence buiten het Derde Kwart de versieschema van 2024. Voor meer informatie over de recentste eigenschappen, zie [ de versieactiviteit van de Fusie van Adobe Workfront ](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

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

Voor informatie over de onderhoudsupdates die tijdens de Derde Kwartaal 2024 versie worden gemaakt, zie {de Updates van het Onderhoud van 0} Workfront ](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).[

### Training-updates

Ontdek de nieuwste updates van leerprogramma&#39;s, leerpaden, video&#39;s en handleidingen voor elke Adobe Workfront-productrelease. Voor meer informatie, zie &quot;wat&quot;sectie van de [ pagina van de Tutorials van Workfront ](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html) Nieuw is.
