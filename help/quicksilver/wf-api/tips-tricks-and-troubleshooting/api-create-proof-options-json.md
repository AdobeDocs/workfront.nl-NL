---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Geavanceerde opties voor proefdrukken toevoegen met Adobe Workfront API
description: Geavanceerde opties voor proefdrukken toevoegen met Adobe Workfront API
author: Becky
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---


# Geavanceerde opties voor proefdrukken toevoegen bij het maken van een proefdruk via de Adobe Workfront API

Als u een proefdruk maakt in de Workfront API, kunt u geavanceerde proefdrukopties toevoegen.

Gebruik een van de volgende workflows om proefdrukopties aan een proefdruk toe te voegen met behulp van de API:

* (Aanbevolen) Maak een eenvoudige proefdruk met de Workfront API en voeg vervolgens geavanceerde proefdrukopties toe aan de proefdruk met de API ProefHQ

* Een proefdruk maken met geavanceerde opties voor proefdrukken met JSON in de Workfront API

## Een proefdruk maken met de API&#39;s Workfront en ProofHQ (aanbevolen) {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

In deze sectie wordt beschreven hoe u een proefdruk maakt met geavanceerde opties voor proefdrukken via de Workfront API, met behulp van een combinatie van Workfront- en ProofHQ-API&#39;s.

De API ProofHQ bevat een aantal acties die niet beschikbaar zijn voor proefdrukken in de Workfront API. Door deze acties te gebruiken, kunt u de proef wijzigen of vormen met nauwkeuriger dan beschikbaar in Workfront API.

