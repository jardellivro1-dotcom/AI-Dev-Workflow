# AGENTS - AI Dev Workflow

## Objetivo

Definir regras de trabalho para agentes de Inteligencia Artificial que atuem neste repositorio.

Todo agente deve ler os documentos principais antes de realizar alteracoes relevantes.

## Ordem de leitura recomendada

Antes de implementar ou modificar o projeto, consultar:

1. PROJECT.md
2. REQUIREMENTS.md
3. ARCHITECTURE.md
4. TASKS.md
5. DECISIONS.md
6. AGENTS.md

Quando existirem, consultar tambem:

- README.md
- CHANGELOG.md
- SECURITY.md
- TESTING.md
- DATABASE.md
- API.md
- DEPLOYMENT.md
- DESIGN_SYSTEM.md

## Fonte de verdade

O repositorio e sua documentacao constituem a memoria persistente do projeto.

Nao assumir que o historico de conversas esta disponivel.

Quando uma decisao importante for tomada, ela deve ser refletida nos arquivos apropriados.

## Regra principal de execucao

Nao tentar implementar grandes partes do sistema de uma unica vez.

Preferir tarefas:

- pequenas;
- claras;
- testaveis;
- reversiveis;
- documentadas.

Exemplo inadequado:

Crie todo o sistema.

Exemplo adequado:

Implemente apenas o formulario de cadastro de clientes conforme os requisitos definidos.

## Antes de modificar codigo

O agente deve:

1. compreender a tarefa;
2. consultar requisitos relacionados;
3. verificar a arquitetura;
4. identificar arquivos afetados;
5. verificar riscos;
6. planejar uma alteracao pequena.

## Durante a implementacao

O agente deve:

- alterar somente o necessario;
- evitar mudancas nao solicitadas;
- preservar funcionalidades existentes;
- seguir os padroes do projeto;
- utilizar nomes claros;
- evitar duplicacao de codigo;
- tratar erros;
- validar entradas;
- manter seguranca;
- nao inserir credenciais.

## Depois da implementacao

O agente deve, conforme aplicavel:

1. executar testes;
2. executar lint;
3. executar build;
4. verificar erros;
5. revisar o diff;
6. atualizar documentacao;
7. informar o que foi alterado;
8. informar como validar.

## Seguranca

Nunca inserir diretamente no codigo ou documentacao:

- senhas;
- tokens;
- chaves de API;
- secrets;
- credenciais de banco;
- dados pessoais sensiveis desnecessarios.

Utilizar variaveis de ambiente.

O arquivo .env nao deve ser versionado.

## Git

Alteracoes devem ser pequenas e organizadas.

Preferir um objetivo principal por commit.

Padroes recomendados:

feat: nova funcionalidade
fix: correcao de erro
docs: documentacao
test: testes
refactor: refatoracao
chore: configuracao ou manutencao
ci: integracao continua

Nao executar alteracoes destrutivas no historico Git sem autorizacao explicita.

## Revisao

Quando possivel, utilizar agentes diferentes para:

CONSTRUTOR
-> REVISOR
-> TESTE
-> CORRECAO

O agente revisor deve procurar:

- erros funcionais;
- regressao;
- falhas de seguranca;
- codigo desnecessariamente complexo;
- falta de testes;
- inconsistencias com os requisitos;
- inconsistencias com a arquitetura.

## Criterio de qualidade

Uma tarefa nao deve ser considerada concluida apenas porque o codigo foi escrito.

Quando aplicavel, deve:

- funcionar;
- passar nos testes;
- passar no build;
- respeitar requisitos;
- respeitar arquitetura;
- nao expor segredos;
- manter documentacao atualizada.

## Custos

Antes de adicionar novas ferramentas, bibliotecas, APIs ou servicos pagos, verificar se existe alternativa:

1. gratuita;
2. ja incluida nas assinaturas existentes;
3. open source;
4. de baixo custo.

Servicos pagos somente devem ser sugeridos quando houver beneficio concreto.

## Complexidade

Preferir a solucao mais simples que cumpra os requisitos adequadamente.

Nao adicionar:

- microsservicos;
- filas;
- containers;
- novas camadas;
- novas plataformas;
- novas dependencias;

sem necessidade real.

## Documentacao

Atualizar quando necessario:

PROJECT.md
REQUIREMENTS.md
ARCHITECTURE.md
TASKS.md
DECISIONS.md
CHANGELOG.md

## Tarefas

Antes de iniciar uma implementacao, verificar TASKS.md.

Depois de concluir e validar uma tarefa, atualizar seu status quando apropriado.

## Decisoes

Mudancas significativas de arquitetura, ferramenta, integracao ou processo devem ser registradas em DECISIONS.md.

## Principio final

O objetivo nao e produzir a maior quantidade de codigo.

O objetivo e produzir software funcional, seguro, compreensivel, testavel, documentado e facil de manter.
