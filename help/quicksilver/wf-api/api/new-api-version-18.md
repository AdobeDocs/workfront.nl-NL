---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuwe functies in API-versie 18
description: Adobe Workfront heeft API-versie 18 uitgebracht op 6 april 2022. API-versie 18 bevat de volgende wijzigingen ten opzichte van versie 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: d0675dc1-b2d9-4d80-8c12-f26284cfb4cf
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 0%

---

# Nieuwe functies in API-versie 18

Adobe Workfront heeft API-versie 18 uitgebracht op 8 april 2024. API-versie 18 bevat de volgende wijzigingen ten opzichte van versie 15.

## Toegevoegde bronnen

Er zijn geen bronnen toegevoegd voor API-versie 18.

## Verwijderde bronnen

Er zijn geen bronnen verwijderd voor API-versie 18

## Gewijzigde bronnen

### AccessLevelPermissions (ALVPER)

Een AccessLevelPermissions-object vertegenwoordigt een specifieke machtiging om een Workfront-object te openen, maken of wijzigen. Deze toestemmingen kunnen dan met een Niveau van de Toegang worden geassocieerd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostentarieven weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Factureringssnelheden weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Algemene financiering bekijken)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kosttarieven bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Factureringssnelheden bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Algemene financiering bewerken)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostentarieven weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Factureringssnelheden weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Algemene financiering bekijken)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kosttarieven bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Factureringssnelheden bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Algemene financiering bewerken)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secundairActions</b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostentarieven weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Factureringssnelheden weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Algemene financiering bekijken)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kosttarieven bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Factureringssnelheden bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Algemene financiering bewerken)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest (ACSREQ)

Als een gebruiker in Workfront geen toegang heeft tot een object dat hij of zij nodig heeft, kan hij of zij toegang tot dat object aanvragen. Het AccessRequest-object vertegenwoordigt deze aanvraag.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>action</b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostentarieven weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Factureringssnelheden weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Algemene financiering bekijken)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kosttarieven bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Factureringssnelheden bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Algemene financiering bewerken)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRule (ACSRUL)

Een voorwerp AccessRule vertegenwoordigt een regel die in de niveaus van de douanetoegang wordt geplaatst die bepaalt hoe de gebruikers projecten kunnen delen zij tot stand brengen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostentarieven weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Factureringssnelheden weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Algemene financiering bekijken)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kosttarieven bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Factureringssnelheden bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Algemene financiering bewerken)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostentarieven weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Factureringssnelheden weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Algemene financiering bekijken)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kosttarieven bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Factureringssnelheden bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Algemene financiering bewerken)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secundairActions</b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostentarieven weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Factureringssnelheden weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Algemene financiering bekijken)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kosttarieven bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Factureringssnelheden bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Algemene financiering bewerken)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Goedkeuring (goedkeuring)

Een bepaald het werkpunt, zoals een taak, een document, of een timesheet, kunnen vereisen dat een supervisor of een andere gebruiker weg op het het werkpunt ondertekent. Een voorwerp van de Goedkeuring vertegenwoordigt de actie van het ondertekenen van op een het werkpunt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>De volgende velden zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>SchedulNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Wachtende goedkeuring (AWAPVL)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Bewerkingen</td>
      <td>
        <ul>
          <li>
            <p>De volgende bewerkingen zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p><b>ADD</b>
                </p>
              </li>
              <li>
                <p><b>DELETE</b>
                </p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Basislijn (BLIN)

Basislijnen zijn momentopnamen van hoe de prestaties van een project er op een bepaald moment uitzagen. Ze slaan belangrijke informatie over het project op, zoals belangrijke data, voortgang, kosten en inkomstenwaarden.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>De volgende velden zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>SchedulNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### BaselineTask (BSTSK)

Basislijnen zijn momentopnamen van hoe de prestaties van een project er op een bepaald moment uitzagen. Ze slaan belangrijke informatie over het project op, zoals belangrijke data, voortgang, kosten en inkomstenwaarden. Wanneer u een basislijn maakt, worden de taakgegevens ook vastgelegd op de basislijntaken van die basislijn.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>De volgende velden zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>SchedulNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Categorie (CTGY)

Een object Categorie is een aangepast formulier.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>:
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:
            <ul>
              <li>
                <p><code>NLBRCY</code> (categorie niet-arbeidsmiddelen)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Uur)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Creditcard)
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>objTypes</b>:
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:
            <ul>
              <li>
                <p><code>NLBRCY</code> (categorie niet-arbeidsmiddelen)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Uur)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Creditcard)
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Document (DOCU)

Een object Document vertegenwoordigt een bestand (zoals geschreven materiaal, afbeeldingen of andere vormen van informatie).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b>:
            </p>
            <p>De volgende parameter toegevoegd:
            <ul>
              <li>
                <p><code>documentID</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>moveToFolder</b>:
            </p>
            <p>Toegevoegd. Deze nieuwe actie voert de volgende parameters uit:
            <ul>
              <li>
                <p><code>documentIDs</code>
                </p>
              </li>
              <li>
                <p><code>folderID</code> 
                </p>
              </li>
              <li>
                <p><code>moveToFolder</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### FinancialData (FINDAT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>De volgende velden zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>SchedulNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Standaardvelden</td>
      <td>
        <ul>
          <li>
            <p>De volgende velden zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>SchedulNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalEntry (JRNLE)

