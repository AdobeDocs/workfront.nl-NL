---
content-type: api
navigation-topic: general-api
title: Abonnementsversie voor gebeurtenis
description: API voor abonnementen voor gebeurtenissen
author: Becky
feature: Workfront API
role: Developer
exl-id: 151b9d0d-0dd6-4ece-9601-dda04356b436
source-git-commit: f34f48d974db200d9ce1815c805885707ab27f6d
workflow-type: tm+mt
source-wordcount: '1288'
ht-degree: 0%

---

# Abonnementsversie voor gebeurtenissen

Workfront heeft twee versies van gebeurtenisabonnementen. In dit artikel worden de verschillen tussen de koppelingen beschreven.

De nieuwe versie is geen wijziging in de Workfront API, maar een wijziging in de functionaliteit voor abonnementen voor gebeurtenissen.

De capaciteit om gebeurtenisabonnementen te bevorderen of te degraderen zorgt ervoor dat wanneer de veranderingen in de structuur van gebeurtenissen worden aangebracht, de bestaande abonnementen niet breken, toestaand u om aan de nieuwe versie zonder een hiaat in uw gebeurtenisabonnement te testen en te bevorderen.


Wanneer u uw gebeurtenissenabonnement upgradet of downloadt naar een andere versie, ontvangt u dubbele gebeurtenissen voor elke gebeurtenislevering gedurende een venster van vijf minuten na de versiewijziging. De duplicaten bevatten een van de versies 1 en 2 van het gebeurtenisabonnement. Dit zorgt ervoor dat u geen gebeurtenissen mist toe te schrijven aan het veranderen van de versie van het gebeurtenisabonnement.

