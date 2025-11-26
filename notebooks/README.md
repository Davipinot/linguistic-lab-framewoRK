# 🧪 Notebooks de Experimentação & Validação

> **Este diretório é o seu Workspace.**
> As ferramentas de validação (Engine) estão centralizadas no nosso **Scientific Validation Hub**, mas os resultados dos seus experimentos devem ser salvos aqui.

---

## 🔗 Acesso às Ferramentas (Engine)

Seguindo a filosofia federada, não duplicamos código. Utilizamos os validadores oficiais do [Scientific Validation Hub](https://github.com/aleeepassarelli/scientific-validation-hub).

**Clique para abrir e rodar no Google Colab:**


| Ferramenta de Validação | O que ela testa? | Executar Agora |
| :--- | :--- | :---: |
| **🔍 Semantic Density (SD)** | Mede a densidade informacional e precisão vetorial dos seus prompts. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/aleeepassarelli/scientific-validation-hub/blob/main/notebooks/sd_validator.ipynb) |
| **🧠 Behavior Contract (CCC)** | Audita se o Agente manteve a aderência à missão (evita alucinação). | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/aleeepassarelli/scientific-validation-hub/blob/main/notebooks/behavior_validator.ipynb) |

---
| Experimento | Conceito | Executar |
| :--- | :--- | :---: |
| **🧪 01. Experiment Tracking** | **MLflow**: Rastreando métricas sem servidor. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/aleeepassarelli/scientific-validation-hub/blob/main/notebooks/01_tracking.ipynb) |
| **🧬 02. Data Versioning** | **DVC**: Versionamento de Prompts e Dados. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/aleeepassarelli/scientific-validation-hub/blob/main/notebooks/02_data_version.ipynb) |
| **📦 03. Metadata Packaging** | **RO-Crate**: Empacotamento FAIR para pesquisa. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/aleeepassarelli/scientific-validation-hub/blob/main/notebooks/03_metadata.ipynb) |
| **🏛️ 04. Digital Archiving** | **Zenodo**: Gerando DOIs para seu código (Sandbox). | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/aleeepassarelli/scientific-validation-hub/blob/main/notebooks/04_archiving.ipynb) |
| **✅ 05. Notebook Testing** | **nbval**: Testes unitários para células de código. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/aleeepassarelli/scientific-validation-hub/blob/main/notebooks/05_testing.ipynb) |

---

> *Estas ferramentas são puxadas diretamente do nosso [Scientific Validation Hub](https://github.com/aleeepassarelli/scientific-validation-hub).*


---

## 📝 Como usar esta pasta?

Esta pasta `/notebooks` no repositório do Laboratório deve permanecer limpa de *ferramentas*, servindo apenas para armazenar **seus experimentos validados**.

### O Fluxo de Trabalho Recomendado:

1.  **Abra a Ferramenta:** Clique em um dos botões "Open in Colab" acima.
2.  **Execute o Teste:** Rode a validação do seu prompt ou agente na nuvem.
3.  **Validou?** Se o resultado for `PASS`:
    * No Colab, vá em **Arquivo > Salvar uma cópia no GitHub**.
    * Escolha **este repositório** (`linguistic-lab-framework`).
    * Salve nesta pasta: `notebooks/experimento_nome_data.ipynb`.

### Estrutura de Arquivos Sugerida

Ao salvar seus notebooks aqui, recomendamos o seguinte padrão de nomenclatura para manter a organização científica:

* `exp_01_analise_sintaxe_gpt4.ipynb`
* `exp_02_validacao_prompt_gemini.ipynb`
* `meta_analise_final.ipynb`

---

## ⚡ Por que não colocar os validadores aqui?

Para garantir **Rigor 1.0**.
Ao centralizar o código dos validadores no *Scientific Validation Hub*, garantimos que você esteja sempre usando a versão mais atualizada, segura e auditada dos algoritmos de densidade (SD) e comportamento (CCC), sem precisar atualizar este repositório manualmente.
