# IFRI - Licence Sécurité Informatique

Notes de cours et préparation pour la Licence Professionnelle en Sécurité Informatique à l'IFRI (Institut de Formation et de Recherche en Informatique), Université d'Abomey-Calavi, Bénin.

J'intègre la première année cette année et je documente ici ma préparation, puis mes notes au fil de la formation. Le repo est public au cas où il puisse servir aux futurs étudiants de la filière.

## La cybersécurité, c'est quoi ?

### Définition

La cybersécurité, également désignée sous les termes de sécurité informatique ou sécurité des systèmes d'information, est la discipline qui s'intéresse à la protection des actifs numériques d'une organisation ou d'un individu contre les menaces, qu'elles soient humaines (cybercriminels, acteurs étatiques, employés malveillants) ou techniques (logiciels malveillants, vulnérabilités logicielles, erreurs de configuration).

Elle s'inscrit à l'intersection de plusieurs champs : l'informatique, les mathématiques (notamment la cryptographie), les sciences sociales (analyse des comportements, ingénierie sociale) et le droit (réglementation, protection des données).

### Les enjeux

Les motivations d'une protection sérieuse sont multiples :

- **Économiques** : le coût mondial de la cybercriminalité se chiffre en milliers de milliards de dollars par an. Une seule fuite de données peut coûter des dizaines de millions à une entreprise, sans compter la perte de confiance.
- **Géopolitiques** : les États mènent des opérations d'espionnage, de sabotage et d'influence par voie numérique. La cyberguerre est devenue une dimension à part entière des conflits modernes.
- **Sociétaux** : protection de la vie privée, des processus démocratiques, des infrastructures critiques (énergie, santé, transports).
- **Individuels** : prévention du vol d'identité, des fraudes, de la surveillance abusive.

### Les trois propriétés fondamentales

La théorie de la sécurité des systèmes d'information repose sur trois propriétés, appelées la triade **DIC** (ou **CIA** en anglais) :

1. **Disponibilité** : l'information et les systèmes doivent être accessibles aux utilisateurs autorisés lorsqu'ils en ont besoin.
2. **Intégrité** : l'information ne doit pas être altérée de manière non autorisée, accidentelle ou volontaire.
3. **Confidentialité** : l'accès à l'information doit être limité aux personnes ou systèmes autorisés.

Ces propriétés sont parfois complétées par la traçabilité, l'authenticité et la non-répudiation, selon les modèles utilisés.

### Approches défensive et offensive

La cybersécurité comprend deux approches complémentaires :

