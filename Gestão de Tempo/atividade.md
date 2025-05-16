## Análise de um Histórico de Commits (Individual)

🔗 **Repositório GitHub:** [commenthol/astronomia](https://github.com/commenthol/astronomia)

## Análise de um Histórico de Commits

**Primeira Commit**
- `fix(mars): correct longPeri`
* **Arquivos modificados:**

  * `lib/planetposition/data.vsop87Bearth.js`
* **Intenção do desenvolvedor:**
  O desenvolvedor corrigiu um erro relacionado ao parâmetro `longPeri` de Marte (longitude do periélio). Isso provavelmente melhora a precisão dos cálculos de posição do planeta.

---

### 📌 Commit 2

* **Mensagem:** `chore: add vitest`
* **Arquivos modificados:**

  * `package.json`
  * `pnpm-lock.yaml`
* **Intenção do desenvolvedor:**
  Foi adicionada a biblioteca de testes `vitest` ao projeto. Essa mudança prepara o projeto para ter testes automatizados, o que ajuda a garantir que o código funcione corretamente no futuro.

---

### 📌 Commit 3

* **Mensagem:** `docs(readme): update badges`
* **Arquivos modificados:**

  * `README.md`
* **Intenção do desenvolvedor:**
  Atualizou os badges do README (aqueles ícones com informações como "build passando", "versão", etc.). Isso melhora a documentação e a apresentação do projeto para visitantes no GitHub.

---

### 🔁 **Evolução com esses commits:**

1. Primeiro corrigiram uma falha em um cálculo importante (Marte).
2. Depois, adicionaram uma ferramenta para testar o projeto.
3. Por fim, melhoraram a documentação.

Ou seja, o projeto está sendo mantido com:

* precisão (ciência),
* qualidade (testes),
* e clareza (documentação).

---

## ✅ **Parte 2: A Importância das Mensagens de Commit**

### 🟢 Boas mensagens do repositório:

* `fix(mars): correct longPeri` → clara, mostra o que foi corrigido e onde.
* `docs(readme): update badges` → mostra que é documentação, exatamente o que foi atualizado.
* `chore: add vitest` → mostra que é uma tarefa de configuração.

Essas mensagens seguem boas práticas:

* Usam prefixos (`fix`, `docs`, `chore`) para indicar o tipo de mudança.
* São curtas e informativas.
* Ajudam a entender rapidamente o histórico.

### 🔴 Exemplo de mensagem ruim (hipotético):

* `mudança geral`
* `teste`
* `coisas novas`

Essas não ajudam ninguém a entender o que mudou. Num projeto com várias pessoas, isso atrapalha bastante.

---

## ✅ **Parte 3: O Conceito de Branching**

### 💡 O que é uma branch?

Branch é como um **caminho alternativo** do projeto. Você pode fazer testes e alterações nele, e só depois juntar ao projeto principal.

### 🧪 Exemplo prático:

Imagine que alguém no projeto *astronomia* quer adicionar um novo cálculo de eclipses.

Ao invés de alterar direto no código principal (`main` ou `master`), ele pode criar uma branch chamada `eclipse-calculator`, trabalhar lá, testar tudo e, quando estiver pronto, **fazer um merge** com a branch principal.

---

### 📍 Vantagens das branches:

* Segurança: você não quebra o projeto principal.
* Organização: cada nova ideia ou correção pode ser feita separadamente.
* Colaboração: cada dev pode trabalhar em uma branch diferente.

---

Se quiser, posso montar um PDF bonitinho com tudo isso pronto para você entregar. Quer?

