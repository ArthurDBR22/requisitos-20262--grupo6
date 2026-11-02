# Backlog priorizado

**Projeto:** Plataforma de Gestão do Conhecimento e Aprendizagem ENADE — Engenharia da Computação  
**Identificador:** BL-ENADE-01  
**Versão:** 0.2 — 01/11/2026  
**Situação:** proposta inicial de priorização, pendente de revisão do grupo e validação com interessados.  
**Responsável:** grupo do projeto — nomes a definir.

## 1. Objetivo e referências

Organizar as capacidades propostas para o produto e as tarefas necessárias à entrega acadêmica da Sprint 1, Milestone M1, de 20/10 a 02/11/2026. O produto é conceitual nesta etapa; a Sprint 1 não exige implementar estas funcionalidades.

Referências utilizadas:

- [Visão da Demanda](visao-demanda-enade-computacao.md), versão 0.1.
- [Stakeholders](stakeholders.md), versão 0.1.
- [Roteiro de entrevistas](roteiro-entrevistas.md), versão 0.2.
- [Requisitos funcionais](requisitos-funcionais.md), versão 0.1.
- [Requisitos não funcionais](requisitos-nao-funcionais.md), versão 0.2.
- [Regras de negócio](regras-negocio.md), versão 0.2, incluindo os desdobramentos dos IDs originais.

Não foram fornecidos resultados de entrevistas, números de issues, endereço do repositório ou responsáveis nominais. Os IDs BP, BQ e M1 deste documento são identificadores locais propostos e não números de issues já criadas no GitHub.

## 2. Critério de priorização

A priorização considera contribuição ao objetivo de aprendizagem, dependências e incertezas de viabilidade. Mantém as categorias dos requisitos funcionais:

| Prioridade | Significado | Aplicação ao projeto |
| --- | --- | --- |
| Essencial | Necessária ao núcleo proposto | Conteúdo revisado, acesso, biblioteca, questões, simulados e resultados |
| Importante | Agrega valor; pode ter alternativa temporária delimitada | Relação curricular e orientação de reforço |
| Desejável | Pode ser adiada sem impedir o núcleo | Importação assistida e análise histórica de temas |

A ordem abaixo indica prioridade de refinamento e valor proposto, não uma sequência rígida de programação. Dependências podem exigir antecipar trabalho de um item de menor prioridade. Não foram estimados esforço, pontos ou datas de implementação: dependem da equipe, do escopo validado e da arquitetura.

**Dependência curricular:** a classificação mínima por tema deve ser definida junto com acervo e banco de questões. O detalhamento de competências e disciplinas de BP-10 é dependência dos filtros completos de BP-03 e das análises correspondentes. Se essa dependência se tornar impeditiva, o grupo deve antecipar BP-10 ou revisar explicitamente o recorte; não considerar completa uma funcionalidade com filtros previstos ainda ausentes.

## 3. Backlog do produto

Todos os itens BP estão em **proposta, não implementados e não validados**. A aceitação resumida abaixo complementa os critérios detalhados dos RF e deverá ser revisada após a elicitação.

| Ordem | ID | Item | Prioridade proposta | RF cobertos |
| --- | --- | --- | --- | --- |
| 1 | BP-01 | Controlar acesso e perfis | Essencial | RF-01, RF-02 |
| 2 | BP-02 | Organizar e revisar o acervo | Essencial | RF-05 |
| 3 | BP-03 | Consultar a biblioteca de conteúdos | Essencial | RF-03, RF-04 |
| 4 | BP-04 | Manter o banco de questões | Essencial | RF-06 |
| 5 | BP-05 | Praticar questões por tema | Essencial | RF-17 |
| 6 | BP-06 | Montar e publicar simulados | Essencial | RF-08 |
| 7 | BP-07 | Realizar, encerrar e corrigir simulados | Essencial | RF-09, RF-10, RF-11 |
| 8 | BP-08 | Acompanhar desempenho individual | Essencial | RF-12 |
| 9 | BP-09 | Consultar resultados consolidados | Essencial | RF-13 |
| 10 | BP-10 | Associar conteúdos ao currículo | Importante | RF-07 |
| 11 | BP-11 | Indicar e consultar reforço | Importante | RF-14 |
| 12 | BP-12 | Importar provas em PDF com revisão | Desejável — em avaliação | RF-15 |
| 13 | BP-13 | Consultar frequência histórica de temas | Desejável — em avaliação | RF-16 |

