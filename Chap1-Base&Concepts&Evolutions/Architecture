# Partie 1 – Architecture vs Organisation

> *« Comprendre la différence entre architecture et organisation est indispensable pour tout ingénieur ou développeur travaillant avec des systèmes informatiques. »*

Cette première partie pose la distinction fondamentale qui traverse tout le domaine informatique. Ces deux concepts, bien que complémentaires, sont profondément distincts et leur compréhension est essentielle avant d'aborder tout système informatique.

---

## 🎯 Objectifs de cette partie

- Comprendre la différence entre **architecture** (ISA) et **organisation**
- Savoir identifier ce qui relève de l'architecture (visible par le programmeur) et de l'organisation (transparent)
- Illustrer cette distinction avec l'exemple concret de l'instruction `MULTIPLY`
- Découvrir l'exemple historique de l'**IBM System/370**

---

## 📐 Définitions fondamentales

| Concept | Définition | Visibilité |
|---------|------------|-------------|
| **Architecture (ISA)** | Attributs d'un système visibles par le programmeur ayant un impact direct sur l'exécution logique d'un programme. | **Visible** par le programmeur |
| **Organisation** | Unités opérationnelles et leurs interconnexions qui réalisent concrètement les spécifications architecturales. | **Transparente** pour le programmeur |

### L'ISA (Instruction Set Architecture) définit précisément :

- Les **formats d'instructions**
- Les **codes opération** (opcodes)
- Les **registres**
- La mémoire d'**instructions** et de **données**
- L'**effet** des instructions exécutées sur les registres et la mémoire
- L'**algorithme de contrôle** d'exécution des instructions

### L'organisation inclut tous les détails matériels transparents :

- Les **signaux de contrôle internes**
- Les **interfaces** entre l'ordinateur et ses périphériques
- La **technologie mémoire** utilisée

---

## 🔍 Illustration pratique : l'instruction MULTIPLY

L'exemple le plus parlant pour illustrer cette distinction est celui de l'instruction de multiplication :


┌─────────────────────────────────────────────────────────────────┐
│ DÉCISION ARCHITECTURALE │
│ Est-ce que l'ordinateur aura une instruction │
│ MULTIPLY ? │
│ → Visible par le programmeur │
│ → Fait partie de l'ISA │
└─────────────────────────────────────────────────────────────────┘
│
▼
┌─────────────────────────────────────────────────────────────────┐
│ DÉCISION ORGANISATIONNELLE │
│ Comment implémenter MULTIPLY ? │
│ │
│ Option A Option B │
│ Unité matérielle dédiée Additions répétées │
│ (rapide mais cher) (moins cher, plus lent) │
│ │
│ → Invisible pour le programmeur │
└─────────────────────────────────────────────────────────────────┘



> 💡 **Le programmeur écrit simplement** : `MULT R1, R2` — il ne sait pas (et n'a pas besoin de savoir) comment l'opération est réalisée matériellement.

---

## 📊 Tableau comparatif Architecture vs Organisation

| Critère | Architecture (ISA) | Organisation |
|---------|====================|==============|
| **Visibilité** | Visible par le programmeur | Transparente pour le programmeur |
| **Contenu** | Jeu d'instructions, registres, formats de données, E/S | Signaux de contrôle, technologies mémoire, interconnexions |
| **Stabilité** | Doit rester compatible sur de nombreuses années | Change avec les nouvelles technologies |
| **Exemple** | L'instruction `MULTIPLY` existe dans l'ISA | Implémentée par une ALU dédiée ou additions répétées |
| **Impact** | Détermine ce qu'on peut programmer | Détermine les performances et le coût |
| **Niveau** | Abstrait / logique | Concret / matériel |

---

## 🏢 Cas d'étude : IBM System/370 (1970)

L'IBM System/370 est l'exemple historique parfait illustrant ces concepts. Introduite en **1970**, cette architecture a traversé des décennies tout en maintenant la **compatibilité ascendante** :




### Le point clé à retenir

> **L'investissement logiciel est protégé grâce à la stabilité de l'architecture.**

Un client peut :
- Acheter un modèle moins cher au départ
- Puis monter en gamme sans réécrire ses programmes

> ⚠️ L'architecture peut être améliorée (ajout d'instructions) mais **jamais réduite** — c'est la **compatibilité ascendante**.

---

## 💻 Cas particulier : les microprocesseurs

Dans la classe des **microordinateurs**, la relation entre architecture et organisation est **beaucoup plus étroite** qu'avec les mainframes :

- Les changements technologiques influencent **à la fois** l'organisation **et** l'architecture
- Moins d'exigence de compatibilité entre générations pour ces machines plus petites

### Exemple : l'émergence du RISC

Le **RISC** (Reduced Instruction Set Computer) est un exemple fascinant de cette interaction :
- La **simplification de l'architecture** (jeu d'instructions réduit)
- A permis d'**optimiser l'organisation matérielle** pour des performances maximales

---

## 📝 Résumé des concepts clés

```markdown
┌─────────────────────────────────────────────────────────────────┐
│                      ARCHITECTURE (ISA)                         │
│  "QUOI" l'ordinateur peut-il faire ?                            │
│  → Contrat stable entre le matériel et le logiciel              │
│  → Ce que le programmeur voit et utilise                        │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                      ORGANISATION                               │
│  "COMMENT" l'architecture est-elle implémentée ?                │
│  → Détails matériels évolutifs                                  │
│  → Transparente pour le programmeur                             │
└─────────────────────────────────────────────────────────────────┘
