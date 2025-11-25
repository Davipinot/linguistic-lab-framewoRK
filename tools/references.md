# 📚 Referências Bibliográficas & Benchmarks

> **A base epistemológica do Linguistic Laboratory Framework.**
> Esta curadoria reúne os papers canônicos, repositórios de código e teorias físicas que fundamentam o **Rigor 1.0** e a **Semantic Latent Engineering (SLE)**.

---

### 🏆 Tier 1: O Cânone (Leitura Obrigatória)

Estes trabalhos definem os axiomas operacionais do laboratório. Se está aqui, é porque o método foi validado empiricamente e adotado pela indústria.

| Paper / Tecnologia | Citação / ArXiv | Relevância para o Lab (SLE) | Status |
| :--- | :--- | :--- | :---: |
| **RepE (Representation Engineering)** | [Zou et al. (2023)](https://arxiv.org/abs/2310.01405) | Base do operador `>>` (Steering). Prova que podemos controlar IAs via vetores, não apenas prompts. | 💎 Core |
| **Reflexion** | [Shinn et al. (NeurIPS 2023)](https://arxiv.org/abs/2303.11366) | Base do ciclo de auto-correção e agentes autônomos verbais. | 💎 Core |
| **RAGAS** | [Es et al. (EACL 2024)](https://arxiv.org/abs/2309.15217) | Framework padrão para métricas de validação semântica (Faithfulness, Relevance). | 💎 Metric |
| **TransformerLens** | [Nanda & Meyer](https://github.com/TransformerLensOrg/TransformerLens) | A "lente" principal para mechanistic interpretability. | 🛠️ Tool |
| **DARE** | [Yu et al. (2023)](https://arxiv.org/abs/2311.03099) | Algoritmo de reconstrução e *merging* de modelos sem retreino. | ⚡ SOTA |
| **CoVe (Chain of Verification)** | [Dhuliawala et al. (2023)](https://arxiv.org/abs/2309.11495) | Mitigação de alucinação via verificação passo-a-passo. | 🛡️ Safety |

---

### 🌌 1. Física do Espaço Latente (Geometria & Manifolds)

A teoria por trás da "Álgebra da Intenção". Como a informação se organiza geometricamente dentro da rede.

* **Linear Representations:** [The Linear Representation Hypothesis](https://arxiv.org/abs/2311.03658) — *Por que vetores funcionam como conceitos.*
* **Monosemanticity:** [Scaling Monosemanticity (Anthropic)](https://transformer-circuits.pub/2024/scaling-monosemanticity/) — *Como extrair conceitos puros (features) de redes neurais.*
* **Latent Space Physics:** [Papers sobre Dinâmica de Manifolds](https://arxiv.org/html/2406.12159v1) — *Estudos sobre a topologia do pensamento da IA.*
* **Emergent World Models:** [Othello-GPT & World Models](https://arxiv.org/abs/2210.13382) — *Prova de que IAs constroem modelos de mundo internos.*

---

### ⚙️ 2. Mecânica da Inferência (Circuitos & Residual Stream)

Como o motor funciona "debaixo do capô". Estudos de *Mechanistic Interpretability*.

* **Induction Heads:** [In-context Learning and Induction Heads](https://transformer-circuits.pub/2022/in-context-learning-and-induction-heads/index.html) — *A mecânica biológica do "few-shot learning".*
* **Residual Stream:** [Mathematical Framework for Transformer Circuits](https://transformer-circuits.pub/2021/framework/index.html) — *O fluxo de informação através das camadas.*
* **AutoInterp:** [Automated Interpretability (EleutherAI)](https://blog.eleuther.ai/autointerp/) — *Usando IA para explicar IA.*
* **ACDC:** [Automated Circuit DisCovery](https://arxiv.org/abs/2304.14997) — *Mapeamento automático de circuitos computacionais.*

---

### 🧪 3. Técnicas SOTA (Steering & Controle)

Métodos avançados para guiar o comportamento (Behavior) sem retreino.

* **Activation Steering:** [Activation Addition/Steering](https://arxiv.org/abs/2308.10248) — *Injeção direta de vetores de comportamento.*
* **ITI (Inference-Time Intervention):** [Li et al. (2023)](https://arxiv.org/abs/2306.03341) — *Cirurgia em tempo real para aumentar a veracidade.*
* **TIES-Merging:** [Resolving Interference when Merging Models](https://arxiv.org/abs/2306.01708) — *Como combinar múltiplos modelos especialistas.*
* **ToT (Tree of Thoughts):** [Yao et al. (2023)](https://arxiv.org/abs/2305.10601) — *Navegação não-linear de raciocínio.*

---

### 📊 4. Validação Científica & Métricas

Ferramentas e papers que fundamentam o nosso **Scientific Validation Hub**.

* **Probing Classifiers:** [Linear Probes for Concept Extraction](https://arxiv.org/abs/2102.12452) — *A base matemática do nosso SD Validator.*
* **Faithfulness Metrics:** [RAGAS Documentation & Metrics](https://docs.ragas.io/en/stable/concepts/metrics/available_metrics/faithfulness/) — *Como medir se a IA manteve o contexto.*
* **Semantic Entropy:** [Kuhn et al. (2023)](https://arxiv.org/abs/2302.09664) — *Detectando alucinação através da incerteza semântica.*

---

### 🛠️ 5. Repositórios de Implementação (Open Source)

Onde o código vive. Links diretos para implementações de referência.

* **[TransformerLens](https://github.com/TransformerLensOrg/TransformerLens):** A biblioteca definitiva para análise mecanicista.
* **[Pythia](https://github.com/EleutherAI/pythia):** Suite de modelos para pesquisa de interpretabilidade.
* **[Mechanistic Interpretability (Awesome List)](https://github.com/gauravfs-14/awesome-mechanistic-interpretability):** Curadoria da comunidade.
* **[PEFT (HuggingFace)](https://huggingface.co/docs/peft/package_reference/lora):** Parameter-Efficient Fine-Tuning (LoRA, etc.).

---

### 🔍 Notas de Curadoria

> **Critério de Inclusão:**
> Para constar nesta lista, o trabalho deve ter:
> 1.  Código aberto disponível ou algoritmo replicável.
> 2.  Validação empírica (Benchmarks) ou teórica robusta.
> 3.  Relevância direta para a engenharia de prompts ou agentes.

**Última Atualização:** 2025-11-24
**Rigor Level:** 1.0 (Canonical Sources Only)