### Detalhamento dos itens

#### BP-01 — Controlar acesso e perfis

Como administrador, quero administrar contas e permissões para que cada usuário acesse somente suas operações e informações autorizadas.

- **Prioridade:** Essencial.
- **Justificativa:** É necessário controlar acesso aos dados antes de disponibilizar operações restritas.
- **Referências:** RF-01, RF-02; NEC-07; F-01.
- **Dependências:** Nenhuma funcional; depende da matriz de acesso.
- **Aceitação proposta:** Autenticação válida permite acesso conforme perfil; credenciais inválidas, conta desativada e perfil sem permissão têm acesso recusado, inclusive por acesso direto.
- **Regras relacionadas:** RN-01.
- **Pendências:** Cadastro, recuperação de acesso, atribuição de perfis e eventual consulta pública.

#### BP-02 — Organizar e revisar o acervo

Como professor, quero cadastrar, revisar e publicar materiais para oferecer conteúdos de estudo com origem identificada.

- **Prioridade:** Essencial.
- **Justificativa:** O acervo revisado fornece o conteúdo da biblioteca, proposta central do projeto.
- **Referências:** RF-05; NEC-01, NEC-06; F-03.
- **Dependências:** BP-01; classificação de BP-10 para associações curriculares.
- **Aceitação proposta:** Rascunhos permanecem indisponíveis para estudo; publicação exige revisão, origem e verificação das condições de uso; retirada impede novas consultas comuns ao item.
- **Regras relacionadas:** RN-02, RN-02.1, RN-03, RN-03.1, RN-04.
- **Pendências:** Responsável pela revisão, formatos, limites de arquivo e atualização.

#### BP-03 — Consultar a biblioteca de conteúdos

Como estudante, quero localizar e abrir materiais por tema, competência ou disciplina para organizar meus estudos.

- **Prioridade:** Essencial.
- **Justificativa:** Entrega acesso direto aos materiais que o estudante precisa encontrar.
- **Referências:** RF-03, RF-04; NEC-01; F-02.
- **Dependências:** BP-02; BP-10 para filtros curriculares completos; BP-01 conforme acesso definido.
- **Aceitação proposta:** Busca e filtros retornam itens publicados compatíveis; o usuário consulta metadados e abre o recurso; ausência de resultados é informada; itens retirados não aparecem na consulta comum.
- **Regras relacionadas:** RN-02, RN-03, RN-04, RN-06.
- **Pendências:** Campos de busca, organização pedagógica e tratamento de links indisponíveis.

#### BP-04 — Manter o banco de questões

Como professor, quero cadastrar e revisar questões com gabarito e comentário para disponibilizar prática e avaliações confiáveis.

- **Prioridade:** Essencial.
- **Justificativa:** O banco revisado sustenta a prática, os simulados e a análise por tema.
- **Referências:** RF-06; NEC-02, NEC-06; F-04.
- **Dependências:** BP-01; BP-10 para associações curriculares.
- **Aceitação proposta:** Questão incompleta permanece em rascunho; publicação exige os elementos obrigatórios e revisão; versões usadas em tentativas concluídas permanecem identificáveis.
- **Regras relacionadas:** RN-02, RN-02.1, RN-03, RN-03.1, RN-05, RN-05.1.
- **Pendências:** Imagens, fórmulas, correções posteriores e classificação inicial.

#### BP-05 — Praticar questões por tema

Como estudante, quero responder questões e consultar comentários para entender meus erros durante o estudo.

