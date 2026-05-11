# EUROPROD SMART INFRASTRUCTURE ADVISOR
## README COMPLET — Développement MVP V1
### Agent Conversationnel IoT / GTB / EMS / Edge AI

---

# 1. PRÉSENTATION DU PROJET

EUROPROD Smart Infrastructure Advisor est un moteur conversationnel de qualification technique destiné aux bâtiments intelligents.

Le système permet :
- de qualifier un prospect,
- de comprendre les besoins bâtimentaires,
- de détecter automatiquement les contraintes réglementaires,
- de recommander des technologies adaptées :
  - IoT,
  - LoRaWAN,
  - GTB / BMS,
  - EMS,
  - Edge AI,
  - Digital Twin.

Le moteur agit comme :
# un ingénieur avant-vente digital.

---

# 2. OBJECTIF DU MVP

Le MVP doit permettre :

## Entrée
L’utilisateur répond à une série de questions guidées.

---

## Traitement
Le moteur :
- détecte le segment,
- applique les règles métier,
- détecte les réglementations,
- construit une architecture recommandée.

---

## Sortie
Le système génère :
- recommandations capteurs,
- stack technologique,
- contraintes réglementaires,
- rapport imprimable.

---

# 3. INITIALISATION DU PROJET

## Création du projet

```bash
mkdir europrod-agent
cd europrod-agent
---
```

# 3. STRUCTURE PROJET

europrod-agent/
│
├── backend/
│   ├── main.py
│   │
│   ├── engine/
│   │   ├── loaders.py
│   │   ├── inference_engine.py
│   │   ├── regulations_engine.py
│   │   ├── recommendation_engine.py
│   │   └── report_builder.py
│   │
│   ├── models/
│   │   └── schemas.py
│   │
│   ├── utils/
│   │   └── helpers.py
│   │
│   ├── requirements.txt
│   └── .env
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   ├── app.js
│   │
│   └── assets/
│
├── data/
│   ├── 01_questions_master.csv
│   ├── 02_answers_master.csv
│   ├── 03_regulations_master.csv
│   ├── 05_answer_impacts_rules.csv
│   ├── 06_regulation_requirements.csv
│   ├── 07_catalogue_items_dictionary.csv
│   ├── 08_segment_baseline_matrix.csv
│   ├── 09_stack_rules.csv
│   ├── 10_report_output_schema.csv
│   └── 12_capabilities_electric_metering.csv
│
├── reports/
│
├── logs/
│
└── README.md

---

# 4. INITIALISATION DU PROJET

| Dataset                 | Fonction                  |
| ----------------------- | ------------------------- |
| questions_master        | Questions frontend        |
| answers_master          | Réponses utilisateur      |
| impacts_rules           | Règles métier             |
| regulations_master      | Décrets                   |
| regulation_requirements | Technologies obligatoires |
| catalogue_items         | Mapping catalogue         |
| segment_baseline        | Recommandations segment   |
| stack_rules             | Construction stack        |
| report_schema           | Structure rapport         |


# 5. RÔLE DES MODULES BACKEND

| Fichier                  | Fonction                  |
| ------------------------ | ------------------------- |
| loaders.py               | Chargement CSV            |
| inference_engine.py      | Détection segment         |
| regulations_engine.py    | Détection réglementations |
| recommendation_engine.py | Recommandations           |
| report_builder.py        | Génération rapport        |



