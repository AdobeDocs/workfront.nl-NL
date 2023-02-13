---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Gebruikersgegevens configureren met [!DNL Workfront Proof]
description: Gebruikersgegevens configureren met [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 0%

---

# Gebruikersgegevens configureren met [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

1. Beginnen met het maken of bewerken van een gebruiker zoals beschreven in [Gebruikers maken met [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. Geef de volgende informatie op:

   * In de **[!UICONTROL Personal Details]** sectie:

      * **E-mailadres:** Het e-mailadres van de gebruiker.
      * **Voornaam:** De voornaam van de gebruiker.
      * **Achternaam:** De achternaam van de gebruiker.
      * **Positie:** De positie van de gebruiker in het bedrijf.
      * **Machtigingsprofiel:** De machtigingen van de gebruiker voor het proefdrukaccount.
      * **Taal:** De primaire taal van de gebruiker.
      * **Tijdzone:** Selecteer de tijdzone van de gebruiker.
      * **Datumnotatie:** Selecteer de datumnotatie van de voorkeur van de gebruiker.
      * **Inschakelen - E-mails over producten en marketing:** Geef op of u de gebruiker wilt aanmelden voor e-mails over producten en marketing.
      * **Alleen API:** Hiermee kan de gebruiker zich alleen via de API aanmelden.
   * In de **[!UICONTROL User Details]** in, typt u de contactgegevens van de gebruiker, zoals het adres en het telefoonnummer van de straat.
   * In de **[!UICONTROL Default proof settings]** , configureert u de instellingen die van invloed zijn op de manier waarop de gebruiker proefdrukken maakt of maakt.

      * **Standaardproefdrukrol:** Selecteer een standaardproefdrukrol voor de gebruiker. Rolopties zijn **[!UICONTROL Read only]**, **[!UICONTROL Reviewer]**, **[!UICONTROL Approver]**, **[!UICONTROL Reviewer & Approver]**, **[!UICONTROL Author]**, of **[!UICONTROL Moderator]**.

         Voor meer informatie over proefdrukrollen, zie [Proefrollen beheren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **Het bewijs vergrendelen wanneer alle beslissingen worden genomen:** Hiermee wordt het bewijs automatisch vergrendeld van verdere wijzigingen nadat alle beslissingen over het bewijs zijn genomen.
      * **Aanmelding vereist. De proef kan slechts met andere gebruikers worden gedeeld:** Hiermee stelt u de proefdruk alleen beschikbaar voor gebruikers met [!DNL Workfront Proof] aanmeldingsgegevens.
      * **Slechts één beslissing vereist:** Er is slechts één beslissing vereist op een bewijs.
      * **Origineel bestand downloaden:** Hiermee kan de gebruiker het oorspronkelijke bestand downloaden om het te controleren. Deze optie is standaard ingeschakeld.

         Ga voor meer informatie over het downloaden van originele bestanden naar [Bestanden downloaden die zijn opgeslagen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

         <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Abonnement. Personen kunnen zich aanmelden voor de proefdruk via de openbare URL of de insluitcode:** Hiermee kunnen revisoren die geen deel uitmaken van de organisatie zich aanmelden voor de proefdruk via de openbare URL of de insluitcode.

         Wanneer deze optie is geselecteerd, **Abonnees moeten op een koppeling in een e-mailbericht klikken om een proefdruk te openen** is ook beschikbaar. Selecteer deze optie als de externe controleur op een koppeling in de e-mail moet klikken om de proefdruk te openen.
Deze optie is standaard ingeschakeld als de optie **Openbare delen** is geselecteerd.

      * **Standaardrol voor nieuwe gastrevisoren:** Selecteer een standaardproefdrukrol voor gastrevisoren. De opties zijn gelijk aan die in **Standaardproefdrukrol.**
   * In de **[!UICONTROL Default email alert settings]** sectie:

      * **Standaard-e-mailwaarschuwing:** Selecteer hoe vaak de gebruiker e-mailupdates ontvangt. Selecteren **Alle activiteiten, antwoorden op mijn opmerkingen, besluiten, eindbesluit, samenvatting, dagelijks overzicht,** of **Uitgeschakeld**.

         Zie voor meer informatie over standaardopties voor e-mailwaarschuwingen [Instellingen voor e-mailmeldingen configureren in [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **Standaard-e-mailwaarschuwing voor nieuwe gastrevisoren:** Selecteer hoe vaak gasten updates per e-mail ontvangen. De opties zijn hetzelfde als die voor **Standaard-e-mailwaarschuwing.**

      * **Een e-mailbevestiging verzenden wanneer proefdrukken gereed zijn:** Schakel deze optie in om de gebruiker automatisch een bevestigingsbericht te sturen wanneer de proefdrukken gereed zijn.
      * **Indeling van de e-mails die naar deze gebruiker zijn verzonden:** Selecteren **[!UICONTROL HTML]** of **[!UICONTROL Plain text]** als de standaardindeling voor e-mailberichten die naar de gebruiker worden verzonden.
   * In de **[!UICONTROL Custom message settings]** sectie: Instellingen maken voor proefdruksjablonen.

      Zie voor meer informatie over sjablonen:

      * **Sjabloon proefonderwerp:** Een sjabloon maken voor een proefdrukonderwerp.
      * **Sjabloon van proefberichten:** Maak een sjabloon voor een proefdrukbericht en de opmaak ervan.