- **Prioridade:** Essencial.
- **Justificativa:** Permite prática individual antes de depender de uma avaliação montada por professor.
- **Referências:** RF-17; NEC-02; F-07.
- **Dependências:** BP-04; BP-01 conforme permissão de prática.
- **Aceitação proposta:** O estudante seleciona questão publicada, registra resposta e recebe comparação com o gabarito e comentário; a prática é distinguida de simulado nos registros.
- **Regras relacionadas:** RN-02, RN-05, RN-14.
- **Pendências:** Repetições e inclusão da prática no histórico.

#### BP-06 — Montar e publicar simulados

Como professor, quero selecionar questões e configurar simulados para avaliar conteúdos definidos.

- **Prioridade:** Essencial.
- **Justificativa:** Viabiliza avaliações organizadas e com condições explícitas de aplicação.
- **Referências:** RF-08; NEC-02; F-06.
- **Dependências:** BP-01, BP-04.
- **Aceitação proposta:** A publicação exige questões revisadas, público, duração e políticas de tentativas e liberação do gabarito; simulado incompleto não é publicado.
- **Regras relacionadas:** RN-05, RN-07, RN-07.1.
- **Pendências:** Público participante, janela de aplicação, adaptações de tempo e políticas de tentativas.

#### BP-07 — Realizar, encerrar e corrigir simulados

Como estudante, quero responder um simulado e consultar sua correção quando liberada para compreender meu resultado.

- **Prioridade:** Essencial.
- **Justificativa:** Produz as respostas e os resultados necessários ao acompanhamento da aprendizagem.
- **Referências:** RF-09, RF-10, RF-11; NEC-02; F-07.
- **Dependências:** BP-01, BP-06.
- **Aceitação proposta:** Respostas confirmadas persistem; envio ou término de tempo encerra a tentativa uma única vez; respostas ficam bloqueadas após encerramento; correção usa a versão aplicada e gabarito só é exibido quando liberado.
- **Regras relacionadas:** RN-07, RN-07.1, RN-08, RN-08.1, RN-09, RN-09.1, RN-09.2, RN-05.1.
- **Pendências:** Interrupção, retomada, cálculo, anulação e momento de liberação. Item amplo: dividir em tarefas menores antes de implementação.

#### BP-08 — Acompanhar desempenho individual

Como estudante, quero consultar meu histórico e resultados por tema para identificar o que precisa de revisão.

- **Prioridade:** Essencial.
- **Justificativa:** Atende diretamente ao objetivo de identificar dificuldades a partir das avaliações.
- **Referências:** RF-12; NEC-03; F-08.
- **Dependências:** BP-07; BP-10 para classificação; BP-01.
- **Aceitação proposta:** O relatório informa período, itens válidos, acertos e percentual reproduzível; ausência de dados não vira zero por cento; acesso individual respeita autorização; diagnósticos dependem de critérios aprovados.
- **Regras relacionadas:** RN-01, RN-09, RN-09.1, RN-09.2, RN-10, RN-10.1, RN-10.2.
- **Pendências:** Quantidade suficiente de questões, comparação de tentativas e limites da interpretação.

#### BP-09 — Consultar resultados consolidados

Como professor ou coordenador, quero consultar resultados do conjunto autorizado de estudantes para planejar ações pedagógicas.

- **Prioridade:** Essencial.
- **Justificativa:** Apoia decisões pedagógicas para grupos de estudantes e para o curso.
- **Referências:** RF-13; NEC-03; F-08.
- **Dependências:** BP-01, BP-07; BP-10 para análise por tema.
- **Aceitação proposta:** O relatório identifica período, participantes e respostas considerados; consolidação segue a fórmula documentada; quem tem acesso apenas consolidado não visualiza resultados individuais.
- **Regras relacionadas:** RN-01, RN-09.3, RN-10, RN-10.1, RN-10.2.
- **Pendências:** Grupos, tentativas consideradas, grupos pequenos e necessidade de exportação.

