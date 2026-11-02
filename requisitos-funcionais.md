# Requisitos funcionais

**Projeto:** Plataforma de Gestão do Conhecimento e Aprendizagem ENADE — Engenharia da Computação  
**Versão:** 0.1 — 01/11/2026  
**Situação:** proposta inicial, pendente de elicitação e validação.  
**Elaboração:** grupo do projeto; identificação nominal a preencher.

Os itens deste documento foram derivados da [Visão da Demanda](visao-demanda-enade-computacao.md), versão 0.1. Não são resultados de entrevistas. O detalhamento representa uma proposta da equipe a revisar com os [stakeholders](stakeholders.md), usando o [roteiro de entrevistas](roteiro-entrevistas.md). A alternativa de Google Forms permanece em consideração, sem alteração do método de coleta até a consulta ao professor.

As fontes SRC-01 a SRC-04, necessidades NEC-01 a NEC-08, funcionalidades F-01 a F-11 e atores AT-01 a AT-04 são os identificadores da visão. Requisitos candidatos não devem ser tratados como aprovados. Prioridades são sugestões, não decisões institucionais. Os critérios descrevem como verificar uma implementação futura; não indicam testes executados ou software entregue na Sprint 1.

## 1. Convenções

RF identifica um comportamento esperado. Cada item aponta para a funcionalidade e a necessidade da visão, além das [regras de negócio](regras-negocio.md) aplicáveis. Os [requisitos não funcionais](requisitos-nao-funcionais.md) complementam os critérios de qualidade.

## 2. Catálogo preliminar

### RF-01 — Autenticar usuários

- **Atores:** AT-01, AT-02, AT-03, AT-04.
- **Rastreabilidade:** F-01; NEC-07; SRC-02.
- **Prioridade proposta:** Essencial.
- **Requisito:** O sistema deve autenticar o usuário antes de permitir operações restritas e permitir que ele encerre sua sessão.
- **Critério de aceitação proposto:** Com credenciais válidas, o usuário acessa as operações permitidas ao seu perfil; com credenciais inválidas, o acesso é recusado. Após sair, uma operação restrita exige nova autenticação.
- **Regras relacionadas:** RN-01.
- **A confirmar:** Forma de cadastro, recuperação de acesso, provedor de autenticação e eventual acesso público à biblioteca a definir.

### RF-02 — Gerenciar perfis e contas

- **Atores:** AT-04.
- **Rastreabilidade:** F-01; NEC-07; SRC-02.
- **Prioridade proposta:** Essencial.
- **Requisito:** O sistema deve permitir ao administrador autorizado atribuir e remover perfis e ativar ou desativar contas.
- **Critério de aceitação proposto:** Uma conta desativada não pode executar operações restritas, inclusive por sessão existente; um perfil removido deixa de permitir suas operações.
- **Regras relacionadas:** RN-01.
- **A confirmar:** Quem autoriza a criação de contas e a atribuição dos perfis a confirmar.

### RF-03 — Consultar a biblioteca

- **Atores:** AT-01, AT-02.
- **Rastreabilidade:** F-02; NEC-01; SRC-01, SRC-04.
- **Prioridade proposta:** Essencial.
- **Requisito:** O sistema deve permitir buscar materiais publicados por texto e filtrar por tema, competência e disciplina.
- **Critério de aceitação proposto:** A combinação de filtros retorna apenas materiais que atendam aos critérios informados. Se não houver resultados, o sistema informa isso e permite ajustar os filtros.
- **Regras relacionadas:** RN-02, RN-03.
- **A confirmar:** Campos abrangidos pela busca textual e classificação inicial a validar.

### RF-04 — Consultar um material

- **Atores:** AT-01, AT-02.
- **Rastreabilidade:** F-02; NEC-01; SRC-04.
- **Prioridade proposta:** Essencial.
- **Requisito:** O sistema deve apresentar título, descrição, formato, origem, classificação e data de revisão do material, permitindo abrir seu arquivo ou link.
- **Critério de aceitação proposto:** Ao selecionar um material publicado, os metadados e o recurso correspondente ficam acessíveis conforme a permissão do usuário. Materiais retirados não aparecem na consulta comum.
- **Regras relacionadas:** RN-03, RN-04.
- **A confirmar:** Formatos aceitos, limites dos arquivos e tratamento de links indisponíveis a definir.

### RF-05 — Gerenciar materiais do acervo

- **Atores:** AT-02.
- **Rastreabilidade:** F-03; NEC-01, NEC-06; SRC-01, SRC-04.
- **Prioridade proposta:** Essencial.
- **Requisito:** O sistema deve permitir cadastrar e editar rascunhos de materiais, submetê-los à revisão, publicá-los após aprovação e retirá-los de circulação.
- **Critério de aceitação proposto:** Um rascunho não aparece na biblioteca pública aos usuários de estudo; a publicação exige os dados e a aprovação previstos; a retirada preserva o registro de origem.
- **Regras relacionadas:** RN-03, RN-04.
- **A confirmar:** Quem revisa e se autor e revisor podem ser a mesma pessoa a confirmar.

