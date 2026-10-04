# REQUIREMENTS - AI Dev Workflow

## 1. Objetivo

Definir os requisitos obrigatorios do workflow integrado de desenvolvimento de software assistido por Inteligencia Artificial.

## 2. Requisitos funcionais

### RF-001 - Entrada em linguagem natural

O usuario deve poder iniciar um projeto descrevendo uma necessidade, problema ou ideia em linguagem natural.

### RF-002 - Analise da ideia

O ChatGPT deve transformar a solicitacao inicial em uma analise estruturada contendo, conforme necessario:

- objetivo;
- publico;
- usuarios;
- funcionalidades;
- restricoes;
- riscos;
- prioridades.

### RF-003 - Especificacao

O workflow deve ser capaz de produzir:

- requisitos funcionais;
- requisitos nao funcionais;
- historias de usuario quando aplicavel;
- criterios de aceitacao;
- regras de negocio;
- escopo do MVP.

### RF-004 - Arquitetura

Cada projeto deve possuir uma arquitetura definida antes das implementacoes relevantes, incluindo quando aplicavel:

- frontend;
- backend;
- banco de dados;
- autenticacao;
- armazenamento;
- APIs;
- infraestrutura;
- hospedagem;
- seguranca.

### RF-005 - Planejamento por tarefas

Projetos devem ser divididos em:

EPICOS
-> FUNCIONALIDADES
-> TAREFAS
-> SUBTAREFAS

As tarefas devem ser pequenas, compreensiveis, testaveis e reversiveis.

### RF-006 - Controle de versao

Todo projeto profissional deve utilizar:

- Git;
- GitHub;
- commits descritivos;
- branch principal main;
- branches adicionais quando necessario;
- pull requests quando necessario;
- tags e releases quando aplicavel.

### RF-007 - Desenvolvimento assistido por IA

O workflow deve permitir utilizar agentes de IA para:

- implementar codigo;
- revisar codigo;
- corrigir bugs;
- executar refatoracoes;
- criar testes;
- atualizar documentacao.

### RF-008 - Revisao

Sempre que possivel, o processo deve seguir:

CONSTRUTOR
-> REVISOR
-> TESTE
-> CORRECAO

### RF-009 - Testes

Cada aplicacao deve possuir testes adequados ao seu contexto, podendo incluir:

- testes unitarios;
- testes de integracao;
- testes de interface;
- testes responsivos;
- validacao de formularios;
- verificacao de build.

### RF-010 - Seguranca

O workflow deve verificar, conforme aplicavel:

- autenticacao;
- autorizacao;
- validacao de entrada;
- exposicao de credenciais;
- seguranca de APIs;
- permissoes;
- dependencias vulneraveis;
- configuracao do banco de dados.

### RF-011 - Credenciais

Senhas, tokens, chaves de API e secrets nao podem ser armazenados diretamente no codigo.

Devem ser utilizadas variaveis de ambiente.

O arquivo .env deve permanecer fora do Git.

Um arquivo .env.example deve ser mantido sem dados secretos quando necessario.

### RF-012 - Deploy

O workflow deve conduzir o projeto ate a publicacao quando o objetivo da aplicacao exigir deploy.

O processo deve considerar:

- build;
- variaveis de ambiente;
- banco de producao;
- dominio;
- HTTPS;
- CI/CD;
- logs;
- backups;
- monitoramento.

### RF-013 - Documentacao

Cada projeto deve manter documentacao suficiente para permitir que humanos e agentes de IA compreendam seu estado sem depender exclusivamente das conversas anteriores.

### RF-014 - Atualizacao da documentacao

Mudancas relevantes de arquitetura, requisitos, decisoes e implementacao devem ser registradas nos documentos correspondentes.

### RF-015 - Criterio de conclusao

Uma aplicacao somente pode ser considerada concluida quando, conforme aplicavel:

- executar sem erros criticos;
- cumprir os requisitos;
- possuir interface funcional;
- ser responsiva;
- possuir persistencia de dados quando necessaria;
- possuir seguranca minima;
- possuir testes essenciais;
- estar versionada;
- estar documentada;
- estar publicada quando necessario;
- permitir manutencao futura.

## 3. Requisitos nao funcionais

### RNF-001 - Simplicidade

O workflow deve priorizar solucoes simples antes de arquiteturas complexas.

### RNF-002 - Custo-beneficio

A prioridade de ferramentas e servicos deve ser:

gratuito
-> incluido nas assinaturas atuais
-> open source
-> baixo custo
-> pago somente quando necessario

### RNF-003 - Manutencao

O codigo e a documentacao devem facilitar manutencao futura.

### RNF-004 - Clareza

Tarefas, commits, documentos e decisoes devem utilizar nomes claros e compreensiveis.

### RNF-005 - Reprodutibilidade

Outro agente ou desenvolvedor deve conseguir compreender como executar, testar e continuar o projeto utilizando a documentacao do repositorio.

### RNF-006 - Seguranca por padrao

Configuracoes inseguras ou exposicao de segredos devem ser evitadas desde o inicio.

### RNF-007 - Responsividade

Aplicacoes com interface devem funcionar adequadamente em desktop, tablet e dispositivos moveis quando aplicavel.

### RNF-008 - Automacao progressiva

Processos repetitivos devem ser automatizados somente depois que o fluxo manual correspondente estiver funcionando corretamente.

## 4. Regras de execucao

Durante a configuracao pratica do workflow:

1. executar uma etapa por vez;
2. explicar o objetivo;
3. informar o terminal ou ferramenta;
4. fornecer o comando exato;
5. informar o resultado esperado;
6. verificar o resultado;
7. corrigir erros antes de avancar;
8. avancar somente apos confirmacao.

## 5. Prioridade atual

Construir primeiro o fluxo minimo funcional:

ChatGPT
-> repositorio local
-> Git
-> GitHub
-> Antigravity IDE + Codex
-> testes
-> GitHub
-> CI/CD
-> deploy

Integracoes e automacoes avancadas serao adicionadas progressivamente.