Voor een overzicht van API ProofHQ, zie het [ Overzicht PoofHQ ](../../proofhq-api/general/overview.md). U kunt ook naar de [ Documentatie ProofHQ ](https://api.proofhq.com/home.html) verwijzen.

>[!NOTE]
>
>* De Workfront API is een REST-ful API. De API ProofHQ is een SOAP API.
>* Proofs die zijn gemaakt in de API ProefHQ worden niet automatisch gekoppeld aan Workfront. Daarom raden we u aan proefdrukken te maken in de Workfront API voordat u ze bijwerkt met de API ProofHQ.
>

### Een proefdruk maken met geavanceerde opties voor proefdrukken

1. Maak een proefdruk met de handeling `Document createProof` in de Workfront API.

   >[!NOTE]
   >
   >Wanneer u de proefdruk maakt, stelt u `{}` in als de waarde voor de parameter `advancedProofingOptions` .

1. Nadat de proefdruk is gemaakt, gebruikt u de API ProofHQ om geavanceerde opties toe te voegen.

### Voorbeelden

In deze sectie worden enkele voorbeeldupdates weergegeven die u kunt maken met de API ProofHQ.

**Voorbeelden:**

* [ A Bewijs kan worden gedownload, heeft een bericht, en wordt openbaar gedeeld ](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [ werk een stadium bij zodat het niet privé, niet verplicht is, en vereist slechts één goedkeuring ](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [Twee ontvangers toevoegen aan een bewijs zonder primaire beslisser](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**A Bewijs kan worden gedownload, heeft een bericht, en wordt openbaar gedeeld**

De documentatie voor dit eindpunt kan op [ ProofHQ API updateProof ](https://api.proofhq.com/home/proofs/updateproof.html) pagina worden gevonden.

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateProof>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{file_id}}</FileID>
            <OwnerID>0</OwnerID>
            <Name>{{proof_name}}}</Name>
            <Subject>Email subject here</Subject>
            <Message>Email message here</Message>
            <EnableDownload>true</EnableDownload>
            <EnableTeamURL>true</EnableTeamURL>
        </soap:updateProof>
    </soapenv:Body>
</soapenv:Envelope>
```

**werk een stadium bij zodat het niet privé, niet verplicht is, en vereist slechts één goedkeuring**

De documentatie voor dit eindpunt kan op de [ ProofHQ API updateWorkflowProofStage ](https://api.proofhq.com/updateworkflowproofstage.html) pagina worden gevonden.

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateWorkflowProofStage>
        <SessionID>{{session_id}}</SessionID>
        <FileID>{{proof_id}}</FileID>
        <Stage>
            <stage_id>{{stage_id}}</stage_id>
            <name>{{stage_name}}</name>
                <stage_one_decision_only>true</stage_one_decision_only>
                <stage_private>false</stage_private>
                <mandatory>false</mandatory>
            </Stage>
        </soap:updateWorkflowProofStage>
    </soapenv:Body>
</soapenv:Envelope>
```

**voeg twee ontvangers aan een bewijs zonder primaire besluitvormer toe**

De documentatie voor dit eindpunt kan op [ ProofHQ API addWorkflowProofReviewers ](https://api.proofhq.com/addworkflowproofreviewers.html) pagina worden gevonden.

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:addWorkflowProofReviewers>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{proof_id}}</FileID>
            <Recipients>
                <item>
                <email>{{recipient_email_1}}</email>
                <role>5</role>
                <name>{{recipient_name_1}}</name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
                <item>
                <email> {{recipient_email_2}} </email>
                <role>5</role>
                <name> {{recipient_name_2}} </name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
            </Recipients>
            <SuppressNewProofNotification></SuppressNewProofNotification>
        </soap:addWorkflowProofReviewers>
    </soapenv:Body>
</soapenv:Envelope>
```

## Een proefdruk maken met JSON in de Workfront API

In deze sectie wordt beschreven hoe u een proefdruk maakt met geavanceerde opties voor proefdrukken via de Workfront API en JSON gebruikt als parameterwaarde in de Workfront API

### Een proefdruk maken met geavanceerde opties voor proefdrukken

Met de handeling `Document createProof` kunt u proefdrukken maken via de Workfront API. Deze handeling accepteert de parameter `advancedProofingOptions` , die het waardetype `string` heeft. Als u geavanceerde proefdrukopties wilt opnemen in de `createProof` -actie, moet u de opties in de `advancedProofingOptions` -parameter invoeren in JSON-indeling.

>[!NOTE]
>
>Het kan moeilijk zijn om de gebieden te voorspellen om in uw advancedProofingOptions JSON te omvatten. U kunt de netwerkgegevens van uw organisatie willen onderzoeken terwijl het gebruiken van geavanceerd proef in Workfront, en uw JSON baseren op de gebieden en de waarden die algemeen door uw organisatie worden gebruikt.
>
>Omdat deze velden moeilijk te voorspellen zijn, raden we u aan een proefdruk te maken met de Workfront API en deze vervolgens bij te werken met de ProofHQ-API. Voor meer informatie, zie [ een proef creëren gebruikend Workfront en ProofHQ APIs (Geadviseerd) ](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended) in dit artikel

### Voorbeeld

In dit voorbeeld worden velden en opmaak weergegeven die u kunt gebruiken bij het maken van uw JSON voor de parameter `advancedProofingOptions` . Uw `advancedProofingOptions` JSON-bestand kan meer of minder velden hebben dan hier wordt weergegeven.

**Voorbeeld:**

<!-- [Copy](javascript:void(0);) -->

```
{
    "stages": [
        {
            "name": "stage1",
            "lockOn": 1,
            "position": 1,
            "isPrivate": false,
            "activateOn": 1,
            "recipients": [
                {
                    "name": "",
                    "role": 5,
                    "email": "user1_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": null
                },
                {
                    "name": "",
                    "role": 5,
                    "email": "user2_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": false
                }
            ],
            "isMandatory": false,
            "deadlineDate": null,
            "deadlineTime": null,
            "isOneApproval": true,
            "activateOnDate": null,
            "parentPosition": null,
            "activateOnDecision": null,
            "deadlineCalculateOn": null,
            "deadlineBusinessDays": null
        }
    ],
    "message": "",
    "subject": "",
    "templates": [],
    "hasMessage": true,
    "canDownload": true,
    "customfields": [],
    "hasPublicSharing": true,
    "isAutomatedWorkflow": true,
    "stageBasedVisibility": 0
}
```