### RF-06 — Gerenciar questões

- **Atores:** AT-02.
- **Rastreabilidade:** F-04; NEC-02, NEC-06; SRC-01, SRC-02.
- **Prioridade proposta:** Essencial.
- **Requisito:** O sistema deve permitir cadastrar, editar, revisar, publicar e retirar questões objetivas, com enunciado, alternativas, gabarito, comentário, origem, ano, componente e classificação.
- **Critério de aceitação proposto:** Questões incompletas podem permanecer em rascunho, mas não podem ser publicadas. Uma questão publicada apresenta gabarito e comentário revisados e sua referência de origem.
- **Regras relacionadas:** RN-02, RN-03, RN-05.
- **A confirmar:** Tratamento de figuras e fórmulas e correção de erros após uso a detalhar.

### RF-07 — Associar conteúdos ao currículo

- **Atores:** AT-02, AT-03.
- **Rastreabilidade:** F-05; NEC-04; SRC-01.
- **Prioridade proposta:** Importante.
- **Requisito:** O sistema deve permitir associar questões e materiais a temas, competências e disciplinas da grade adotada.
- **Critério de aceitação proposto:** As associações salvas podem ser consultadas nos itens correspondentes e utilizadas nos filtros. Itens podem ter múltiplas associações quando aprovadas pedagogicamente.
- **Regras relacionadas:** RN-02, RN-06.
- **A confirmar:** Grade, vocabulário de classificação e responsável por mantê-los a confirmar.

### RF-08 — Montar simulados

- **Atores:** AT-02.
- **Rastreabilidade:** F-06; NEC-02; SRC-01, SRC-02.
- **Prioridade proposta:** Essencial.
- **Requisito:** O sistema deve permitir selecionar questões publicadas, definir título, público participante e duração e publicar um simulado.
- **Critério de aceitação proposto:** Um simulado sem questões ou sem configurações obrigatórias não é publicado. Após publicação, os estudantes autorizados conseguem localizá-lo.
- **Regras relacionadas:** RN-05, RN-07.
- **A confirmar:** Critérios de público, período de aplicação, limite de tentativas e adaptações de tempo a validar.

### RF-09 — Realizar simulados

- **Atores:** AT-01.
- **Rastreabilidade:** F-07; NEC-02; SRC-01, SRC-02.
- **Prioridade proposta:** Essencial.
- **Requisito:** O sistema deve permitir iniciar uma tentativa autorizada, navegar entre questões, registrar e alterar respostas durante a tentativa e consultar o tempo restante.
- **Critério de aceitação proposto:** Respostas confirmadas como salvas permanecem associadas à tentativa. O usuário não consegue responder em nome de outro estudante nem iniciar tentativa sem autorização.
- **Regras relacionadas:** RN-01, RN-07, RN-08.
- **A confirmar:** Retomada após interrupção e frequência de salvamento a detalhar.

### RF-10 — Finalizar e corrigir tentativas

- **Atores:** AT-01; encerramento automático pelo sistema.
- **Rastreabilidade:** F-07; NEC-02; SRC-02.
- **Prioridade proposta:** Essencial.
- **Requisito:** O sistema deve encerrar a tentativa por envio confirmado do estudante ou término do tempo e corrigir as respostas objetivas com o gabarito da versão aplicada.
- **Critério de aceitação proposto:** A tentativa encerrada não aceita novas respostas. Reenvio do mesmo encerramento não cria outra tentativa. O resultado respeita o tratamento de itens não respondidos e anulados.
- **Regras relacionadas:** RN-08, RN-09, RN-10.
- **A confirmar:** Regras propostas de cálculo, anulação e término de tempo precisam de revisão pedagógica.

### RF-11 — Consultar gabarito comentado

- **Atores:** AT-01.
- **Rastreabilidade:** F-07; NEC-02; SRC-02.
- **Prioridade proposta:** Essencial.
- **Requisito:** O sistema deve permitir ao estudante consultar sua resposta, o gabarito e o comentário de cada questão após a liberação prevista para a avaliação.
- **Critério de aceitação proposto:** Antes da liberação, o gabarito não fica acessível; depois dela, o estudante consulta os dados da versão de questão utilizada na tentativa.
- **Regras relacionadas:** RN-05, RN-07.
- **A confirmar:** Momento da liberação: imediatamente após a tentativa ou após encerramento da aplicação; a definir.

### RF-12 — Consultar desempenho individual

