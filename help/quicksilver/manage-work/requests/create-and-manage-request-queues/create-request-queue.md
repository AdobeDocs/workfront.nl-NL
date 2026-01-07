---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Een aanvraagwachtrij maken
description: U kunt opstelling een Rij van het Verzoek waar de gebruikers occasionele verzoeken kunnen ingaan die niet gepland werk aan een project zijn. Bijvoorbeeld, kan een rij van het hulpdeskverzoek opstelling zijn om alle gebruikersverzoeken te vangen die aan een afdeling van IT komen.
author: Becky
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '2843'
ht-degree: 0%

---


# Een aanvraagwachtrij maken

<!--Audited: 12/2023-->

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

<!--hide/ comment out the entire "create requests in Production" section and just edit and leave  only the preview section when it releases to Production; also remove the template blurb when the queue details is unshimmed for templates-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


U kunt opstelling een Rij van het Verzoek waar de gebruikers occasionele verzoeken kunnen ingaan die niet gepland werk aan een project zijn. Bijvoorbeeld, kan een rij van het hulpdeskverzoek opstelling zijn om alle gebruikersverzoeken te vangen die aan een afdeling van IT komen.

Verzoeken worden kwesties in Adobe Workfront en ze worden toegevoegd aan projecten.

Het opzetten van een verzoekrij helpt informatie over kwesties formaliseren die aan een project zullen worden toegevoegd. Alle kwesties die aan het project worden voorgelegd zullen op dezelfde wijze worden voorgelegd en zullen dezelfde weg naar voltooiing volgen.

U kunt de volgende objecten instellen als aanvraagrijen in Workfront:

* Projecten
* Sjablonen. De projecten die van malplaatjes worden gecreeerd opstelling als verzoekrijen zullen verzoekrijen worden.

Aan opstelling moet een project of een malplaatje als verzoekrij, u het gebied van de Details van de Rij van het project of het malplaatje uitgeven.

Dit artikel beschrijft hoe u een project als verzoekrij kunt vormen waar de gebruikers verzoeken kunnen voorleggen. De Details van de Rij van de vestiging voor een malplaatje is gelijkaardig aan vestiging hen op het project.

Voor informatie over hoe te om een nieuw verzoek aan een verzoekrij voor te leggen, zie [ Exemplaar en verzend verzoeken ](../create-requests/copy-and-submit-requests.md).