#### BP-10 — Associar conteúdos ao currículo

Como professor ou coordenador, quero relacionar questões e materiais a temas, competências e disciplinas para manter coerência com a formação do curso.

- **Prioridade:** Importante.
- **Justificativa:** Fortalece a organização dos conteúdos e viabiliza os filtros e análises curriculares previstos.
- **Referências:** RF-07; NEC-04; F-05.
- **Dependências:** Referências curriculares; BP-02 e BP-04 fornecem os itens a associar.
- **Aceitação proposta:** As associações utilizam grade e referências aprovadas, permitem múltiplos temas pertinentes e ficam disponíveis nos filtros e itens correspondentes.
- **Regras relacionadas:** RN-02.1, RN-06, RN-06.1.
- **Pendências:** Grade, vocabulário e responsável por manter as classificações. Deve ser antecipado quando bloquear um item essencial.

#### BP-11 — Indicar e consultar reforço

Como professor, quero indicar materiais ou atividades por tema; como estudante, quero consultar essas orientações para revisar dificuldades identificadas.

- **Prioridade:** Importante.
- **Justificativa:** Conecta a análise dos resultados a ações de estudo orientadas.
- **Referências:** RF-14; NEC-05; F-09.
- **Dependências:** BP-01, BP-02, BP-03; resultados de BP-08 ou BP-09 apoiam a indicação.
- **Aceitação proposta:** Professor autorizado identifica destinatário, tema e orientação; o estudante consulta suas indicações e materiais publicados relacionados; usuários não autorizados não indicam reforço fora de seu acompanhamento.
- **Regras relacionadas:** RN-01, RN-11.
- **Pendências:** Tipos de atividade e acompanhamento da conclusão. Não pressupõe recomendação automática.

#### BP-12 — Importar provas em PDF com revisão

Como professor, quero aproveitar questões extraídas de provas para reduzir trabalho de cadastro, mantendo conferência pedagógica.

- **Prioridade:** Desejável — em avaliação.
- **Justificativa:** Pode reduzir trabalho manual, mas o cadastro manual permite iniciar o banco sem essa automação.
- **Referências:** RF-15; NEC-06; F-10.
- **Dependências:** BP-04; estudo de extração em amostras.
- **Aceitação proposta:** Importação gera rascunhos com origem, permite corrigir ou descartar itens e não publica automaticamente; falhas são informadas; itens são conferidos com a prova.
- **Regras relacionadas:** RN-03, RN-05, RN-12.
- **Pendências:** OCR, imagens, fórmulas, gabaritos, duplicatas e viabilidade da extração.

#### BP-13 — Consultar frequência histórica de temas

Como estudante ou professor, quero conhecer a distribuição dos temas em provas anteriores para contextualizar os estudos.

- **Prioridade:** Desejável — em avaliação.
- **Justificativa:** Complementa o estudo, mas depende de dados revisados e de método que ainda não foi definido.
- **Referências:** RF-16; NEC-08; F-11.
- **Dependências:** BP-04, BP-10; conjunto documental e método de contagem.
- **Aceitação proposta:** A análise identifica curso, provas, anos, unidade e método de contagem; dados insuficientes são informados; frequência histórica não é apresentada como previsão.
- **Regras relacionadas:** RN-13.
- **Pendências:** Provas analisadas, denominador e tratamento de questões com múltiplos temas e anulações.

## 4. Qualidade e trabalhos de definição

Os RNF são condições transversais dos itens BP, não melhorias a deixar automaticamente para o fim. A prioridade de resolver suas lacunas é alta porque afeta a especificação e a modelagem. Todos os itens BQ estão **pendentes de refinamento e validação**.

