---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuwe functies in API-versie 19
description: Adobe Workfront heeft API-versie 19 uitgebracht op 6 april 2022. API versie 19 heeft de volgende wijzigingen ten opzichte van versie 18.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 13910328903744aa9bf619e8b4c376520c21b89e
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 0%

---

# Nieuwe functies in API-versie 19

Adobe Workfront heeft API-versie 19 uitgebracht op 8 april 2024. API versie 19 heeft de volgende wijzigingen ten opzichte van versie 18.

## Toegevoegde bronnen

Er zijn geen bronnen toegevoegd voor API-versie 19.

## Verwijderde bronnen

Er zijn geen bronnen verwijderd voor API-versie 19

## Gewijzigde bronnen

### AccessLevel (ACSLVL)

Een voorwerp AccessLevel wordt geassocieerd met gebruikers, en beschrijft de reeks van AccessLevelPermissions die bepalen wat de gebruiker tot toegang heeft.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>accessRestrictions</b><p>De volgende mogelijke waarden zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p>De Workfront AI Assistant (AIOFF) uitschakelen
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Toewijzing (ASSGN)

Een voorwerp van de Toewijzing vertegenwoordigt de verbinding tussen een het werkpunt en de gebruiker, het team, of de groep die wordt toegewezen om aan het te werken.

Het voorwerp van de Toewijzing voegde de vlag **DATA_EXTENDIBLE** toe.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>De volgende directe velden zijn toegevoegd:
        <ul>
          <li>
            <p><b>categoryID</b><p>Een categorie is een aangepast formulier. Dit veld ondersteunt de mogelijkheid om een aangepast formulier aan een toewijzing toe te voegen.
            </p>
          </li>
          <li>
            <p><b>prioriteit</b><p>In dit veld zijn de volgende waarden mogelijk:
            <ul>
              <li>0 (geen)</li>
              <li>1 (laag)</li>
              <li>2 (normaal)</li>
              <li>3 (Hoog)</li>
              <li>4 (Dringend)</li>
             </ul>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Referentievelden</td>
      <td>De volgende referentievelden zijn toegevoegd:
        <ul>
          <li>
            <p><b>categorie</b><p>Een categorie is een aangepast formulier. Dit veld ondersteunt de mogelijkheid om een aangepast formulier aan een toewijzing toe te voegen.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>De volgende verzamelingsvelden zijn toegevoegd:
        <ul>
          <li>
            <p><b>objectCategories</b><p>Een categorie is een aangepast formulier. Dit veld ondersteunt de mogelijkheid om een aangepast formulier aan een toewijzing toe te voegen.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



### Categorie (CTGY)

Een object Categorie is een aangepast formulier.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>De volgende velden zijn toegevoegd ter ondersteuning van de mogelijkheid om een aangepast formulier aan een toewijzing toe te voegen.
        <ul>
          <li>
            <p><b>catObjCode</b><p>De volgende mogelijke waarden zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p>Toewijzing (ASSGN)
                </p>
              </li>
             </ul>
          </li>
          <li>
            <p><b>objTypes</b><p>De volgende mogelijke waarden zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p>Toewijzing (ASSGN)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Classifier (CLSF)

Een classificator is een plaats.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>De volgende handelingen zijn toegevoegd:
        <ul>
          <li>
            <b> activateClassifiers </b>
          </li>
          <li>
            <b> deactivateClassifiers </b>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Klant

Een object van de Klant vertegenwoordigt een organisatie die een instantie van Workfront gebruikt.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>customEnumTypes</b><p>De volgende mogelijke waarden zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p>Toewijzingsprioriteiten (PRIORITY_ASSIGNMENT)
                </p>
              </li>
             </ul>
          </li>
              <p>Het object CustomEnum helpt bij het omzetten van statuscodes in leesbare tekst.</p>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### CustomerPreferences (CUSTPR)

