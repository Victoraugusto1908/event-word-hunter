# vue-project

This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VS Code](https://code.visualstudio.com/) + [Vue (Official)](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur).

## Recommended Browser Setup

- Chromium-based browsers (Chrome, Edge, Brave, etc.):
  - [Vue.js devtools](https://chromewebstore.google.com/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd)
  - [Turn on Custom Object Formatter in Chrome DevTools](http://bit.ly/object-formatters)
- Firefox:
  - [Vue.js devtools](https://addons.mozilla.org/en-US/firefox/addon/vue-js-devtools/)
  - [Turn on Custom Object Formatter in Firefox DevTools](https://fxdx.dev/firefox-devtools-custom-object-formatters/)

## Type Support for `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) to make the TypeScript language service aware of `.vue` types.

## Customize configuration

See [Vite Configuration Reference](https://vite.dev/config/).

## Project Setup

```sh
bun install
```

### Compile and Hot-Reload for Development

```sh
bun dev
```

### Type-Check, Compile and Minify for Production

```sh
bun run build
```

## 🤝 Como contribuir

A branch `main` deste repositório é **protegida**. Por esse motivo, não é permitido realizar alterações diretamente nela, incluindo commits e pushes.

Toda contribuição deve ser feita por meio de uma **Pull Request (PR)**.

### Fluxo de contribuição

1. Atualize sua branch `main` local:

   ```bash
   git switch main
   git pull origin main
   ```

2. Crie uma nova branch para sua alteração:

   ```bash
   git switch -c tipo/descricao-da-alteracao
   ```

   Exemplos:

   ```bash
   git switch -c feat/adicionar-autenticacao
   git switch -c fix/corrigir-validacao-email
   git switch -c docs/atualizar-readme
   ```

3. Faça as alterações necessárias e crie o commit:

   ```bash
   git add .
   git commit -m "feat: adiciona autenticação de usuários"
   ```

4. Envie a branch para o repositório remoto:

   ```bash
   git push -u origin tipo/descricao-da-alteracao
   ```

5. No GitHub, abra uma **Pull Request** da sua branch para a branch `main`.

> [!IMPORTANT]
> Não faça commits ou pushes diretamente na branch `main`. Todas as alterações devem passar por uma Pull Request antes de serem integradas ao projeto.

### Requisitos para aprovação

Antes de realizar o merge, a Pull Request poderá passar por:

* revisão de código;
* resolução das conversas e comentários;
* aprovação de pelo menos um responsável;
* execução dos testes e verificações automatizadas do projeto.

Após a aprovação, a alteração poderá ser integrada à branch `main`.

## 💡 Propostas de implementação e Issues

Toda ideia de nova funcionalidade, melhoria, correção ou alteração relevante deve ser registrada em uma **Issue** antes do início da implementação.

As Issues funcionam como o ponto central para:

* documentar a necessidade da alteração;
* discutir possíveis soluções;
* definir prioridade e escopo;
* registrar decisões técnicas;
* acompanhar o andamento da implementação;
* relacionar a demanda à Pull Request correspondente.

> [!IMPORTANT]
> Não inicie uma implementação relevante sem uma Issue previamente cadastrada e discutida.

### Estrutura mínima de uma Issue

Toda Issue deve conter, no mínimo, as seguintes informações:

#### Título

O título deve ser curto, objetivo e representar claramente a demanda.

Formato recomendado:

```text
[categoria] Descrição resumida da demanda
```

Exemplos:

```text
[Feature] Adicionar autenticação por e-mail
[Bug] Corrigir falha ao salvar o perfil
[Improvement] Melhorar desempenho da listagem
[Documentation] Documentar variáveis de ambiente
```

#### Descrição

A descrição deve explicar:

* qual problema precisa ser resolvido;
* qual é o comportamento atual;
* qual é o comportamento esperado;
* quem ou qual parte do sistema é afetada;
* quais regras, limitações ou dependências devem ser consideradas.

Sempre que possível, inclua exemplos, imagens, logs, mensagens de erro ou passos para reprodução.

#### Categoria

A Issue deve ser classificada em uma das categorias abaixo:

| Categoria       | Uso                                                          |
| --------------- | ------------------------------------------------------------ |
| `Feature`       | Nova funcionalidade ou capacidade do sistema                 |
| `Bug`           | Correção de comportamento incorreto                          |
| `Improvement`   | Melhoria em uma funcionalidade existente                     |
| `Refactor`      | Alteração interna de código sem mudança funcional esperada   |
| `Documentation` | Criação ou atualização de documentação                       |
| `Maintenance`   | Atualização de dependências, configurações ou infraestrutura |
| `Research`      | Investigação técnica ou análise antes da implementação       |

#### Urgência

A urgência deve indicar o impacto e a necessidade de atendimento da Issue:

| Urgência  | Critério                                                                |
| --------- | ----------------------------------------------------------------------- |
| `Baixa`   | Não afeta o uso atual e pode ser planejada futuramente                  |
| `Média`   | Possui impacto limitado, mas deve entrar no planejamento                |
| `Alta`    | Afeta uma funcionalidade importante ou bloqueia parte do trabalho       |
| `Crítica` | Indisponibilidade, perda de dados, falha de segurança ou bloqueio geral |

A classificação de urgência deve refletir o impacto real da demanda, e não apenas a preferência de quem abriu a Issue.

### Modelo sugerido

```markdown
## Descrição

Explique de forma clara o problema, a necessidade ou a oportunidade identificada.

## Comportamento atual

Descreva como o sistema funciona atualmente.

## Comportamento esperado

Descreva o resultado esperado após a implementação.

## Categoria

- [ ] Feature
- [ ] Bug
- [ ] Improvement
- [ ] Refactor
- [ ] Documentation
- [ ] Maintenance
- [ ] Research

## Urgência

- [ ] Baixa
- [ ] Média
- [ ] Alta
- [ ] Crítica

## Critérios de aceite

- [ ] Critério 1
- [ ] Critério 2
- [ ] Critério 3

## Informações adicionais

Adicione referências, imagens, logs, dependências, riscos ou observações relevantes.
```

### Relação entre Issue e Pull Request

Toda Pull Request deve referenciar a Issue relacionada em sua descrição.

Exemplo:

```text
Closes #42
```

Ao utilizar palavras-chave como `Closes`, `Fixes` ou `Resolves`, o GitHub poderá encerrar automaticamente a Issue quando a Pull Request for integrada à branch `main`.

