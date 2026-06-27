# Ubuntu Desktop — Guide d'installation complet

> Ce guide s'adresse à deux profils : ceux qui souhaitent créer une **machine virtuelle (VM)** Ubuntu sur leur poste de travail, et ceux qui veulent **redonner vie à un ancien PC** en y installant Ubuntu nativement. Les deux approches sont couvertes pas à pas, avec captures d'écran à chaque étape.

---

## Table des matières

- [Prérequis & Téléchargement de l'ISO](#prérequis--téléchargement-de-liso)
- [Option A — Installation via Machine Virtuelle (VMware)](#option-a--installation-via-machine-virtuelle-vmware)
  - [Création de la VM](#1-création-de-la-vm)
  - [Configuration matérielle](#2-configuration-matérielle)
  - [Montage de l'ISO et démarrage](#3-montage-de-liso-et-démarrage)
- [Option B — Installation sur PC physique](#option-b--installation-sur-pc-physique)
  - [Création d'une clé USB bootable](#1-création-dune-clé-usb-bootable)
  - [Démarrage depuis la clé USB](#2-démarrage-depuis-la-clé-usb)
- [Installation d'Ubuntu Desktop](#installation-dubuntu-desktop)
- [Premier démarrage](#premier-démarrage)

---

## Prérequis & Téléchargement de l'ISO

📥 Téléchargez l'image ISO d'Ubuntu Desktop sur le site officiel :
**[ubuntu.com/download/desktop](https://ubuntu.com/download/desktop)**

> La version **LTS** (Long Term Support) est recommandée pour une stabilité maximale.

---

## Option A — Installation via Machine Virtuelle (VMware)

Cette méthode permet de faire tourner Ubuntu dans une fenêtre de votre système actuel (Windows, macOS ou Linux), sans modifier votre machine. Elle est idéale pour tester ou développer dans un environnement isolé.

### 1. Création de la VM

Ouvrez **VMware Workstation** (ou VMware Player) et cliquez sur **"Create a New Virtual Machine"**.

![Accueil VMware](https://github.com/user-attachments/assets/3d4632c2-9bb2-4c90-b764-41bb3e298f87)

Sélectionnez **"Typical (recommended)"** puis cliquez sur **Next**.

![Type d'installation](https://github.com/user-attachments/assets/110331a2-fd4d-403f-bcd3-e76c93326b3f)

Choisissez **"Installer disc image file (iso)"**, puis parcourez vos fichiers pour sélectionner l'ISO Ubuntu téléchargée précédemment.

![Sélection de l'ISO](https://github.com/user-attachments/assets/87ab0fac-f911-4b4d-89fd-931495e412e6)

### 2. Configuration matérielle

Renseignez un **nom d'utilisateur** et un **mot de passe** pour la session Ubuntu qui sera créée automatiquement.

![Création du compte utilisateur](https://github.com/user-attachments/assets/a2ab2e59-77ff-489b-9435-1845f6daca82)

Donnez un **nom à votre VM** et choisissez l'emplacement où elle sera stockée sur le disque.

![Nom et emplacement de la VM](https://github.com/user-attachments/assets/27440a34-f611-48e6-b1a7-3574f48a7867)

Définissez la **taille du disque virtuel** alloué à la VM (20 Go minimum recommandés). Sélectionnez l'option **"Store virtual disk as a single file"** pour de meilleures performances.

![Taille du disque](https://github.com/user-attachments/assets/ac73d4c4-60ba-4b30-8f5f-0212de3f023e)

Un récapitulatif de la configuration s'affiche. Cliquez sur **"Customize Hardware..."** si vous souhaitez ajuster la RAM ou le nombre de cœurs CPU avant de finaliser.

![Récapitulatif de la configuration](https://github.com/user-attachments/assets/5c6ad93f-8806-47b8-b491-2f268273a72a)

### 3. Montage de l'ISO et démarrage

La VM démarre automatiquement et VMware lance l'installation d'Ubuntu en mode **Easy Install**. L'avancement est visible directement dans la fenêtre.

![Démarrage de la VM](https://github.com/user-attachments/assets/1293c2f1-d1d8-413a-9b4d-5adafa3152e7)

![Installation en cours](https://github.com/user-attachments/assets/e580048c-66fb-4cc7-81ee-85acb31ad705)

![Progression de l'installation](https://github.com/user-attachments/assets/ab04b431-ab30-4d87-882d-6dbf3e87c796)

![Fin de l'installation automatique](https://github.com/user-attachments/assets/b365a5e9-6e02-4022-b54c-2fabcf4f25d6)

Une fois l'installation terminée, la VM redémarre automatiquement sur le bureau Ubuntu.

![Redémarrage de la VM](https://github.com/user-attachments/assets/f4be0e1e-e1c3-4632-aa32-c5e792900cd3)

---

## Option B — Installation sur PC physique

Cette méthode consiste à installer Ubuntu directement sur le disque d'un PC existant — idéal pour **redonner une seconde vie à un ancien ordinateur**. Elle remplace (ou coexiste avec) le système d'exploitation actuel.

### 1. Création d'une clé USB bootable

> Vous aurez besoin d'une clé USB d'au moins **8 Go** et du logiciel **[Rufus](https://rufus.ie)** (Windows) ou **[Balena Etcher](https://etcher.balena.io)** (multiplateforme).

Branchez la clé USB, ouvrez Rufus, sélectionnez l'ISO Ubuntu téléchargée et cliquez sur **Start**. L'opération prend quelques minutes.

### 2. Démarrage depuis la clé USB

Redémarrez le PC cible et accédez au **Boot Menu** (généralement via `F2`, `F11`, `F12` ou `Suppr` selon la marque). Sélectionnez la clé USB comme périphérique de démarrage.

---

## Installation d'Ubuntu Desktop

Que vous soyez en VM ou sur PC physique, l'assistant d'installation Ubuntu est identique à partir de cette étape.

Sélectionnez votre **langue** puis cliquez sur **"Install Ubuntu"**.

![Écran d'accueil de l'installeur](https://github.com/user-attachments/assets/1c81180a-2783-4a22-8c66-166063444d87)

Choisissez la **disposition du clavier** correspondant à votre matériel (ex. : French pour un clavier AZERTY).

![Choix du clavier](https://github.com/user-attachments/assets/842dfb4c-80a9-49d7-8ffc-5a9661c9a3e6)

Sélectionnez le type d'installation. L'option **"Normal installation"** est recommandée pour un usage courant. Cochez également les mises à jour et pilotes tiers si vous avez une connexion Internet.

![Type d'installation](https://github.com/user-attachments/assets/98b5e3ef-d5db-4a88-ad67-25fabaac1ffd)

Choisissez le **type de partitionnement** du disque. Pour un PC dédié à Ubuntu, l'option **"Erase disk and install Ubuntu"** est la plus simple.

> ⚠️ Cette option efface l'intégralité du disque sélectionné. Sauvegardez vos données importantes avant de continuer.

![Partitionnement du disque](https://github.com/user-attachments/assets/a8ffb485-0f97-4539-997e-353a2e772790)

Confirmez l'écriture sur le disque en cliquant sur **"Continue"**.

![Confirmation du partitionnement](https://github.com/user-attachments/assets/7580d129-98d1-4d31-bd08-c5fdf89a916b)

Sélectionnez votre **fuseau horaire** sur la carte interactive.

![Choix du fuseau horaire](https://github.com/user-attachments/assets/aa8adf72-f979-49d7-b7d5-ed25b9dfc8b8)

Créez votre **compte utilisateur** : renseignez votre nom, le nom de la machine, votre nom d'utilisateur et un mot de passe.

![Création du compte](https://github.com/user-attachments/assets/3d657dfd-8291-4f9b-8280-ce7a63cdb46c)

L'installation démarre. Cette étape prend généralement entre 5 et 15 minutes selon les performances de la machine.

![Installation en cours](https://github.com/user-attachments/assets/bbc97950-2704-4dae-afbf-f2e072fa3f9f)

![Copie des fichiers](https://github.com/user-attachments/assets/0b5d62bb-dfa7-4a52-ba6e-6e87c7b3cd21)

![Fin de l'installation](https://github.com/user-attachments/assets/ba9cb96f-8158-438d-85dd-1228e3751aba)

Une fois l'installation terminée, un message vous invite à **redémarrer**. Retirez la clé USB si vous étiez en mode PC physique, puis appuyez sur Entrée.

![Invitation au redémarrage](https://github.com/user-attachments/assets/22120e38-3cae-494b-97a8-c2a0618156fd)

---

## Premier démarrage

Au premier lancement, Ubuntu affiche un assistant de bienvenue. Vous pouvez configurer votre compte en ligne, les paramètres de confidentialité et les applications recommandées.

![Assistant de bienvenue](https://github.com/user-attachments/assets/3ccea4b7-5fc0-45ed-9a74-78f96d410100)

![Configuration initiale](https://github.com/user-attachments/assets/b7d35c45-fa9f-41aa-a1c1-511d10cff1ec)

![Paramètres de confidentialité](https://github.com/user-attachments/assets/fb82c846-973e-4c6d-af9f-67423b8e8d9f)

![Applications recommandées](https://github.com/user-attachments/assets/609a5ae5-c528-407b-8536-cc88f8226b3f)

![Fin de la configuration](https://github.com/user-attachments/assets/7bf68df6-d3ee-455a-a496-6c7b1564d19e)

Vous arrivez sur le **bureau Ubuntu Desktop**. L'environnement est prêt à l'emploi.

![Bureau Ubuntu Desktop](https://github.com/user-attachments/assets/85488b2b-572a-4c41-8002-3077ec4bd2f0)

![Vue du bureau avec dock](https://github.com/user-attachments/assets/e40be6b0-b128-4482-9f39-a2f5f8e8e2a9)

![Menu des applications](https://github.com/user-attachments/assets/a9fc304f-3564-43c3-b27f-b49582d0a0f0)

![Gestionnaire de fichiers](https://github.com/user-attachments/assets/83728765-45d7-423a-b96d-ae737252deca)

![Terminal Ubuntu](https://github.com/user-attachments/assets/275a9a37-734d-4aba-b8f8-895847220af2)

![Bureau finalisé](https://github.com/user-attachments/assets/16b21205-615f-4136-abb4-a0395b725fb7)

Ubuntu Desktop est désormais pleinement opérationnel. Vous pouvez commencer à installer vos applications via le gestionnaire de logiciels ou directement depuis le terminal.

---

> 🔗 Ce repository est utilisé comme référence dans [yacinehrc/nextcloud](https://github.com/yacinehrc/nextcloud) pour la mise en place d'une infrastructure cloud privée sous Docker.

*Réalisé par [Yacine Harrache](https://github.com/yacinehrc) — BTS SIO SLAM | EPSI Lille*


























