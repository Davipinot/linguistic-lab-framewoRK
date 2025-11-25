
# 🧰 Catálogo de Ferramentas — Linguistic Laboratory Framework

> **Ecossistema federado, gratuito e reprodutível para análise, síntese e validação linguística.**
> Este diretório contém a documentação operacional de todas as ferramentas utilizadas na metodologia LLF.

---

### 🧭 1. Propósito da Pasta `/tools/`

A pasta `tools/` serve como a base metodológica da orquestração. Não contém código-fonte (que fica em `/notebooks`), mas sim os manuais de operação.

**Aqui você encontra:**
* **Inovações Nativas:** As ferramentas exclusivas de validação semântica (SLE).
* **Orquestração:** Como combinar múltiplas IAs (Federated AI).
* **Execução:** Onde rodar experimentos sem custo.
* **Datasets:** Fontes de dados canônicas.

---

### 🧩 2. Visão Geral do Ecossistema

```mermaid
flowchart LR
  A[Curador] --> B{Orquestração}
  B --> C[Análise & Leitura]
  B --> D[Síntese & Crítica]
  B --> E[Validação Científica]
  C --> F[NotebookLM / PDF]
  D --> H[ChatGPT / Claude]
  E --> I[Scientific Validation Hub]
  I --> J[Resultados Aprovados]
````

-----

### 🔬 3. Inovações Nativas (Scientific Validation Hub)

Estas são as ferramentas de **Rigor 1.0** integradas ao laboratório. Elas rodam diretamente no navegador via Google Colab e fornecem a auditoria matemática dos experimentos.

| Ferramenta | Função | Status | Acesso Rápido |
| :--- | :--- | :---: | :---: |
| **🔍 Semantic Density (SD)** | Valida a precisão vetorial de prompts. |  | [](https://www.google.com/search?q=https://github.com/aleeepassarelli/scientific-validation-hub/blob/main/notebooks/sd_validator.ipynb) |
| **🧠 Behavior Contract (CCC)** | Audita a aderência do agente à missão. |  | [](https://www.google.com/search?q=https://github.com/aleeepassarelli/scientific-validation-hub/blob/main/notebooks/behavior_validator.ipynb) |
| **🧪 Lab Notebooks** | Suite de tracking (MLflow, DVC, Zenodo). |  | [Acessar Labs](https://www.google.com/search?q=https://github.com/aleeepassarelli/scientific-validation-hub) |

-----

### 🌐 4. Mapa Geral das Ferramentas de Mercado

Organização funcional das IAs gratuitas utilizadas no fluxo federado.

#### 4.1 Orquestração Multi-LLM

| Ferramenta | Função Primária | Ponto Forte | Link |
| :--- | :--- | :--- | :--- |
| **ChatGPT (Free)** | Crítica e Síntese | Raciocínio estruturado e dialética. | [OpenAI](https://chat.openai.com) |
| **Gemini (Free)** | Exploração | Visão panorâmica e multimodalidade. | [Google](https://gemini.google.com) |
| **Claude (Free)** | Estrutura | Organização de textos longos e nuances. | [Anthropic](https://claude.ai) |
| **NotebookLM** | Leitura Científica | "Grounding" em fontes PDF/Docs. | [NotebookLM](https://notebooklm.google) |
| **DeepSeek** | Lógica Pura | Matemática e validação de código. | [DeepSeek](https://chat.deepseek.com) |
| **Grok** | Sandbox | Testes rápidos de execução. | [xAI](https://x.ai) |

#### 4.2 Ferramentas de Execução e Prototipagem

| Ferramenta | Tipo | Uso no Laboratório |
| :--- | :--- | :--- |
| **Google Colab** | Runtime | Ambiente Python gratuito para rodar os validadores SD/CCC. |
| **Grok Sandbox** | Runtime | Testes de snippets isolados. |
| **DeepSeek Coder** | Validador | Verificação estática de lógica. |

#### 4.3 Fontes de Dados & Datasets

  * **Papers With Code:** Benchmarks e SOTA (State of the Art).
  * **ArXiv:** Fontes científicas primárias.
  * **HuggingFace Datasets:** Dados públicos para treino e validação.
  * **Google Dataset Search:** Buscador multi-domínio.

-----

### 🎛️ 5. Mapa Visual de Capacidades

```mermaid
graph TD
  A[NotebookLM] -->|Extrai Contexto| B(Base de Conhecimento)
  B --> C{Orquestrador Humano}
  C -->|Exploração| D[Gemini]
  C -->|Crítica| E[ChatGPT]
  C -->|Estrutura| F[Claude]
  F -->|Draft Final| G[Validação]
  G -->|Matemática| H[DeepSeek]
  G -->|Semântica| I[Hub SD/CCC]
  I -->|Aprovado| J[Publicação]
```

-----

### 📚 6. Estrutura da Pasta

```text
tools/
├── README.md               # Este documento (Catálogo)
├── llm_orchestration.md    # Guia: Como fazer as IAs conversarem
├── analysis_tools.md       # Guia: Como usar NotebookLM para ler papers
├── validation_tools.md     # Guia: Como usar o Hub SD/CCC na prática
└── references.md           # Links canônicos e benchmarks
```

-----

### 🧠 7. Princípios de Uso

1.  **Função, não preferência:** Não usamos "a IA favorita", usamos a IA certa para a etapa (ex: Claude para escrever, DeepSeek para calcular).
2.  **Convergência de Inteligências:**
      * Divergência entre modelos = Ponto de investigação.
      * Convergência entre modelos = Evidência sintética.
3.  **Custo Zero:** Nenhuma etapa exige cartão de crédito.
4.  **Reprodutibilidade:** Se o prompt não passa no **Semantic Density**, ele não entra no relatório final.

-----

### 🧪 8. Quickstart (5 minutos)

1.  Abra o arquivo [`llm_orchestration.md`](https://www.google.com/search?q=./llm_orchestration.md).
2.  Entenda o papel de cada IA no diagrama.
3.  Copie um Template de Prompt.
4.  Teste no **Gemini** (Exploração) e **Claude** (Estrutura).
5.  **Valide** o resultado usando o botão "Open in Colab" na tabela de Inovações Nativas acima.

-----