- **L'approche défensive** (*blue team*) regroupe les activités de prévention (durcissement, contrôles d'accès), de détection (supervision, analyse comportementale) et de réaction (gestion d'incident, investigation numérique).
- **L'approche offensive** (*red team*) consiste à simuler des attaques pour identifier les vulnérabilités avant qu'elles ne soient exploitées par des acteurs malveillants. Elle inclut notamment le test d'intrusion (*pentest*) et la recherche de vulnérabilités.

Une bonne compréhension des deux approches est aujourd'hui considérée comme nécessaire à toute personne souhaitant exercer dans ce domaine.

### Apprentissage continu

La cybersécurité est un domaine en évolution permanente. Les technologies se transforment, les vecteurs d'attaque se renouvellent, des vulnérabilités sont découvertes en continu. Un professionnel de la sécurité consacre une partie significative de son temps à la veille technologique, à la formation continue, et à la pratique sur des plateformes dédiées (Capture The Flag, laboratoires virtuels, programmes de *bug bounty*).

## Les grands domaines

La cybersécurité regroupe une diversité de spécialités, chacune avec ses outils, ses méthodes et ses problématiques propres. Les principales sont présentées ci-dessous.

### Cryptographie

La cryptographie est la science qui étudie les techniques permettant de protéger l'information par des transformations mathématiques. Elle couvre le chiffrement (rendre une information illisible aux personnes non autorisées), la signature numérique (prouver l'identité de l'auteur), les fonctions de hachage (vérifier l'intégrité d'un message) et l'échange de clés. C'est l'un des fondements théoriques les plus mathématiques du domaine.

### Sécurité réseau

La sécurité réseau s'intéresse à la protection des communications entre systèmes : pare-feux, systèmes de détection et de prévention d'intrusion (IDS/IPS), réseaux privés virtuels (VPN), segmentation, surveillance du trafic. Elle s'appuie sur une compréhension fine des protocoles (TCP/IP, DNS, HTTP, etc.) et des architectures réseau.

### Sécurité applicative et web

Ce domaine concerne la sécurité des logiciels eux-mêmes — applications web, mobiles ou de bureau. Il couvre les vulnérabilités classiques (injection SQL, XSS, CSRF, désérialisation non sécurisée), les pratiques de développement sécurisé et l'audit de code. Le projet OWASP (Open Web Application Security Project) est la référence du domaine.

### Sécurité système et infrastructure

Protection des systèmes d'exploitation, des serveurs, des conteneurs et de l'infrastructure sous-jacente : durcissement (*hardening*), gestion des correctifs, contrôle d'accès, supervision des journaux. Inclut les questions de sécurité spécifiques au cloud (AWS, Azure, GCP).

### Test d'intrusion (pentest) et red team

Discipline offensive qui consiste à simuler des attaques réelles pour identifier les vulnérabilités d'un système avant qu'elles ne soient exploitées. Le pentester utilise les mêmes outils et techniques qu'un attaquant, mais dans un cadre légal et contractuel. La red team va plus loin en simulant des opérations adverses complètes, souvent sur la durée.

### Centre opérationnel de sécurité (SOC) et blue team

Côté défensif, les équipes de SOC (Security Operations Center) surveillent les systèmes en temps réel, détectent les incidents, analysent les alertes et coordonnent la réponse. Elles s'appuient sur des outils comme les SIEM (Security Information and Event Management) et les EDR (Endpoint Detection and Response), et nécessitent une connaissance approfondie des indicateurs de compromission.

### Réponse à incident et investigation numérique (forensics)

Lorsqu'un incident se produit, il faut comprendre ce qui s'est passé, contenir les dégâts, et préserver des preuves exploitables (notamment en cas de poursuites judiciaires). L'investigation numérique consiste à analyser les disques, la mémoire, le trafic réseau et les journaux pour reconstituer la chronologie d'une attaque.

### Analyse de logiciels malveillants et rétro-ingénierie

Étude des logiciels malveillants pour comprendre leur fonctionnement, identifier leurs auteurs potentiels et développer des contre-mesures. Implique l'analyse statique (étude du code sans exécution), l'analyse dynamique (observation du comportement à l'exécution) et la rétro-ingénierie (*reverse engineering*) pour décompiler des programmes sans accès au code source.

### Gestion des identités et des accès (IAM)

Garantir que les bonnes personnes ont accès aux bonnes ressources, et seulement à celles-là. Couvre l'authentification (mots de passe, biométrie, authentification multifacteur), l'autorisation, la fédération d'identité (SSO, SAML, OAuth) et la gestion des accès privilégiés.

### Sécurité de l'IoT et des systèmes embarqués

Les objets connectés (caméras, capteurs, équipements médicaux, véhicules, infrastructures industrielles) posent des problèmes de sécurité spécifiques : ressources limitées, mises à jour difficiles, exposition physique. C'est un domaine en forte expansion avec la multiplication des objets connectés.

### Gouvernance, risque et conformité (GRC)

Aspect organisationnel et juridique : politiques de sécurité, évaluation des risques, audits, conformité aux normes (ISO 27001, NIST CSF, PCI-DSS) et aux réglementations (RGPD, NIS2). Domaine moins technique mais essentiel pour structurer la sécurité d'une organisation.

### Ingénierie sociale et facteur humain

Beaucoup d'attaques ne sont pas techniques mais visent les utilisateurs : hameçonnage (*phishing*), hameçonnage vocal (*vishing*), prétextage, manipulation psychologique. La sensibilisation, la formation et l'organisation des procédures internes sont aussi importantes que les outils techniques.

## Quelques métiers concrets

La cybersécurité offre une grande variété de débouchés, qui peuvent être classés selon quatre grandes orientations : défensive, offensive, ingénierie et gouvernance. Voici quelques rôles représentatifs.

### Métiers orientés défense

#### Analyste SOC (Security Operations Center)

L'analyste SOC surveille en temps réel l'activité des systèmes d'information d'une organisation à partir d'outils de supervision (SIEM, EDR). Son travail consiste à trier les alertes, qualifier les incidents et déclencher la réponse appropriée. Le métier est généralement structuré en niveaux (N1, N2, N3) correspondant à des degrés croissants de complexité et d'autonomie.

#### Analyste en réponse à incident (*incident responder*)

Lorsqu'un incident de sécurité avéré se produit, l'analyste en réponse à incident intervient pour contenir la menace, éradiquer l'attaquant, restaurer les systèmes et documenter les événements. Il travaille souvent en équipe avec des analystes forensiques pour reconstituer la chronologie de l'attaque.

#### Analyste forensique / investigateur numérique

L'analyste forensique conduit l'investigation technique après un incident : analyse de disques, de mémoire, de journaux, de trafic réseau, pour comprendre l'attaque et préserver des preuves exploitables judiciairement. Ce métier requiert une grande rigueur méthodologique et une bonne connaissance des cadres légaux.

#### Analyste en *threat intelligence* (CTI)

Le rôle consiste à suivre les groupes d'attaquants, leurs tactiques, techniques et procédures (TTP), les vulnérabilités exploitées activement, et à transformer ces informations en renseignement actionnable pour la défense. C'est un métier qui mêle technique, géopolitique et analyse.

### Métiers orientés offensive

#### Pentester (testeur d'intrusion)

Le pentester simule des attaques contre les systèmes d'un client, dans un cadre légal et contractuel, afin d'identifier des vulnérabilités avant qu'elles ne soient exploitées. Selon les missions, le périmètre peut couvrir des applications web, des infrastructures internes, des réseaux sans fil, des objets connectés ou des opérations d'hameçonnage.

#### Chercheur en vulnérabilités / *bug bounty hunter*

Le chercheur en vulnérabilités cherche des failles dans des logiciels ou services, soit dans un cadre académique ou industriel (R&D), soit via des programmes de *bug bounty* qui récompensent la découverte responsable de vulnérabilités. Une partie d'entre eux exercent en indépendant.

#### Membre de *red team*

La red team simule des opérations adverses complètes et persistantes, sur des durées longues (semaines, mois), pour tester la capacité d'une organisation à détecter et à réagir face à une menace sophistiquée. Plus poussé qu'un pentest classique, le rôle requiert des compétences avancées en techniques d'attaque, en discrétion et en simulation d'acteurs réels.

### Métiers orientés ingénierie et conception

#### Ingénieur sécurité

L'ingénieur sécurité conçoit, déploie et maintient les solutions techniques de protection : pare-feux, systèmes d'authentification, chiffrement, segmentation réseau, sécurisation cloud. Le poste peut être spécialisé (réseau, cloud, applicative, etc.) ou généraliste.

#### Architecte sécurité

L'architecte sécurité intervient en amont pour concevoir des systèmes sécurisés *by design*. Il définit les principes, les politiques techniques et les modèles d'architecture, en intégrant les contraintes métier, réglementaires et techniques.

#### Ingénieur DevSecOps

À l'intersection du développement et de la sécurité, ce rôle intègre les pratiques de sécurité dans les pipelines de développement et de déploiement : analyse statique et dynamique de code, gestion des dépendances, sécurisation des conteneurs, automatisation des contrôles de sécurité.

#### Cryptologue

Métier rare et exigeant, le cryptologue conçoit ou analyse des algorithmes cryptographiques. Le poste se trouve majoritairement dans la recherche académique, les agences gouvernementales et quelques grandes entreprises technologiques.

### Métiers orientés gouvernance

#### Responsable de la sécurité des systèmes d'information (RSSI / CISO)

Le RSSI définit la stratégie de sécurité d'une organisation et en pilote la mise en œuvre. Il rapporte généralement à la direction générale, gère les budgets et les équipes, et coordonne l'ensemble des activités de sécurité, techniques comme organisationnelles.

#### Consultant en cybersécurité

Le consultant intervient chez des clients sur des missions variées : audits, accompagnement à la mise en conformité, gestion de crise, conception de stratégies. Le rôle nécessite une excellente compréhension du domaine, une forte capacité de communication et une adaptabilité aux contextes clients.

#### Spécialiste GRC (gouvernance, risque, conformité)

Ce métier consiste à structurer la gouvernance de la sécurité, évaluer les risques, assurer la conformité aux normes et réglementations (ISO 27001, RGPD, NIS2) et conduire des audits internes. Il combine compétences techniques, juridiques et organisationnelles.

## La filière à l'IFRI

L'Institut de Formation et de Recherche en Informatique (IFRI) propose, au sein de l'Université d'Abomey-Calavi (UAC) au Bénin, une **Licence Professionnelle en Sécurité Informatique**. La formation se déroule sur trois années (L1, L2, L3) réparties en six semestres, pour un total de 180 crédits.

### Une formation professionnalisante

Contrairement à une licence générale orientée vers la poursuite d'études, une licence professionnelle vise une insertion directe sur le marché du travail à la sortie. Elle reste cependant compatible avec une poursuite en master ou en école spécialisée, sous réserve d'admission.

### Le contenu général

Le cursus articule trois grands blocs :

- **Les fondations scientifiques** — mathématiques (logique, arithmétique, algèbre linéaire, analyse, probabilités, statistiques), algorithmique, bases théoriques de l'informatique
- **Les compétences techniques en informatique** — programmation (C, Python), systèmes d'exploitation, réseaux, bases de données, technologies web
- **Les compétences spécifiques à la sécurité** — qui se renforcent progressivement au fil des années, couvrant la cryptographie appliquée, la sécurité des réseaux, des systèmes et des applications, la gestion des incidents et la gouvernance

À cela s'ajoutent des unités transversales : déontologie et droit liés aux TIC, anglais technique, expression écrite et orale, ainsi qu'un projet intégrateur dès la fin de la L1.

### À l'issue de la formation

Un diplômé de la filière peut prétendre à des postes d'analyste sécurité junior, technicien SOC, technicien réseau et sécurité, ou poursuivre en master pour se spécialiser (cryptographie, pentest, audit, gouvernance, etc.). Le bagage acquis correspond principalement aux métiers orientés défense et ingénierie présentés plus haut, avec la possibilité de basculer vers l'offensive ou la gouvernance après quelques années d'expérience ou une spécialisation complémentaire.

### Le détail par année

Le contenu précis de chaque année et de chaque semestre est documenté dans les dossiers correspondants :

- [Première année (L1)](./L1/) — fondations mathématiques et informatiques
- Deuxième année (L2) — à venir
- Troisième année (L3) — à venir

## Communauté, pratique et compétitions

La cybersécurité est l'un des domaines de l'informatique où la communauté joue un rôle particulièrement important. L'apprentissage en classe ne suffit pas : la pratique régulière sur des cas concrets, l'échange avec d'autres passionnés et la participation à des compétitions constituent des leviers essentiels de progression.

### Les CTF (Capture The Flag)

Les CTF sont des compétitions de cybersécurité dans lesquelles les participants doivent résoudre des défis techniques pour récupérer des « drapeaux » (*flags*) — des chaînes secrètes qui prouvent qu'un objectif a été atteint. Il existe deux grands formats :

- **Jeopardy** : les participants choisissent des épreuves indépendantes classées par catégorie et difficulté. Le format le plus courant.
- **Attaque-défense** : chaque équipe défend ses propres services tout en attaquant ceux des adversaires. Plus exigeant, généralement réservé aux compétitions de haut niveau.

Les catégories classiques en CTF couvrent l'essentiel des domaines techniques de la cybersécurité :

- **Web** — exploitation de vulnérabilités d'applications web (injection, XSS, etc.)
- **Pwn / exploitation binaire** — exploitation de programmes natifs (dépassements de tampon, attaques mémoire, etc.)
- **Cryptographie** — cassage de schémas cryptographiques mal conçus ou mal implémentés
- **Rétro-ingénierie** — analyse de binaires pour comprendre leur fonctionnement
- **Forensique** — analyse de fichiers, captures réseau, images disque
- **Stéganographie** — détection et extraction d'informations cachées dans des fichiers
- **OSINT** — recherche d'information à partir de sources publiques
- **Programmation** — résolution algorithmique de problèmes en temps limité

### Plateformes d'entraînement

Plusieurs plateformes en ligne permettent de s'entraîner toute l'année, à son rythme, sur des défis allant du niveau débutant au niveau expert :

- **TryHackMe** — orienté apprentissage progressif, parfait pour débuter
- **Hack The Box** — défis plus complexes, machines à compromettre en autonomie
- **PicoCTF** — CTF permanent éducatif, géré par l'université Carnegie Mellon
- **Root-Me** — plateforme francophone très complète
- **OverTheWire** — *wargames* axés sur les fondamentaux Linux et binaire
- **PortSwigger Web Security Academy** — référence pour la sécurité web
- **CryptoHack** — défis de cryptographie
- **HackerOne CTF / Bugcrowd University** — proches du contexte *bug bounty*

### Le HackerLab au Bénin

Le **HackerLab** est la compétition nationale de cybersécurité du Bénin. Initiée par Ouanilo Medegan Fagla, elle est organisée par l'**Agence des Systèmes d'Information et du Numérique (ASIN)**, anciennement ANSSI. La première édition a eu lieu en 2017.

Le format est celui du Capture the Flag, dans un environnement simulé où les participants résolvent des défis de cybersécurité. Une phase de qualification en ligne est suivie d'une finale intensive de 48 heures à Cotonou. Les épreuves couvrent toutes les grandes catégories techniques : forensique numérique, stéganographie, rétro-ingénierie, exploitation binaire et applicative, programmation, auxquelles s'ajoutent l'OSINT et la cryptographie selon les éditions.

Au-delà de la compétition elle-même, le HackerLab joue un rôle de détection de talents : les meilleurs participants sont régulièrement recrutés par le **bjCSIRT** (l'équipe gouvernementale de réponse aux incidents de sécurité informatique), par le Laboratoire d'Investigations Numérique, ou par des acteurs du secteur privé. Depuis 2025, la compétition s'organise conjointement avec le **Cyber Africa Forum (CAF)** et accueille des finalistes venus de toute l'Afrique.

Pour un étudiant à l'IFRI, c'est l'un des rendez-vous les plus stratégiques de l'année : participer, c'est se faire repérer.

### Autres compétitions en Afrique

D'autres événements de cybersécurité existent à l'échelle régionale et continentale :

- **Cyber Africa Forum (CAF)** — événement panafricain en marge duquel se déroule désormais le HackerLab
- **CTF nationaux** organisés dans plusieurs pays voisins (Togo, Côte d'Ivoire, etc.)
- **Compétitions régionales CEDEAO** dans le cadre des programmes de coopération (OCWAR-C, etc.)

### Compétitions internationales notables

Pour avoir une vue plus large, quelques compétitions internationales de référence :

- **DEFCON CTF** — la finale du plus prestigieux CTF mondial, à Las Vegas chaque été
- **Google CTF** — CTF annuel organisé par Google
- **PlaidCTF** — organisé par les Plaid Parliament of Pwning (Carnegie Mellon)
- **CSAW CTF** — organisé par l'université de New York
- **Hack The Box University CTF** — réservé aux étudiants

Le site **CTFtime.org** recense l'essentiel des CTF internationaux et publie un classement mondial des équipes.

### Bug bounty

En parallèle des CTF, les programmes de ***bug bounty*** permettent à des chercheurs en sécurité de signaler des vulnérabilités à des entreprises en échange de récompenses financières. Les plateformes principales sont **HackerOne**, **Bugcrowd**, **Intigriti** et **YesWeHack** (côté francophone). Pour un débutant, c'est une pratique exigeante : il vaut mieux d'abord se faire les dents sur des CTF et des labs avant de se lancer dans des programmes réels.

## Structure du repo

- [`L1/`](L1) - Première année (en cours)
- `L2/` - Deuxième année (à venir)
- `L3/` - Troisième année (à venir)

Chaque année est divisée en deux semestres (`S1/`, `S2/`), et chaque semestre contient un dossier par UE.

## Format des notes

Chaque matière (UE simple ou EC d'une UE composée) suit la même structure :

- `cours/` - notes de cours par chapitre
- `exercices/` - énoncés (TD, TPE, anciens sujets)
- `solutions/` - corrections personnelles
- `fiches/` - résumés synthétiques pour la révision
- `ressources.md` - livres, vidéos, exos en ligne

Les matières de programmation ont en plus un dossier `code/` avec les fichiers source.

---

*Notes d'étudiant en cours d'apprentissage. Peuvent contenir des erreurs — issues et corrections bienvenues.*
