---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: Rechten van objecten verwijderen
description: U kunt machtigingen van andere gebruikers verwijderen voor objecten die u toegang hebt tot Delen. Het verwijderen van machtigingen uit objecten is identiek voor alle objecten die kunnen worden gedeeld.
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 0%

---

# Rechten van objecten verwijderen

U kunt machtigingen van andere gebruikers verwijderen voor objecten die u toegang hebt tot Delen. Het verwijderen van machtigingen uit objecten is identiek voor alle objecten die kunnen worden gedeeld. 

Gelijkaardige overwegingen zoals voor het delen van voorwerpen zijn van toepassing voor het verwijderen van toestemmingen uit voorwerpen. Zie de sectie voor meer informatie [Overwegingen bij het delen van objecten](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) in het artikel [Overzicht van het delen van machtigingen voor objecten](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

## Toegangsvereisten

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or  
   <p>Legacy license: Request or higher</p>
   <p><b>NOTE</b></p>

   <p>Some objects require a higher access than Request. </p>
   
   <p>For example, for the current license, a Contributor can share issues, but only Standard-license users can share a project.</p>
   
   <p>For the legacy license, a Requestor can share issues, but only Workers or Planners can share a project.</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you want to share</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to the objects you want to share</p> <p>Manage permissions to remove inherited permissions on objects</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

U moet het volgende hebben om objecten te delen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront-licentie*</td> 
   <td> <p>Aanvraag of hoger</p>
   <p><b>OPMERKING</b></p>

Voor sommige objecten is een hogere toegang vereist dan Aanvraag. Een aanvrager kan bijvoorbeeld problemen delen, maar alleen Workers of Planners kunnen een project delen.

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot of hoger weergeven voor de objecten die u wilt delen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen of hoger weergeven voor de objecten die u wilt delen</p> <p>Rechten beheren om overgeërfde machtigingen voor objecten te verwijderen</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Entiteiten verwijderen uit de lijst voor delen van een object {#remove-entities-from-the-sharing-list-of-an-object}

U kunt entiteiten (gebruikers, taakrollen, teams, groepen, bedrijven) verwijderen uit de lijst voor gedeeld gebruik van een object. Hierdoor worden hun machtigingen voor het object verwijderd.

1. Ga naar het object dat u wilt delen.

   Voor informatie over welke objecten kunnen worden gedeeld, raadpleegt u [Overzicht van het delen van machtigingen voor objecten](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Klik op de knop **Meer** pictogram ![](assets/more-icon.png)naast de objectnaam klikt u op **Delen** of **Delen.**

   ![](assets/share-a-document-350x160.png)

1. Klik op de knop **x** naast de naam van een gebruiker, team, groep, bedrijf, taakrol om hen in het vakje van de objecten toegang te verwijderen.

   ![](assets/remove-permissions-on-project-nwe-350x479.png)

1. In de `<User Name>`De Workfront-toegang van wordt verwijderd uit dit keuzemenu. Selecteer of u de toegang ervan alleen wilt verwijderen uit het object dat u hebt geselecteerd of uit alle onderliggende objecten die eraan zijn gekoppeld.\
   De volgende scenario&#39;s bestaan:

   * Als u de entiteit alleen uit het object verwijdert, verliest die entiteit haar machtigingen voor het object en de overgeërfde machtigingen voor de onderliggende objecten. Als ze eerder machtigingen hadden gekregen voor de onderliggende items afzonderlijk, behouden ze dezelfde machtigingen voor alle onderliggende objecten die eraan zijn gekoppeld wanneer u deze optie selecteert. 
   * Als u de entiteit van het voorwerp en alle kindvoorwerpen verwijdert, verliest die entiteit hun toestemmingen aan het voorwerp evenals alle kindvoorwerpen, zelfs toen zij eerder individuele toestemming op elk kindvoorwerp werden verleend. 

1. Klikken **Opslaan**.

## Rechten van meerdere objecten bulksgewijs verwijderen

U kunt entiteiten (gebruikers, taakrollen, teams, groepen, bedrijven) uit verscheidene voorwerpen verwijderen tegelijkertijd wanneer u hen in een lijst in bulk selecteert. 

>[!NOTE]
>
>U kunt niet bekijken wat de toegangsentiteiten voor alle geselecteerde voorwerpen hebben wanneer u hen in massa selecteert. Voordat u de machtigingen verwijdert, moet u weten welke entiteit u uit het delen van de geselecteerde objecten wilt verwijderen.

1. Ga naar de lijst met objecten die u wilt delen.

   Voor informatie over welke objecten kunnen worden gedeeld, raadpleegt u [Overzicht van het delen van machtigingen voor objecten](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Selecteer meerdere objecten in de lijst en klik op de knop **Delen** pictogram ![](assets/share-icon.png)boven aan de lijst.
1. Typ de naam van de gebruiker, de rol, het team, de groep, of het bedrijf waarvoor u de toegang in wilt verwijderen **Bewerken `<Object Name>` toegang tot** veld.
1. Selecteer in het keuzemenu Toegang de optie **Geen toegang**.

   ![](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. In de `<User Name>`De Workfront-toegang van wordt verwijderd uit dit keuzemenu. Selecteer of u de toegang ervan alleen wilt verwijderen uit de objecten die u hebt geselecteerd of uit alle andere onderliggende objecten die eraan zijn gekoppeld.\
   De volgende scenario&#39;s bestaan:

   * Als u de entiteit alleen uit het object verwijdert, verliest die entiteit haar machtigingen voor het object en de overgeërfde machtigingen voor de onderliggende objecten. Als ze eerder machtigingen hadden gekregen voor de onderliggende items afzonderlijk, behouden ze dezelfde machtigingen voor alle onderliggende objecten die eraan zijn gekoppeld wanneer u deze optie selecteert. 
   * Als u de entiteit van het voorwerp en alle kindvoorwerpen verwijdert, verliest die entiteit hun toestemmingen aan het voorwerp evenals alle kindvoorwerpen, zelfs toen zij eerder individuele toestemming op elk kindvoorwerp werden verleend.

   **Voorbeeld:** Selecteer of u alleen machtigingen wilt verwijderen voor de taken die u in een lijst hebt geselecteerd, of voor de problemen en documenten die bij de taken horen.

   ![](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. (Optioneel) Als u machtigingen in bulk wilt wijzigen voor meerdere objecten, selecteert u een ander niveau voor delen voor de geselecteerde entiteit.

   Als zij bijvoorbeeld beheermachtigingen hebben, selecteert u Contribute of Weergeven.

1. Klikken **Opslaan**.

## Overerfde machtigingen verwijderen

Overerfde machtigingen kunnen worden verwijderd van objecten, zodat eigenaars specifiek kunnen bepalen wie toegang krijgt tot onderliggende objecten, ongeacht de toegang van een gebruiker tot een bovenliggend object.

>[!IMPORTANT]
>
>Alleen gebruikers met de machtiging Beheren kunnen overgeërfde machtigingen verwijderen.

Overerfde machtigingen verwijderen:

1. Ga naar een object waarvoor u beheerdersmachtigingen hebt. Ga bijvoorbeeld naar een taak.
1. Ga naar het vak met objecttoegang zoals wordt beschreven in het dialoogvenster [Entiteiten verwijderen uit de lijst voor delen van een object](#remove-entities-from-the-sharing-list-of-an-object) in dit artikel.
1. Selecteer **x** naast **Overgenomen machtiging** in het vak voor delen om iedereen te verwijderen die daar wordt vermeld.

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

   Dit zorgt ervoor dat niemand die toestemmingen aan het oudervoorwerp (bijvoorbeeld, het project) wordt verleend toestemmingen aan deze taak door gebrek heeft. U moet afzonderlijke entiteiten weergeven in de lijst voor gedeeld gebruik van de taak om machtigingen voor de taak te verlenen.

   >[!TIP]
   >
   >U kunt afzonderlijke entiteiten niet verwijderen uit de lijst Overgenomen machtigingen. U kunt de Overgenomen machtigingen alleen uitschakelen voor alle vermelde entiteiten.

1. Klikken **Opslaan**. 

## Een object privé maken

Als u een object in het hele systeem hebt gedeeld of dit hebt gedeeld met externe toepassingen door het openbaar te maken, kunt u het opnieuw privé maken door de systeembrede of openbare machtigingen te verwijderen. 

Voor meer informatie over het beschikbaar maken van een voorwerp voor het gehele systeem, of openbaar, zie [Een object delen](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

Een object privé maken:

1. Ga naar het object dat u privé wilt maken.\
   Navigeer bijvoorbeeld naar een rapport.
1. Klikken **Handelingen rapporteren** vervolgens **Delen**.

   ![](assets/report-permissions-make-private-nwe-350x477.png)

1. Klikken **Openbare toegang verwijderen** om de toegang van externe gebruikers tot het bekijken van het rapport te verwijderen.
1. Klikken **Toegang voor het hele systeem verwijderen** om te stoppen met het delen met alle Workfront-gebruikers. 
1. Klikken **Opslaan**.
