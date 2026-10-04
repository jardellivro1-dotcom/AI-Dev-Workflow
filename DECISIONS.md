# DECISIONS - AI Dev Workflow

## Objetivo

Registrar decisoes importantes de arquitetura, ferramentas, processo, custos e integracoes da Fabrica de Software com IA.

Cada decisao relevante deve conter, quando aplicavel:

- contexto;
- decisao;
- motivo;
- alternativas consideradas;
- impacto;
- data;
- status.

## Formato

### DEC-XXX - Titulo da decisao

Data:
Status:

Contexto:

Decisao:

Motivo:

Alternativas consideradas:

Impacto:

---

## DEC-001 - GitHub como fonte oficial do projeto

Data: 2026-10-03
Status: Aceita

Contexto:

O workflow precisa de uma fonte central e persistente para codigo, documentacao e historico.

Decisao:

Utilizar o GitHub como fonte oficial do codigo, documentacao e historico dos projetos.

Motivo:

Permite:

- controle de versao;
- historico de alteracoes;
- colaboracao;
- branches;
- pull requests;
- releases;
- integracao com CI/CD;
- integracao com ferramentas de desenvolvimento.

Impacto:

Todos os projetos profissionais devem ser versionados e sincronizados com GitHub.

---

## DEC-002 - ChatGPT como coordenador geral

Data: 2026-10-03
Status: Aceita

Contexto:

O workflow utiliza varias ferramentas de IA e precisa evitar uso isolado e desorganizado.

Decisao:

Utilizar o ChatGPT Project como camada principal de coordenacao, requisitos, planejamento, arquitetura e documentacao.

Motivo:

Centraliza o raciocinio de produto e engenharia e transforma ideias em tarefas executaveis para os demais agentes.

Impacto:

Decisoes importantes devem ser refletidas nos arquivos do repositorio e nao permanecer apenas no historico da conversa.

---

## DEC-003 - Antigravity IDE como ambiente principal de desenvolvimento

Data: 2026-10-03
Status: Aceita

Contexto:

E necessario um ambiente principal para trabalhar diretamente nos arquivos e no codigo.

Decisao:

Utilizar o Antigravity IDE como um dos ambientes principais de desenvolvimento.

Motivo:

O ambiente permite trabalhar nos arquivos, implementar, executar, testar e corrigir codigo com apoio de agentes.

Impacto:

O repositorio GitHub devera ser aberto e utilizado diretamente no Antigravity IDE nas proximas etapas.

---

## DEC-004 - Codex como agente de engenharia de software

Data: 2026-10-03
Status: Aceita

Contexto:

O workflow precisa de um agente especializado para implementacao, revisao e manutencao tecnica.

Decisao:

Utilizar Codex principalmente como engenheiro de software.

Responsabilidades:

- implementar tarefas;
- revisar codigo;
- corrigir bugs;
- refatorar;
- criar testes;
- realizar auditorias tecnicas.

Impacto:

As tarefas entregues ao Codex devem ser pequenas, claras, testaveis e verificaveis.

---

## DEC-005 - Antigravity 2.0 sera introduzido progressivamente

Data: 2026-10-03
Status: Aceita

Contexto:

Integrar varias ferramentas e agentes desde o inicio aumentaria a complexidade do workflow.

Decisao:

Nao utilizar inicialmente o Google Antigravity 2.0 como centro do processo.

Ele sera introduzido depois que o fluxo basico estiver funcionando de ponta a ponta.

Motivo:

Primeiro validar:

ChatGPT
-> GitHub
-> Antigravity IDE + Codex
-> testes
-> GitHub
-> CI/CD
-> deploy

Depois automatizar e adicionar orquestracao de agentes.

Impacto:

Automacoes avancadas ficam fora do escopo inicial.

---

## DEC-006 - Gemini como ferramenta complementar

Data: 2026-10-03
Status: Aceita

Contexto:

O Gemini faz parte das ferramentas disponiveis, mas nao precisa duplicar funcoes executadas por outros agentes.

Decisao:

Utilizar Gemini quando apresentar vantagem concreta.

Casos principais:

- pesquisa;
- grandes contextos;
- revisao;
- documentacao;
- planejamento;
- exploracao de alternativas;
- integracao com o ecossistema Google.

Impacto:

Gemini nao sera obrigatorio em todas as etapas.

---

## DEC-007 - Uma etapa pratica por vez

Data: 2026-10-03
Status: Aceita

Contexto:

O projeto tambem possui finalidade educacional e o excesso de configuracoes simultaneas aumenta complexidade e risco de erro.

Decisao:

Executar a construcao pratica do workflow uma etapa por vez.

Cada passo deve apresentar:

1. objetivo;
2. ferramenta ou terminal;
3. comando ou acao exata;
4. resultado esperado;
5. verificacao.

Somente depois da confirmacao do resultado deve-se avancar.

Impacto:

Erros devem ser corrigidos antes da proxima etapa.

---

## DEC-008 - Prioridade para baixo custo

Data: 2026-10-03
Status: Aceita

Contexto:

O workflow deve ser profissional sem criar assinaturas desnecessarias.

Decisao:

Utilizar esta ordem de prioridade:

gratuito
-> incluido nas assinaturas atuais
-> open source
-> baixo custo
-> pago somente quando necessario

Impacto:

Toda nova ferramenta deve demonstrar beneficio concreto antes de ser adicionada.

---

## DEC-009 - Documentacao como memoria persistente

Data: 2026-10-04
Status: Aceita

Contexto:

Agentes diferentes precisam compreender e continuar projetos sem depender exclusivamente das conversas anteriores.

Decisao:

Manter no repositorio documentos estruturados como:

- README.md;
- PROJECT.md;
- REQUIREMENTS.md;
- ARCHITECTURE.md;
- TASKS.md;
- DECISIONS.md;
- AGENTS.md;
- CHANGELOG.md;
- .env.example.

Motivo:

O proprio repositorio deve funcionar como memoria persistente do projeto.

Impacto:

Mudancas relevantes devem atualizar a documentacao correspondente.

---

## DEC-010 - Automacao somente depois do fluxo manual

Data: 2026-10-04
Status: Aceita

Contexto:

Automatizar um processo ainda nao validado pode esconder problemas e aumentar a complexidade.

Decisao:

Primeiro executar e validar manualmente os processos essenciais.

Depois automatizar tarefas repetitivas.

Ordem desejada:

1. processo manual;
2. documentacao;
3. identificacao de repeticao;
4. automacao;
5. integracao;
6. orquestracao de agentes.

Impacto:

Automacoes nao devem ser adicionadas apenas porque sao tecnicamente possiveis.
