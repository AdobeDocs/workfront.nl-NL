---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: connections-annd-webhooks
title: Verbindingen maken in [!DNL Adobe Workfront Fusion]
description: Een verbinding moet voldoen aan de vereisten die zijn ingesteld door de API van de app of webservice waarmee de verbinding wordt gemaakt. Daarom zijn de instructies voor het instellen van een verbinding afhankelijk van de app of webservice. Dit artikel kan u helpen de instructies voor het verbinden identificeren en vinden [!DNL Adobe Workfront Fusion] naar de door u gekozen app of webservice.
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# Verbindingen maken in [!DNL Adobe Workfront Fusion]

Een verbinding moet voldoen aan de vereisten die zijn ingesteld door de API van de app of webservice waarmee de verbinding wordt gemaakt. Daarom zijn de instructies voor het instellen van een verbinding afhankelijk van de app of webservice. Dit artikel kan u helpen de instructies voor het verbinden identificeren en vinden [!DNL Adobe Workfront Fusion] naar de door u gekozen app of webservice.

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td>

</tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Verbinden [!DNL Adobe Workfront] tot [!DNL Workfront Fusion]

Workfront en [!DNL Workfront Fusion] zijn ontworpen om samen te werken. De verbinding die u maakt, bepaalt de account die [!DNL Workfront Fusion] gebruiken om handelingen uit te voeren in Workfront.

Zie voor instructies [Verbinden [!DNL Workfront] tot [!DNL Workfront Fusion]](../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect) in [[!DNL Adobe Workfront] modules](../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

## Verbinding maken met een app of webservice waarvoor geen configuratie is vereist

In de meeste gevallen kunt u de module gebruiken om een verbinding te maken met weinig of geen extra informatie. [!DNL Workfront Fusion] handelt de authentificatie automatisch af.

Voor instructies over het maken van een verbinding zonder speciale overwegingen raadpleegt u [Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies](../../workfront-fusion/connections/connect-to-fusion-general.md).

## Verbinding maken met een [!DNL Microsoft] app of webservice

De meeste [!DNL Microsoft] apps in [!DNL Workfront Fusion] kunt u zonder extra informatie een verbinding maken.

De volgende omstandigheden vereisen extra stappen bij het maken van een verbinding:

* Gebruiken [!DNL Microsoft Dynamics 365] modules.

   Zie voor instructies [[!DNL Microsoft Dynamics 365] modules](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

* Verbinding maken met de [!DNL Microsoft Graph API] met een [!UICONTROL HTTP] module

   Zie voor instructies [Roep de [!DNL MS Graph REST API] via de [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module](../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md).

## Verbinding maken met een [!DNL Google] app of webservice

Het proces voor verbinding maken met [!DNL Google] apps kunnen verschillen op basis van het type [!DNL Google] account die u gebruikt. Daarnaast [!DNL Google] beveiligingsmaatregelen vereisen mogelijk een extra configuratie wanneer u verbinding maakt met [!DNL Workfront Fusion].

Zie voor meer informatie:

* [Verbinden [!DNL Adobe Workfront Fusion] tot [!DNL Google Services] een aangepaste OAuth-client gebruiken](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [Verbinden [!DNL Adobe Workfront Fusion] tot [!DNL Google Services] met bijgewerkte veiligheidsmaatregelen](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## Andere toepassingen waarvoor aanvullende configuratie vereist is

De volgende apps volgen de basisconfiguratie niet voor [!DNL Workfront Fusion] verbindingen. U vindt instructies voor het verbinden van deze apps in het artikel voor die app.

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>App-/webservice</th> 
   <th>Aanvullende informatie over verbindingen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref">Verbinden [!DNL Adobe Workfront] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref">Verbinden [!DNL Allocadia] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref">Verbinden [!DNL Anaplan] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan] modules</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref">Verbinden [!DNL AWS] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref">Verbinden [!DNL Azure DevOps] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref">Verbinden [!DNL Bynder] tot [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref">Verbinden [!DNL CloudConvert] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert] modules</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref">Verbinden [!DNL Cvent] tot [!DNL Adobe Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref">Verbinden [!DNL Datadog] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref">Verbinden [!DNL DocuSign] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>E-mail</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref">Uw e-mail verbinden met [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref">[!UICONTROL Email] modules</a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref">Verbinden [!DNL Gmail] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Intacct]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/intacct-modules.md#connecti" class="MCXref xref">Verbinden [!DNL Intacct] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/intacct-modules.md" class="MCXref xref">[!DNL Intacct] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref">Verbinden [!DNL Jira Cloud] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref">Verbinden [!DNL Jira Server] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">Verbinden [!DNL MariaDB] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">Verbinden [!DNL Marketo] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">Verbinding maken [!DNL Qualtrics] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">Verbinden [!DNL ServiceNow] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">SFTP verbinden met [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref">[!UICONTROL SFTP] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">Verbinden [!DNL SharePoint] tot [!DNL Workfront Fusion]</a> in <a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">Verbinden [!DNL Split.io] tot [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io] modules</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Breiden</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">Verbinden [!DNL Widen] tot [!DNL Workfront Fusion] </a> in <a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen] modules</a></td> 
  </tr> 
 </tbody> 
</table>
