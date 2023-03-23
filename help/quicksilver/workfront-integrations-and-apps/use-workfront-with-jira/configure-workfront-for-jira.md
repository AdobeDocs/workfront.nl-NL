---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Configureren [!DNL Adobe Workfront for Jira]
description: U kunt [!DNL Adobe Workfront for Jira] om uw [!DNL Jira] en [!DNL Workfront] systemen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: d2c366a69b986bd8d559a18994810011c6d33441
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Configureren [!DNL Adobe Workfront for Jira]

U kunt [!DNL Adobe Workfront for Jira] om uw [!DNL Jira] en [!DNL Workfront] systemen.

Nadat u de invoegtoepassing hebt geïnstalleerd, kunt u workflows definiëren die [!DNL Jira] automatisch uitgaven wanneer [!DNL Workfront] tijdelijke items worden gemaakt. De items in beide toepassingen worden gekoppeld en sommige van de gegevens worden automatisch bijgewerkt in beide systemen.

Alle gebruikers in [!DNL Workfront] en [!DNL Jira] kan van deze integratie profiteren. Ze hebben alleen een licentie nodig voor het systeem waarin ze het meest werken, en niet voor beide systemen.

Deze invoegtoepassing is beschikbaar voor de [!UICONTROL Server] en [!UICONTROL OnDemand] (of [!UICONTROL Cloud]) versies van [!DNL Jira] Software.

Voor een lijst met [!DNL Jira] versies die [!DNL Workfront for Jira] momenteel wordt ondersteund, zie [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) bij de [!DNL Atlassian Marketplace].

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] overzicht van licenties</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] toegang</td> 
   <td> <p>Toegang tot systeembeheerder</p> <p>Belangrijk: Wij adviseren u afzonderlijke rekeningen van de systeembeheerder in [!DNL Jira] en [!DNL Workfront] om aan deze integratie te wijden, eerder dan het gebruiken van bestaande degenen die aan gebruikers zouden kunnen worden vastgemaakt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder. Voor informatie over [!DNL Workfront] beheerders, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Vereisten

Voordat u kunt configureren [!DNL Workfront for Jira]moet u

