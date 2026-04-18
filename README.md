# Explorando Práticas de Teste

Neste exercício, vamos explorar práticas de teste em sistemas reais utilizando a ferramenta [TestMiner](https://andrehora.github.io/testminer).

O TestMiner permite visualizar e analisar testes de software em repositórios do GitHub, fornecendo dados sobre como os projetos organizam seus testes, como eles evoluem entre versões e quais bibliotecas de teste são utilizadas.
Explore a ferramenta antes de começar para se familiarizar com seu funcionamento.

---

## Passo 1: Selecionar um repositório

Escolha um repositório real que possua testes escritos na linguagem de sua preferência.
Abaixo estão alguns links para ajudá-lo a encontrar projetos interessantes:

- **Python:** https://github.com/topics/python?l=python
- **JavaScript:** https://github.com/topics/javascript?l=javascript
- **TypeScript:** https://github.com/topics/typescript?l=typescript
- **Java:** https://github.com/topics/java?l=java

## Passo 2: Explorar o repositório selecionado

Busque o repositório escolhido no [TestMiner](https://andrehora.github.io/testminer) e analise os dados de teste gerados pela ferramenta.

## Passo 3: Explicar uma prática de teste

Com base nos dados obtidos, selecione uma prática ou dado de teste relevante e explique-o com suas próprias palavras.

---

## Instruções de entrega

1. Faça um `fork` deste repositório (saiba mais sobre forks [aqui](https://docs.github.com/pt/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)).
2. Responda às questões abaixo diretamente neste arquivo `README.md` do seu fork. Pode adicionar imagens para enriquecer sua explicação.
3. No Moodle, submeta apenas a URL do seu fork.

---

## Respostas

**1. Repositório selecionado:** `(https://github.com/airbnb/javascript) / https://github.com/airbnb/javascript/blob/master/packages/eslint-config-airbnb/test/test-react-order.js `

**2. Explicação:** `O código analisado aplica a prática de Testes de Unidade para Validação de Regras de Linting, utilizando a biblioteca tape e a API do ESLint. O objetivo central não é testar o funcionamento de um software final, mas sim garantir a integridade das regras de padronização impostas pelo guia de estilo da Airbnb.

A prática foca especificamente na regra react/sort-comp, que estabelece uma hierarquia rígida para a declaração de métodos em classes React. O teste funciona simulando o comportamento de um desenvolvedor: ele injeta blocos de código propositalmente desordenados em uma função auxiliar (wrapComponent) e executa o linter programaticamente. A validação é bem-sucedida quando o linter identifica o erro de ordenação esperado (ex: um método customizado declarado antes de um método de ciclo de vida como o componentDidMount). Essa abordagem garante que qualquer alteração futura nas configurações de estilo não comprometa a consistência estética e estrutural dos projetos que utilizam essa biblioteca.`