Het object JournalEntry kan worden ingesteld om informatie over specifieke objectvelden te registreren wanneer deze velden worden gewijzigd. Wanneer een gebied opstelling is om als deel van het voorwerp van de Ingang van het Dagboek worden geregistreerd, zal een overeenkomstig Ingang van het Dagboek worden gecreeerd telkens als dat gebied wordt gewijzigd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p><code>AAO</code> (enum.actiontypeenum.assetapproval.opened)</p>
              </li>
              <li>
                <p><code>ADM</code> (enum.actiontypeenum.assetapproval.locked.all.decisions.made)</p>
              </li>
              <li>
                <p><code>AUL</code> (enum.actiontypeenum.assetapproval.unlocked.manual)</p>
              </li>
              <li>
                <p><code>ALM</code> (enum.actiontypeenum.assetapproval.locked.manual)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OpTask (OPTASK)

Een voorwerp OpTask is algemeen genoemd als Kwestie. Een kwestie is een het werkpunt dat gewoonlijk wijst op een probleem verhinderend de voltooiing van een taak of een project. Een probleem kan ook een verzoek van de Helpdesk zijn. Wijzigingsorders, verzoeken en bugs zijn ook problemen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <ul>
          <li>
            <p><b>convertToProject</b>:
            </p>
            <p>De volgende velden zijn toegevoegd:
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>convertToTask</b>:
            </p>
            <p>De volgende velden zijn toegevoegd:
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Project (PROJ)

Projecten zijn werkitems binnen Workfront en vormen een belangrijke bouwsteen voor de manier waarop Workfront mensen helpt om te werken. Een voorwerp van het Project vertegenwoordigt een groep taken met een gemeenschappelijk, specifiek doel.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>De volgende velden zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>SchedulNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <ul>
          <li>
            <p><b>createProjectWithOverride</b>
            </p>
             <p>Toegevoegd.
            </p>
           </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### ProjectUserRole (PTEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>Het volgende veld is toegevoegd:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p>Het volgende veld is toegevoegd:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Een voorwerp QueueDef vertegenwoordigt een Rij, die een project is dat aan het gebied van de Desk van de Hulp is gepubliceerd om gebruikers toe te staan om kwesties aan het voor te leggen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>aanvragerCoreAction</b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostentarieven weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Factureringssnelheden weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Algemene financiering bekijken)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kosttarieven bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Factureringssnelheden bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Algemene financiering bewerken)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostentarieven weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Factureringssnelheden weergeven)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Algemene financiering bekijken)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kosttarieven bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Factureringssnelheden bewerken)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Algemene financiering bewerken)</p>
              </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tarief (SNELHEID)

Een object Rate vertegenwoordigt een factureringssnelheid in Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>companyID</b></p><p>De volgende markeringen zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p>AUTO_LOAD
                </p>
              </li>
              <li>
                <p>DYNAMISCH
                </p>
              </li>
             </ul>
          </li>
          <li>
          <p><b>displayName</b></p><p>Toegevoegd.</p>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p><b>displayName</b>
            </p><p>Toegevoegd.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Taak (TASK)

Een voorwerp van de Taak vertegenwoordigt een het werkpunt dat als stap naar het bereiken van een definitief doel (het voltooien van een Project) moet worden uitgevoerd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>De volgende velden zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>SchedulNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <ul>
          <li>
            <p><b>convertToProject</b>
            </p>
             <p>Het volgende veld is toegevoegd:
             <ul><li><code>copyCategories</code></li></ul>
            </p>
           </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Sjabloon (TMPL)

Een voorwerp van het Malplaatje vertegenwoordigt een patroon voor een project. Projecten kunnen worden gemaakt op basis van sjablonen om tijd te besparen. Een malplaatje bevat een team en taken, die aan om het even welk project zullen worden gekopieerd dat van het malplaatje wordt gecreeerd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>De volgende velden zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>SchedulNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### TemplateTask (TTSK)

Een voorwerp TemplateTask vertegenwoordigt een Taak die deel van een Malplaatje uitmaakt. De Taken van het malplaatje worden Taken in het Project waar het Malplaatje wordt gebruikt.<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>De volgende velden zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>SchedulNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateUserRole (TTEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>Het volgende veld is toegevoegd:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p>Het volgende veld is toegevoegd:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
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
            <p>Het volgende veld is verwijderd:
            </p>
            <ul>
              <li>
                <p><b>objCode</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Bijwerken (UPDATE)

Werkonderdelen in Workfront kunnen worden bijgewerkt om gebruikers op de hoogte te houden van de huidige status. Een object Update vertegenwoordigt een van deze updates. Updates kunnen door gebruikers worden ingevoerd of door het Workfront-systeem worden gemaakt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>updateType</b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
             <ul>
              <li>
                <p><code>assetapprovalsLockedAllDecisionsMade</code></p>
              </li>
              <li>
                <p><code>assetapprovalsUnlockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalsLockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalOpened</code> </p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <ul>
          <li>
            <p><b>recentUpdatesObjIDs</b>
            </p>
            <p>Toegevoegd.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserPrefValue (USERPF)

Een object UserPrefValue vertegenwoordigt een gebruikersvoorkeur.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b>value</b>
            </p>
            <p>De validator toegevoegd <code>MAX_LENGTH</code></p>
      </td>
    </tr>
  </tbody>
</table>

### Werken (WERKEN)

Een voorwerp van het Werk is een gemeenschappelijke interface die zowel Taak als OpTask erft, en gemeenschappelijke code tussen twee deelt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p>De volgende velden zijn toegevoegd:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>SchedulNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

