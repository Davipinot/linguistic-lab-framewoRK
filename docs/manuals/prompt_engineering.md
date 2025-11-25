# 🛠️ Manual de Engenharia de Prompts Validada

> **Como escrever instruções que passam no Crivo Matemático (Rigor 1.0).**
> Pare de "conversar" com a IA. Comece a injetar vetores.

-----

## 1\. O Alvo: O que o Validador quer?

O [link suspeito removido] não julga se seu prompt é "bonito". Ele julga se é **Denso**.

Para ganhar o badge `Scientific Validation: PASSING`, seu prompt deve satisfazer:

1.  **Similaridade Vetorial ($\ge 0.70$):** O prompt deve ativar os mesmos neurônios que a tarefa alvo, sem ruído.
2.  **Minimalismo Léxico:** Usar o menor número de palavras possível para atingir essa ativação.

> **Regra de Ouro:** "Se uma palavra não altera o vetor de direção, ela é ruído. Apague."

-----

## 2\. A Técnica de Compressão Semântica

Para transformar um prompt natural (Reprovado) em um prompt SLE (Aprovado), siga o processo de destilação:

### Passo A: Remoção de Ruído (Stop Words)

Artigos, preposições e polidez social ("por favor", "gostaria", "o", "a", "um") diluem a densidade. A IA não precisa de educação, precisa de direção.

  * ❌ *Ruim:* "Olá, você poderia por favor criar uma função para calcular a média?"
  * ✅ *Melhor:* "Criar função cálculo média."

### Passo B: Ancoragem Terminológica (HDSAs)

Substitua descrições vagas por termos técnicos precisos (**High-Density Semantic Anchors**). Um termo técnico vale por dez palavras comuns.

  * ❌ *Ruim:* "O código deve rodar rápido e não travar se tiver muitos dados."
  * ✅ *Melhor:* "Otimizar Big-O. Implementar Error Handling robusto."

### Passo C: Sintaxe Operacional ($\Gamma$)

O uso dos operadores `>>`, `@`, `//` elimina a necessidade de conectivos gramaticais.

  * ✅ *Perfeito:* `@Dev >> Optimize(O(n)) // Python`

-----

## 3\. Antes e Depois (Estudo de Caso)

Vamos submeter dois prompts ao **SD Validator** para a mesma tarefa: *"Criar um script Python para ler um CSV e plotar um gráfico."*

### 🔴 O Prompt "Natural" (FAIL)

```text
Olá, estou precisando de uma ajuda. Queria um código em Python que conseguisse ler um arquivo CSV que eu tenho aqui. Depois de ler, ele precisa gerar um gráfico de barras mostrando as vendas. Se der, comenta o código pra eu entender.
```

  * **Contagem de Palavras:** 42
  * **Densidade Semântica:** 0.45 (Baixa)
  * **Veredito:** **REPROVADO**. Muito ruído ("estou precisando", "que eu tenho aqui"). A intenção está diluída em conversa.

### 🟢 O Prompt "SLE" (PASS)

```sle
@Data_Scientist >> Plot_Chart(Type=Bar, Source=CSV) ::Column=Sales // Code_Comments
```

  * **Contagem de Palavras:** 8 (Tokens funcionais)
  * **Densidade Semântica:** 0.88 (Extrema)
  * **Veredito:** **APROVADO**. Cada token carrega informação crítica. O vetor aponta exatamente para "Python Data Viz".

-----

## 4\. Checklist de Aprovação

Antes de colar seu prompt no validador, verifique:

1.  [ ] **Eliminei a saudação?** (Nada de "Oi", "Bom dia").
2.  [ ] **Defini a Persona com `@`?** (Isso carrega o contexto implícito).
3.  [ ] **Usei verbos no imperativo ou infinitivo?** ("Gerar", "Analisar", não "Eu queria que...").
4.  [ ] **Substituí frases por termos técnicos?** ("Deixar mais rápido" $\to$ "Otimizar Latência").
5.  [ ] **Usei `//` para formatar a saída?** (Evita que você tenha que escrever "Me dê apenas o código").

-----

## 5\. Troubleshooting: Por que meu prompt falhou?

Se o validador retornou `FAIL`, verifique o diagnóstico:

| Sintoma | Causa Provável | Correção |
| :--- | :--- | :--- |
| **Score \< 0.70** | Ambiguidade | Você usou palavras com múltiplos significados (polissemia). Troque por termos técnicos unívocos (Ex: troque "ver" por "analisar" ou "auditar"). |
| **Score Alto, mas Fail** | Falta de Minimalismo | Você atingiu o sentido, mas usou muitas palavras. Aplique o Passo A (Corte de Ruído). |
| **Score Aleatório** | Falta de Contexto | O prompt é curto demais e vago (ex: "Fazer"). Use `@Persona` para dar direção vetorial. |

-----

> **Lembre-se:** Um prompt validado não é apenas "melhor para a IA". Ele é **reprodutível**. Se você enviar o prompt SLE para outro pesquisador, ele obterá o mesmo resultado de alta qualidade, independentemente do dia ou da temperatura do modelo.