Voor informatie over de eindpunten die voor bevordering of het degraderen van gebeurtenisabonnementen worden gebruikt, zie [&#x200B; het abonnement van de Gebeurtenis versioning &#x200B;](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) in het abonnement API van de artikelgebeurtenis.

>[!IMPORTANT]
>
>De volgende releases zijn van invloed op het versiebeheer van abonnementen voor gebeurtenissen:
>
>* **25.2 Versie** (10 April, 2025): Alle nieuwe abonnementen die na de versie 25.2 worden gecreeerd worden gecreeerd als Versie 2.
>* **Januari 15, 2026**: Alle resterende versies 1 abonnementen worden gemigreerd aan Versie 2.

## Wijzigingen tussen versie 1 en versie 2

De volgende wijzigingen zijn aangebracht voor gebeurtenisabonnementen versie 2:


### Algemene wijzigingen


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><b>Betrokken velden</b></p> </th> 
   <th> <p><b>Versie 1 (vorig gedrag)</b></p> </th> 
   <th> <p><b>Versie 2 (wijzigen)</b></p> </th> 
   <th> <p><b>Actie tot herstel</b></p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Berekende parameterwaarden</p> </td> 
   <td> <p>Elk object dat is gemaakt op basis van een sjabloon dat een aangepast formulier met berekende parameterwaarden bevat, wordt een gebeurtenis <code>CREATE</code> verzonden en vervolgens wordt een <code>UPDATE</code> verzonden met de parameterwaarden (inclusief berekende velden en de waarden ervan). </p> </td> 
   <td> <p>Wanneer een object wordt gemaakt op basis van een sjabloon die een aangepast formulier met berekende parameterwaarden bevat, wordt alleen een <code>CREATE</code> -gebeurtenis verzonden die parameterwaarden bevat, inclusief berekende velden.</p> </td> 
   <td> <p>Als u een abonnement op <code>UPDATE</code> -gebeurtenissen hebt en verwacht dat u een <code>UPDATE</code> -gebeurtenis ontvangt nadat een object met berekende parameterwaarden is gemaakt, ontvangt u niet langer die <code>UPDATE</code> -gebeurtenis. Als u berekende parameterwaarden wilt zien bij het maken van objecten, moet u een extra <code>CREATE</code> -abonnement maken.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tekstvelden met meerdere selecties</p> </td> 
   <td> <p>Voor elk type gebeurtenis dat een wijziging bevat op een tekstveld met meerdere selecties geldt dat als het veld slechts één waarde bevat, deze waarde wordt omgezet in en verzonden als een tekenreeks. Anders wordt het als een array verzonden. </p><p>Voorbeelden:</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> wordt geconverteerd en verzonden als <code>myMultiSelectField: "oneValue"</code> .</li><li><code>myMultiSelectField: ["first", "second"]</code> wordt verzonden als <code>myMultiSelectField: ["first", "second"]</code>.</li></ul> </td> 
   <td> <p>Ongeacht het aantal waarden in de array, wordt deze als een array verzonden. </p><p>Voorbeelden:</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> wordt verzonden als <code>myMultiSelectField: ["oneValue"]</code>.</li><li><code>myMultiSelectField: ["first", "second"]</code> wordt verzonden als <code>myMultiSelectField: ["first", "second"]</code>.</li></ul> </td> 
   <td> <p>Als u een abonnement hebt met een filter op een veld met meerdere keuzen en de waarde als tekenreeks, moet u een nieuw abonnement maken met hetzelfde filter dat de waarde als een array heeft. </p> </td> 
  </tr> 
 </tbody> 
</table>

### Objectspecifieke wijzigingen

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <b> de code van Objecten </b> </th> 
   <th> <b> Betrokken gebieden </b> </th> 
   <th> <b> Versie 1 (Vorig gedrag) </b></th> 
   <th> <b> Versie 2 (Verandering) </b> </th> 
   <th> <b> de actie van de Vergoeding </b> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th rowspan="1">ASSGN</th> 
   <td>
    <ul>
     <li><code>projectID</code></li>
     <li><code>taskID</code></li>
     <li><code>opTaskID</code></li>
     <li><code>customerID</code></li>
    </ul> 
   </td> 
   <td>Wanneer dit object is bijgewerkt, geeft de gebeurtenis <code>UPDATE</code> soms ten onrechte aan dat de desbetreffende velden zijn gewijzigd van <code>null</code> in <code>ID value</code> .</td> 
   <td>Alle <code>UPDATE</code> -gebeurtenissen geven de juiste waarde voor de desbetreffende velden aan.</td> 
   <td>Geen. Als u een filter op de betrokken gebieden hebt, ontvangt u een gebeurtenis <code>UPDATE</code> slechts als deze gebieden werkelijk zijn veranderd, niet als een andere waarde is veranderd.
   </td> 
  </tr> 
  <tr> 
   <th rowspan="2">DOCU</th> 
   <td>
    <ul>
     <li><code>referenceObjID</code></li>
    </ul> 
   </td> 
   <td>Wanneer een parameterwaarde op dit object is bijgewerkt, geeft de gebeurtenis <code>UPDATE</code> een onjuiste wijziging van het desbetreffende veld van <code>null</code> in <code>object id</code> weer. </td> 
   <td>Alle <code>UPDATE</code> -gebeurtenissen geven de juiste waarde voor de desbetreffende velden aan.</td> 
   <td>Geen. Als u een filter op de betrokken gebieden hebt, ontvangt u een gebeurtenis <code>UPDATE</code> slechts als deze gebieden werkelijk zijn veranderd, niet als een andere waarde is veranderd.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>groups</code></li>
    </ul> 
   </td> 
   <td>Wanneer een document is verwijderd, wordt het desbetreffende veld door de gebeurtenis <code>DELETE</code> onjuist weergegeven als een lege array in de status voor.    </td> 
   <td>De gebeurtenis <code>DELETE</code> geeft het desbetreffende veld correct vóór de status weer.</td> 
   <td>Geen. De gebeurtenis <code>DELETE</code> wordt wel verzonden, maar nu worden de juiste gegevens voor het desbetreffende veld weergegeven. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">DOCV</th> 
  <td>
    <ul>
     <li><code>proofDecision</code></li>
     <li><code>proofName</code></li>
     <li><code>proofProgress</code></li>
    </ul> 
   </td> 
   <td>Wanneer dit object werd bijgewerkt, worden twee <code>UPDATE</code> -gebeurtenissen verzonden. Het eerste veld bevatte niet de betrokken velden, terwijl het tweede evenement dat wel deed.</td> 
   <td>Alle veldupdates, inclusief de betrokken velden, zijn aanwezig in slechts één <code>UPDATE</code> -gebeurtenis en er wordt geen tweede onnodige gebeurtenis verzonden.     </td> 
   <td>Geen. Als u een filter op de betrokken gebieden hebt, worden de gebeurtenissen geleverd in de eerste gebeurtenis. 
</td> 
  </tr> 
  <tr> 
   <th rowspan="2">EXPNS</th> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>Wanneer een willekeurige parameterwaarde op een kostenwaarde is bijgewerkt, heeft de gebeurtenis <code>UPDATE</code> een onjuiste wijziging van topReferenceObjCode van <code>EXPNS</code> naar <code>PROJ</code> getoond en wordt <code>referenceObjectName</code> gewijzigd van <code>null</code> naar <code>string value of project name</code> .      </td> 
   <td>Alle <code>UPDATE</code> -gebeurtenissen geven de juiste waarde voor de desbetreffende velden aan.</td> 
   <td>Geen. Als u een filter op de betrokken gebieden hebt, ontvangt u een gebeurtenis <code>UPDATE</code> slechts als deze gebieden werkelijk zijn veranderd, niet als een andere waarde is veranderd.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>Wanneer een object Expense werd verwijderd, werd een gebeurtenis <code>UPDATE</code> verzonden waarbij de betrokken velden werden gewijzigd in null voordat de gebeurtenis <code>DELETE</code> werd verzonden.    </td> 
   <td>De extra <code>UPDATE</code> -gebeurtenis wordt niet verzonden. De gebeurtenis <code>DELETE</code> heeft juiste waarden voor de desbetreffende velden in de status vóór. </td> 
   <td>Als u een filter hebt voor de desbetreffende velden op <code>UPDATE</code> -gebeurtenissen en verwacht dat u dit filter ontvangt wanneer het object wordt verwijderd, ontvangt u niet langer de gebeurtenis <code>UPDATE</code> . Als u deze velden wilt zien wanneer het object wordt verwijderd, moet u een extra abonnement voor <code>DELETE</code> maken.
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">UUR</th> 
  <td>
    <ul>
     <li><code>projectID </code></li>
     <li><code>taskID </code></li>
     <li><code>roleID</code></li>
     <li><code>timesheetID</code></li>
     <li><code>hourTypeID </code></li>
     <li><code>projectOverheadID</code></li>
     <li><code>referenceObjID</code></li>
     <li><code>referenceObjCode</code></li>
     <li><code>securityRootID</code></li>
    </ul> 
   </td> 
   <td>Wanneer dit object is verwijderd, worden de desbetreffende velden door de gebeurtenis <code>DELETE</code> onjuist weergegeven als <code>null</code> in de status voor. </td> 
   <td>De gebeurtenis <code>DELETE</code> geeft de desbetreffende velden correct weer in de toestand Voor.</td> 
   <td>Geen. De gebeurtenis <code>DELETE</code> wordt nog steeds verzonden, maar geeft nu de juiste gegevens voor de desbetreffende velden weer. </td> 
  </tr> 
  <tr> 
   <th rowspan="2">OPTASK</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>Wanneer een parameterwaarde op dit object is bijgewerkt, geeft de gebeurtenis <code>UPDATE</code> een onjuiste wijziging van het desbetreffende veld van <code>null</code> in <code>ID value</code> weer. </td> 
   <td>Alle <code>UPDATE</code> -gebeurtenissen geven de juiste waarde voor het desbetreffende veld aan.</td> 
   <td>Geen. Als u een filter op het beïnvloede gebied hebt, ontvangt u een <code>UPDATE</code> gebeurtenis slechts als dat gebied eigenlijk is veranderd, niet als een andere parameterwaarde is veranderd.
</td> 
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>resolveProjectID</code></li>
     <li><code>resolveTaskID</code></li>
     <li><code>resolvingObjID</code></li>
    </ul> 
   </td> 
   <td>Wanneer dit object is bijgewerkt, geeft de gebeurtenis <code>UPDATE</code> soms ten onrechte aan dat de desbetreffende velden zijn gewijzigd van <code>null</code> in <code>ID value</code> .</td> 
   <td>In alle <code>UPDATE</code> -gebeurtenissen wordt de juiste waarde voor de desbetreffende velden weergegeven.    </td> 
   <td></td> 
  </tr> 
  <tr> 
   <th rowspan="2">PROJ</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   <td>Wanneer een parameterwaarde op dit object is bijgewerkt, geeft de gebeurtenis <code>UPDATE</code> een onjuiste wijziging van het desbetreffende veld van <code>null</code> in <code>ID value</code> weer. </td> 
   <td>Alle <code>UPDATE</code> -gebeurtenissen geven de juiste waarde voor het desbetreffende veld aan.</td> 
   <td>Geen. Als u een filter op het beïnvloede gebied hebt, ontvangt u een <code>UPDATE</code> gebeurtenis slechts als dat gebied eigenlijk is veranderd, niet als een andere parameterwaarde is veranderd.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>Wanneer dit object is bijgewerkt, geeft de gebeurtenis <code>UPDATE</code> soms ten onrechte aan dat de desbetreffende velden zijn gewijzigd van <code>null</code> in <code>ID value</code> .</td> 
   <td>Alle <code>UPDATE</code> -gebeurtenissen geven de juiste waarde voor het desbetreffende veld aan.</td> 
   <td>Geen. Als u een filter op het beïnvloede gebied hebt, ontvangt u een <code>UPDATE</code> gebeurtenis slechts als dat gebied eigenlijk is veranderd, niet als een andere parameterwaarde is veranderd.
  </tr> 
  <tr> 
   <th rowspan="2">TAAK</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>Wanneer een parameterwaarde op dit object is bijgewerkt, geeft de gebeurtenis <code>UPDATE</code> een onjuiste wijziging van het desbetreffende veld van <code>null</code> in <code>ID value</code> weer. </td> 
   <td>Alle <code>UPDATE</code> -gebeurtenissen geven de juiste waarde voor het desbetreffende veld aan.</td> 
   <td>Geen. Als u een filter op het beïnvloede gebied hebt, ontvangt u een <code>UPDATE</code> gebeurtenis slechts als dat gebied eigenlijk is veranderd, niet als een andere parameterwaarde is veranderd.
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>Wanneer dit object is bijgewerkt, geeft de gebeurtenis <code>UPDATE</code> soms ten onrechte aan dat de desbetreffende velden zijn gewijzigd van <code>null</code> in <code>ID value</code> .</td> 
   <td>Alle <code>UPDATE</code> -gebeurtenissen geven de juiste waarde voor het desbetreffende veld aan.</td> 
   <td>Geen. Als u een filter op het beïnvloede gebied hebt, ontvangt u een <code>UPDATE</code> gebeurtenis slechts als dat gebied eigenlijk is veranderd, niet als een andere parameterwaarde is veranderd.
 </tbody> 
</table>


## De versie van het gebeurtenisabonnement in een scenario van Workfront Fusion bijwerken

Workfront Fusion gebruikt gebeurtenisabonnementen om op veranderingen in Workfront te letten om scenario&#39;s teweeg te brengen. U kunt de versie van de gebeurtenisbeschrijving die Fusion direct in een scenario gebruikt bijwerken, gebruikend Workfront > de module van de Versie van de Payload van Gebeurtenissen bijwerken.

Voor instructies bij het gebruiken van deze module, zie [&#x200B; modules van Workfront &#x200B;](https://experienceleague.adobe.com/nl/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules) in de documentatie van de Fusie van Workfront.

Voor middelen bij het bewaren van uw scenario&#39;s van de Fusie van Workfront tijdens de verbetering van het gebeurtenisabonnement, met inbegrip van een webinar opname, zie [&#x200B; het Behouden van Uw Scenario&#39;s van de Fusie tijdens de Verbetering van de Abonnementen V2 van de Gebeurtenis &#x200B;](https://experienceleaguecommunities.adobe.com/t5/workfront-discussions/event-follow-up-preserving-your-fusion-scenarios-during-the/td-p/754182?profile.language=nl).