Voor informatie over hoe te om een verzoekvorm in de Planning van Workfront te vormen, zie [ creeer en beheer een verzoekvorm in de Planning van Adobe Workfront ](/help/quicksilver/planning/requests/create-request-form.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Standard </p>
   <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p> Rechten voor het project beheren</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overzicht aanvraagrijen

U plaatst opstelling een verzoekrij als project. Wanneer u het project als Rij van het Verzoek aanwijst, wordt de rij toegankelijk van het gebied van Verzoeken van Adobe Workfront. Wanneer u de aanvraagwachtrij aanpast, past u ook de invulling van de formuliergebruikers aan wanneer ze de aanvragen verzenden.

Dit artikel beschrijft hoe te om een verzoekrij van een bestaand project tot stand te brengen. Nochtans, om consistentie voor uw proces van de verzoekinname te bouwen of veelvoudige lagen aan het voor rapporteringsdoeleinden en beter beheer toe te voegen, kunt u extra bouwstenen van een verzoekrij ook vormen die in de volgende lijst worden beschreven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Wachtrij</td> 
   <td> <p>U moet opstelling een project als verzoekrij in het gebied van de Details van de Rij. Deze stap is verplicht. </p> <p>Voor meer informatie, zie <a href="#create-a-request-queue" class="MCXref xref"> een sectie van de Rij van het Verzoek </a> in dit artikel creëren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Onderwerpgroepen</td> 
   <td> <p>Het zijn extra menu's die verzoeken classificeren die op gemeenschappelijke eigenschappen worden gebaseerd. Bijvoorbeeld, voor een Rij van het Verzoek van IT, zou u "On-site"en "Verre"onderwerpgroepen kunnen willen hebben. </p> <p>Voor meer informatie, zie <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref"> de Groepen van het Onderwerp </a> creëren. </p> <p>Dit is optioneel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Werkvoorraadonderwerpen</td> 
   <td> <p>Zij zijn extra menu's die verzoeken classificeren die tot de zelfde Groep van het Onderwerp behoren die op gemeenschappelijke eigenschappen wordt gebaseerd. Een onderwerpgroep kan verscheidene rijonderwerpen bevatten. </p> <p>Bijvoorbeeld, kan de "On-site"onderwerpgroep voor de Rij van het Verzoek van IT de "Hardware", "Software"en "Netwerk"rijonderwerpen bevatten. </p> <p>Voor meer informatie, zie <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref"> de Onderwerpen van de Rij </a> creëren. </p> <p>Dit is optioneel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Routeringsregels</td> 
   <td> <p>Zij staan u toe om elk verzoek aan een gebruiker, baanrol, team, of aan een project te leiden. </p> <p>Voor meer informatie, zie <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref"> het Verpletteren van Regels </a> creëren. </p> <p>Dit is optioneel.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Een aanvraagwachtrij maken

<!--at production release on April 10, do the following: take the first sentence here out; hide/ comment out the first section (Create a Request Queue in the Production environment); remove the title of the "Create a Request Queue in the Preview environment and leave that section as the only way to create request queues; search for any visible references of production/ preview and remove them from the entire article-->

Het maken van een aanvraagwachtrij is afhankelijk van de omgeving die u gebruikt.

<!--

### Create a Request Queue in the Production environment

This section describes how you can define Queue Details for the following objects:

* A project in the Production environment
* A template in the Production or Preview environment

When you set up a project as a Request Queue, the project status must be Current in order to display in the Requests area of Workfront.

>[!TIP]
>
>Your Workfront or group administrator might assign you to a custom Layout Template that might not include some of the sections described in the following steps.


To create a Request Queue:

1. Go to the project that you want to set up as a Request Queue.
1. (Optional) Click **Project Details** in the left panel and add a **Description** to the project in the **Overview** area. This information displays on all new requests.
1. Click **Queue Details** in the left panel. 

   This opens the Queue Details section.

   ![Queue Details top of the section](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)   

1. Specify the following information:

   * **Publish as Help Request Queue:** Select this option to identify this project as a request queue. All incoming issues are considered Requests.  
     When this option is not selected, the project behaves like a standard project in Workfront and all incoming issues are issues.
   
   * **Who can add requests to this queue:** Select which users have access to add requests to this queue. You can allow the following groups of people to see the Request Queue in their Requests area of the Global Navigation Bar when they add a new request:

     |Who can enter requests | Description|
     |---|---|
     | Anyone  |Any Workfront user with an active account can view this request queue and add requests to it |
     | People with view access to this project |Users with View permissions to the project can view and add requests to this queue |
     | People in this project's company |Users who belong to the company associated with this project can view and add requests to this queue. If there is a company associated with the project, the name of the company is listed in parentheses after this setting.  |
     | People in this project's group |Users who belong to the group associated with this project can view and add requests to this queue. If there is a group associated with the project, the name of the group is listed in parentheses after this setting, in gray font.  |

   * **Share with these links:** The following options enable you to provide direct access to the Request Queue and the forms associated with it to users outside of Workfront or to Workfront users using an external page. For information about embedding a request queue in a dashboard as an external page, see [Embed a request queue in a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

     Users must already have access rights to the Request Queue in order to gain direct access. Using either option described here does not automatically grant access to users.

     >[!TIP]
     >
     >Users must first log in to Workfront before gaining access to the request queue when they access the Request Queue page from another application.

      * **Direct Access URL:** When a user accesses this URL from a browser, the user is taken directly to the New Request  section in the Requests area and this request is selected by default for them.

        ![Share request queue with direct URL embedded in dashboard](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

        >[!NOTE]
        >
        >You can display a Request Queue in a dashboard as an external page. In this case, the request queue is preselected, but you can select any other request queue from the Request Type field. users can change the Request Type. Navigation components of the Requests also display.

      * **Embed Code:** Use this HTML code to embed the request queue form as an iframe within any HTML page.  
        If users are not already authenticated to Workfront when they view the page where the code is embedded, the Workfront login dialog box is displayed. After users log in, the Request Queue form is displayed.

        >[!NOTE]
        >
        >When displaying a Request Queue in an iframe, only the request form displays, the request name is preselected and dimmed. User cannot change the Request type. Navigation components of the Requests area do not display.

        In order for the request queue form to be displayed when using this embed code, you must enable the "Allow embedding of Workfront in an iframe" setting in your system setup. For more information about enabling embedding of Workfront in an iframe, see [Configure system security preferences](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). If this setting is not enabled, the iframe is displayed as blank.

        You can adjust various aspects of how the embedded form is displayed, as follows:

        <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Functionality</strong> </p> </th> 
           <th> <p><strong>Solution</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>Adjust the size of the frame</p> </td> 
           <td> <p>Modify the "width" and "height" attributes.</p> <p>By default, the width is "500" and the height is "600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Direct users to a specific Queue Topic or Topic Group</p> </td> 
           <td> <p>Add the "path" parameter to the src URL. You can find the path parameter by navigating to the desired Queue Topic or Topic Group in the non-embedded form and inspecting the URL.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Show and allow users to change the pre-configured Topic Group drop-down list</p> </td> 
           <td> <p>Use the "path" parameter by adding the <code>showPreSelectedOptions=true</code> parameter to the <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Detect when the form has been submitted</p> </td> 
           <td> <p>Add a "message" event listener to your web page's window and checking if <code>event.data.type</code> is <code>requestSubmitted</code>. <code>event.data.newIssueID</code> will be set to the ID of the created issue.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Request Types:** Select from the default options below.

     The Workfront administrator can rename the default request types. For more information about renaming the request types, see [Customize default issue types](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Bug Report
      * Change Order
      * Issue
      * Request

        This is a required field and you must select at least one option.

     >[!NOTE]
     >
     >Request Types display as a selection in the Requests area only if the Request Type is selected in both the Queue Details and the Queue Topic pages. For information about setting up the Queue Details area of a project, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Each type selected here will be available on the form (you can select more than one). Selecting more than one type can help organize multiple requests coming in.  
     For example, if you are using the form on a request queue for an IT project, the following request types can come in to the queue: hardware, software, bug fixes, and issues.

   * **Default Duration:** The default duration is the length of time it typically takes to complete an issue. This becomes the default for all incoming issues and can be modified manually. Duration is generally set in hours, days, or weeks. The Default Duration of an issue is the same as the Planned Hours on the issue. The Planned Completion Date of the issue calculates based on this field.  
     The default for the issue Duration is 1 day or 8 hours. If your Workfront administrator set the Typical Hours per Work Day as less than 8 hours, the Default Duration for issues is still 8 hours. For example, if the Typical Hours per Work Day is set to 7 hours, the Default Duration for issues is 1.14 Days or 8 hours. For more information about how to set up the system Typical Hours per Work Day, see the "Timeline Calculations" section in the article [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
   
   * **People from the same company will inherit the same permissions for all requests.:** When selected, all requests submitted to the queue are visible for users in the same company. Users can view these requests in the All Requests  section , located within the Requests area. At the time that this setting is enabled or disabled, it impacts all future requests; it does not retroactively impact information. 
   * **When someone makes a request, automatically grant:** When a user makes a request to the request queue, the user is automatically granted the level of permission that you choose to that request. Select from the following permissions levels: 

      * **View Access** 
      * **Contribute Access**. This is the default selection.
      * **Manage Access**

     For information about the Workfront permissions model, see [Overview of sharing permissions on objects](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).   
     Setting permissions here saves time, rather than having to grant permissions for each individual incoming request. Choosing this option impacts all future requests, but does not retroactively impact existing requests. 
   
   * **Default Approval**: Associate an approval process with this request queue. Only Issue Approval Processes are visible in this drop-down menu. All issues submitted to this queue will be associated with this approval process. Your Workfront administrator must define system-level approval processes before you can associate them with request queues. Users with administrative access to Approval processes can also create group-specific approval processes.

     >[!IMPORTANT]
     >
     >If the group of the project changes, the group-specific approval process attached to existing issues becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see [How group and approval process changes affect assigned approval processes](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     If you have multiple queue topics associated with a request queue, we recommend that you associate approval processes with the queue topics instead. For more information about creating queue topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md). 
   
     Consider the following when adding approval processes to request queues:

      * Only active approval processes display in the list. 
      * System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the project does not display in the list.

   * **Default Route**: Associate a Routing Rule with this request queue. Use Routing Rules to automatically assign new issues submitted to a Request Queue to the correct resource (user, job role, or team), and to the correct project. All issues submitted to this queue will be associated with this Routing Rule. You must configure Routing Rules before they display in the Queue Details section and before you can associate them with request queue.  
     If you have multiple queue topics associated with a request queue, we recommend that you associate routing rules with the queue topics instead. For more information about creating routing rules, see [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
   
   * **New Issue Fields:** In the **Show the following selected fields to all users** section, select any fields that you want to be visible to all users who submit a request to the project or add an issue to the project or the tasks.

     >[!TIP]
     >
     >New Issue Fields selected in the Queue Details section are also associated with any new issue added to the project <!--this is confusing: or to the tasks in the Issues section-->.

<!--     When you enable any of the Assigned to, Job Role, or the Team fields, they are always renamed to Assignments in the request form, but you can only specify the type of assignment selected here.

      >[!NOTE]
      >
      >If you selected Assigned To in the Queue Details area, you can enter only users in the Assignments field on the request form. In this case, you cannot enter job roles or a team. 
   
   * **Documents**: If you select to display the Documents section in the new request form, select where the document uploading section should be positioned. Select from the following:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">After custom forms</td> 
        <td><span>The Documents section displays at the bottom of the request form.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Before custom forms</td> 
        <td> <p><span>The Documents section displays between the Workfront fields and the custom fields of the request form.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>   
   
     ![New issue fields area with documents](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **Show all selected and unselected fields to:** Select which users you want to see all the fields on the new request form. The following options control the access to the fields on the form.
    
      |Which users can see all fields on the request form | Description|
      |---|---|
      | All Users (Plan Licenses) |All users who have a Plan license can see the selected as well as the unselected fields. |
      | People with view access to this project (Plan License) |Those users with a Plan license that also have View rights to this project can see the selected as well as the unselected fields. The rest of the users who can submit requests to this project can see just the selected fields. |
      | No Users |No users can see the unselected fields. All users who can submit requests to this project can only see the fields selected.  |
  
   * **Custom Forms**: Select a custom form to associate with the Request Queue. Only Issue Custom Forms are available to select from this drop-down menu. All issues submitted to the Request Queue will have the selected forms associated with them. You must create issue custom forms before you can see them displayed in the Queue Details section. 
     If you have multiple Queue Topics associated with a Request Queue, we recommend that you associate custom forms with the Queue Topics instead. For more information about creating sub-sections for the Request Queue, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![Custom forms on Queue Details](assets/custom-forms-on-queue-details.png)

     If you have multiple custom forms associated with the Request Queue, drag and drop the forms to sort them in the desired order, in the **Reorder Forms** section.

     >[!TIP]
     >
     >Custom forms added to the Queue Details section are also associated with any new issue added to the project <!--this is confusiong: or the tasks in the Issues  section-->.

<!--1. Continue selecting information for the settings in the **Email Queue Settings** area, to allow users to email requests to the request queue project. 

    For more information, see [Enable users to email an issue into a Request Queue project](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Click **Save**.  
   Your project has now been configured to be a Request Queue and users can now add requests to it. 

1. (Optional) To enhance the Request Queue functionality, build additional sub-sections for your queue, as well as rules to route the incoming requests to the correct team, assignee or project.

   * For information about creating sub-sections for the Request Queue, see the articles [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) and [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).  
   * For information about routing the requests to the appropriate assignee, team, and appropriate project, see [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   -->


### Een aanvraagwachtrij maken

Wanneer u opstelling een project als Rij van het Verzoek, de projectstatus moet Actief zijn om op het gebied van Verzoeken van Workfront te tonen.

>[!TIP]
>
>Uw Workfront- of groepsbeheerder kan u toewijzen aan een aangepaste lay-outsjabloon die wellicht niet alle secties bevat die in de volgende stappen worden beschreven.

Een aanvraagwachtrij maken:

1. Ga naar het project dat u opstelling als Rij van het Verzoek wilt.
1. (Facultatief) klik **Details van het Project** in het linkerpaneel en voeg a **Beschrijving** aan het project in het **Overzicht** gebied toe. Deze informatie wordt weergegeven bij alle nieuwe aanvragen.
1. Klik **Details van de Rij** in het linkerpaneel.

   Hiermee opent u de sectie met gegevens van de wachtrij.

   ![ sectie van het Type van Rij in het gebied van de Details van de Rij ](assets/unshimmed-queue-type-section-queue-details-area.png)

1. Geef de volgende informatie op:

   * **publiceer als Rij van het Verzoek van de Hulp**: Selecteer deze optie om dit project als verzoekrij te identificeren. Alle inkomende kwesties worden beschouwd als Verzoeken.\
     Als deze optie niet is geselecteerd, gedraagt het project zich als een standaardproject in Workfront en zijn alle binnenkomende problemen van belang.

   * **wie verzoeken aan deze rij kan toevoegen?**: Selecteer welke gebruikers toegang hebben om aanvragen aan deze wachtrij toe te voegen. U kunt de volgende groepen mensen toestaan om de Rij van het Verzoek in hun gebied van Verzoeken van de Globale Bar van de Navigatie te zien wanneer zij een nieuw verzoek toevoegen:

     | Wie aanvragen kan invoeren | Beschrijving |
     |---|---|
     | Iedereen | Elke Workfront-gebruiker met een actief account kan deze aanvraagwachtrij bekijken en er aanvragen aan toevoegen |
     | Personen met toegang tot dit project | Gebruikers met de machtiging Weergeven aan het project kunnen aanvragen weergeven en toevoegen aan deze wachtrij |
     | Personen in het bedrijf van dit project | De gebruikers die tot het bedrijf behoren verbonden aan dit project kunnen verzoeken aan deze rij bekijken en toevoegen. Als er een bedrijf verbonden aan het project is, is de naam van het bedrijf vermeld tussen haakjes na dit het plaatsen. |
     | Personen in de projectgroep | De gebruikers die tot de groep behoren verbonden aan dit project kunnen verzoeken aan deze rij bekijken en toevoegen. Als er een groep is die aan het project is gekoppeld, wordt de naam van de groep na deze instelling tussen haakjes weergegeven, in een grijs lettertype. |

     {style="table-layout:auto"}

   * Gebruik de volgende opties om gebruikers buiten Workfront of Workfront-gebruikers die een ingesloten externe pagina gebruiken rechtstreeks toegang te geven tot de wachtrij met aanvragen en de bijbehorende formulieren.

   Voor informatie over het inbedden van een verzoekrij in een dashboard als externe pagina, zie [ een verzoekrij in een dashboard ](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md) inbedden.

   De gebruikers moeten toestemmingen aan de Rij van het Verzoek eerst hebben om directe toegang te krijgen. Het gebruik van een van de hier beschreven opties verleent niet automatisch toegang aan gebruikers.

   >[!TIP]
   >
   >Gebruikers moeten zich eerst aanmelden bij Workfront voordat ze toegang krijgen tot de wachtrij met aanvragen wanneer ze vanuit een andere toepassing toegang krijgen tot de pagina Wachtrij aanvragen.

   * **Directe Toegang URL:** wanneer een gebruiker tot dit URL van browser toegang heeft, wordt de gebruiker rechtstreeks genomen aan de Nieuwe sectie van het Verzoek in het gebied van Verzoeken en dit verzoek wordt geselecteerd door gebrek voor hen.

     ![ Nieuwe verzoekdoos van het Directe aandeel URL ](assets/new-request-box-from-direct-url-share.png)

     >[!NOTE]
     >
     >U kunt een verzoekwachtrij in een dashboard weergeven als een externe pagina. In dit geval is de wachtrij met aanvragen vooraf geselecteerd, maar u kunt een andere wachtrij met aanvragen selecteren in het veld Type verzoek. Gebruikers die de aanvraag indienen, kunnen een ander aanvraagtype selecteren. De Groepen van het onderwerp en de Onderwerpen van de Rij tonen ook.

   * **bed Code in:** gebruik deze code van HTML om de vorm van de verzoekrij als iframe binnen om het even welke pagina van HTML in te bedden.\
     Als gebruikers nog niet zijn geverifieerd bij Workfront wanneer ze de pagina bekijken waarop de code is ingesloten, wordt het Workfront-aanmeldingsvenster weergegeven. Nadat gebruikers zich hebben aangemeld, wordt het formulier Wachtrij aanvragen weergegeven.

     >[!NOTE]
     >
     >Als een aanvraagwachtrij wordt weergegeven in een iframe, wordt alleen het aanvraagformulier weergegeven. De naam van de aanvraag wordt dan vooraf geselecteerd en grijs weergegeven. Gebruiker kan het aanvraagtype niet wijzigen. Navigatiecomponenten van het gebied Verzoeken worden niet weergegeven.

     Uw Workfront-beheerder moet de instelling Insluiten van Workfront in een iFrame toestaan inschakelen in het gedeelte System Setup (Systeeminstellingen) om het formulier voor de aanvraagwachtrij weer te geven wanneer deze insluitcode wordt gebruikt.

     Voor meer informatie over het toelaten van het inbedden van Workfront in een iframe, zie [ de voorkeur van de systeemveiligheid ](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md) vormen. Als deze instelling niet is ingeschakeld, wordt het iframe leeg weergegeven.

     U kunt als volgt verschillende aspecten van de weergave van het ingesloten formulier aanpassen:

     <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong> Functionaliteit </strong> </p> </th> 
           <th> <p><strong> Oplossing </strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>De grootte van het frame aanpassen</p> </td> 
           <td> <p>Wijzig de kenmerken "width" en "height".</p> <p>De breedte is standaard "500" en de hoogte is "600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Directe gebruikers aan een specifiek Onderwerp van de Rij of een Groep van het Onderwerp</p> </td> 
           <td> <p>Voeg de parameter "path" toe aan de URL van de bron. U kunt de wegparameter vinden door aan het gewenste Onderwerp of de Groep van het Onderwerp van de Rij in de niet ingebedde vorm te navigeren en URL te inspecteren.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Toon en sta gebruikers toe om de vooraf gevormde drop-down lijst van de Groep van het Onderwerp te veranderen</p> </td> 
           <td> <p>Gebruik de parameter "path" door de parameter <code>showPreSelectedOptions=true</code> aan <code>src URL</code> toe te voegen.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Detecteren wanneer het formulier is verzonden</p> </td> 
           <td> <p>Voeg een "message"-gebeurtenislistener toe aan het venster van uw webpagina en controleer of <code>event.data.type</code> <code>requestSubmitted</code> is. <code>event.data.newIssueID</code> wordt ingesteld op de id van het gemaakte probleem.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **de Types van Verzoek:** in de **sectie van de Eigenschappen van de Rij**, selecteer van de volgende opties:

   * Foutrapport
   * Volgorde wijzigen
   * Probleem
   * Verzoek

   Dit is een verplicht veld en u moet ten minste één optie selecteren.

   De Workfront-beheerder kan de standaardaanvraagtypen een andere naam geven. Voor meer informatie over het anders noemen van de verzoektypes, zie [ de types van standaardkwestie ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md) aanpassen.

   >[!NOTE]
   >
   >Wanneer de gebruikers tot de verzoekrij van het gebied van Verzoeken toegang hebben, tonen de Types van Verzoek als selectie slechts als het Type van Verzoek in zowel de Details van de Rij als de pagina&#39;s van het Onderwerp van de Rij wordt geselecteerd.
   >
   >Voor informatie over vestiging het gebied van de Onderwerpen van de Rij van een project, zie [ de Onderwerpen van de Rij ](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) creëren.

   Elk hier geselecteerd type is beschikbaar op het formulier (u kunt meerdere typen selecteren). Als u meerdere typen selecteert, kunt u meerdere aanvragen ordenen die binnenkomen.\
   Als u bijvoorbeeld het formulier op een aanvraagwachtrij voor een IT-project gebruikt, kunnen de volgende aanvraagtypen in de wachtrij worden geplaatst: hardware, software, foutoplossingen en problemen.

   * **StandaardDuur:** ga een aantal voor de Duur in, dan selecteer van het drop-down menu één van de volgende duureenheden:

      * Dagen
      * Uren
      * Minuten
      * Weken

   De standaardduur is de tijdsduur het typisch neemt om een kwestie te voltooien die aan deze verzoekrij wordt voorgelegd. Dit wordt de standaardinstelling voor alle binnenkomende uitgaven en kan handmatig worden gewijzigd.
De standaardduur van een uitgave is gelijk aan de geplande uren voor het probleem. De geplande afwerkingsdatum van de uitgave wordt berekend op basis van dit veld.\
   Als deze optie niet wordt gewijzigd, is de standaardduur voor de uitgave 1 dag of 8 uur.
Als uw Workfront-beheerder de typische uren per werkdag instelt op minder dan 8 uur in het gedeelte Setup, is de standaardduur voor uitgaven nog steeds 8 uur.
Als de instelling voor de typische uren per werkdag bijvoorbeeld is ingesteld op 7 uur in het gedeelte Setup van Workfront, is de standaardduur voor uitgaven 1,14 dagen of 8 uur.
Voor meer informatie over hoe te opstelling ziet de systeem Typische Uren per Dag van het Werk, de &quot;sectie van de Berekeningen van de Chronologie&quot;in het artikel [ systeembrede projectvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

   * **de Mensen van het zelfde bedrijf zullen de zelfde toestemmingen voor alle verzoeken erven.**: Als deze optie is geselecteerd, zijn alle aanvragen die naar de wachtrij worden verzonden zichtbaar voor gebruikers in hetzelfde bedrijf. De gebruikers kunnen deze verzoeken in de Al sectie van Verzoeken bekijken, die binnen het gebied van Verzoeken wordt gevestigd. Op het moment dat deze instelling wordt in- of uitgeschakeld, heeft deze invloed op alle toekomstige aanvragen. De instelling heeft geen retroactieve invloed op informatie.
   * **wanneer iemand een verzoek indient, automatisch verlenen..:** wanneer een gebruiker een verzoek aan de verzoekrij indient, wordt de gebruiker automatisch verleend het niveau van toestemming dat u aan dat verzoek kiest. Klik op de knop Toegang om een van de volgende machtigingsniveaus te selecteren:

      * **Toegang van de Mening**
      * **draag Toegang** bij. Dit is de standaardselectie en de naam van de knoop van de Toegang.
      * **beheert Toegang**

     Voor informatie over het de toestemmingenmodel van Workfront, zie [ Overzicht van het delen van toestemmingen op voorwerpen ](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
     Het plaatsen van toestemmingen bewaart hier tijd, eerder dan het moeten toestemmingen individueel, voor elk inkomend verzoek verlenen. Het kiezen van deze optie is van invloed op alle toekomstige verzoeken, maar heeft geen terugwerkende invloed op bestaande verzoeken.

   * **StandaardGoedkeuring**: Klik het drop-down menu om een goedkeuringsproces voor deze verzoekrij te selecteren. In dit keuzemenu worden alleen processen voor goedkeuring van uitgaven weergegeven. Alle kwesties die aan deze rij worden voorgelegd zullen met dit goedkeuringsproces worden geassocieerd. Uw Workfront-beheerder moet goedkeuringsprocessen op systeemniveau definiëren voordat u deze kunt koppelen aan aanvraagwachtrijen. Gebruikers met administratieve toegang tot goedkeuringsprocessen kunnen ook groepsspecifieke goedkeuringsprocessen maken.

     >[!IMPORTANT]
     >
     >Als de groep van het project verandert, wordt het groep-specifieke goedkeuringsproces verbonden aan bestaande kwesties een enig-gebruiks goedkeuringsproces. Voor meer informatie over hoe de veranderingen in de groep van het project of de veranderingen in het goedkeuringsproces goedkeuringsmontages beïnvloeden, zie [ hoe de groep en de veranderingen van het goedkeuringsproces aangewezen goedkeuringsprocessen ](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md) beïnvloeden.

     Als u veelvoudige rijonderwerpen verbonden aan een verzoekrij hebt, adviseren wij dat u goedkeuringsprocessen met de rijonderwerpen in plaats daarvan associeert.

     Voor meer informatie over het creëren van rijonderwerpen, zie [ de Onderwerpen van de Rij ](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) creëren.

     Overweeg het volgende wanneer het toevoegen van goedkeuringsprocessen om rijen te verzoeken:

      * Alleen actieve goedkeuringsprocessen worden in de lijst weergegeven.
      * Systeemspecifieke en groepsspecifieke goedkeuringsprocessen worden in de lijst weergegeven. Een goedkeuringsproces verbonden aan een groep buiten die van het project toont niet in de lijst.

   * **StandaardRoute**: Klik het drop-down menu om een verpletterende regel voor deze verzoekrij te selecteren. Het verpletteren van regels wijst automatisch nieuwe kwesties toe die aan een verzoekrij aan het correcte middel (gebruiker, baanrol, of team) worden voorgelegd, en aan het correcte project. Alle kwesties die aan deze rij worden voorgelegd zullen met deze verpletterende regel worden geassocieerd. U moet het Verpletteren van Regels vormen alvorens zij in de sectie van de Details van de Rij tonen en alvorens u hen met verzoekrij kunt associëren.\
     Als u veelvoudige rijonderwerpen verbonden aan een verzoekrij hebt, adviseren wij dat u het verpletteren van regels met de rijonderwerpen in plaats daarvan associeert. Voor meer informatie over het creëren van het verpletteren van regels, zie [ het Verpletteren van Regels ](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md) creëren.

   * **Nieuwe Velden van de Uitgave:** In **toon de volgende geselecteerde gebieden aan alle gebruikers** sectie, selecteer de gebieden die u aan alle gebruikers zichtbaar wilt zijn die een verzoek aan het project voorleggen of een kwestie aan dit project of aan de taken van het project toevoegen.

     >[!NOTE]
     >
     >* Wanneer u een van de velden Toegewezen aan, Functie of Team inschakelt, wordt de naam van de toegewezen taken altijd gewijzigd in Toewijzingen in het aanvraagformulier wanneer gebruikers de aanvraag indienen. U kunt het type toewijzing alleen opgeven in het gebied Wachtrij details.
     >
     >* Als u Toegewezen aan in het gebied van de Details van de Rij selecteerde, kunt u slechts gebruikers op het gebied van Toewijzingen op het verzoekformulier ingaan. In dit geval kunt u geen taakrollen of een team invoeren.

   * **Documenten**: Selecteer deze optie om de sectie van Documenten in de nieuwe verzoekvorm te tonen, dan te selecteren waar het document uploadende sectie zou moeten worden geplaatst. Selecteer een van de volgende opties:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Na aangepaste formulieren</td> 
        <td><span> de sectie van Documenten toont bij de bodem van de verzoekvorm.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Voor aangepaste formulieren</td> 
        <td> <p><span> de sectie van Documenten toont tussen de gebieden van Workfront en de douanegebieden van de verzoekvorm.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![ Nieuwe de kwesties gebieden en documenten op de Details van de Rij ](assets/new-issue-fields-and-documents-on-queue-details.png)

   * **toon alle geselecteerde en niet geselecteerde gebieden aan:** selecteer welke gebruikers alle gebieden op de nieuwe verzoekvorm zouden moeten zien. De volgende opties bepalen de toegang tot de velden op het formulier.

     | Welke gebruikers alle velden op het aanvraagformulier kunnen zien | Beschrijving |
     |---|---|
     | Alle gebruikers (abonnementslicenties) | Alle gebruikers met een licentie voor abonnementen kunnen zowel de geselecteerde als de niet-geselecteerde velden zien. |
     | Personen met toegang tot dit project (licentie voor abonnementen) | Gebruikers met een licentie voor een abonnement die ook weergaverechten voor dit project hebben, kunnen zowel de geselecteerde als de niet-geselecteerde velden zien. De rest van de gebruikers die aanvragen kunnen indienen voor dit project, kunnen alleen de geselecteerde velden zien. |
     | Geen gebruikers | De niet-geselecteerde velden kunnen niet door gebruikers worden weergegeven. Alle gebruikers die aanvragen naar dit project kunnen verzenden, kunnen alleen de geselecteerde velden zien. Dit is de standaardselectie. |

   * **Aangepaste Forms**: Selecteer een douanevorm om met de Rij van het Verzoek van het drop-down menu te associëren. U kunt meerdere formulieren selecteren en vervolgens slepen en neerzetten in de volgorde die u ze in het aanvraagformulier wilt weergeven.
Alleen aangepaste formulieren kunnen worden geselecteerd in dit keuzemenu. Aan alle kwesties die aan deze verzoekrij worden voorgelegd, die aan het project of aan zijn taken worden toegevoegd zullen de geselecteerde vormen verbonden hebben die aan hen worden toegevoegd.
U moet aangepaste formulieren maken voor uitgaven voordat u deze kunt weergeven in de sectie Wachtrijdetails.
Als u veelvoudige rijonderwerpen verbonden aan een verzoekrij hebt, adviseren wij dat u douaneformulieren met de rijonderwerpen in plaats daarvan associeert.
Voor meer informatie, zie [ de Onderwerpen van de Rij ](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) creëren.

     ![ de vormendoos van de Douane op de Details van de Rij ](assets/custom-forms-box-on-queue-details.png)

1. Ga door selecterend informatie voor de montages in het **E-mailE van de Montages van de Rij** gebied, om gebruikers toe te staan om verzoeken aan het project van de verzoekrij te e-mailen.

   Voor meer informatie, zie [ gebruikers toelaten om een kwestie in een project van de Rij van het Verzoek ](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md) te e-mailen.

1. Klik **sparen**.\
   Uw project is nu gevormd om een Rij van het Verzoek te zijn en de gebruikers kunnen verzoeken aan het nu toevoegen.

1. (Facultatief) om de functionaliteit van de Rij van het Verzoek te verbeteren, bouw extra ondersecties voor uw rij, evenals regels om de inkomende verzoeken aan het correcte team, de ontvanger of het project te leiden.

   * Raadpleeg de volgende artikelen voor informatie over het maken van subsecties voor de aanvraagwachtrij
   * [ creeer de Onderwerpen van de Rij ](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)
   * [ creeer de Groepen van het Onderwerp ](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

     Voor informatie over het verpletteren van de verzoeken aan aangewezen ontvanger, team, en aangewezen project, zie [ het Verpletteren van Regels ](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md) creëren.