| ID | Trabalho e prioridade de definição | RNF relacionados | Itens afetados | Evidência para concluir a definição |
| --- | --- | --- | --- | --- |
| BQ-01 | Definir permissões, proteção de acesso e finalidade dos dados — alta | RNF-01, RNF-02, RNF-10 | BP-01 e todo item com dados pessoais ou operação restrita | Matriz de acesso, mecanismo proposto, campos/finalidades e condições de retenção revisados com responsáveis |
| BQ-02 | Definir e avaliar experiência de uso e acessibilidade — alta | RNF-03, RNF-04, RNF-05 | BP-03, BP-05, BP-07, BP-08, BP-09, BP-11 e demais telas | Tarefas de uso, critérios de teclado e apresentação, dispositivos e navegadores identificados; metas justificadas |
| BQ-03 | Definir integridade das tentativas e histórico de conteúdo — alta | RNF-06, RNF-07 | BP-02, BP-04, BP-06, BP-07, BP-08, BP-09 | Política de salvamento, encerramento único, versões e correções documentada e revisada |
| BQ-04 | Levantar carga, disponibilidade e recuperação — alta | RNF-08, RNF-09 | Busca, aplicação de simulados e ambiente de operação | Carga, volumes, tempos, janela de operação e recuperação definidos com fonte; sem valores pendentes apresentados como aprovados |

Outras categorias do template RNF permanecem em levantamento conforme o documento correspondente. Na aceitação futura de cada item, aplicar os RNF pertinentes já especificados e resolver as lacunas que impeçam verificar o resultado. Nenhum teste de software foi executado nesta fase documental.

## 5. Backlog de trabalho da Sprint 1 — M1

Esta tabela acompanha a documentação obrigatória. Todos os responsáveis nominais e links de issues estão **a definir pelo grupo**. O prazo da atividade é **02/11/2026**; a ordem é sugerida e admite elaboração paralela de rascunhos, seguida de revisão baseada nas evidências coletadas.

| Ordem | ID local | Tarefa | Prioridade | Entrega e critério de conclusão | Situação registrada |
| --- | --- | --- | --- | --- | --- |
| 1 | M1-01 | Confirmar representantes e responsabilidades | Alta | Cadastro de stakeholders com participantes disponíveis e responsáveis designados | Rascunho existente; nomes e participação pendentes |
| 2 | M1-02 | Revisar roteiro e esclarecer o método com o professor | Alta | Roteiro revisado e decisão registrada sobre formato de coleta; Forms somente se aceito | Roteiro 0.2 preparado; decisão sobre Forms pendente |
| 3 | M1-03 | Realizar e registrar entrevistas | Alta | Registros reais com participantes, datas, perguntas, respostas e limitações | Pendente; nenhuma resposta fornecida |
| 4 | M1-04 | Consolidar resultados e revisar necessidades | Alta | Síntese com referência às entrevistas, divergências e decisões; arquivo de resultados produzido | Pendente; depende de M1-03 |
| 5 | M1-05 | Revisar o Documento de Visão | Alta | Visão no template, fontes e escopo consistentes, representantes e pendências registrados; validação documentada no limite do que ocorreu | Versão 0.1 em rascunho |
| 6 | M1-06 | Refinar RF, RNF e regras de negócio | Alta | IDs, critérios verificáveis, fontes e pendências revisados; templates RN e RNF respeitados | RF 0.1, RNF 0.2 e RN 0.2 em rascunho |
| 7 | M1-07 | Revisar e priorizar o backlog | Alta | Todos os RF e RNF cobertos; prioridades justificadas e revisão do grupo registrada | Este documento preparado; revisão e validação pendentes |
| 8 | M1-08 | Elaborar diagrama de Casos de Uso | Alta | Atores e objetivos coerentes com RF e visão; imagem/diagrama legível e referência aos requisitos | [Rascunho 0.1 elaborado](casos-uso.md); revisão e validação pendentes |
| 9 | M1-09 | Elaborar diagrama de Componentes | Alta | Responsabilidades e dependências dos componentes propostas e relacionadas aos requisitos; decisões ainda hipotéticas identificadas | [Rascunho 0.1 elaborado](componentes.md); revisão e validação pendentes |
| 10 | M1-10 | Elaborar diagrama de Implantação | Alta | Nós, ambientes e distribuição dos componentes representados, coerentes com a arquitetura proposta; nenhuma hospedagem presumida como contratada | [Rascunho 0.1 elaborado](implantacao.md); revisão e validação pendentes |
| 11 | M1-11 | Revisar e organizar a entrega no GitHub | Alta | Arquivos revisados, links funcionais, diagramas legíveis e vínculos às issues reais de M1; envio conforme orientação do professor | Pacote e README preparados; revisão do grupo e envio pendentes; repositório e issues não fornecidos |

