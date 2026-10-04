# ARCHITECTURE - AI Dev Workflow

## 1. Objetivo

Este documento descreve a arquitetura geral da Fabrica de Software com IA.

A arquitetura deve permanecer simples, modular e evolutiva.

O principio central e construir primeiro um fluxo minimo funcional e somente depois adicionar automacoes e orquestracao avancada.

## 2. Arquitetura principal

USUARIO
-> ChatGPT Project
-> Repositorio local
-> Git
-> GitHub
-> Antigravity IDE + Codex
-> Testes e revisao
-> GitHub
-> CI/CD
-> Deploy e hospedagem
-> Aplicacao publicada

## 3. Fonte oficial de verdade

O GitHub sera a fonte oficial para:

- codigo;
- documentacao;
- historico de alteracoes;
- commits;
- branches;
- pull requests;
- releases;
- configuracoes de CI/CD.

O repositorio local sera a area de trabalho sincronizada com o GitHub.

O historico de conversas das ferramentas de IA nao deve ser considerado a unica memoria do projeto.

As decisoes importantes devem ser registradas nos arquivos do repositorio.

## 4. Camada de orquestracao

### ChatGPT Project

Responsabilidades principais:

- receber a ideia inicial;
- realizar descoberta;
- estruturar requisitos;
- criar especificacoes;
- propor arquitetura;
- dividir trabalho em tarefas;
- coordenar ferramentas;
- manter documentacao;
- revisar decisoes;
- acompanhar o estado do workflow.

O ChatGPT atua como coordenador geral do processo.

## 5. Camada de versionamento

### Git

Responsavel pelo controle de versao local.

Funcoes:

- registrar alteracoes;
- criar commits;
- gerenciar branches;
- permitir reversao;
- comparar versoes.

### GitHub

Responsavel pelo repositorio remoto e historico oficial.

Funcoes:

- armazenar o repositorio;
- sincronizar alteracoes;
- permitir colaboracao;
- hospedar pull requests;
- executar CI/CD;
- manter releases;
- integrar ferramentas externas.

## 6. Camada de desenvolvimento

### Antigravity IDE

Ambiente principal para:

- abrir o repositorio;
- navegar nos arquivos;
- editar codigo;
- executar aplicacoes;
- executar comandos;
- testar funcionalidades;
- inspecionar erros;
- utilizar agentes de desenvolvimento.

### Codex

Agente de engenharia de software utilizado para:

- implementar tarefas;
- corrigir bugs;
- refatorar codigo;
- criar testes;
- revisar codigo;
- analisar problemas tecnicos;
- realizar auditorias.

## 7. Camada complementar

### Gemini

Utilizado quando apresentar vantagem em:

- pesquisa;
- grandes contextos;
- documentacao;
- planejamento;
- revisao;
- exploracao de alternativas;
- recursos do ecossistema Google.

### Google Antigravity 2.0

Nao sera inicialmente o centro do workflow.

Sera introduzido progressivamente depois que o fluxo basico estiver funcionando.

Seu objetivo futuro sera atuar como camada de orquestracao de agentes e automacao de tarefas.

## 8. Fluxo de uma funcionalidade

Fluxo desejado:

REQUISITO
-> TAREFA
-> IMPLEMENTACAO
-> REVISAO
-> TESTE
-> CORRECAO
-> COMMIT
-> GITHUB

Sempre que possivel:

CONSTRUTOR
-> REVISOR
-> TESTE
-> CORRECAO

## 9. Fluxo de um projeto completo

IDEIA
-> DESCOBERTA
-> REQUISITOS
-> ARQUITETURA
-> PLANEJAMENTO
-> PREPARACAO DO AMBIENTE
-> DESENVOLVIMENTO
-> TESTES
-> REVISAO
-> SEGURANCA
-> GITHUB
-> CI/CD
-> DEPLOY
-> VALIDACAO
-> DOCUMENTACAO
-> MANUTENCAO

## 10. Estrutura documental

Documentos principais:

README.md
PROJECT.md
REQUIREMENTS.md
ARCHITECTURE.md
TASKS.md
CHANGELOG.md
DECISIONS.md
AGENTS.md
.env.example

Documentos opcionais conforme o projeto:

API.md
DATABASE.md
SECURITY.md
DEPLOYMENT.md
TESTING.md
DESIGN_SYSTEM.md

## 11. Estrategia de branches

Padrao inicial:

main

A branch main deve representar o estado principal e estavel do projeto.

Branches adicionais poderao ser utilizadas futuramente para funcionalidades, correcoes e experimentos.

A estrategia de branches sera ampliada somente quando a complexidade do projeto justificar.

## 12. Estrategia de commits

Os commits devem ser:

- pequenos;
- compreensiveis;
- relacionados a uma unica mudanca principal;
- descritivos;
- reversiveis quando possivel.

Exemplos:

docs: add project overview
docs: add workflow requirements
feat: add authentication
fix: correct login validation
test: add authentication tests
refactor: simplify user service

## 13. Seguranca

Nunca armazenar no repositorio:

- senhas;
- tokens;
- chaves de API;
- secrets;
- credenciais de banco.

Utilizar variaveis de ambiente.

O arquivo .env deve permanecer fora do Git.

O arquivo .env.example deve conter apenas nomes de variaveis e exemplos sem segredos reais.

## 14. CI/CD

A camada de CI/CD sera implementada progressivamente.

Objetivos futuros:

- validar codigo automaticamente;
- executar lint;
- executar testes;
- validar build;
- impedir deploy com falhas criticas;
- automatizar deploy quando seguro.

## 15. Deploy

A plataforma de deploy nao sera fixa para todos os projetos.

A escolha dependera da aplicacao.

Opcoes prioritarias:

- Vercel;
- Netlify;
- Cloudflare;
- outras plataformas gratuitas ou de baixo custo quando justificadas.

## 16. Principio de evolucao

A arquitetura deve evoluir nesta ordem:

1. fluxo manual funcionando;
2. processo documentado;
3. tarefas repetiveis identificadas;
4. automacao das tarefas;
5. integracao entre ferramentas;
6. orquestracao de agentes;
7. monitoramento e melhoria continua.

Nao adicionar complexidade sem beneficio concreto.
