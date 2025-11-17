**Axepta Online – PrestaShop Payment Module**

![License](https://img.shields.io/badge/License-MIT-green)
![PHP](https://img.shields.io/badge/PHP-%3E=7.2-blue)
![PrestaShop](https://img.shields.io/badge/PrestaShop-1.7.5.0%20→%208.2-orange)
![Release](https://img.shields.io/github/v/release/AxeptaBNPParibas/AxeptaOnline-Prestashop-plugin)
![Downloads](https://img.shields.io/github/downloads/AxeptaBNPParibas/AxeptaOnline-Prestashop-plugin/total)

Overview

The Axepta Online module for PrestaShop enables merchants to process secure online payments through Axepta BNP Paribas.

💳 Supported Payment Methods
- CB  
- Visa  
- Mastercard  
- American Express  
- Apple Pay (on checkout page)  
- Google Pay (on checkout page)  
- PayPal

⚙️ Features
- Automatic capture  
- Manual capture  
- Delayed capture  

📦 Installation

Method 1 — PrestaShop Back-office

Go to Modules > Module Manager

Click Upload a module

Upload the ZIP

Follow instructions

Method 2 — Manual Installation

Extract the ZIP

Copy the folder to /modules/

Install the module from the Module Manager

⬇️ Download

Download the latest version here:

[📥 Download Latest Release](../../releases/latest)

Each release includes:

ZIP package

SHA256 hash

> ⚠️ Security Warning: Only use this release if signature verification succeeds. A failed verification means the file may have been tampered with, you can check verification steps in release page.

📞 Support

📧 assistance.ecommerce@bnpparibas.com

-----------------------------------------------------------

 **Axepta Online – Module de paiement PrestaShop**
![License](https://img.shields.io/badge/License-MIT-green)
![PHP](https://img.shields.io/badge/PHP-%3E=7.2-blue)
![PrestaShop](https://img.shields.io/badge/PrestaShop-1.7.5.0%20→%208.2-orange)
![Release](https://img.shields.io/github/v/release/AxeptaBNPParibas/AxeptaOnline-Prestashop-plugin)
![Downloads](https://img.shields.io/github/downloads/AxeptaBNPParibas/AxeptaOnline-Prestashop-plugin/total)


Présentation

Le module Axepta Online pour PrestaShop permet aux marchands d’accepter des paiements sécurisés en ligne via Axepta BNP Paribas.
Il s’intègre de manière fluide et supporte un ensemble complet de moyens de paiement.

💳 Moyens de paiement
- CB  
- Visa  
- Mastercard  
- American Express  
- Apple Pay (intégré sur la page de paiement)  
- Google Pay (intégré sur la page de paiement)  
- PayPal

⚙️ Fonctionnalités
- Capture **automatique**  
- Capture **manuelle**  
- Capture **différée**  

📦 Installation

Méthode 1 — Back-office PrestaShop

    Aller dans Modules > Module Manager
    
    Cliquer sur Upload a module
    
    Importer le fichier ZIP
    
    Suivre les instructions à l’écran

Méthode 2 — Installation manuelle

    Dézipper l'archive
    
    Copier le dossier dans /modules/
    
    Installer le module via Module Manager
  

⬇️ Téléchargement

Téléchargez la dernière version ici :
👉 GitHub → Releases

Chaque version contient :

Le ZIP du module

Le hash SHA256

La signature numérique RSA


| Version | Taille | SHA256 |
|---------|--------|------------------------------------------------------------------|
| 2.0.0   | 799.36 KB | ff80b0dea4629eaeb1dca54f9ad8e3c05aee8f0208dc4d79e8c90ead566fda02 |


🔐 Vérification de l’authenticité
1) Télécharger la clé publique


`curl -LO https://raw.githubusercontent.com/AxeptaBNPParibas/.github/refs/heads/main/axepta-online-github.crt`

4) Vérifier la signature

      `openssl x509 -in axepta-online-github.crt -pubkey -noout > public_key.pem`\
     `openssl dgst -sha256 -verify public_key.pem -signature axepta-prestashop-2.0.0.zip.sig axepta-prestashop-2.0.0.zip`

Résultat attendu :

✅ Verified OK


⚠️ N’installez pas le module si la vérification échoue.

📞 Support

📧 assistance.ecommerce@bnpparibas.com


