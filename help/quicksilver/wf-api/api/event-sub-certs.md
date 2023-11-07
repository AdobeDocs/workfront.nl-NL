---
content-type: api
navigation-topic: api-navigation-topic
title: Abonnementscertificaten voor gebeurtenissen
description: Abonnementscertificaten voor gebeurtenissen
author: Becky
feature: Workfront API
role: Developer
exl-id: 3606b6c3-b373-47ea-9cb5-813bd3af8da7
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Client-TLS configureren voor gebeurtenisabonnement

<!--Configuring Client TLS for Event Subscription
Steps to Verify Workfront's Client Certificate
Examples for Server configuration
NGINX
Apache
Certificate to Environment Mapping
Certificates
Production
Preview
Sandbox 1
Sandbox 2
-->

Met client-TLS kunt u controleren of het abonnementsbericht voor gebeurtenissen dat u ontvangt, daadwerkelijk afkomstig is van Adobe Workfront. Om deze functionaliteit in te schakelen, moet uw server zijn geconfigureerd om een Workfront x509-certificaat aan te vragen en te valideren.


## Workfront-clientcertificaat verifiëren

Deze procedure veronderstelt uw server wordt gevormd om de verbindingen van TLS goed te keuren. Workfront biedt geen ondersteuning voor zelfondertekende certificaten.

Over het algemeen zijn dit de stappen die nodig zijn om clientverificatie voor uw server in te schakelen:

1. Download de PEM-versie van het DigiCert Global Root CA-certificaat.
1. Schakel verificatie van clientcertificaten in.

   Geef het CA-certificaat van stap 1 op als vertrouwd.

1. Stel de verificatiediepte in op 2 omdat ons certificaat is ondertekend door de DigiCert SHA2 Secure Server CA. Dit is een tussenliggende CA onder DigiCert Global Root CA.
1. Controleer of het clientcertificaat daadwerkelijk afkomstig is van Workfront door de betreffende domeinnaam te controleren.

## Voorbeelden voor serverconfiguratie

### NGINX

```
server {

    listen 443 ssl default_server;
    # ... existing SSL configuration for server authentication ...

    ssl_verify_client on;
    ssl_client_certificate /path/to/DigiCert_Global_Root_CA.pem;
    ssl_verify_depth 2;

        # ... existing location configuration ...
    }
}
```

Zie de klasse [NGiNX-documentatie voor ngx_http_ssl_module](http://nginx.org/en/docs/http/ngx_http_ssl_module.html).

### Apache

```
Listen 443
<VirtualHost *:443>
    # ... existing SSL configuration for server authentication ...

    SSLVerifyClient require
    SSLCACertificateFile "/path/to/DigiCert_Global_Root_CA.pem"
    SSLVerifyDepth 2
</VirtualHost>

<Directory /var/www/>
    Require expr "%{SSL_CLIENT_S_DN_CN} == <>"

    # ... existing directory configuration ...
</Directory>
```

Zie voor meer informatie

* [Clientverificatie en toegangsbeheer](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Mod Apache Module_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## Toewijzing certificaat aan omgeving

| WF-omgeving | Algemene naam certificaat | Certificaatonderwerp (DN) |
| -- | -- | -- |
| Productie | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com |
| Voorvertoning | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com |
| Sandbox 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |
| Sandbox 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## Certificaten downloaden

Klik op de volgende koppelingen om de clientcertificaten te downloaden.

* [Clientcertificaat - Productieomgeving](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_production.crt)
* [Clientcertificaat - Voorvertoningsomgeving](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_preview.crt)
* [Clientcertificaat - Sandbox-omgeving](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_sandboxes.crt)

>[!NOTE]
>
>U kunt hetzelfde clientcertificaat gebruiken voor beide Sandbox-omgevingen.
