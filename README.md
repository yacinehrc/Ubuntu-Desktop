# Ubuntu Desktop — Guide d'installation complet
<img width="1919" height="1034" alt="Capture d&#39;écran 2026-06-26 135323" src="https://github.com/user-attachments/assets/4efec2e8-ade4-48e5-9eee-81e6d96ec9bb" />

> Ce guide couvre deux scénarios : installer Ubuntu dans une **machine virtuelle (VMware)** pour tester sans risque, ou installer Ubuntu **directement sur un PC** pour lui donner une seconde vie. Les deux parcours sont documentés pas à pas avec captures d'écran.

---

## Table des matières

- [Prérequis & Téléchargement de l'ISO](#prérequis--téléchargement-de-liso)
- [Option A — Installation via Machine Virtuelle (VMware)](#option-a--installation-via-machine-virtuelle-vmware)
  - [Création de la VM](#1-création-de-la-vm)
  - [Configuration matérielle](#2-configuration-matérielle)
- [Option B — Installation sur PC physique](#option-b--installation-sur-pc-physique)
- [Installation d'Ubuntu Desktop](#installation-dubuntu-desktop)
- [Premier démarrage & Configuration](#premier-démarrage--configuration)
- [Bureau Ubuntu — Prise en main](#bureau-ubuntu--prise-en-main)

---

## Prérequis & Téléchargement de l'ISO

📥 Téléchargez l'image ISO d'Ubuntu Desktop sur le site officiel :
**[ubuntu.com/download/desktop](https://ubuntu.com/download/desktop)**

> La version **LTS** (Long Term Support) est recommandée pour sa stabilité à long terme.

---

## Option A — Installation via Machine Virtuelle (VMware)

Une machine virtuelle (VM) permet de faire tourner Ubuntu dans une fenêtre de votre système actuel (Windows, macOS, Linux) sans modifier votre disque dur. C'est la solution idéale pour tester ou développer dans un environnement isolé.

### 1. Création de la VM

Ouvrez **VMware Workstation** et lancez la création d'une nouvelle machine virtuelle.

<img width="1919" height="1029" alt="Capture d&#39;écran 2026-06-26 132832" src="https://github.com/user-attachments/assets/d2f72d8e-9a25-4d4f-a5b6-4570ad9e7c7e" />
<img width="1919" height="1032" alt="Capture d&#39;écran 2026-06-26 132851" src="https://github.com/user-attachments/assets/31ac2dcf-a361-4109-b14b-2d8d14835818" />

Sélectionnez **"Personnalisée (avancée)"** pour un paramétrage plus précis ou alors **"Typique (recommandé)"** pour un processus guidé simplifié.

<img width="1919" height="1029" alt="Capture d&#39;écran 2026-06-26 132904" src="https://github.com/user-attachments/assets/d74e0bb0-f75c-4454-abba-fd3958073b3e" />

Appuyez sur **"Suivant"** pour la compatibilité matérielle, celle proposée sera la **"Workstation 25H2"**, il se peut que vous ayez une version un peu plus ancienne, mais qui fonctionnera correctement.

<img width="1919" height="1031" alt="Capture d&#39;écran 2026-06-26 132916" src="https://github.com/user-attachments/assets/a5c2bad3-9701-4194-92fa-2b37e3a7ef68" />

Choisissez **"Fichier image du disque d'installation (iso)"** et sélectionnez l'ISO Ubuntu téléchargée. VMware détecte automatiquement le système et active le mode **Easy Install**.

<img width="1919" height="1029" alt="Capture d&#39;écran 2026-06-26 132950" src="https://github.com/user-attachments/assets/a073a464-ce50-4022-9af8-afe416121f2e" />

Renseignez le **nom d'utilisateur** et le **mot de passe** du compte Ubuntu qui sera créé automatiquement lors de l'installation.

<img width="1919" height="1031" alt="Capture d&#39;écran 2026-06-26 133040" src="https://github.com/user-attachments/assets/99b8568f-b075-494e-88d5-cef47deeabd1" />

### 2. Configuration matérielle

Donnez un **nom à votre VM** et choisissez l'emplacement de stockage sur votre disque.

<img width="1919" height="1032" alt="Capture d&#39;écran 2026-06-26 133056" src="https://github.com/user-attachments/assets/2ad6f4db-3200-4217-98cd-f70ceba23049" />

Indiquez le **nombre de processeur** que vous partagerez à votre VM.

<img width="1919" height="1032" alt="Capture d&#39;écran 2026-06-26 133115" src="https://github.com/user-attachments/assets/818f6757-3a52-483b-b40b-f64604252461" />

Puis la **mémoire vive** (RAM).

<img width="1919" height="1034" alt="Capture d&#39;écran 2026-06-26 133135" src="https://github.com/user-attachments/assets/3004199b-b6a7-4193-a91e-a850402098ac" />

Choisissez le type de réseau à utiliser (priviligiez "*NAT*" ou "*par un pont*").

<img width="1919" height="1029" alt="Capture d&#39;écran 2026-06-26 133143" src="https://github.com/user-attachments/assets/bdb6c6c7-6305-4784-a9ec-242dbc15cdac" />

Ensuite, appuyez sur **"Suivant"** pour laisser par défaut jusqu'à arriver sur les paramètres de **taille du disque dur**.

<img width="1919" height="1034" alt="Capture d&#39;écran 2026-06-26 133150" src="https://github.com/user-attachments/assets/fe3802d8-3c9b-4c7b-a601-b664c9645696" />
<img width="1919" height="1029" alt="Capture d&#39;écran 2026-06-26 133157" src="https://github.com/user-attachments/assets/05044f43-dd7c-4cf4-a390-22d36e306593" />
<img width="1919" height="1032" alt="Capture d&#39;écran 2026-06-26 133204" src="https://github.com/user-attachments/assets/57c6524b-f5fc-4656-ac3d-daaf5ca0d100" />

Définissez la **taille du disque virtuel** allouée à la VM. Un minimum de **20 Go** est recommandé. Sélectionnez "Store virtual disk as a single file" pour de meilleures performances. Puis, choisissez l'emplacement du disque dur virtuel.

<img width="1919" height="1032" alt="Capture d&#39;écran 2026-06-26 133215" src="https://github.com/user-attachments/assets/1fc03a1b-d334-4a0b-9c22-1f54da5e4af2" />
<img width="1919" height="1027" alt="Capture d&#39;écran 2026-06-26 133225" src="https://github.com/user-attachments/assets/c986494c-18ae-44ad-8ed0-431c49f76c59" />

Un récapitulatif de la configuration s'affiche. Cliquez sur **"Customize Hardware..."** si vous souhaitez ajuster la RAM ou les cœurs CPU, puis sur **Finish** pour démarrer la VM.

<img width="1919" height="1032" alt="Capture d&#39;écran 2026-06-26 133247" src="https://github.com/user-attachments/assets/c13e413f-3c0e-4194-a2a6-1e1e06ba7e33" />

> VMware lance alors l'installation automatiquement. Passez directement à la section [Installation d'Ubuntu Desktop](#installation-dubuntu-desktop).

---

## Option B — Installation sur PC physique

Cette méthode installe Ubuntu directement sur le disque d'un PC existant — idéal pour **redonner une seconde vie à un ancien ordinateur**. Elle remplace (ou coexiste avec) le système d'exploitation actuel.

### Matériel nécessaire

- Une clé USB d'au moins **8 Go**
- Le logiciel **[Rufus](https://rufus.ie)** (Windows) ou **[Balena Etcher](https://etcher.balena.io)** (multiplateforme)

### Création de la clé USB bootable

Branchez la clé USB, ouvrez Rufus, sélectionnez l'ISO Ubuntu téléchargée et cliquez sur **Start**. L'opération prend quelques minutes.

### Démarrage depuis la clé USB

Redémarrez le PC cible et accédez au **Boot Menu** via la touche correspondant à votre constructeur :

| Constructeur | Touche |
|---|---|
| HP | `F9` ou `Esc` |
| Dell | `F12` |
| Lenovo | `F12` ou `F11` |
| ASUS | `F8` ou `Esc` |
| Acer | `F12` |

Sélectionnez la clé USB comme périphérique de démarrage, puis continuez vers la section suivante.

---

## Installation d'Ubuntu Desktop

À partir d'ici, le processus est identique que vous soyez en VM ou sur PC physique.

Choisissez la **disposition du clavier** correspondant à votre matériel (ex. : French pour un clavier AZERTY).

<img width="1919" height="1032" alt="Capture d&#39;écran 2026-06-26 134131" src="https://github.com/user-attachments/assets/e2f84068-704b-4dee-ae8c-ddafcb853fb9" />

Sélectionnez le **type d'installation**. L'option **"Normal installation"** convient à la majorité des usages. Cochez également l'installation des mises à jour et des pilotes tiers si vous avez une connexion Internet.

<img width="1919" height="1032" alt="Capture d&#39;écran 2026-06-26 134150" src="https://github.com/user-attachments/assets/ddbd87f2-edc5-46e7-94bd-e06aa8414cc6" />

Choisissez le **type de partitionnement**. Pour un PC dédié à Ubuntu, l'option **"Erase disk and install Ubuntu"** est la plus simple et la plus rapide.

> ⚠️ Cette option efface l'intégralité du disque sélectionné. Sauvegardez vos données importantes avant de continuer.

<img width="1917" height="1034" alt="Capture d&#39;écran 2026-06-26 134216" src="https://github.com/user-attachments/assets/24367e5b-2686-4c28-b3a3-41d43cd30fc2" />

Confirmez l'écriture sur le disque en cliquant sur **"Continue"**.

<img width="1917" height="1034" alt="Capture d&#39;écran 2026-06-26 134229" src="https://github.com/user-attachments/assets/696cc29c-e19e-40a5-a0c8-65678d9fae48" />

Sélectionnez votre **fuseau horaire** sur la carte interactive.

<img width="1919" height="1034" alt="Capture d&#39;écran 2026-06-26 134242" src="https://github.com/user-attachments/assets/39d838bf-2416-43f8-9dfc-41b2fc6a23ef" />

Créez votre **compte utilisateur** : renseignez votre nom complet, le nom de la machine, votre identifiant et un mot de passe.

<img width="1919" height="1031" alt="Capture d&#39;écran 2026-06-26 134345" src="https://github.com/user-attachments/assets/8a6d829b-86b9-44f9-984d-d22d218cebaf" />

L'installation démarre. Cette étape prend généralement entre **5 et 15 minutes** selon les performances de la machine.

<img width="1919" height="1032" alt="Capture d&#39;écran 2026-06-26 134428" src="https://github.com/user-attachments/assets/156d8642-74c1-4396-9218-949722c6ee9a" />

Une fois l'installation terminée, un message vous invite à **redémarrer**. Si vous étiez en mode PC physique, retirez la clé USB avant de relancer.

<img width="1919" height="1034" alt="Capture d&#39;écran 2026-06-26 135045" src="https://github.com/user-attachments/assets/c8ed2ae1-9faf-4417-86d0-ff22e9b31d86" />

---

## Premier démarrage & Configuration

Au premier lancement, Ubuntu affiche un écran de connexion. Saisissez le mot de passe défini lors de l'installation.

<img width="1919" height="1032" alt="Capture d&#39;écran 2026-06-26 135142" src="https://github.com/user-attachments/assets/7e01cae7-c23a-4991-9cff-1963c62dbb7e" />
<img width="1919" height="1032" alt="Capture d&#39;écran 2026-06-26 135157" src="https://github.com/user-attachments/assets/4be2448e-b006-440d-9aa3-ad4b33e3b111" />

Un assistant de bienvenue se lance automatiquement pour configurer les derniers paramètres.

<img width="1919" height="1032" alt="Capture d&#39;écran 2026-06-26 135221" src="https://github.com/user-attachments/assets/f123de28-f11b-41e8-811d-ac21ba965c41" />

Ubuntu propose un abonnement **Ubuntu Pro** (optionnel et gratuit pour usage personnel). Vous pouvez ignorer cette étape.

<img width="1919" height="1034" alt="Capture d&#39;écran 2026-06-26 135232" src="https://github.com/user-attachments/assets/9f392ad8-0af1-4134-8e85-4ecc9cef2330" />

Configurez vos **préférences de confidentialité** (partage de données, géolocalisation).

<img width="1919" height="1034" alt="Capture d&#39;écran 2026-06-26 135254" src="https://github.com/user-attachments/assets/c91377d4-7f6b-4aa1-aced-2fdd30e505fb" />
<img width="1919" height="1036" alt="Capture d&#39;écran 2026-06-26 135244" src="https://github.com/user-attachments/assets/83e9e915-2374-449d-b81d-67699ed924f0" />

L'assistant se conclut avec un message de bienvenue. Cliquez sur **"Done"** pour accéder au bureau.

<img width="1919" height="1032" alt="Capture d&#39;écran 2026-06-26 135310" src="https://github.com/user-attachments/assets/626e5317-cc33-4da5-8b9a-6985a6c63e1a" />


---

## Bureau Ubuntu — Prise en main

Vous accédez désormais au **bureau Ubuntu Desktop**. L'environnement GNOME est prêt à l'emploi.

<img width="1919" height="1034" alt="Capture d&#39;écran 2026-06-26 135323" src="https://github.com/user-attachments/assets/ebf4309f-a124-44dc-93a2-af05a45aaec2" />

Vous avez les applications disponibles en appuyant sur **l'icône à 9 boutons**.

Ubuntu Desktop est maintenant pleinement opérationnel. Vous pouvez installer vos applications via le **gestionnaire de logiciels** ou directement depuis le terminal avec `apt`.

---

> 🔗 Ce repository est utilisé comme prérequis dans [yacinehrc/nextcloud](https://github.com/yacinehrc/nextcloud) pour la mise en place d'une infrastructure cloud privée sous Docker.

*Réalisé par [Yacine Harrache](https://github.com/yacinehrc) — BTS SIO SLAM | EPSI Lille*
