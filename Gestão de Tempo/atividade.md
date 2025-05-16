## Análise de um Histórico de Commits (Individual)

🔗 **Repositório GitHub:** [commenthol/astronomia](https://github.com/commenthol/astronomia)

## Análise de um Histórico de Commits

**Primeira Commit**

`fix(mars): correct longPeri`

*Arquivos modificados:*

`lib/planetposition/data.vsop87Bearth.js`

*Qual foi a intenção do desenvolvedor?*

O desenvolvedor corrigiu um erro do parâmetro `longPeri` de Marte (longitude do periélio). Isso provavelmente pode melhorar a precisão dos cálculos de posição do planeta.

**Segunda Commit**

`chore: add vitest`

*Arquivos modificados:*

`package.json`
`pnpm-lock.yaml`

*Qual foi a intenção do desenvolvedor?*

Foi adicionada uma biblioteca de testes `vitest` no projeto para testes automatizados e garantir o funcionamento correto do código.

**Terceira Commit**

`docs(readme): update badges`

*Arquivos modificados:*

`README.md`

*Qual foi a intenção do desenvolvedor?*

Atualizou os badges do README (aqueles ícones com informações como "build passando", "versão", etc.) para melhorar a documentação e a apresentação do projeto.

**Evolução do Projeto**

Primeiro corrigiram uma falha em um cálculo importante de um planeta para precisão, depois adicionaram uma ferramenta para testar o projeto, afim de testar a qualidade e melhoraram a documentação para clareza.

## A Importância das Mensagens de Commit 

* `fix(mars): correct longPeri` mostra o que foi corrigido e onde.
* `docs(readme): update badges` mostra que é documentação, exatamente o que foi atualizado.
* `chore: add vitest` mostra que é uma tarefa de configuração.

Conclusão: Mensagens bem feitas ajudam a entender rapidamente o histórico.

## O Conceito de Branching

Branch é como um **caminho alternativo** do projeto para poder fazer testes e alterações nele, e só depois juntar ao projeto principal.

*Vantagens das branches:*

* Segurança: você não quebra o projeto principal.
* Organização: cada nova ideia ou correção pode ser feita separadamente.
* Colaboração: cada dev pode trabalhar em uma branch diferente.

*Exemplo*

Se alguém do projeto *astronomia* quer adicionar um novo cálculo de eclipses, ao invés de alterar direto no código principal (`main` ou `master`), ele pode criar uma branch chamada `eclipse-calculator`, trabalhar lá, testar tudo e, quando estiver pronto, fazer um merge (combinar as alterações de uma branch com outra) com a branch (linha de desenvolvimento separada de um projeto, que permite aos desenvolvedores trabalharem em novas funcionalidades, correções de bugs ou experimentos sem interferir na versão principal do código) principal.
