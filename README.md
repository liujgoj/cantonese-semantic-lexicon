# cantonese-semantic-lexicon
A machine-readable Cantonese lexicon based on cognitive semantics, encoding lexemes and sense networks in JSON for linguistic research, ASR, and AI training.

# 📘 Overview

This repository is an open Cantonese semantic lexicon that represents lexemes (not just words or characters) and their sense networks in a machine-readable JSON format.

Instead of organizing entries by traditional parts of speech, this project models Cantonese vocabulary around:

cognitive core meanings

image schemas and event structures

semantic extensions (metonymy, metaphor, abstraction, grammaticalization)

lexeme-level disambiguation (homophones, constructionalized forms, loan blends)

The goal is to build a resource that is linguistically grounded, computationally usable, and scalable for AI systems.

#  🎯 Goals

Build a lexeme-based semantic lexicon for Cantonese

Model sense networks instead of flat word lists

Support:

semantic disambiguation

ASR and NLP pipelines

grammar and construction modeling

cognitively informed AI training

Provide data in a clean, explicit JSON structure

Encourage open and community-oriented development

# 🧠 Core Principles

Lexemes, not characters
Homophones with unrelated meanings are split into separate lexemes.

Cognitive semantics first
Each lexeme is anchored by a core schema (event, control, motion, information, evaluation, etc.).

Sense networks, not sense lists
Senses are linked through extension mechanisms:

prototype

metonymy

metaphor

abstraction

grammaticalization

Machine-readable by design
All entries are encoded in structured JSON to support:

feature extraction

clustering

embedding alignment

grammar induction

# 📂 Repository Structure


```
cantonese-semantic-lexicon/
│
├── lexemes/
│   ├── zapj.json
│   ├── svj.json
│   ├── lukj.json
│   └── ...
│
├── schema/
│   └── msfs.json        # Minimal Semantic Feature Set
│
├── docs/
│   ├── methodology.md
│   ├── annotation-guide.md
│   └── roadmap.md
│
├── examples/
│   └── annotated-sentences.json
│
└── README.md
```



# 🧩 Data Model

Each lexeme entry is encoded using a Minimal Semantic Feature Set (MSFS), including:

lexeme-level features

cognitive domain

core schema

prototype type

sense-level features

ontological type (object, event, process, state, relation)

semantic dimensions (force, motion, control, information, evaluation, etc.)

participant structure

directionality and result states

extension mechanisms

constructional behavior

Example (simplified):

{
  "lexeme_id": "zapj1",
  "homophone_group": "zapj",
  "core_schema": "manual control and acquisition of an entity",
  "senses": [
    {
      "sense_id": "zapj1-1",
      "gloss": "pick up",
      "ontological_type": "event",
      "semantic_dimensions": ["force","control","motion"],
      "extension_type": "prototype"
    }
  ]
}


# 🔬 Intended Use

This lexicon is designed for:

Cantonese linguistic research

cognitive-semantic modeling

ASR and speech technology

NLP and LLM pretraining / fine-tuning

grammar induction and construction analysis

semantic annotation projects

# 🤝 Contributions

Contributions are welcome, especially in:

adding new lexeme entries

expanding sense networks

refining semantic features

improving documentation

providing annotated examples

If you contribute:

please keep entries lexeme-based

clearly state core schemas

indicate semantic extension paths

include authentic Cantonese examples where possible

A detailed annotation guide will be provided in docs/annotation-guide.md.

# 🗺 Roadmap (initial)

 Formalize MSFS schema

 Publish annotation guidelines

 Seed lexicon with high-frequency Cantonese lexemes

 Build cross-lexeme semantic indices

 Provide example applications (disambiguation, grammar modeling)

 Explore links to corpora and ASR datasets

 # 📜 License

To be determined.
(Open data licenses such as CC BY 4.0 or CC BY-SA 4.0 are recommended.)

# ✨ Philosophy

This project treats Cantonese not as a list of words, but as a structured semantic system.

The aim is not only to record meanings,
but to model how meanings are organized, extended, and cognitively grounded.

# 


