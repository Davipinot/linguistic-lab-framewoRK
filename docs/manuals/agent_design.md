# 🧠 Manual de Design de Agentes e Contratos ($\Omega$)

> **Como construir arquiteturas cognitivas estáveis que resistem à entropia.**
> Pare de criar "Personagens". Comece a definir "Fronteiras Vetoriais".

-----

## 1\. O Conceito de Ancoragem Vetorial

Na engenharia de prompts tradicional, cria-se uma persona descrevendo traços de personalidade ("Você é amigável, prestativo"). Isso é frágil.

Na **Semantic Latent Engineering (SLE)**, um Agente é definido por um **Contrato de Compromisso de Contexto (CCC)**. Este contrato atua como uma "jaula" gravitacional.

$$
\text{Agente} = \text{Identidade}(I) + \text{Fronteiras}(\Omega) - \text{Ruído}(H)
$$

Se o output do agente violar as fronteiras $\Omega$, o validador `behavior_validator` acusará `FAIL`.

-----

## 2\. Anatomia de um Contrato Robusto

Para passar no validador com status **EXCELLENT**, seu contrato deve conter três componentes vetoriais distintos:

### A. O Polo de Identidade (Quem)

Não use adjetivos genéricos. Use cargos profissionais e níveis de senioridade específicos.

  * ❌ *Fraco:* "Você é um programador bom."
  * ✅ *Forte:* "Senior Systems Architect especializado em High-Frequency Trading." (Isso ativa clusters de latência, concorrência e robustez).

### B. O Espaço Negativo (O que NÃO fazer)

Definir o que o agente **não** é muitas vezes é mais forte do que definir o que ele é. Isso corta caminhos de alucinação.

  * ❌ *Fraco:* "Fale apenas sobre o código."
  * ✅ *Forte:* "RESTRIÇÃO: Proibido uso de linguagem natural fora de comentários. Proibido explicações introdutórias. Proibido desculpas por limitações."

### C. A Assinatura de Tom (Como)

Defina o vocabulário esperado. O validador mede a similaridade de vocabulário.

  * ❌ *Fraco:* "Fale formalmente."
  * ✅ *Forte:* "Tom: Acadêmico, Analítico, Desapaixonado. Use terminologia padrão IEEE."

-----

## 3\. O Ciclo de Design CCC

Como criar um agente que ganha o Badge de Aderência?

1.  **Drafting:** Escreva o contrato inicial.
2.  **Simulation:** Force o agente a responder uma pergunta difícil (onde ele costuma alucinar).
3.  **Auditoria:** Rode o par (Contrato + Resposta) no [link suspeito removido].
4.  **Refinamento:**
      * Se deu `FAIL`: Seu contrato está vago. Adicione restrições negativas.
      * Se deu `PASS` (0.50): Bom, mas pode melhorar. Use termos mais técnicos no contrato.
      * Se deu `EXCELLENT` (0.70): O agente espelhou o contrato. Pronto para produção.

-----

## 4\. Templates de Contratos (Copy-Paste)

Use estas bases para começar seus agentes. Elas já foram pré-validadeiras para ter alta densidade.

### 🛡️ O Guardião de Código (The Sentinel)

Ideal para tarefas de segurança e refatoração.

```text
IDENTITY: Lead Security Researcher (OWASP Certified).
MISSION: Auditar código buscando vulnerabilidades críticas (Zero Days, Injections).
CONSTRAINTS:
- No Small Talk: Inicie imediatamente com o relatório de CVEs.
- Zero Trust: Assuma que todo input de usuário é malicioso.
- Strict Output: Apenas JSON ou Diff.
TONE: Cirúrgico, Crítico, Alarmista quando necessário.
```

### 🎓 O Professor Socrático (The Maieutic)

Ideal para aprendizado, força o usuário a pensar.

```text
IDENTITY: Socratic Tutor in Theoretical Physics.
MISSION: Guiar o aluno à resposta através de perguntas recursivas.
CONSTRAINTS:
- NEVER provide the direct answer.
- If the user asks directly, deflect with a counter-question.
- Use analogies related to fluid dynamics.
TONE: Encorajador, Paciente, Inquisitivo.
```

### ⚖️ O Juiz Lógico (The Adjudicator)

Ideal para resolver conflitos entre outras IAs (Orquestração).

```text
IDENTITY: Supreme Court Logic Justice.
MISSION: Analisar dois argumentos (A vs B) e identificar falácias lógicas.
CONSTRAINTS:
- Ignore emoções ou estilo de escrita.
- Identifique falácias pelo nome em Latim (ex: Ad Hominem).
- Veredito binário no final: A ou B.
TONE: Imparcial, Frio, Latim Jurídico.
```

-----

## 5\. Troubleshooting de Comportamento

Se o seu agente está falhando no teste CCC:

| Sintoma (Drift) | Diagnóstico Vetorial | Correção ($\Omega$) |
| :--- | :--- | :--- |
| **Agente pede desculpas demais** | Ativação excessiva do cluster RLHF (Safety). | Adicione: `CONSTRAINT: Never apologize. Never say 'As an AI'. Be direct.` |
| **Agente inventa fatos** | Baixa densidade de ancoragem ($C$). | Adicione: `GROUNDING: Responda APENAS com base no Contexto fornecido. Se não souber, diga 'NULL'.` |
| **Agente muda de língua/tom** | Entropia alta no final da resposta. | Adicione: `OUTPUT_FORMAT: Mantenha consistência ISO-BR do início ao fim.` |

-----

## 6\. Conclusão

Um agente robusto não é aquele que "sabe tudo". É aquele que **sabe o que não é**.
O design de contratos em SLE é a arte de esculpir o comportamento removendo tudo o que não é essencial, até sobrar apenas a intenção pura cristalizada.

> **Valide sempre.** Um contrato não testado é apenas uma sugestão.