Een object CustomerPreferences vertegenwoordigt de set voorkeuren die een klant heeft ingesteld voor hun exemplaar van Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>name</b><p>De volgende mogelijke waarden zijn verwijderd:
            </p>
            <ul>
              <li>
                <p>Zoom-integratie inschakelen in de updatestream (password:zoomIntegrationEnabled)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Document (DOCU)

Een object Document vertegenwoordigt een bestand (zoals geschreven materiaal, afbeeldingen of andere vormen van informatie).

<table>
  <tbody>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b><p>Het veld toegevoegd <code>folderID</code>.</p>
          </li>
          <li>
            <p><b>sendDocumentsToExternalProvider</b><p>Toegevoegd.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


### ExchangeRate (EXRATE)

Een ExchangeRate-object vertegenwoordigt een wisselkoers die in Workfront is ingesteld. ExchangeRate-objecten zijn niet dynamisch.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
      <ul>
      <li>De volgende velden hebben de validator <code>REQUIRED</code> toegevoegd:
        <ul>
          <li><p><b>valuta</b></li>
          <li><p><b>tarief</b></li></ul>
      <li>De volgende velden zijn toegevoegd:
        <ul>
          <li><p><b>enteredByID</b></li>
          <li><p><b>entryDate</b></li>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referentievelden</td>
      <td>
      <ul>
        <li>De volgende velden zijn toegevoegd:
        <ul>
          <li><p><b>enterBy</b></li>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Groep (GROEP)

Een object Group vertegenwoordigt een set gebruikers en teams. Groepen vertegenwoordigen vaak de afdelingsstructuur.

Het voorwerp van de Groep voegde de vlag **SHARABLE** toe.

### Uur (UUR)

Een voorwerp van het Uur vertegenwoordigt een uur dat door een gebruiker op timesheet wordt geregistreerd.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
      De volgende velden zijn toegevoegd:
        <ul>
          <li><p><b>assignedApproverID</b></li>
          <li><p><b>isBillable</b></li>
          <li><p><b>isBilled</b></li>
          <li><p><b>removedByID</b></li>
          <li><p><b>removedOnDate</b></li>
          <li><p><b>ignoreComment</b></li>
          <li><p><b>submitByID</b></li>
          </ul>
          <p>Het volgende veranderde werd aangebracht in het <b> uren </b> gebied.</p>
          <ul> 
          <li> Verwijderd validator <b> GREATER_THAN </b></li>
          <li> Toegevoegde validator <b> NOT_EQUAL </b></li>
          </ul>
     </td>
    </tr>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
      De volgende acties zijn toegevoegd:
        <ul>
          <li><p><b>goedkeuren</b></li>
          <li><p><b>afkeuren</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalEntry (JRNLE)

Het object JournalEntry kan worden ingesteld om informatie over specifieke objectvelden te registreren wanneer deze velden worden gewijzigd. Wanneer een gebied opstelling is om als deel van het voorwerp van de Ingang van het Dagboek worden geregistreerd, zal een overeenkomstig Ingang van het Dagboek worden gecreeerd telkens als dat gebied wordt gewijzigd.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>vlaggen</b><p>De volgende mogelijke waarden zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p>Is kostenpercentage (CR)
                </p>
              </li>
              <li>
                <p>Heeft factureringssnelheid (BR)
                </p>
              </li>
              <li>
                <p>Is algemene financiering
                </p>
              </li>
              <li>
                <p>Is gecombineerde financiering (CF)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Parameter (PARAM)

