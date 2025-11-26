# 💬 Biblioteca de Prompts (Vetores de Intenção)

> **Coleção oficial de High-Density Semantic Anchors (HDSAs).**
> Instruções validadas matematicamente para operar o Linguistic Laboratory Framework.

-----

## 🧭 O Que São Estes Ficheiros?

Neste diretório, não armazenamos "conversas". Armazenamos **Código Semântico**.
Cada prompt aqui listado foi desenhado seguindo a **Gramática Operacional $\Gamma$** e validado para ter uma Densidade Semântica (SD) superior a **0.80**.

### 📂 O Acervo

| Ficheiro | Nível | Função Vetorial | Quando usar? |
| :--- | :---: | :--- | :--- |
| **[`10_canonical_hdsas.md`](https://www.google.com/search?q=./10_canonical_hdsas.md)** | **Nível 1** | **Fundamentos** | Para ler, escrever, codificar, analisar dados e aprender. O "kit básico" de sobrevivência. |
| **[`11_evolutionary_hdsas.md`](https://www.google.com/search?q=./11_evolutionary_hdsas.md)** | **Nível 2** | **Evolução** | Para refinar o output do Nível 1. Foca em síntese dialética, arquitetura de sistemas e antifragilidade. |

-----

## 🛠 Como Utilizar (Copy-Paste Engineering)

Não tente "conversar" com estes prompts. Use-os como funções de programação.

1.  **Selecione a Função:** Escolha o prompt adequado no ficheiro (ex: `#4 Gerador de Código`).
2.  **Copie o Bloco:** Copie o código `sle` inteiro.
3.  **Injete o Contexto:** Substitua os campos entre colchetes `[...]` pelo seu dado real.
4.  **Execute:** Cole na janela de chat da IA recomendada (Gemini, Claude, GPT).

### Exemplo de Instanciação

**Template Original:**

```sle
@Senior_Dev >> Implement(Function_X)
Specs: [O que o código deve fazer]
// Code_Only
```

**O que você envia para a IA:**

```sle
@Senior_Dev >> Implement(QuickSort_Algorithm)
Specs: Otimizado para memória, em Rust.
// Code_Only
```

-----

## 📐 A Sintaxe ($\Gamma$)

Relembre os operadores lógicos usados nestes prompts.
*(Para a teoria completa, leia [Gramática Operacional](https://www.google.com/search?q=../docs/theory/03_interface.md))*

  * **`@` (Anchor):** Define QUEM fala (Persona/Contrato).
  * **`>>` (Project):** Define O QUE fazer (Ação Vetorial).
  * **`//` (Compress):** Define COMO entregar (Formato de Saída).
  * **`!!` (Force):** Define o que é CRÍTICO (Intervenção).

-----

## 🛡️ Status de Validação

Todos os prompts nesta biblioteca passaram pelo **Scientific Validation Hub**.

> **Nota de Manutenção:** Se você criar um novo prompt que funcione consistentemente, valide-o no [SD Validator](https://www.google.com/search?q=https://github.com/aleeepassarelli/scientific-validation-hub/blob/main/notebooks/sd_validator.ipynb) e submeta um Pull Request para adicionar a esta biblioteca.
