# 📘 Tutoriais de Engenharia de Execução

> **Do Fenômeno ao Axioma: O passo-a-passo operacional do Laboratório.**
> Como executar o ciclo científico utilizando os validadores do Scientific Validation Hub.

-----

## 📘 Tutorial 1 — Definição da Intenção Algébrica ($I_{\Lambda}$)

Toda investigação começa não com uma pergunta vaga, mas com a definição de um vetor de intenção imutável. Se você não sabe para onde aponta o vetor, a IA vai alucinar.

**Passos:**

1.  **Observe o Fenômeno:**
      * *Exemplo:* "O modelo X perde coerência após 4000 tokens."
2.  **Formalize a Equação $I_{\Lambda}$:**
      * Defina os componentes antes de abrir o chat.
      * **S (Semântica):** Context Window Decay.
      * **F (Finalidade):** Identificar o ponto exato de inflexão da perda de memória.
      * **$\Omega$ (Contrato):** Análise técnica, sem antropomorfismo.
3.  **Registro no Log:**
    ```yaml
    Experiment_ID: EXP-001
    Intention_Vector:
      Target: "Context Window Failure Analysis"
      Constraints: ["Technical_Only", "Data_Driven"]
    ```

-----

## 📘 Tutorial 2 — Grounding e Curadoria de Fontes

Antes de gerar texto, precisamos gerar contexto. Usamos o **NotebookLM** como a "Memória de Longo Prazo" do laboratório.

**Passos:**

1.  **Coleta (Rigor 1.0):**
      * Baixe 3-5 PDFs canônicos (ArXiv, ACL) sobre o tema.
      * *Regra:* Se não tem PDF/Link oficial, não entra.
2.  **Ingestão no NotebookLM:**
      * Crie um caderno novo.
      * Arraste os PDFs.
3.  **Extração de Citações (Aterramento):**
      * Não peça resumo. Peça: *"Extraia as 5 definições matemáticas de X citadas no texto."*
      * Isso cria a base de verdade ($C$ - Compromisso) para o seu prompt.

-----

## 📘 Tutorial 3 — Engenharia de Prompt Validada (SLE)

**AQUI MUDAMOS O JOGO.** Não vamos criar "20 prompts". Vamos criar **UM** prompt perfeito, validado matematicamente.

**Passos:**

1.  **Drafting (Rascunho):**
      * Escreva sua intenção usando a **Gramática Operacional** (`>>`, `@`, `//`).
      * *Exemplo:* `@Researcher >> Analyze(Token_Decay) ::Source=[Citações] // Abstract`
2.  **Validação Prévia (O Pulo do Gato):**
      * Abra o **[SD Validator Notebook](https://www.google.com/search?q=https://github.com/aleeepassarelli/scientific-validation-hub/blob/main/notebooks/sd_validator.ipynb)**.
      * Cole seu prompt e o domínio.
      * **Meta:** Conseguir o badge `PASS` (Score \> 0.70).
      * *Se falhar:* Corte palavras. Use termos técnicos. Tente de novo.
3.  **Execução:**
      * Só agora você cola o prompt no Gemini ou Claude.

> *Resultado: Você economiza horas de leitura eliminando respostas ruins na origem.*

-----

## 📘 Tutorial 4 — Orquestração Federada (O Pipeline)

Como passar a informação de uma IA para outra sem perder a densidade (Telefone sem fio).

**Passos:**

1.  **Exploração (Gemini):**
      * Input: Prompt Validado + Fontes.
      * Output: Visão panorâmica e conexões laterais.
2.  **Síntese Lógica (ChatGPT/DeepSeek):**
      * Input: Output do Gemini.
      * Prompt de Passagem: *"@Logician \>\> Extract\_Axioms // List\_Only"*
3.  **Estruturação (Claude):**
      * Input: Lista de Axiomas.
      * Prompt Final: *"@Writer \>\> Compose\_Paper // Academic\_Style"*
4.  **Comparação de Divergência:**
      * Se o Gemini diz A e o Claude diz B, isso é um **Dado**. Investigue a divergência.

-----

## 📘 Tutorial 5 — Validação Final e Versionamento

O texto final está pronto. Mas ele é verdadeiro?

**Passos:**

1.  **Auditoria de Contrato (CCC):**
      * Pegue o texto final do Claude.
      * Abra o **[Behavior Validator Notebook](https://www.google.com/search?q=https://github.com/aleeepassarelli/scientific-validation-hub/blob/main/notebooks/behavior_validator.ipynb)**.
      * Cole o texto e o seu Contrato original ($\Omega$).
      * **Meta:** Badge `Adherence: PASS`.
2.  **Versionamento (DVC/Git):**
      * Salve o prompt, o output e o log de validação no seu repositório.
      * (Opcional) Use o **[Notebook de Archiving](https://www.google.com/search?q=https://github.com/aleeepassarelli/scientific-validation-hub/blob/main/notebooks/04_archiving.ipynb)** para gerar um DOI no Zenodo Sandbox.

-----

### 🏷️ Badges de Conclusão

Ao final deste ciclo, seu experimento ganha o direito de usar os selos:

  * `[SLE Validated]` (Passou no SD)
  * `[CCC Compliant]` (Passou no Behavior)
  * `[Multi-Model]` (Passou por pelo menos 2 IAs)

Este é o método que separa o "usuário de chat" do **Pesquisador Científico**.
