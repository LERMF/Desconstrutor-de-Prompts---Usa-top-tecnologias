# ✦ PROMPT DECONSTRUCTOR: STRUCTURAL ANALYSIS & REVERSE ENGINEERING ✦
*Cognitive Decomposition, Semantic Boundary Parsing & Deterministic Prompt Compiler*

---

## Why Most Prompts Fail Under Production Stress

Prompt engineering has suffered from a culture of cargo-cult alchemy. Teams paste sprawling paragraphs of mixed intent, vague constraints, and decorative adjectives into system prompts, then wonder why the model hallucinates or ignores instructions under load.

**Prompts are typed execution contracts, not polite suggestions.**

The **Prompt Deconstructor** is a developer toolkit and interactive React/TypeScript laboratory that breaks monolithic prompts into typed, modular AST components: **Objective ($\Sigma$)**, **Constraints ($\Delta$)**, **Context ($\Gamma$)**, and **Output Contract ($\Omega$)**. By isolating attention vectors, this architecture eliminates instruction bleeding and forces absolute schema adherence.

---

## The Four-Layer Cognitive Decomposition Model

```
Raw Monolithic Prompt
         │
         ▼
┌─────────────────────────────────────────────────────────────┐
│               PROMPT DECONSTRUCTOR PIPELINE                 │
├────────────────────────────────┬────────────────────────────┤
│ 1. Objective Layer (Intent)    │ Mathematical task boundary │
├────────────────────────────────┼────────────────────────────┤
│ 2. Constraint Layer (Invariants│ Hard operational MUST NOTs │
├────────────────────────────────┼────────────────────────────┤
│ 3. Cognitive Harness (Steps)   │ Topological execution graph│
├────────────────────────────────┼────────────────────────────┤
│ 4. Typed Output Contract       │ Formal JSON/Zod Schema     │
└────────────────────────────────┴────────────────────────────┘
         │
         ▼
Optimized, Irreplicable Deterministic Prompt
```

---

## System Capabilities & Components

| Subsystem | Source Location | Technical Role |
|---|---|---|
| **Interactive Studio** | [`App.tsx`](App.tsx), [`components/`](components/) | React-based visual workbench for real-time prompt tokenization, chunking, and boundary visualization. |
| **Parsing Engine** | [`services/`](services/) | TypeScript AST compiler separating directives from conversational filler. |
| **Analytical Notebook** | [`Generative_AI.ipynb`](Generative_AI.ipynb) | Google Colab / Jupyter laboratory testing prompt sensitivity across Gemini, Claude, and Llama families. |

---

## Getting Started

### Local Workbench (React + Vite)
```bash
# Install dependencies
npm install

# Start local interactive analyzer
npm run dev

# Open in browser
# -> http://localhost:5173
```

### Analytical Notebook Execution
Launch [`Generative_AI.ipynb`](Generative_AI.ipynb) in JupyterLab or VS Code to run comparative entropy analysis against prompt variants.

---

## The SLAP Test for Prompts

Before deploying any system prompt to production, run the **Topic Swap Test**:
1. Swap the primary domain entity with an unrelated subject.
2. If the prompt remains coherent, the instructions are generic slop.
3. High-performance prompts must contain domain-specific constraints, structural schemas, and falsification rules that break immediately if the domain is replaced.