* Installeren [!DNL Workfront for Jira]\
   Voor installatie-instructies [!DNL Workfront for Jira], zie [Installeren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Configureren [!DNL Workfront for Jira]

Door te configureren [!DNL Workfront for Jira] u kunt:

* Definieer triggers die worden gemaakt [!DNL Jira] items wanneer [!DNL Workfront] items worden gemaakt.
* Opgeven welke velden moeten worden gesynchroniseerd tussen items die zijn gekoppeld tussen [!DNL Jira] en [!DNL Workfront].

>[!NOTE]
>
>* Nadat u [!DNL Workfront for Jira] op uw [!DNL Jira] milieu, alle [!DNL Jira] gebruikers zien een [!DNL Workfront] deelvenster rechts op alles [!DNL Jira] objecten. Het deelvenster bevat informatie over de items die kunnen worden gekoppeld vanuit [!DNL Workfront] of geeft aan dat er geen [!DNL Workfront] items zijn gekoppeld aan [!DNL Jira] objecten.
>* Wanneer u de [!DNL Jira Server] -installatie, alleen de problemen die samenhangen met projecten die zijn geïdentificeerd als triggers voor de Workfront-integratie, geven het Workfront-deelvenster weer. Voor meer informatie over het instellen van triggers voor de [!DNL Workfront to Jira] workflow, zie [Triggers configureren voor het automatisch koppelen van items tussen [!DNL Jira] en [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>




Om te vormen [!DNL Workfront for Jira]:

1. Aanmelden [!DNL Jira] als [!DNL Jira] beheerder.
1. Klikken **[!UICONTROL Settings]** in het algemeen [!DNL Jira] -menu.
1. Klikken **[!UICONTROL Add-ons]** en klik vervolgens op **[!UICONTROL Manage add-ons]**.

1. Breid uit **[!DNL Workfront]** invoegtoepassing.
1. Klik op **[!UICONTROL Configure]**.
1. Volg de aanwijzingen om u aan te melden [!DNL Workfront].

   >[!NOTE]
   >
   >De gebruiker moet een geldige `apiKey` in [!UICONTROL Workfront] om een geslaagde verbinding te maken.

   U moet zich aanmelden bij [!DNL Workfront] als [!DNL Workfront] beheerder om de configuratie voort te zetten.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] verbindt met [!DNL Jira] het gebruiken van OAuth 2.0, een norm die door de meeste web-based integratie voor de authentificatie en de vergunning van gebruikers wordt gebruikt.
   >* Wanneer u wordt gevraagd het domein van uw [!DNL Workfront] -account, typt u deze notatie: *yourCompany&#39;sDomain.my.workfront.com*. Het domein van uw bedrijf is gewoonlijk de naam van uw bedrijf.
   >* Verbeterde verificatie is pas beschikbaar na een [!DNL Workfront] de beheerder laat het voor deze integratie toe.



1. Selecteer **[!UICONTROL Triggers]** tab om het automatisch maken van [!DNL Jira] objecten als nieuwe [!DNL Workfront] items worden gemaakt.

   Voor meer informatie over het instellen van triggers voor de Workfront voor [!DNL Jira] workflow, zie [Triggers configureren voor het automatisch koppelen van items tussen [!DNL Jira] en [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Selecteer **[!UICONTROL Setup]** tab om de synchronisatie van velden tussen gekoppelde velden te configureren [!DNL Jira] en [!DNL Workfront] objecten.

   Voor meer informatie over het instellen van de synchronisatie van velden tussen [!DNL Jira] en [!DNL Workfront], zie [Veldsynchronisatie configureren tussen [!DNL Jira] en [!DNL Workfront] Items](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Nadat u de triggers en de synchronisatie van velden tussen de twee toepassingen hebt gedefinieerd, [!DNL Workfront] gebruiker die taken of problemen kan maken, kan het maken van een item in [!DNL Jira]. De gebruiker kan een item maken als de criteria voor het item dat ze maken overeenkomen met de triggers in [!DNL Jira], zelfs als de gebruiker geen [!DNL Jira] licentie. Ook alle [!DNL Jira] gebruiker kan meteen beginnen met het werken aan de [!DNL Jira] en de bijbehorende updates zijn zichtbaar in [!DNL Workfront], zonder dat zij een [!DNL Workfront] licentie. Alle updates in [!DNL Workfront] zijn ook zichtbaar op de [!DNL Jira] objecten.

1. (Optioneel) Selecteer de optie **[!UICONTROL Activity Log]** om eventuele fouten tijdens de integratie te controleren.

   Voor meer informatie over de [!UICONTROL Activity Log], zie [De weergave van [!DNL Jira] [!UICONTROL Activity Log]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Triggers configureren voor het automatisch koppelen van items tussen [!DNL Jira] en [!DNL Workfront]

Als de [!DNL Jira] systeembeheerder, kunt u trekkers bepalen die automatisch kwesties in [!DNL Jira] wanneer een item in [!DNL Workfront] voldoet aan bepaalde criteria.

>[!NOTE]
>
>Het kan tot 10 minuten duren voordat de integratie nieuwe problemen oplevert in [!DNL Jira].

Houd rekening met het volgende wanneer u het maken van [!DNL Jira] objecten als [!DNL Workfront] items worden gemaakt:

* De integratie is eenrichtingsverkeer: U kunt alleen items activeren die u maakt in [!DNL Workfront] automatisch te maken in [!DNL Jira]. U kunt geen items activeren die u maakt in [!DNL Jira] automatisch te maken in [!DNL Workfront].
* Er is geen limiet voor het aantal triggers dat u kunt gebruiken.
* Als u een item maakt in [!DNL Workfront] komt overeen met meerdere triggers, er wordt slechts één item gemaakt in [!DNL Jira]. Het item wordt gemaakt in [!DNL Jira] volgens de eerste trigger (in de volgorde waarin ze zijn gedefinieerd in [!DNL Jira]). Alle andere triggers worden genegeerd.
* Slechts één item in [!DNL Workfront] kan aan één punt in Jira worden verbonden. U kunt er nooit een koppelen [!DNL Workfront] item naar meerdere [!DNL Jira] problemen, of één [!DNL Jira] uitgifte aan meerdere [!DNL Workfront] objecten.

triggers configureren voor het automatisch maken van items in [!DNL Jira]:

1. Aanmelden [!DNL Jira] als systeembeheerder.
1. Klikken **[!UICONTROL Settings]** in het algemeen [!DNL Jira] -menu.
1. Klikken **[!UICONTROL Add-ons]** vervolgens **[!UICONTROL Manage add-ons]**.

1. Breid uit **[!DNL Workfront]** invoegtoepassing.
1. Klik op **[!UICONTROL Configure]**.
1. Aanmelden bij [!DNL Workfront] als systeembeheerder.

   De **[!UICONTROL Triggers]** is standaard geselecteerd.

1. Klikken **[!UICONTROL Add trigger]** om een nieuwe trigger toe te voegen.
1. In de **[!UICONTROL Workfront team/user/role]** veld, geeft u de naam van een [!DNL Workfront] team, gebruiker of taakrol, en klik vervolgens om deze te selecteren wanneer deze in de lijst wordt weergegeven.

   >[!NOTE]
   >
   >U kunt geen veelvoudige trekkers voor het zelfde team, de gebruiker, of de rol hebben.

   Wanneer iemand een taak of een kwestie creeert en het aan één van deze entiteiten toewijst, wordt een kwestie automatisch gecreeerd in [!DNL [!DNL Jira]].

1. In de **[!UICONTROL [!DNL Jira] project]** veld, de naam van een [!DNL Jira] en klik vervolgens om het te selecteren wanneer het in de lijst wordt weergegeven.

   Wanneer de [!DNL Jira] De kwestie wordt gecreeerd, wordt het geplaatst op het project u hier specificeert.

1. Selecteer een **I[!UICONTROL ssue type]** in het keuzemenu.

   Dit geeft het type uitgave aan waarin [!DNL Jira] wanneer aan de voorwaarden van deze trigger is voldaan, op basis van uw instellingen voor dat specifieke project in [!DNL Jira].

1. Klik op **[!UICONTROL Save]**.

   Met deze configuratie, telkens als [!DNL Workfront] gebruiker maakt een item dat overeenkomt met de opgegeven triggers. Er wordt een nieuwe uitgave gemaakt in [!DNL Jira].

## Veldsynchronisatie configureren tussen [!DNL Jira] en [!DNL Workfront] Items

Als de [!DNL Jira] beheerder, kunt u bepalen welke gebieden automatisch op punten zouden moeten synchroniseren die tussen worden verbonden [!DNL Workfront] en Jira. Bepaalde velden kunnen worden gesynchroniseerd via het dialoogvenster [!DNL Workfront] aan de [!DNL Jira] en andere synchroniseren van Jira naar Workfront.

Om te bepalen welke gebieden automatisch op punten zouden moeten synchroniseren die tussen de twee toepassingen worden verbonden:

1. Aanmelden [!DNL Jira] als beheerder van Jira.
1. Klikken **[!UICONTROL Settings]** in het algemeen [!DNL Jira] -menu.
1. Klikken **[!UICONTROL Add-ons]** vervolgens **[!UICONTROL Manage add-ons]**.

1. Breid uit **[!DNL Workfront]** invoegtoepassing.
1. Klik op **[!UICONTROL Configure]**.
1. Aanmelden bij [!DNL Workfront] als Workfront-beheerder.
1. Klik op de knop **[!UICONTROL Setup]** tab.

1. In de **[!UICONTROL Synchronize from Jira to Workfront]** selecteert u de velden waarin u wilt bijwerken [!DNL Jira] wanneer deze in Workfront worden bijgewerkt.

   1. Selecteer een van de volgende frequenties waarmee de velden worden gesynchroniseerd:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL On Creation]</td>
              <td>De velden die u opgeeft, worden gesynchroniseerd tussen de gekoppelde Workfront en [!DNL Jira] objecten wanneer het object in Workfront wordt gemaakt.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>De velden die u opgeeft, worden gesynchroniseerd tussen de gekoppelde Workfront en [!DNL Jira] items wanneer de velden worden bijgewerkt in Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Never]</td>
              <td>De velden die u opgeeft, worden nooit gesynchroniseerd tussen de gekoppelde [!DNL Workfront] en [!DNL Jira] objecten. Er is geen indicatie in [!DNL Jira] dat het veld is bijgewerkt in [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Selecteer deze optie om de volgende velden te synchroniseren vanuit [!DNL Workfront] tot [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>De naam van een taak of een probleem in [!DNL Workfront] wordt de naam van de uitgifte waaraan deze is gekoppeld [!DNL Jira].</p><p>Opmerking: Wanneer nieuwe items worden gemaakt in [!DNL Jira] automatisch [!DNL Workfront] Naam wordt altijd bijgewerkt op het tabblad [!DNL Jira] item, ongeacht of dit veld hier is ingeschakeld of niet. Wanneer een [!DNL Jira] item is handmatig gekoppeld aan een [!DNL Workfront] item, de naam van de [!DNL Workfront] alleen itemupdates in [!DNL Jira] wanneer u <strong>Altijd</strong> dit veld synchroniseren. Zie voor meer informatie over het handmatig of automatisch koppelen van items <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Items koppelen tussen [!DNL Adobe Workfront] en [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Description]</td>
         <td>De beschrijving van een taak of een probleem in [!DNL Workfront] wordt de beschrijving van de uitgifte waaraan deze is gekoppeld in [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Documenten</td>
         <td><p>Documenten die zijn gekoppeld aan een taak of een probleem in [!DNL Workfront] Ook zijn ze gehecht aan de kwestie waarmee ze in Jira verband houdt. Nieuwe documentversies van [!DNL Workfront] worden als afzonderlijke documenten aan Jira toegevoegd en worden toegevoegd met <i>_v&lt;version number=""&gt;</i> om de genummerde versie in Workfront aan te geven. </p><p>Als bijvoorbeeld de naam van een document in [!DNL Workfront] is <strong>Hoofd-advertentie</strong>en voegt u er een nieuwe versie aan toe [!DNL Workfront], wordt de nieuwe versie overgebracht naar [!DNL Jira] als een nieuw document met de naam <strong>Hoofd-advertentie_v2</strong>.</p><p>Belangrijk: <p>Houd rekening met het volgende wanneer u documenten synchroniseert:</p>
           <ul>
            <li><p>Documenten die groter zijn dan 5 MB, worden niet gesynchroniseerd. Als een documentsynchronisatie mislukt omdat het document te groot is, wordt een fout in het activiteitenlogboek geregistreerd. </p><p>Voor meer informatie over het activiteitenlogboek, zie <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Het activiteitenlog van de bevalling weergeven</a>.</p></li>
            <li><p>Documenten die zijn gekoppeld aan taken en uitgaven van externe servers worden niet overgedragen naar de [!DNL Jira] objecten. Alleen documenten die rechtstreeks op de taak of de uitgave in zijn geüpload [!DNL Workfront] worden overgedragen naar de gekoppelde emissie in [!DNL Jira].</p></li>
            <li><p>Als u een proefdruk wilt maken op basis van een document, moet u de proefdruk genereren in [!DNL Workfront]. </p><p>Voor meer informatie over het genereren van een bewijs raadpleegt u <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create" class="MCXref xref">Een proefdruk maken voor een bestaand document </a>in <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Een proefdruk maken voor een document</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Planned Completion Date]</td>
         <td><p>De [!UICONTROL Planned Completion Date] van een taak of een probleem in [!DNL Workfront] wordt de [!UICONTROL Due Date] van de kwestie waarmee zij verband houdt in [!DNL Jira].</p><p>Opmerking: Zorg ervoor dat u <strong>[!UICONTROL Due Date]</strong> op [!DNL Jira] problemen, voor deze waarde die moet worden gesynchroniseerd.</p></td>
        </tr>
       </tbody>
      </table>

1. In de **[!UICONTROL Synchronize from [!DNL Jira] to [!DNL Workfront]]** selecteert u de velden waarin u wilt bijwerken [!DNL Workfront] wanneer ze worden bijgewerkt in [!DNL Jira].

   1. Selecteer een van de volgende frequenties waarmee de velden worden gesynchroniseerd:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>De velden die u opgeeft, worden altijd gesynchroniseerd tussen de gekoppelde [!DNL Workfront] en [!DNL Jira] items wanneer de velden worden bijgewerkt in [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Never]</td>
         <td><p>De velden die u opgeeft, worden nooit gesynchroniseerd tussen de gekoppelde [!DNL Workfront] en [!DNL Jira] objecten. Er is geen indicatie in [!DNL Workfront] dat het veld is bijgewerkt in [!DNL Jira]. </p><p>Opmerking: Wanneer u Nooit selecteert, [!DNL Workfront] velden kunnen nog steeds handmatig worden bijgewerkt vanuit [!DNL Jira] links [!DNL Workfront] van het [!DNL Jira] probleem. Deze updates worden alleen weergegeven op [!DNL Workfront] objecten in [!DNL Jira] en [!DNL Workfront] en niet aan [!DNL Jira] objecten.</p></td>
        </tr>
       </tbody>
      </table>

   1. Selecteer deze optie om de volgende velden te synchroniseren vanuit [!DNL Jira] tot [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>De [!UICONTROL Status] van een kwestie in [!DNL Jira] wordt de [!UICONTROL Status] van de taak of uitgifte waarmee zij is verbonden in [!DNL Workfront].<br>Meer informatie over [!DNL Workfront] statussen, zie <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Een status maken of bewerken</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Assignee]</td>
         <td><p>De [!UICONTROL Assignee] van een kwestie in [!DNL Jira] wordt de [!UICONTROL Assignee] van de taak of uitgifte waarmee zij is verbonden in [!DNL Workfront].</p><p>Belangrijk: Wanneer u een item toewijst in [!DNL Jira] aan een gebruiker die geen [!DNL Workfront] -account, maakt de integratie een nieuwe actieve gebruiker in [!DNL Workfront] alleen wanneer de <strong>Automatisch een gebruiker maken in [!DNL Workfront] als de [!DNL Jira] gebruiker heeft geen [!DNL Workfront] account</strong> is ingesteld op <strong>[!UICONTROL Always]</strong>. Deze gebruiker neemt geen [!DNL Workfront] licentie. Actieve gebruikers kunnen worden toegewezen aan werkitems in [!DNL Workfront], maar kan niet worden opgenomen in updates. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Attachments]</td>
         <td>Bijlagen van een probleem in [!DNL Jira] ook zijn gekoppeld aan de taak of kwestie waarmee deze is verbonden in [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comments]</td>
         <td><p>Een opmerking over een [!DNL Jira] de kwestie wordt ook geplaatst op het verbonden [!DNL Workfront] item in het [!UICONTROL Updates] gebied. Een opmerking die is geplaatst in het dialoogvenster [!UICONTROL Updates] gebied voor een [!DNL Workfront] taak of geeft synoniemen uit aan [!DNL Jira]De native opmerkingstroom van de klant voor de gekoppelde uitgave. </p><p>Deze is ingesteld op <strong>[!UICONTROL Always]</strong> standaard. Als u <strong>[!UICONTROL Never]</strong> hier kunt u nog steeds handmatig opmerkingen op een gekoppeld item plaatsen in [!DNL Workfront] of in [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. In de **[!UICONTROL OTHER]** selecteert u welke extra velden moeten worden bijgewerkt tussen gekoppelde items.

   1. Selecteer een optie om te bepalen of de velden die u opgeeft **[!UICONTROL Always]** of **[!UICONTROL Never]** bijwerken in [!DNL Jira] of [!DNL Workfront] wanneer zij worden gewijzigd.

   1. Selecteer een van de volgende velden en updates:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Aangepaste gegevens in het rechterdeelvenster van [!DNL Jira]]</td>
         <td><p>Hiermee geeft u het dialoogvenster [!DNL Workfront] Aangepaste gegevens van een item in het dialoogvenster [!DNL Workfront] in het rechterdeelvenster.</p><p>Opmerking: De secties Aangepaste formulieren worden weergegeven in het dialoogvenster [!DNL Workfront] het juiste paneel met het toegangsniveau van [!DNL Workfront] Systeembeheerder.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Prioriteit in het rechterdeelvenster in [!DNL Jira]]</td>
         <td>Hiermee geeft u het dialoogvenster [!DNL Workfront] Prioriteit van een item in de [!DNL Workfront] in het rechterdeelvenster.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Add an update in the [!DNL Workfront] Updates, tabblad over wijzigingen in Vervaldatum in [!DNL Jira]]</td>
         <td>Hiermee voegt u een opmerking toe in het dialoogvenster [!UICONTROL Update] tabblad van het dialoogvenster [!DNL Workfront] item wanneer het [!UICONTROL Due Date] wijzigingen in gekoppelde [!DNL Jira] item.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Automatically create a user in [!DNL Workfront] als de [!DNL Jira] gebruiker heeft geen [!DNL Workfront] account]</td>
         <td><p>De volgende scenario's bestaan:</p>
          <ul>
           <li>Wanneer u <strong>[!UICONTROL Always]</strong> u de integratie inschakelt om telkens een nieuwe Workfront-gebruiker te maken [!DNL Jira] gebruiker zonder [!DNL Workfront] account voert de volgende handelingen uit op een gekoppelde [!DNL Jira] probleem:
            <ul>
             <li>Is toegewezen aan een [!DNL Jira] kwestie</li>
             <li><p>Tijd van aanmelding bij een [!DNL Jira] kwestie</p><p>Deze nieuwe gebruiker neemt geen [!DNL Workfront] licentie. De standaardinstelling is Altijd. De gebruiker heeft deze manier op [!DNL Workfront] heeft "[!UICONTROL Jira]" toegevoegd aan hun naam.</p></li>
            </ul></li>
           <li>Wanneer u <strong>[!UICONTROL Never]</strong>De volgende dingen gebeuren:
            <ul>
             <li>U kunt geen [!DNL Jira] toewijzingen op de [!DNL Workfront] objecten. In dit geval worden alleen de in [!DNL Workfront] op de [!DNL Workfront] objecten.</li>
             <li>De tijd die aan verbonden wordt geregistreerd [!DNL Jira] afgifte door een gebruiker zonder [!DNL Workfront] account wordt niet automatisch overgedragen naar de gekoppelde [!DNL Workfront] item. U kunt zich nog steeds aanmelden bij de [!DNL Workfront] item in het rechterdeelvenster van het dialoogvenster [!DNL Jira] probleem.</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Klik op **[!UICONTROL Save]**.

   Nu, telkens als een gebruiker om het even welke gebieden bijwerkt die in deze configuratie op een punt in of worden gespecificeerd [!DNL Jira] of [!DNL Workfront], wordt het gekoppelde item in de andere toepassing ook bijgewerkt.

## Problemen oplossen

### Items kunnen niet worden gemaakt in [!DNL Jira] omdat de triggervelden gemarkeerd zijn &quot;[!UICONTROL Couldn't be found]&quot;

#### Probleem

Als er een fout optreedt met onze [!DNL Workfront for Jira] toepassing, [!DNL Workfront] schakelt de triggers uit om verdere complicaties te voorkomen. Wanneer deze triggers zijn uitgeschakeld, worden deze weergegeven als &quot;[!UICONTROL Couldn't be found]&quot;.

#### Oplossing

Zoek de fout die de triggers heeft uitgeschakeld. U vindt de fout in het dialoogvenster [!DNL Workfront for Jira] &quot;[!UICONTROL Activity Log]&quot;.

De meest voorkomende oorzaak van dit gedrag is de fout &quot;[!UICONTROL Field 'duedate' cannot be set. It is not on the appropriate screen, or unknown.]&quot;

Deze fout houdt in dat u probeert &quot;[!UICONTROL Planned Completion Date]&quot; van [!DNL Workfront] tot [!DNL Jira]. Om dit te doen, moet u ervoor zorgen dat uw [!DNL Jira] objecten hebben een veld met de naam &quot;[!UICONTROL Due Date]&quot;. Als zij dit veld niet hebben, [!DNL Workfront] kan de geplande afsluitdatum niet synchroniseren vanaf [!DNL Workfront] en schakelt de triggers uit.

Voer een van de volgende handelingen uit om deze fout op te lossen:

* Vraag uw [!DNL Jira] beheerder om de betrokken [!DNL Jira] objecten om ervoor te zorgen dat ze een veld voor de vervaldatum hebben.
* Synchronisatie van [!DNL Workfront]Naar verwachting in de Workfront &quot;[!UICONTROL Setup]&quot; pagina
