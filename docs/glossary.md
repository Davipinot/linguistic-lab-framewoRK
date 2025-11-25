# 📚 Glossário e FAQ Oficial

> **O vocabulário controlado do Linguistic Laboratory Framework.**
> Definições precisas para garantir a reprodutibilidade científica e o alinhamento entre pesquisadores e IAs.

---

## 📖 1. Glossário Técnico (SLE & Engenharia)

Termos derivados da **Semantic Latent Engineering**, a física que rege este laboratório.

| Termo | Sigla | Definição Técnica | Contexto de Uso |
| :--- | :---: | :--- | :--- |
| **Algebraic Intention** | $I_{\Lambda}$ | A representação matemática imutável do objetivo do pesquisador. É o "norte magnético" que guia a orquestração. | *Capítulo 1* |
| **Semantic Density** | **SD** | Métrica vetorial que indica a taxa de sinal/ruído de um prompt. Medida via similaridade de cosseno. Alta SD = Máxima precisão com mínimo de tokens. | *Notebook `sd_validator`* |
| **Behavior Contract** | **CCC** | *Context Commitment Contract*. Um conjunto de restrições lógicas que define a "personalidade" e os limites de segurança de um agente. | *Notebook `behavior_validator`* |
| **High-Density Anchor** | **HDSA** | Um termo técnico ou token único que ativa um cluster complexo de conhecimento no modelo (ex: "Otimização O(n)"). | *Engenharia de Prompt* |
| **Operational Grammar** | $\Gamma$ | A sintaxe híbrida (`>>`, `@`, `//`) usada para programar o espaço latente. | *Capítulo 3* |
| **Drift** | - | A "deriva" semântica. Quando o agente, ao longo de uma conversa longa, esquece o contrato original e começa a alucinar ou mudar de tom. | *Validação de Output* |
| **Grounding** | - | O processo de "ancorar" a IA em fontes primárias (PDFs, Docs) para impedir que ela invente fatos. | *NotebookLM* |

---

## 🧩 2. Glossário Operacional (O Fluxo)

Termos relacionados à metodologia de trabalho no laboratório federado.

| Termo | Definição Operacional |
| :--- | :--- |
| **Laboratório Federado** | Um ecossistema onde nenhuma IA é soberana. O conhecimento surge da colaboração entre Gemini (Exploração), Claude (Estrutura) e DeepSeek (Lógica). |
| **Curador-Orquestrador** | O novo papel do pesquisador. Ele não escreve o texto final; ele desenha a intenção, escolhe os agentes e valida o resultado. |
| **Cross-Check** | O ato de usar uma IA para auditar a outra (ex: pedir ao ChatGPT para encontrar falhas lógicas no texto do Gemini). |
| **Checkpoint de Validação** | O momento obrigatório onde o fluxo para e o humano roda um teste no *Scientific Validation Hub* antes de prosseguir. |
| **Scientific Hub** | O repositório auxiliar que contém os notebooks de validação, tracking (MLflow) e versionamento (DVC). |
| **Rigor 1.0** | O padrão de qualidade do lab: nada é publicado sem um badge de validação matemática. |

---

## ❓ 3. FAQ — Perguntas Frequentes

Respostas diretas para desbloquear o pesquisador.

### 🚀 Sobre o Método
**Q: Preciso saber programar (Python) para usar o laboratório?**
**A:** **Não.** O laboratório foi desenhado com um "Fluxo Cyborg".
* Você usa a **Linguagem Natural** e a **Gramática $\Gamma$** (`>>`) para criar.
* Para validar, você usa o **Gemini Assistant no Colab**, que roda o código Python por você. O processo é "Zero-Code" para o operador.

**Q: O que é "Validação Cruzada" neste contexto?**
**A:** É a prática de nunca confiar na primeira resposta.
Se o Claude gera um resumo, o DeepSeek deve validá-lo matematicamente. Isso reduz a alucinação estatística a quase zero.

**Q: Este laboratório substitui pesquisadores humanos?**
**A:** Pelo contrário. Ele **eleva** a exigência cognitiva.
A IA faz o trabalho braçal (texto, resumo). O humano precisa ter a visão arquitetural ($I_{\Lambda}$) para saber se a IA está certa. O humano deixa de ser "redator" para ser "Juiz".

---

### 🛠️ Sobre as Ferramentas
**Q: Posso usar tudo na versão gratuita?**
**A:** **Sim.** O protocolo foi desenhado exclusivamente para o *Free Tier*.
* Usamos **NotebookLM** para RAG (gratuito).
* Usamos **Colab** para execução (gratuito).
* Usamos **GitHub** para hospedagem (gratuito).

**Q: Como sei se meu resultado foi aprovado?**
**A:** Você deve rodar o teste no Hub.
* Se o notebook der **PASS** (Verde), está validado.
* Você deve então colar o Badge no seu README ou documento final.

**Q: O que fazer quando as IAs divergem (ex: Gemini diz A, Claude diz B)?**
**A:** Comemore. Você encontrou um **Dado Científico**.
A divergência entre modelos geralmente aponta para uma ambiguidade na literatura ou uma complexidade real do tema. Use o **DeepSeek** ou o **ChatGPT** como árbitro para desempatar logicamente.

---

### ⚖️ Ética e Dados
**Q: O laboratório aceita dados sensíveis?**
**A:** **Não.**
Como usamos versões gratuitas e públicas de LLMs, seus dados podem ser usados para treino. **Nunca** insira dados médicos reais, senhas ou segredos industriais. Trabalhe apenas com dados públicos ou anonimizados.

**Q: Como citar este trabalho?**
**A:** Se você usou o framework para gerar sua pesquisa, cite o repositório e inclua o DOI do Zenodo (gerado no Notebook 04). Isso garante que sua metodologia seja auditável por pares.

---

> **Dúvida não listada?** Abra uma Issue no GitHub ou pergunte ao Assistente do Lab (Gemini/Claude) usando a base de conhecimento `/docs`.
