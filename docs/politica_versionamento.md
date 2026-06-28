# Política de Versionamento

## Objetivo

Este documento define as políticas de versionamento adotadas no projeto **BookFlow**, com o objetivo de organizar o desenvolvimento, facilitar o controle das alterações e manter um histórico claro das versões do sistema.

---

# Estratégia de Versionamento

O projeto utilizará o **Git** como sistema de controle de versões e o **GitHub** para armazenamento remoto do repositório.

As alterações serão realizadas por meio de **branches**, **commits** e **tags**, garantindo a rastreabilidade das modificações realizadas durante o desenvolvimento.

---

# Organização das Branches

Serão utilizadas as seguintes branches:

## `main`

Contém apenas versões estáveis do projeto.

Todo o conteúdo presente nesta branch representa uma versão pronta para entrega.

---



## `develop`

Branch utilizada para integrar todas as funcionalidades antes de serem incorporadas à `main`.

Após a conclusão e revisão das alterações, a branch `develop` será mesclada com a `main`.

---



## `feature/*`

Cada nova funcionalidade ou documento será desenvolvido em uma branch própria.

Exemplos:

- `feature/requisitos`
- `feature/manual`
- `feature/pseudocodigo`

Após a conclusão da atividade, a branch será integrada à `develop`.

---



# Política de Commits

Os commits devem possuir mensagens curtas, objetivas e padronizadas.

Será utilizado o seguinte padrão:


| Prefixo     | Utilização                                     |
| ----------- | ---------------------------------------------- |
| `feat:`     | Nova funcionalidade                            |
| `docs:`     | Criação ou alteração de documentação           |
| `fix:`      | Correção de erros                              |
| `refactor:` | Refatoração sem alteração de comportamento     |
| `chore:`    | Alterações gerais de configuração ou estrutura |




### Exemplos

```text
chore: cria estrutura inicial do projeto
docs: adiciona documento de requisitos
docs: cria manual do usuário
feat: adiciona pseudocódigo
fix: corrige descrição do requisito RF03
```

---



# Política de Merges

Antes de integrar uma funcionalidade à branch `develop`, deve-se verificar se todas as alterações foram concluídas.

Após a validação, a branch da funcionalidade será mesclada à `develop`.

Ao final do projeto, a branch `develop` será integrada à `main`, representando a versão oficial da entrega.

---



# Política de Tags

As tags serão utilizadas para identificar versões importantes do projeto.


| Tag    | Descrição                           |
| ------ | ----------------------------------- |
| `v0.1` | Estrutura inicial do projeto criada |
| `v0.5` | Documentação concluída              |
| `v1.0` | Versão final entregue               |


---



# Controle dos Artefatos

Todos os documentos do projeto serão armazenados e versionados no repositório Git.

Os principais artefatos são:

- Documento de requisitos;
- Documento de pseudocódigo;
- Manual do usuário;
- Política de versionamento;
- README do projeto.

Cada alteração nesses arquivos deverá ser registrada por meio de um novo commit.

---



# Fluxo de Trabalho

O fluxo de desenvolvimento seguirá as seguintes etapas:

1. Criar uma branch a partir da `develop`;
2. Desenvolver a atividade correspondente;
3. Registrar as alterações com commits;
4. Mesclar a branch na `develop`;
5. Após a conclusão do projeto, mesclar a `develop` na `main`;
6. Criar uma tag representando a nova versão do projeto.

---



# Benefícios da Estratégia

A adoção desta política de versionamento proporciona:

- organização do desenvolvimento;
- rastreabilidade das alterações;
- histórico completo das versões;
- facilidade para identificar modificações;
- maior controle sobre os artefatos do projeto;
- redução de conflitos entre integrantes da equipe.

