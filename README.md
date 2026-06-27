# Ubuntu Desktop — Guide d'installation complet

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

Ouvrez **VMware Workstation** (ou VMware Player) et lancez la création d'une nouvelle machine virtuelle.

![Accueil VMware Workstation](https://github.com/user-attachments/assets/3d4632c2-9bb2-4c90-b764-41bb3e298f87)

Sélectionnez **"Typical (recommended)"** pour un processus guidé simplifié.

![Choix du type d'installation](https://github.com/user-attachments/assets/110331a2-fd4d-403f-bcd3-e76c93326b3f)

Choisissez **"Installer disc image file (iso)"** et sélectionnez l'ISO Ubuntu téléchargée. VMware détecte automatiquement le système et active le mode **Easy Install**.

![Sélection de l'ISO Ubuntu](https://github.com/user-attachments/assets/87ab0fac-f911-4b4d-89fd-931495e412e6)

Renseignez le **nom d'utilisateur** et le **mot de passe** du compte Ubuntu qui sera créé automatiquement lors de l'installation.

![Création du compte utilisateur](https://github.com/user-attachments/assets/a2ab2e59-77ff-489b-9435-1845f6daca82)

### 2. Configuration matérielle

Donnez un **nom à votre VM** et choisissez l'emplacement de stockage sur votre disque.

![Nom et emplacement de la VM](https://github.com/user-attachments/assets/27440a34-f611-48e6-b1a7-3574f48a7867)

Définissez la **taille du disque virtuel** allouée à la VM. Un minimum de **20 Go** est recommandé. Sélectionnez "Store virtual disk as a single file" pour de meilleures performances.

![Taille du disque virtuel](https://github.com/user-attachments/assets/ac73d4c4-60ba-4b30-8f5f-0212de3f023e)

Un récapitulatif de la configuration s'affiche. Cliquez sur **"Customize Hardware..."** si vous souhaitez ajuster la RAM ou les cœurs CPU, puis sur **Finish** pour démarrer la VM.

![Récapitulatif de la configuration](https://github.com/user-attachments/assets/5c6ad93f-8806-47b8-b491-2f268273a72a)

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

Sélectionnez votre **langue** puis cliquez sur **"Install Ubuntu"**.

![Sélection de la langue](https://github.com/user-attachments/assets/1293c2f1-d1d8-413a-9b4d-5adafa3152e7)

Choisissez la **disposition du clavier** correspondant à votre matériel (ex. : French pour un clavier AZERTY).

![Choix du clavier](https://github.com/user-attachments/assets/e580048c-66fb-4cc7-81ee-85acb31ad705)

Sélectionnez le **type d'installation**. L'option **"Normal installation"** convient à la majorité des usages. Cochez également l'installation des mises à jour et des pilotes tiers si vous avez une connexion Internet.

![Type d'installation](https://github.com/user-attachments/assets/ab04b431-ab30-4d87-882d-6dbf3e87c796)

Si disponible, l'installeur propose de vous connecter au réseau pour télécharger les mises à jour pendant l'installation.

![Connexion réseau](https://github.com/user-attachments/assets/b365a5e9-6e02-4022-b54c-2fabcf4f25d6)

Choisissez le **type de partitionnement**. Pour un PC dédié à Ubuntu, l'option **"Erase disk and install Ubuntu"** est la plus simple et la plus rapide.

> ⚠️ Cette option efface l'intégralité du disque sélectionné. Sauvegardez vos données importantes avant de continuer.

![Type de partitionnement](https://github.com/user-attachments/assets/f4be0e1e-e1c3-4632-aa32-c5e792900cd3)

Confirmez l'écriture sur le disque en cliquant sur **"Continue"**.

![Confirmation du partitionnement](https://github.com/user-attachments/assets/1c81180a-2783-4a22-8c66-166063444d87)

Sélectionnez votre **fuseau horaire** sur la carte interactive.

![Choix du fuseau horaire](https://github.com/user-attachments/assets/842dfb4c-80a9-49d7-8ffc-5a9661c9a3e6)

Créez votre **compte utilisateur** : renseignez votre nom complet, le nom de la machine, votre identifiant et un mot de passe.

![Création du compte](https://github.com/user-attachments/assets/98b5e3ef-d5db-4a88-ad67-25fabaac1ffd)

L'installation démarre. Cette étape prend généralement entre **5 et 15 minutes** selon les performances de la machine.

![Installation en cours](https://github.com/user-attachments/assets/a8ffb485-0f97-4539-997e-353a2e772790)

Une fois l'installation terminée, un message vous invite à **redémarrer**. Si vous étiez en mode PC physique, retirez la clé USB avant de relancer.

![Installation terminée — Redémarrer](https://github.com/user-attachments/assets/7580d129-98d1-4d31-bd08-c5fdf89a916b)

---

## Premier démarrage & Configuration

Au premier lancement, Ubuntu affiche un écran de connexion. Saisissez le mot de passe défini lors de l'installation.

![Écran de connexion](https://github.com/user-attachments/assets/aa8adf72-f979-49d7-b7d5-ed25b9dfc8b8)

Un assistant de bienvenue se lance automatiquement pour configurer les derniers paramètres.

![Assistant de bienvenue Ubuntu](https://github.com/user-attachments/assets/3d657dfd-8291-4f9b-8280-ce7a63cdb46c)

Configurez vos **préférences de confidentialité** (partage de données, géolocalisation).

![Paramètres de confidentialité](https://github.com/user-attachments/assets/bbc97950-2704-4dae-afbf-f2e072fa3f9f)

Ubuntu propose un abonnement **Ubuntu Pro** (optionnel et gratuit pour usage personnel). Vous pouvez ignorer cette étape.

![Ubuntu Pro](https://github.com/user-attachments/assets/0b5d62bb-dfa7-4a52-ba6e-6e87c7b3cd21)

L'assistant propose une sélection d'**applications recommandées** selon vos usages.

![Applications recommandées](https://github.com/user-attachments/assets/ba9cb96f-8158-438d-85dd-1228e3751aba)

L'assistant se conclut avec un message de bienvenue. Cliquez sur **"Done"** pour accéder au bureau.

![Fin de l'assistant](https://github.com/user-attachments/assets/22120e38-3cae-494b-97a8-c2a0618156fd)

---

## Bureau Ubuntu — Prise en main

Vous accédez désormais au **bureau Ubuntu Desktop**. L'environnement GNOME est prêt à l'emploi.

![Bureau Ubuntu Desktop](https://github.com/user-attachments/assets/3ccea4b7-5fc0-45ed-9a74-78f96d410100)

![Vue du bureau avec dock latéral](https://github.com/user-attachments/assets/b7d35c45-fa9f-41aa-a1c1-511d10cff1ec)

![Gestionnaire de fichiers Nautilus](https://github.com/user-attachments/assets/fb82c846-973e-4c6d-af9f-67423b8e8d9f)

![Menu des applications](https://github.com/user-attachments/assets/609a5ae5-c528-407b-8536-cc88f8226b3f)

![Paramètres système](https://github.com/user-attachments/assets/7bf68df6-d3ee-455a-a496-6c7b1564d19e)

![Terminal Ubuntu](https://github.com/user-attachments/assets/85488b2b-572a-4c41-8002-3077ec4bd2f0)

![Bureau avec plusieurs fenêtres ouvertes](https://github.com/user-attachments/assets/e40be6b0-b128-4482-9f39-a2f5f8e8e2a9)

![Vue d'ensemble des espaces de travail](https://github.com/user-attachments/assets/a9fc304f-3564-43c3-b27f-b49582d0a0f0)

![Navigation web avec Firefox](https://github.com/user-attachments/assets/83728765-45d7-423a-b96d-ae737252deca)

![Bureau finalisé et fonctionnel](https://github.com/user-attachments/assets/275a9a37-734d-4aba-b8f8-895847220af2)

![Ubuntu Desktop opérationnel](https://github.com/user-attachments/assets/16b21205-615f-4136-abb4-a0395b725fb7)

Ubuntu Desktop est maintenant pleinement opérationnel. Vous pouvez installer vos applications via le **gestionnaire de logiciels** ou directement depuis le terminal avec `apt`.

---

> 🔗 Ce repository est utilisé comme prérequis dans [yacinehrc/nextcloud](https://github.com/yacinehrc/nextcloud) pour la mise en place d'une infrastructure cloud privée sous Docker.

*Réalisé par [Yacine Harrache](https://github.com/yacinehrc) — BTS SIO SLAM | EPSI Lille*
