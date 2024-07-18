---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Gebruikersgegevens configureren met  [!DNL Workfront Proof]
description: Gebruikersgegevens configureren met  [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# Gebruikersgegevens configureren met [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [ het Bewijzen ](../../../review-and-approve-work/proofing/proofing.md).

1. Beginnen creërend of het uitgeven van een gebruiker zoals die in [ wordt beschreven leidt tot Gebruikers gebruikend  [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. Geef de volgende informatie op:

   * In de sectie **[!UICONTROL Personal Details]** :

      * **E-mailadres:** het e-mailadres van de gebruiker.
      * **Voornaam:** de voornaam van de gebruiker.
      * **Familienaam:** de achternaam van de gebruiker.
      * **Positie:** de positie van de gebruiker in het bedrijf.
      * **profiel van de Toestemming:** de toestemmingen van de gebruiker op de proefrekening.
      * **Taal:** de primaire taal van de gebruiker.
      * **streek van de Tijd:** selecteer de tijdzone van de gebruiker.
      * **formaat van de Datum:** selecteer het aangewezen de datumformaat van de gebruiker.
      * **Opt in - product en marketing e-mail:** selecteer of om de gebruiker binnen voor product en marketing e-mail te kiezen.
      * **slechts API:** staat de gebruiker toe om slechts via API het programma te openen.

   * Typ in de sectie **[!UICONTROL User Details]** de contactgegevens van de gebruiker, zoals het adres en het telefoonnummer van de straat.
   * Configureer in de sectie **[!UICONTROL Default proof settings]** de instellingen die van invloed zijn op de manier waarop de gebruiker proefdrukken maakt of bewerkt.

      * **Standaardproefdrukrol:** selecteer een standaardproefdrukrol voor de gebruiker. Rolopties zijn **[!UICONTROL Read only]** , **[!UICONTROL Reviewer]** , **[!UICONTROL Approver]** , **[!UICONTROL Reviewer & Approver]** , **[!UICONTROL Author]** of **[!UICONTROL Moderator]** .

        Voor meer informatie over proefdrukrollen, zie [ de Rollen van het Bewijs binnen beheren  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **vergrendel de proef wanneer alle besluiten worden gemaakt:** sluit automatisch de proef van verdere veranderingen nadat alle besluiten over de proef worden genomen.
      * **vereiste Login. De proefdruk kan alleen met andere gebruikers worden gedeeld:** maakt de proefdruk beschikbaar slechts voor gebruikers met [!DNL Workfront Proof] login geloofsbrieven.
      * **slechts één vereist besluit:** vereist slechts één besluit over een bewijs.
      * **Download van origineel dossier:** laat de gebruiker toe om het originele dossier voor een proef te downloaden. Deze optie is standaard ingeschakeld.

        Voor meer informatie bij het downloaden van originele dossiers, zie [ Opgeslagen Dossiers van de Download  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Abonnement. Mensen kunnen zich aanmelden voor de proefdruk via de openbare URL of de insluitcode:** Hiermee kunnen revisoren die geen deel uitmaken van de organisatie zich aanmelden voor de proefdruk via de openbare URL of de insluitcode.

        Wanneer deze optie wordt geselecteerd, **de Abonnee moet een verbinding in e-mail klikken om tot een proef toegang te hebben** is ook beschikbaar. Selecteer deze optie als de externe controleur op een koppeling in de e-mail moet klikken om de proefdruk te openen.
Deze optie wordt toegelaten door gebrek als de **Openbare het delen** optie wordt geselecteerd.

      * **Standaardrol voor nieuwe gastrevisoren:** selecteer een standaardproefrol voor gastrevisoren. De opties zijn het zelfde als die in **Standaard proefdrukrol**, met uitzondering van Moderator en Auteur.

   * In de sectie **[!UICONTROL Default email alert settings]** :

      * **Standaard e-mailalarm:** selecteer hoe vaak de gebruiker e-mailupdates ontvangt. Selecteer **Alle Activiteit, Antwoorden aan mijn commentaren, Besluiten, Definitief besluit, Uur samenvatting, Dagelijkse samenvatting,** of **Gehandicapten**.

        Voor meer informatie over standaard e-mailwaakzame opties, zie [ de montages van het e-mailbericht in  [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) vormen

      * **Standaard e-mailalarm voor nieuwe gastrevisoren:** selecteer hoe vaak de bezoekersrecensenten e-mailupdates ontvangen. De opties zijn het zelfde als die voor **Standaard e-mailalarm.**

      * **verzend een e-mailbevestiging wanneer de proeven klaar zijn:** selecteer om de gebruiker automatisch een bevestigingsmail te verzenden wanneer de proeven klaar zijn.
      * **Formaat van e-mail die naar deze gebruiker wordt verzonden:** Uitgezochte **[!UICONTROL HTML]** of **[!UICONTROL Plain text]** als standaardformaat voor e-mail die naar de gebruiker wordt verzonden.

   * In de sectie **[!UICONTROL Custom message settings]**: Instellingen maken voor proefdruksjablonen.

     Zie voor meer informatie over sjablonen:

      * **het onderwerpmalplaatje van het Bewijs:** creeer een malplaatje voor een proefproefonderwerp.
      * **het berichtmalplaatje van het Bewijs:** creeer een malplaatje voor een proefdrukbericht en zijn formaat.