- **Atores:** AT-01, AT-02 quando autorizado.
- **Rastreabilidade:** F-08; NEC-03; SRC-01, SRC-02.
- **Prioridade proposta:** Essencial.
- **Requisito:** O sistema deve apresentar histórico de tentativas e desempenho por tema, com período, quantidade de questões válidas, acertos e percentual correspondente.
- **Critério de aceitação proposto:** O percentual pode ser reproduzido a partir dos dados exibidos. Ausência de questões válidas aparece como sem dados, e não como zero por cento. Acesso a resultado de outra pessoa exige autorização.
- **Regras relacionadas:** RN-01, RN-09, RN-10.
- **A confirmar:** Suficiência de evidências para indicar dificuldade e comparação entre tentativas a validar.

### RF-13 — Consultar resultados consolidados

- **Atores:** AT-02, AT-03.
- **Rastreabilidade:** F-08; NEC-03; SRC-01.
- **Prioridade proposta:** Essencial.
- **Requisito:** O sistema deve permitir consultar resultados agrupados por tema e simulado no conjunto de participantes autorizado, exibindo período e quantidade de participantes e respostas considerados.
- **Critério de aceitação proposto:** Os filtros alteram o conjunto analisado de forma explícita; resultados individuais não são expostos a perfis com permissão apenas de consolidação. A agregação segue fórmula documentada.
- **Regras relacionadas:** RN-01, RN-09, RN-10.
- **A confirmar:** Definição de turmas/grupos, proteção de grupos pequenos e necessidade de exportação a investigar.

### RF-14 — Indicar e consultar reforço

- **Atores:** AT-02, AT-01.
- **Rastreabilidade:** F-09; NEC-05; SRC-01, SRC-04.
- **Prioridade proposta:** Importante.
- **Requisito:** O sistema deve permitir ao professor autorizado indicar material publicado ou atividade de reforço a estudantes sob seu acompanhamento, informando tema e orientação; o estudante deve poder consultar suas indicações.
- **Critério de aceitação proposto:** O destinatário encontra a orientação e o material relacionado. Um usuário sem autorização não consegue indicar reforço a estudantes fora de seu acompanhamento.
- **Regras relacionadas:** RN-01, RN-11.
- **A confirmar:** Formas de atividade e acompanhamento da conclusão a validar; recomendação automática não é presumida.

### RF-15 — Importar prova em PDF com revisão

- **Atores:** AT-02.
- **Rastreabilidade:** F-10; NEC-06; SRC-01.
- **Prioridade proposta:** Desejável — em avaliação.
- **Requisito:** O sistema deve permitir enviar PDF e apresentar as questões extraídas como rascunhos editáveis, com referência à origem e sinalização de falhas detectadas.
- **Critério de aceitação proposto:** A extração não publica questões automaticamente. O revisor pode comparar com a prova de origem, corrigir ou descartar itens. Falha na extração não é apresentada como importação concluída com sucesso.
- **Regras relacionadas:** RN-03, RN-05, RN-12.
- **A confirmar:** Suporte a PDFs digitalizados, OCR, imagens, fórmulas, gabaritos e duplicatas depende de estudo de viabilidade.

### RF-16 — Consultar frequência histórica de temas

- **Atores:** AT-01, AT-02.
- **Rastreabilidade:** F-11; NEC-08; SRC-04.
- **Prioridade proposta:** Desejável — em avaliação.
- **Requisito:** O sistema deve apresentar frequência de temas nas provas cadastradas e revisadas, identificando curso, anos, provas e método de contagem.
- **Critério de aceitação proposto:** O usuário consegue identificar o conjunto usado no cálculo. Dados insuficientes ou inexistentes são informados. A apresentação esclarece que os números descrevem provas anteriores.
- **Regras relacionadas:** RN-13.
- **A confirmar:** Conjunto de provas e método para questões com múltiplos temas a validar.

### RF-17 — Praticar questões individualmente

- **Atores:** AT-01.
- **Rastreabilidade:** F-07; NEC-02; SRC-01, SRC-02.
- **Prioridade proposta:** Essencial.
- **Requisito:** O sistema deve permitir ao estudante selecionar questões publicadas por tema, registrar uma resposta e consultar o gabarito comentado após responder.
- **Critério de aceitação proposto:** A resposta escolhida é comparada com o gabarito e o comentário fica disponível. A prática não é confundida com uma tentativa de simulado nos indicadores.
- **Regras relacionadas:** RN-02, RN-05, RN-14.
- **A confirmar:** Inclusão da prática no histórico e política de repetição a confirmar.

## 3. Validação e encaminhamento

Revisar com estudantes os fluxos de consulta, prática e resultados; com professores, as avaliações, o acervo e o reforço; com coordenação e responsáveis institucionais, as permissões e os indicadores. Registrar para cada alteração a fonte de entrevista, decisão e justificativa. Nenhum item foi validado nesta versão.

O backlog e os diagramas deverão referenciar estes IDs após a revisão. Os casos de uso reservados na visão podem detalhar vários RF associados à mesma funcionalidade.

| Data | Versão | Alteração | Responsável |
| --- | --- | --- | --- |
| 01/11/2026 | 0.1 | Especificação preliminar de 17 requisitos funcionais | Grupo — nomes a preencher |