Dependências principais: M1-03 requer participantes e roteiro; M1-04 depende da coleta. Rascunhos de M1-05 a M1-10 podem avançar, mas precisam ser confrontados com os resultados. O diagrama de Implantação deve corresponder aos componentes definidos em M1-09. M1-11 requer conferência de todos os entregáveis e exposição transparente das pendências.

A existência de um arquivo não significa que o entregável foi validado. Os três diagramas têm rascunhos elaborados, ainda pendentes de validação. As entrevistas e seus resultados continuam pendentes.

## 6. Uso como base para issues

Para cada tarefa M1 ou item de produto escolhido pelo grupo, criar uma issue com:

- Título iniciado pelo ID local e nome do item.
- Objetivo e entregável esperado.
- Referências aos documentos e requisitos relacionados.
- Critérios de conclusão ou aceitação.
- Dependências e dúvidas abertas.
- Responsável, prioridade, situação e milestone apropriados.

Na Sprint 1, vincular a M1 as tarefas de elicitação e modelagem efetivamente atribuídas pelo professor. Os BP descrevem o produto e não devem ser assumidos como compromissos de implementação nessa sprint. Quando as issues reais forem fornecidas, registrar seus números e links neste documento, sem renumerar artificialmente o material do professor.

## 7. Critérios para revisão e conclusão

**Para refinar um item de produto:** esclarecer usuário, resultado esperado, fonte, regras aplicáveis, dependências e critérios verificáveis. Registrar estimativa somente quando a equipe tiver base para fazê-la.

**Para concluir uma tarefa documental:** produzir o artefato, conferir consistência com as fontes e demais documentos, revisar no grupo e registrar validações e pendências reais. Aprovação acadêmica ou institucional só pode ser indicada quando obtida.

**Para eventual implementação futura:** cumprir os critérios do item e os RF, RN e RNF aplicáveis, com evidências de verificação. Nada neste backlog declara software concluído.

## 8. Limites e decisões pendentes

- Entrevistas e validação das prioridades ainda não foram realizadas.
- Critérios de cálculo e diagnóstico, matriz de acesso e parâmetros de qualidade precisam ser confirmados.
- Biblioteca e acervo fazem parte do escopo; ranking de temas e importação de PDF continuam em avaliação.
- O recorte permanece Engenharia da Computação, incluindo formação geral pertinente.
- Outros cursos, gestão administrativa de inscrições no ENADE e correção automática de discursivas não entram na proposta inicial.
- Integrações institucionais dependem de investigação; o fórum permanece fora da proposta atual, sujeito ao esclarecimento já registrado na visão.
- Campos pessoais dos participantes e respostas de entrevistas devem ser tratados conforme o procedimento de registro previsto no roteiro, antes de inclusão em repositório público.

## 9. Histórico e registro de revisão

| Data | Versão | Alteração | Autor |
| --- | --- | --- | --- |
| 01/11/2026 | 0.1 | Backlog inicial: 13 itens de produto, 4 trabalhos de qualidade e 11 tarefas documentais de M1 | Grupo — nomes a preencher |
| 01/11/2026 | 0.2 | Atualização dos três diagramas para rascunhos elaborados e organização do pacote | Grupo — nomes a preencher |

| Versão revisada | Responsável | Data | Decisões e justificativas |
| --- | --- | --- | --- |
| A preencher | A definir | Não realizada | Nenhuma validação de prioridades registrada |
