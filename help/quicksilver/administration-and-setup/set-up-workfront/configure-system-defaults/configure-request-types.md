---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Aanvraagtypen configureren
description: Tijdens het werken aan een project, zou u kunnen ontdekken dat de onverwachte gebeurtenissen zich voordoen. U kunt die onverwachte gebeurtenissen als kwesties voor een bepaald project of een taak registreren. U kunt verzoeken ook voorleggen, die als kwesties op een project worden geregistreerd dat als Rij van het Verzoek wordt aangewezen. Kwesties en verzoeken worden in Adobe Workfront als onderling verwisselbaar beschouwd.
author: Lisa, Becky
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: 31e5f5e039e25fa25f3038c23ee579ba1f830bb7
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Aanvraagtypen configureren

Tijdens het werken aan een project, zou u kunnen ontdekken dat de onverwachte gebeurtenissen zich voordoen. U kunt die onverwachte gebeurtenissen als kwesties voor een bepaald project of een taak registreren. U kunt verzoeken ook voorleggen, die als kwesties op een project worden geregistreerd dat als Rij van het Verzoek wordt aangewezen. Kwesties en verzoeken worden in Adobe Workfront als onderling verwisselbaar beschouwd.

Voor informatie over het creëren van kwesties in [!DNL Workfront], zie [ kwesties ](../../../manage-work/issues/manage-issues/create-issues.md) creëren. Voor informatie over het creëren van verzoeken in [!DNL Workfront], zie [  [!DNL Adobe Workfront]  verzoeken ](../../../manage-work/requests/create-requests/create-submit-requests.md) creëren en voorleggen. Voor informatie over het associëren van de Types van Verzoek met projecten, zie [ de Types van Verzoek voor een project ](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md) bepalen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licentie</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
THIS IS DRAFTED IN FLARE
<h2>Set what issue or request types are allowed for a project</h2>
<p>You can organize the kind of issues or requests that are logged in Workfront by Request Types. This organization is useful for reporting reasons and for helping users understand what kind of unexpected work might occur during the lifetime of a project.</p>
<p>You can specify the type of requests that can be logged on a project when you configure the <strong>Queue Details</strong> area for the project. </p>
<ol>
<li value="1"> <p> Click <strong>Projects</strong> in the Main Menu. <img src="assets/main-menu-icon.png"> </p> </li>
<li value="2">Click the name of the project to open it.</li>
<li value="3"> In the left panel, click <strong>Queue Details</strong>. </li>
<li value="4"> <p>In the <strong>Queue Properties</strong> section, select the <strong>Request Types</strong> you want for the project.</p> <note type="note">
You must have at least one request type selected. You can select multiple request types.
</note> </li>
<li value="5"> <p>Click <strong>Save</strong>.</p> <p>The request types you specified will be available to select when you enter a new issue on a task or a project, or when you submit a new request to the project.</p> </li>
</ol>
</div>
-->

## De namen van de aanvraagtypen aanpassen

Als [!DNL Workfront] beheerder, kunt u de namen van de verzoektypes in uw systeem vormen. De nieuwe namen zijn zichtbaar in elk gebied van [!DNL Workfront] waar de **[!UICONTROL Issue Type]** - of **[!UICONTROL Request Type]** -velden worden weergegeven:

* In het **[!UICONTROL Queue Details]** -gebied van een project dat de problemen of aanvragen ontvangt.
* Als er meer dan één aanvraagtype is geselecteerd voor een aanvraagwachtrij, gaat u in het veld **[!UICONTROL New Issue]Formulier** in het veld **[!UICONTROL Issue Type]** naar een nieuwe uitgave of een nieuwe aanvraag.

  Voor meer informatie over het creëren van kwesties in [!DNL Workfront], zie [ kwesties ](../../../manage-work/issues/manage-issues/create-issues.md) creëren

  Voor meer informatie over het creëren van verzoeken in [!DNL Workfront], zie [ creëren en voorleggen  [!DNL Adobe Workfront]  verzoeken ](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Op het **[!UICONTROL Queue Topic Detail]** formulier, wanneer u het onderwerp van de wachtrij configureert.\
   Voor meer informatie over het creëren van de Onderwerpen van de Rij, zie [ de Onderwerpen van de Rij ](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) creëren.

U kunt als volgt de namen van de aanvraagtypen aanpassen:

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Project Preferences]** > **[!UICONTROL Statuses]** .

1. Klik op de tab **[!UICONTROL Issues]** .
1. Klik boven aan het tabblad **[!UICONTROL Issues]** op het vervolgkeuzemenu, selecteer een type dat u zoekt en klik op het pictogram **[!UICONTROL Edit]** dat wordt weergegeven.

   ![ geef verzoektype naam ](assets/edit-request-type-name-nwe.png) uit

1. Typ een nieuwe naam in het vak dat wordt weergegeven en druk op **[!UICONTROL Enter]** .

## Uitgavestatus binnen verschillende aanvraagtypen configureren

U kunt elk aanvraagtype aan verschillende uitgavestatussen koppelen. U kunt ook de volgorde wijzigen waarin de statussen op een uitgave worden weergegeven, afhankelijk van het type uitgave.

Voor meer informatie over het veranderen van de standaardorde van uitgevende statussen en het vormen van uitgavestatus, zie [ een status ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) sectie in [ creëren of uitgeven een status ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