Een object Parameter is een aangepast veld.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>dataType</b></p><p>De volgende mogelijke waarde is toegevoegd:
            <ul>
            <li>Duur (DRTN)</li>
            </ul>
          </li>
          <li>
            <p><b>displayType</b></p><p>Om een meer gebruikersvriendelijk en flexibel systeem tot stand te brengen, is het <b> Widget (WIDGET) </b> gebiedstype afgekeurd, en in de volgende gebiedstypes gesplitst:
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>Afbeelding (AFBEELDING)</li>
            <li>PDF (PDF)</li>
            <li>Video (VIDEO)</li>
            <li>Extern opzoeken (EXTRNL)</li>
            <li>Multi-Select External Lookup (MULTEXTRNL)</li>
            <li>Oorspronkelijk veld (WFNATIVE)</li>
            <li>Planning (WFPLANNING)</li>
            <li>TIJDELIJKE KPI (TIMEPHASED)</li>
            <li>Rollup (ROLLUP)</li>
            <li>Documenten (DOCUMENT)</li>
           </ul>
          </li>
          <li>
            <p><b>configuraties</b><p>Toegevoegd.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Rol (ROLE)

Een object Role (taakrol) vertegenwoordigt een functionele capaciteit of een vaardigheid die een gebruiker zou kunnen opvullen, zoals Designer of Product Manager.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
    De volgende velden zijn toegevoegd:
        <ul>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referentievelden</td>
      <td>
        De volgende velden zijn toegevoegd:
        <ul>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion {#scorecardquestion}

Een ScoreCardQuestion-object vertegenwoordigt een vraag die aan een Scorecard is toegevoegd. Deze vragen worden gewoonlijk bepaald door de manager van het Portfolio, en hun antwoorden staan de manager toe om te begrijpen hoe goed een project zich op de doelstellingen van de portefeuille richt.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
            <p><b>displayType</b></p><p>Om een meer gebruikersvriendelijk en flexibel systeem tot stand te brengen, is het <b> Widget (WIDGET) </b> gebiedstype afgekeurd, en in de volgende gebiedstypes gesplitst:
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>Afbeelding (AFBEELDING)</li>
            <li>PDF (PDF)</li>
            <li>Video (VIDEO)</li>
            <li>Extern opzoeken (EXTRNL)</li>
            <li>Multi-Select External Lookup (MULTEXTRNL)</li>
            <li>Oorspronkelijk veld (WFNATIVE)</li>
            <li>Planning (WFPLANNING)</li>
            <li>TIJDELIJKE KPI (TIMEPHASED)</li>
            <li>Rollup (ROLLUP)</li>
            <li>Documenten (DOCUMENT)</li>
           </ul>
      </td>
  </tbody>
</table>

### TemplateAssignment (TASSGN)

Een voorwerp TemplateAssignment vertegenwoordigt de verbinding tussen een malplaatjetaak en de gebruiker, het team, of de groep die wordt toegewezen om aan het te werken. Wanneer het malplaatje voor een project wordt gebruikt, wordt die gebruiker, team, of groep toegewezen aan de taak.

Het voorwerp TemplateAssignment voegde de vlag **DATA_EXTENDIBLE** toe.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>De volgende directe velden zijn toegevoegd:
        <ul>
          <li>
            <p><b>categoryID</b><p>Een categorie is een aangepast formulier. Dit veld ondersteunt de mogelijkheid om een aangepast formulier aan een toewijzing toe te voegen.
            </p>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Referentievelden</td>
      <td>De volgende referentievelden zijn toegevoegd:
        <ul>
          <li>
            <p><b>categorie</b><p>Een categorie is een aangepast formulier. Dit veld ondersteunt de mogelijkheid om een aangepast formulier aan een toewijzing toe te voegen.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>De volgende verzamelingsvelden zijn toegevoegd:
        <ul>
          <li>
            <p><b>objectCategories</b><p>Een categorie is een aangepast formulier. Dit veld ondersteunt de mogelijkheid om een aangepast formulier aan een toewijzing toe te voegen.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tijdschema (TSHET)

Een voorwerp Timesheet vertegenwoordigt virtuele timecard dat Gebruikers toestaat om werkelijk gewerkte uren voor Taken, Projecten, en de Types van uren van overheaduren in te gaan.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b></p><p>Verwijderd.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


