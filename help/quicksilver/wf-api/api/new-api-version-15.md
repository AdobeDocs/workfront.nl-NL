---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuwe functies in API-versie 15
description: Adobe Workfront heeft API-versie 14 uitgebracht op 14 juni 2022. API-versie 15 bevat de volgende wijzigingen ten opzichte van versie 14.
author: Becky
feature: Workfront API
role: Developer
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2286'
ht-degree: 0%

---

# Nieuwe functies in API-versie 15

Adobe Workfront heeft API-versie 15 uitgebracht op 14 juni 2022. API-versie 15 bevat de volgende wijzigingen ten opzichte van versie 14.

## Toegevoegde bronnen

* [Initiatief (INITIV)](#Initiati)

* [IssueDef (ISSDEF)](#IssueDef)

* [ObjectIntegration (OBJINT)](#ObjectIn)

* [RichTextGroupParameterValue (GRCVAL)](#RichText)

* [TaskDef (TSKDEF)](#TaskDef)

* [Gebruikersgoedkeuring (USRAPV)](#UserAppr)

### Initiatief (INITIV)

Het object Initiative maakt in de Workfront Scenario Planner ramingen voor het soort en het aantal functies, de vaste kosten en het geplande voordeel.

Voor meer informatie over Initiatieven, zie [ Overzicht van Initiatieven in de Planner van het Scenario ](../../scenario-planner/initiatives-overview.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> customerID </b>
            </p>
            <p>Dit is een intern object.</p>
          </li>
          <li>
            <p><b> duur </b>
            </p>
            <p>De hoeveelheid tijd tussen endDate en startDate.</p>
          </li>
          <li>
            <p><b> endDate </b>
            </p>
            <p>De geplande datum voor de voltooiing van het initiatief.</p>
          </li>
          <li>
            <p><b> enteredByID </b>
            </p>
            <p>De id die is gekoppeld aan de gebruiker die het verzoek heeft verzonden.</p>
          </li>
          <li>
            <p><b> identiteitskaart </b>
            </p>
            <p>De id die aan de handeling is gekoppeld</p>
          </li>
          <li>
            <p><b> initiativeID </b>
            </p>
            <p>De id die aan het initiatief is gekoppeld.</p>
          </li>
          <li>
            <p><b> lastPublishedDate </b>
            </p>
            <p>De datum waarop het initiatief voor het laatst is gepubliceerd in de Workfront Scenario Planner.</p>
          </li>
          <li>
            <p><b> naam </b>
            </p>
            <p>De naam van het initiatief</p>
          </li>
          <li>
            <p><b> planID </b>
            </p>
            <p>De id van het plan dat aan het initiatief is gekoppeld.</p>
          </li>
          <li>
            <p><b> planName </b>
            </p>
            <p>De naam van het plan dat bij het initiatief hoort.</p>
          </li>
          <li>
            <p><b> projectID </b>
            </p>
            <p>De id van het project dat aan het initiatief is gekoppeld.</p>
          </li>
          <li>
            <p><b> scenarioID </b>
            </p>
            <p>De id van het scenario in Workfront Scenario Planner die verband houdt met het initiatief.</p>
          </li>
          <li>
            <p><b> startDate </b>
            </p>
            <p>De geplande aanvangsdatum van het initiatief.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referentievelden</td>
      <td >
        <ul>
          <li>
            <p><b> klant </b>
            </p>
          </li>
          <li>
            <p><b> enteredBy </b>
            </p>
          </li>
          <li>
            <p><b> project </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p><b> identiteitskaart </b>
            </p>
          </li>
          <li>
            <p><b> naam </b>
            </p>
          </li>
          <li>
            <p><b> objCode </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Bewerkingen</td>
      <td>
        <ul>
          <li>
            <p><b> TELLING </b>
            </p>
          </li>
          <li>
            <p><b> GET </b>
            </p>
          </li>
          <li>
            <p><b> RAPPORT </b>
            </p>
          </li>
          <li>
            <p><b> ZOEKEN </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### IssueDef (ISSDEF)

Het IssueDef-object vertegenwoordigt een set gegevens met betrekking tot de indeling van problemen. Dit voorwerp kan aan Projecten of Malplaatjes worden vastgemaakt, en beïnvloedt de kwesties die aan dat Project of Malplaatje worden toegevoegd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> identiteitskaart </b>
            </p>
          </li>
          <li>
            <p><b> isInlineAddEnabled </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p><b> identiteitskaart </b>
            </p>
          </li>
          <li>
            <p><b> objCode </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ObjectIntegration (OBJINT)

In sommige gevallen is het mogelijk om Workfront-werkitems rechtstreeks te koppelen aan objecten in een extern softwareproduct. Het object ObjectIntegration vertegenwoordigt deze koppeling.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> customerID </b>
            </p>
            <p>Dit is een intern object.</p>
          </li>
          <li>
            <p><b> entryDate </b>
            </p>
            <p>De datum en de tijd dat ObjectIntegration in het Systeem van Workfront werd ingegaan.</p>
          </li>
          <li>
            <p><b> identiteitskaart </b>
            </p>
            <p>De unieke Workfront-id van het specifieke ObjectIntegration-object.</p>
          </li>
          <li>
            <p><b> integrationType </b>
            </p>
            <p>De externe software waarmee het object ObjectIntegration een koppeling maakt. Mogelijke waarden zijn:</p>
            <ul>
              <li>
                <p>JIRA</p>
              </li>
              <li>
                <p>SALESFORCE</p>
              </li>
              <li>
                <p>ANAPLAN</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b> linkedObjectID </b>
            </p>
          </li>
          <li>
            <p><b> objID </b>
            </p>
            <p>Het object in Workfront waaraan de ObjectIntegration is gekoppeld.</p>
          </li>
          <li>
            <p><b> objObjCode </b>
            </p>
            <p>De objectcode van het object in Workfront waaraan ObjectIntegration is gekoppeld.</p>
          </li>
          <li>
            <p><b> param1 </b>
            </p>
          </li>
          <li>
            <p><b> param2 </b>
            </p>
          </li>
          <li>
            <p style="font-weight: bold;">param3</p>
          </li>
          <li>
            <p><b> URL </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referentievelden</td>
      <td >
        <ul>
          <li>
            <p><b> klant </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p><b> identiteitskaart </b>
            </p>
          </li>
          <li>
            <p><b> objCode </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TaskDef (TSKDEF)

Het TaskDef-object vertegenwoordigt een set gegevens met betrekking tot de indeling van taken. Dit voorwerp kan aan Projecten of Malplaatjes worden vastgemaakt, en beïnvloedt de taken die aan dat Project of Malplaatje worden toegevoegd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> autoCalcPlannedHours </b>
            </p>
          </li>
          <li>
            <p><b> identiteitskaart </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referentievelden</td>
      <td >
        <ul>
          <li>
            <p><b> defaultApprovalProcess </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
          <li>
            <p><b> objectCategories
</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p><b> identiteitskaart </b>
            </p>
          </li>
          <li>
            <p><b> objCode </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Gebruikersgoedkeuring (USRAPV)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden </td>
      <td>
        <ul>
          <li>
            <p><b> ApproverID </b>
            </p>
          </li>
          <li>
            <p><b> customerID </b>
            </p>
          </li>
          <li>
            <p><b> identiteitskaart </b>
            </p>
          </li>
          <li>
            <p><b> requestedDate </b>
            </p>
          </li>
          <li>
            <p><b> requestID </b>
            </p>
          </li>
          <li>
            <p><b> status </b>
            </p>
          </li>
          <li>
            <p><b> userID </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referentievelden</td>
      <td >
        <ul>
          <li>
            <p><b> fiatteur </b>
            </p>
          </li>
          <li>
            <p><b> klant </b>
            </p>
          </li>
          <li>
            <p><b> aanvrager </b>
            </p>
          </li>
          <li>
            <p><b> gebruiker </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <ul>
          <li>
            <p><b> identiteitskaart </b>
            </p>
          </li>
          <li>
            <p><b> objCode </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Standaardvelden</td>
      <td >
        <ul>
          <li>
            <p><b> ApproverID </b>
            </p>
          </li>
          <li>
            <p><b> requestID </b>
            </p>
          </li>
          <li>
            <p><b> status </b>
            </p>
          </li>
          <li>
            <p><b> userID </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <ul>
          <li>
            <p><b> keurt </b> goed
            </p>
          </li>
          <li>
            <p><b> verwerpen </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Bewerkingen</td>
      <td>
        <ul>
          <li>
            <p><b> TOEVOEGEN </b>
            </p>
          </li>
          <li>
            <p><b> TELLING </b>
            </p>
          </li>
          <li>
            <p><b> DELETE </b>
            </p>
          </li>
          <li>
            <p><b> GET </b>
            </p>
          </li>
          <li>
            <p><b> RAPPORT </b>
            </p>
          </li>
          <li>
            <p><b> ZOEKEN </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Verwijderde bronnen

Er zijn geen bronnen verwijderd voor API-versie 15.

## Gewijzigde bronnen

* [AccessLevel (ACSLVL)](#AccessLe)

* [AccessLevelPermissions (ALVPER)](#AccessLe2)

* [AccessRequest (ACSREQ)](#AccessRe)

* [AccessRule (ACSRUL)](#AccessRu)

* [Goedkeuring (goedkeuring)](#Approval)

* [Categorie (CTGY)](#Category)

* [CategorieParameter (CTGYPA)](#Category2)

* [CustomerPreferences (CUSTPR)](#Customer)

* [DocumentFolder (DOCFDR)](#Document)

* [DocumentVersion (DOCV)](#Document2)

* [Groep (GROEP)](#Group)

* [JournalEntry (JRNLE)](#JournalE)

* [LinkedFolder (LNKFDR)](#LinkedFo)

* [OpTask/Issue (OPTASK)](#OpTask)

* [Parameter (PARAM)](#Paramete)

* [Portfolio (HAVEN)](#Portfoli)

* [Programma (PRGM)](#Program)

* [Project (PROJ)](#Project)

* [QueueDef (QUED)](#QueueDef)

* [ScoreCardQuestion (SCOREQ)](#ScoreCar)

* [Taak (TASK)](#Task)

* [Sjabloon (TMPL)](#Template)

* [Tijdschema (TSHET)](#Timeshee)

* [Weergave (UIVIEW)](#View)

* [Bijwerken (UPDATE)](#Update)

* [Gebruiker (GEBRUIKER)](#User)

* [UserNote (USRNOT)](#UserNote)

* [Werken (WERKEN)](#Work)

### AccessLevel (ACSLVL)

Een voorwerp AccessLevel wordt geassocieerd met gebruikers, en beschrijft de reeks van AccessLevelPermissions die bepalen wat de gebruiker tot toegang heeft.

Voor meer informatie over toegangsniveaus, zie [ niveaus van de Toegang ](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> fieldAccessPrivileges </b> (koord [])</p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p>VTMAWMG (teams weergeven die bij mijn groepen horen)</p>
              </li>
              <li>
                <p>VALLTM (alle teams weergeven)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

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
            <p><b> coreAction </b> (koord [])</p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (teams bewerken waarop ik sta)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (teams bewerken in groepen die ik beheer (alleen groepbeheerders))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b> forbiddenActions </b> (koord [])</p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (teams bewerken waarop ik sta)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (teams bewerken in groepen die ik beheer (alleen groepbeheerders))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b> secundairActions </b> (koord [])</p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (teams bewerken waarop ik sta)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (teams bewerken in groepen die ik beheer (alleen groepbeheerders))</p>
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
            <p><b> actie </b> (koord)</p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (teams bewerken waarop ik sta)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (teams bewerken in groepen die ik beheer (alleen groepbeheerders))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b> autoShareAction </b> (koord)</p>
            <p>De volgende mogelijke waarde is toegevoegd:</p>
            <ul>
              <li>
                <p>WDL</p>
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
            <p><b> coreAction </b> (koord [])</p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (teams bewerken waarop ik sta)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (teams bewerken in groepen die ik beheer (alleen groepbeheerders))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b> forbiddenActions </b> (koord [])</p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (teams bewerken waarop ik sta)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (teams bewerken in groepen die ik beheer (alleen groepbeheerders))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b> secundairActions </b> (koord [])</p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (teams bewerken waarop ik sta)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (teams bewerken in groepen die ik beheer (alleen groepbeheerders))</p>
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
            <p><b> resourcePlannerBudgetedHours </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referentievelden</td>
      <td >
        <ul>
          <li>
            <p><b> initiatief </b>
            </p>
            <p>Toegevoegd.</p>
            <p>Het object Initiative maakt in de Workfront Scenario Planner ramingen voor het soort en het aantal functies, de vaste kosten en het geplande voordeel. </p>
          </li>
          <li>
            <p><b> issueDef </b>
            </p>
            <p>Toegevoegd.</p>
          </li>
          <li>
            <p><b> taskDef </b>
            </p>
            <p>Toegevoegd.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
          <li>
            <p style="font-weight: bold;"><b> objectIntegrations
</b>
            </p>
            <p style="font-weight: normal;">Toegevoegd.</p>
            <p>In sommige gevallen is het mogelijk om Workfront-werkitems rechtstreeks te koppelen aan objecten in een extern softwareproduct. Het object ObjectIntegration vertegenwoordigt deze koppeling.</p>
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
            <p><b> catObjCode </b> (koord)</p>
            <p>De volgende mogelijke waarde is toegevoegd:</p>
            <ul>
              <li>
                <p>GROEP (groep)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b> objTypes </b> (koord [])</p>
            <p>Toegevoegd.</p>
            <p style="font-weight: normal;">Deze parameter is een array van mogelijke objecten waaraan het aangepaste formulier kan worden gekoppeld. Deze is toegevoegd ter ondersteuning van de mogelijkheid om een aangepast formulier aan meerdere typen objecten te koppelen.</p>
            <p>Mogelijke waarden: </p>
            <p>CMPY, PORT, PRGM, PROJ, TASK, OPTASK, USER, DOCU, EXPNG, ITRN, BILL, GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
          <li>
            <p><b> objTypes </b> (koord [])</p>
            <p>Toegevoegd.</p>
            <p style="font-weight: normal;">Deze parameter is een array van mogelijke objecten waaraan het aangepaste formulier kan worden gekoppeld. Deze is toegevoegd ter ondersteuning van de mogelijkheid om een aangepast formulier aan meerdere typen objecten te koppelen.</p>
            <p>Mogelijke waarden: </p>
            <p>CMPY, PORT, PRGM, PROJ, TASK, OPTASK, USER, DOCU, EXPNG, ITRN, BILL, GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CategorieParameter (CTGYPA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> hideFormulaFromDescription </b>
            </p>
            <p>Toegevoegd.</p>
          </li>
          <li>
            <p><b> journaledObjCodes </b>
            </p>
            <p>Toegevoegd.</p>
          </li>
          <li>
            <p><b> rawCustomExpression </b>
            </p>
            <p>Toegevoegd.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CustomerPreferences (CUSTPR)

Een object CustomerPreferences vertegenwoordigt de set voorkeuren die een klant heeft ingesteld voor hun exemplaar van Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> naam </b>
            </p>
            <p>De volgende waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> (SharePoint (Graph API) Integration Enabled)</p>
                <p>Deze waarde ondersteunt de bijgewerkte integratie met SharePoint.</p>
              </li>
              <li>
                <p><code>project.mgmt:default.project.allowcreatewithouttemplate</code> (Gebruikers toestaan projecten te maken zonder een sjabloon te gebruiken)</p>
              </li>
              <li>
                <p><code>project.mgmt:taskissue.delegate</code> (config.taskissue.delegate)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder (DOCFDR)

Documenten kunnen in mappen worden ingedeeld. U kunt persoonlijke mappen maken in het gebied Persoonlijke documenten. Het object DocumentFolder vertegenwoordigt een van deze mappen.

Het object DocumentFolder heeft de markering `SHARABLE` toegevoegd.

### DocumentVersion (DOCV)

Een object DocumentVersion vertegenwoordigt een specifieke versie van een bestand (zoals geschreven materiaal, afbeeldingen of andere vormen van informatie).

Voor meer informatie over documentversies, zie [ een nieuwe versie van een document ](../../documents/managing-documents/upload-new-document-version.md) uploaden.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> externalIntegrationType </b>
            </p>
            <p>De volgende waarde is toegevoegd: </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API)</p>
                <p>Deze waarde ondersteunt de bijgewerkte integratie met SharePoint.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Groep (GROEP)

Een object Group vertegenwoordigt een set gebruikers en teams. Groepen vertegenwoordigen vaak de afdelingsstructuur.

Voor meer informatie over groepen, zie Groepen vs. teams.

Het Group-object heeft de vlag toegevoegd `DATA_EXTENDIBLE`

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <p>De volgende velden zijn toegevoegd:</p>
        <ul>
          <li>
            <p><b> categoryID </b>
            </p>
            <p>Een categorie is een aangepast formulier. Deze parameter is toegevoegd ter ondersteuning van de mogelijkheid om aangepaste Forms toe te voegen aan Group-objecten. </p>
          </li>
          <li>
            <p><b> isActive </b>
            </p>
            <p>Dit is een Booleaanse parameter die de waarde true heeft als een object Actief is en false als dit niet het geval is. Objecten die zijn ingesteld op Actief, worden weergegeven in vervolgkeuzemenu's en keuzelijsten die kunnen worden gekoppeld aan andere objecten.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referentievelden</td>
      <td >
        <p>De volgende velden zijn toegevoegd:</p>
        <ul>
          <li>
            <p><b> fiatteur </b>
            </p>
          </li>
          <li>
            <p><b> klant </b>
            </p>
          </li>
          <li>
            <p><b> aanvrager </b>
            </p>
          </li>
          <li>
            <p><b> gebruiker </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <p>De volgende velden zijn toegevoegd:</p>
        <ul>
          <li>
            <p><b> objectCategories </b>
            </p>
          </li>
          <li>
            <p><b> objectIntegrations </b>
            </p>
            <p>In sommige gevallen is het mogelijk om Workfront-werkitems rechtstreeks te koppelen aan objecten in een extern softwareproduct. Het object ObjectIntegration vertegenwoordigt deze koppeling.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Standaardvelden</td>
      <td >
        <p>Het volgende veld is toegevoegd:</p>
        <ul>
          <li>
            <p><b> isActive </b>
            </p>
            <p>Dit is een Booleaanse parameter die de waarde true heeft als een object Actief is en false als dit niet het geval is. Objecten die zijn ingesteld op Actief, worden weergegeven in vervolgkeuzemenu's en keuzelijsten die kunnen worden gekoppeld aan andere objecten.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <p>De volgende velden zijn toegevoegd:</p>
        <ul>
          <li>
            <p><b> calculateDataExtension </b>
            </p>
            <p>Met deze handeling worden de expressies in aangepaste formuliervelden opnieuw berekend.</p>
          </li>
          <li>
            <p><b> completeGroupInfo </b>
            </p>
          </li>
          <li>
            <p><b> linkExternalObject </b>
            </p>
          </li>
          <li>
            <p><b> unlinkExternalObject </b>
            </p>
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
        <p><b> changeType </b>
        </p>
        <p>De volgende waarde is toegevoegd: </p>
        <ul>
          <li>
            <p>DW (downloaden)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### LinkedFolder (LNKFDR)

Een object LinkedFolder vertegenwoordigt een map die is gekoppeld vanuit een externe documentprovider, zoals Google Drive of Dropbox.

Zie Documenten van externe toepassingen koppelen voor meer informatie over Gekoppelde mappen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> externalIntegrationType </b>
            </p>
            <p>De volgende waarde is toegevoegd: </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API)</p>
                <p>Deze waarde ondersteunt de bijgewerkte integratie met SharePoint.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OpTask/Issue (OPTASK)

Een voorwerp OpTask is algemeen genoemd als Kwestie. Een kwestie is een het werkpunt dat gewoonlijk wijst op een probleem verhinderend de voltooiing van een taak of een project. Een probleem kan ook een verzoek van de Helpdesk zijn. Wijzigingsorders, verzoeken en bugs zijn ook problemen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <p>De volgende acties zijn toegevoegd:</p>
        <ul>
          <li>
            <p><b> bulkMoveWithOptions </b>
            </p>
          </li>
          <li>
            <p><b> getRequestPath </b>
            </p>
          </li>
        </ul>
        <p>De volgende handeling is gewijzigd:</p>
        <ul>
          <li>
            <p><b> copyIssue </b>
            </p>
            <p>Toegevoegd veld <code>parentID</code></p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Parameter (PARAM)

Een object Parameter is een aangepast veld.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <p>Het volgende veld is toegevoegd:</p>
        <ul>
          <li>
            <p><b> fieldDefinition </b>
            </p>
          </li>
        </ul>
        <p>De volgende velden zijn gewijzigd:</p>
        <ul>
          <li>
            <p><b> dataType </b>
            </p>
            <p>De mogelijke waarde <code>WIDGET </code> (Widget) toegevoegd </p>
            <p>Deze waarde ondersteunt het gebruik van afbeeldingen in aangepaste formulieren.</p>
          </li>
          <li>
            <p><b> displayType </b>
            </p>
            <p>De mogelijke waarde <code>WIDGET </code> (Widget) toegevoegd</p>
            <p>Deze waarde ondersteunt het gebruik van afbeeldingen in aangepaste formulieren.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio (HAVEN)

Een object Portfolio is een verzameling projecten die concurreren om dezelfde bronnen, meestal geld of mensen om deze te voltooien.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
          <li>
            <p><b> objectIntegrations </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <ul>
          <li>
            <p><b> linkExternalObject </b>
            </p>
          </li>
          <li>
            <p><b> unlinkExternalObject </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Programma (PRGM)

Een programmaobject is een subset van projecten binnen een portfolio, waarin vergelijkbare projecten kunnen worden gegroepeerd.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
          <li>
            <p><b> objectIntegrations </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <ul>
          <li>
            <p><b> linkExternalObject </b>
            </p>
          </li>
          <li>
            <p><b> unlinkExternalObject </b>
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
            <p><b> resourcePlannerBudgetedHours </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referentievelden</td>
      <td >
        <ul>
          <li>
            <p><b> initiatief </b>
            </p>
            <p>Het object Initiative maakt in de Workfront Scenario Planner ramingen voor het soort en het aantal functies, de vaste kosten en het geplande voordeel. </p>
          </li>
          <li>
            <p><b> issueDef </b>
            </p>
          </li>
          <li>
            <p><b> taskDef </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
          <li>
            <p><b> objectIntegrations </b>
            </p>
            <p>In sommige gevallen is het mogelijk om Workfront-werkitems rechtstreeks te koppelen aan objecten in een extern softwareproduct. Het object ObjectIntegration vertegenwoordigt deze koppeling.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Een voorwerp QueueDef vertegenwoordigt een Rij, die een project is dat aan het gebied van de Desk van de Hulp is gepubliceerd om gebruikers toe te staan om kwesties aan het voor te leggen.

Voor meer informatie over de Rijen van het Verzoek, zie [ een Rij van het Verzoek ](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> requestorCoreAction </b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (teams bewerken waarop ik sta)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (teams bewerken in groepen die ik beheer (alleen groepbeheerders))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b> requestForForbiddenActions </b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (teams bewerken waarop ik sta)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (teams bewerken in groepen die ik beheer (alleen groepbeheerders))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Een ScoreCardQuestion-object vertegenwoordigt een vraag die aan een Scorecard is toegevoegd. Deze vragen worden gewoonlijk bepaald door de manager van het Portfolio, en hun antwoorden staan de manager toe om te begrijpen hoe goed een project zich op de doelstellingen van de portefeuille richt.

Voor meer informatie over Scorecard Vragen, zie [ een scorecard ](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md) creëren.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> displayType </b>
            </p>
            <p>De mogelijke waarde <code>WIDGET </code> (Widget) toegevoegd</p>
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
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
          <li>
            <p><b> objectIntegrations </b>
            </p>
            <p>In sommige gevallen is het mogelijk om Workfront-werkitems rechtstreeks te koppelen aan objecten in een extern softwareproduct. Het object ObjectIntegration vertegenwoordigt deze koppeling.</p>
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
      <td role="rowheader">Referentievelden</td>
      <td>
        <ul>
          <li>
            <p><b> issueDef </b>
            </p>
          </li>
          <li>
            <p><b> taskDef </b>
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
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Kernvelden</td>
      <td>
        <p>Het volgende veld is verwijderd:</p>
        <ul>
          <li>
            <p><b> objCode </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Weergave (UIVIEW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> uiviewType </b>
            </p>
            <p>De volgende mogelijke waarden zijn verwijderd:</p>
            <ul>
              <li>
                <p><code>FOUR_COL</code> (Lay-out met vier kolommen)</p>
              </li>
              <li>
                <p><code>UPDATES</code> (Updates)</p>
              </li>
              <li>
                <p><code>UPDATESTOOLBAR_FEED</code> (Updates)</p>
              </li>
              <li>
                <p><code>WORKINGON</code> (Werken aan)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA</code> (Aangepaste gegevens)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA_UPDATE</code> (Aangepaste gegevens bijwerken)</p>
              </li>
              <li>
                <p><code>STATUS_UPDATE</code> (Status bijwerken)</p>
              </li>
              <li>
                <p><code>OPTASK_STATUS_UPDATE</code> (Status bijwerken)</p>
              </li>
              <li>
                <p><code>PROJ_STATUS_UPDATE</code> (Status bijwerken)</p>
              </li>
              <li>
                <p><code>PROJECT_TIMEENTRY</code> (Status bijwerken)</p>
              </li>
              <li>
                <p><code>DLIST</code> (Detaillijst)</p>
              </li>
              <li>
                <p><code>DLIST_SECTION</code> (Sectie Detaillijst)</p>
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
            <p><b> updateType </b>
            </p>
            <p>De mogelijke waarde <code>documentVersionDownload </code> (enum.updatetypeenum.documentversiondownload) toegevoegd</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Gebruiker (GEBRUIKER)

Een object User vertegenwoordigt een persoon met een account in Workfront die zich kan aanmelden en met het systeem kan communiceren.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Referentievelden</td>
      <td>
        <ul>
          <li>
            <p><b> userApproval </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Handelingen</td>
      <td>
        <ul>
          <li>
            <p><b> getUsersAvailableTime </b>
            </p>
          </li>
          <li>
            <p><b> resetRopgPassword </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserNote (USRNOT)

Een object UserNote is een melding.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Directe velden</td>
      <td>
        <ul>
          <li>
            <p><b> eventType </b>
            </p>
            <p>De volgende mogelijke waarden zijn toegevoegd:</p>
            <ul>
              <li>
                <p><code>DUP </code>(Gevraagd dat u een document bewijst)</p>
              </li>
              <li>
                <p><code>DUV </code>(Toestaan dat u een document weergeeft)</p>
              </li>
            </ul>
          </li>
        </ul>
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
      <td role="rowheader">Verzamelingsvelden</td>
      <td>
        <ul>
          <li>
            <p><b> objectIntegrations </b>
            </p>
            <p>In sommige gevallen is het mogelijk om Workfront-werkitems rechtstreeks te koppelen aan objecten in een extern softwareproduct. Het object ObjectIntegration vertegenwoordigt deze koppeling.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
