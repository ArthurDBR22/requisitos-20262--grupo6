# Especificação de Requisitos Não Funcionais

***LAPIS***

**Projeto:** Plataforma de Gestão do Conhecimento e Aprendizagem ENADE — Engenharia da Computação  
**Versão:** 0.2 — 01/11/2026  
**Situação:** rascunho adaptado ao template; elicitação e validação pendentes.  
**Elaboração:** grupo do projeto — nomes a preencher.

Os conteúdos são propostas derivadas da [Visão da Demanda](visao-demanda-enade-computacao.md), não resultados de entrevistas nem decisões institucionais aprovadas. SRC, NEC, F, AT, STK e PQ mantêm os significados dos documentos existentes. Consultar os [stakeholders](stakeholders.md), o [roteiro de entrevistas](roteiro-entrevistas.md) e os [requisitos funcionais](requisitos-funcionais.md). A alternativa de Google Forms continua pendente de consulta ao professor.

**Modelo utilizado:** `template-requisitosNaoFuncionais.md`. Os IDs RNF-01 a RNF-10 foram preservados. Cada requisito é especificado uma única vez; outras categorias fazem referência a ele quando pertinente.

**Escopo:** biblioteca, acervo, questões, simulados e acompanhamento de aprendizagem de Engenharia da Computação. Acesso web é uma hipótese de solução a validar. Não há implementação, entrevistas concluídas ou conformidade normativa atestada.

**Leitura dos estados:** proposta = conteúdo a validar; incompleto = faltam parâmetros necessários à aceitação; a levantar = categoria pertinente sem requisito fechado; não se aplica ao escopo atual = exclusão justificada, passível de revisão se o escopo mudar. As verificações são planejadas, não executadas.

## Histórico de Versões

| Data | Versão | Descrição | Autor |
| --- | --- | --- | --- |
| 01/11/2026 | 0.1 | Proposta inicial de 10 requisitos de qualidade | Grupo — nomes a preencher |
| 01/11/2026 | 0.2 | Reorganização nas categorias LAPIS, referências cruzadas e registro das lacunas e aplicabilidade | Grupo — nomes a preencher |

## 1. Requisitos de Produto

Categorias e condições aplicáveis registradas nas subseções abaixo.

### 1.1. Eficiência de Desempenho

Categorias e condições aplicáveis registradas nas subseções abaixo.

#### 1.1.1. Comportamento temporal

**RNF-08 — Desempenho — incompleto**

- **Requisito proposto:** A busca de materiais e questões e o salvamento de respostas deverão atender a limites de tempo definidos sob uma carga de uso conhecida.
- **Verificação planejada:** Medir percentil de tempo de resposta e taxa de erros com carga, volume de dados e cenário acordados. Sem esses parâmetros, o requisito não está pronto para aceitação.
- **Rastreabilidade:** RF-03, RF-09; condições de qualidade da visão.
- **A confirmar:** Definir com STK-04: usuários simultâneos, quantidade de materiais e questões, limite de tempo e taxa de erros. Nenhum valor foi confirmado.

**Fonte:** detalhamento proposto pela equipe a partir da visão, seção 9; validação pelos responsáveis indicados ainda pendente.


#### 1.1.2. Capacidade

**A levantar:** usuários simultâneos, volume de questões e materiais e limites de arquivos com STK-04. São parâmetros do RNF-08, não limites já aprovados.

#### 1.1.3. Uso de recursos

**A levantar:** restrições de processamento, memória, armazenamento e tráfego no ambiente proposto. Consultar STK-04 antes de especificar limites.

### 1.2. Flexibilidade (portabilidade)

Categorias e condições aplicáveis registradas nas subseções abaixo.

#### 1.2.1. Escalabilidade

**A levantar:** necessidade de aumento de capacidade durante aplicações de simulados, a partir dos cenários de carga do RNF-08. Não há meta de escalabilidade confirmada.

#### 1.2.2. Adaptabilidade

**RNF-05 — Compatibilidade e adaptação de tela**

- **Requisito proposto:** As telas principais devem se adaptar aos dispositivos e navegadores definidos para o público, sem perda de controles ou informações necessárias às tarefas.
- **Verificação planejada:** Verificar busca, realização de simulado e consulta de resultados na matriz de dispositivos acordada; tabelas e enunciados devem continuar utilizáveis.
- **Rastreabilidade:** RF-03, RF-09, RF-12; condições de uso da visão.
- **A confirmar:** Hipótese inicial: acesso web em computador e celular. Navegadores, versões e dimensões mínimas a levantar com STK-01 e STK-04.

**Fonte:** detalhamento proposto pela equipe a partir da visão, seção 9; validação pelos responsáveis indicados ainda pendente.


#### 1.2.3. Instalabilidade

**A levantar:** ambiente de instalação e procedimentos de configuração. A Sprint 1 entrega modelagem, mas a futura solução ainda exige essa definição com STK-04.

#### 1.2.4. Substituibilidade

**Não se aplica ao escopo atual:** não foi decidida a substituição de uma plataforma existente. Reavaliar após investigar PreparaEdu e a plataforma da Unifor (PQ-06).

### 1.3. Confiabilidade

Categorias e condições aplicáveis registradas nas subseções abaixo.

#### 1.3.1. Maturidade

**A levantar:** cenários de falha, janela de observação e taxa tolerável de incidentes. O RNF-06 já especifica uma condição verificável de preservação de respostas, sem comprovar maturidade global.

#### 1.3.2. Disponibilidade

**RNF-09 — Disponibilidade e recuperação — incompleto**

- **Requisito proposto:** A solução deverá atender a condições de disponibilidade e recuperação compatíveis com a aplicação dos simulados e a preservação dos dados.
- **Verificação planejada:** Verificar disponibilidade no período acordado e executar restauração controlada, comparando perda de dados e tempo de recuperação aos limites definidos.
- **Rastreabilidade:** RF-08, RF-09, RF-10; condições de qualidade da visão.
- **A confirmar:** Definir janela de operação, disponibilidade-alvo, tolerância a perda, tempo de recuperação, cópias e responsáveis; depende de STK-02 e STK-04.

**Fonte:** detalhamento proposto pela equipe a partir da visão, seção 9; validação pelos responsáveis indicados ainda pendente.


#### 1.3.3. Tolerância a falhas

**RNF-06 — Integridade das respostas**

- **Requisito proposto:** Uma resposta confirmada como salva deve permanecer vinculada à tentativa após atualização da página. Repetições do mesmo pedido de encerramento não devem produzir tentativas ou resultados duplicados.
- **Verificação planejada:** Salvar uma resposta, recarregar e conferir o estado; repetir encerramento da mesma tentativa e verificar existência de um único resultado.
- **Rastreabilidade:** RF-09, RF-10; NEC-02.
- **A confirmar:** Comportamento de respostas ainda não salvas, reconexão e confirmação de entrega a detalhar com STK-01, STK-02 e STK-04.

**Fonte:** detalhamento proposto pela equipe a partir da visão, seção 9; validação pelos responsáveis indicados ainda pendente.


#### 1.3.4. Recuperabilidade

**Referência:** RNF-09, seção 1.3.2. Definir tempo máximo de recuperação, perda máxima tolerável de dados, frequência de cópias e evidência de restauração com STK-02 e STK-04. Esses valores continuam pendentes.

### 1.4. Segurança

Categorias e condições aplicáveis registradas nas subseções abaixo.

#### 1.4.1. Confidencialidade

**RNF-01 — Autorização**

- **Requisito proposto:** O sistema deve verificar permissões a cada operação restrita, inclusive quando acessada diretamente, e não apenas ocultar opções na interface.
- **Verificação planejada:** Tentar cada operação e acesso a registro com perfis permitidos e não permitidos; operações não autorizadas devem ser recusadas sem exposição do conteúdo.
- **Rastreabilidade:** RF-01, RF-02, RF-12, RF-13; NEC-07.
- **A confirmar:** Matriz de perfis e acesso a grupos a confirmar com STK-02, STK-03 e STK-04.

**Fonte:** detalhamento proposto pela equipe a partir da visão, seção 9; validação pelos responsáveis indicados ainda pendente.

**RNF-02 — Proteção de credenciais e comunicação**

- **Requisito proposto:** A solução deve proteger credenciais e dados de sessão contra exposição em páginas, mensagens e registros operacionais e proteger a comunicação autenticada por canal cifrado.
- **Verificação planejada:** Inspeção futura dos fluxos, configurações e registros deve verificar ausência de segredos expostos e proteção da comunicação.
- **Rastreabilidade:** RF-01; NEC-07.
- **A confirmar:** Mecanismo de autenticação e medidas técnicas detalhadas a especificar com STK-04.

**Fonte:** detalhamento proposto pela equipe a partir da visão, seção 9; validação pelos responsáveis indicados ainda pendente.


#### 1.4.2. Integridade

**RNF-07 — Rastreabilidade de conteúdo**

- **Requisito proposto:** Alterações de questões, materiais e gabaritos devem permitir identificar responsável, data e versão, preservando as referências usadas em avaliações concluídas.
- **Verificação planejada:** Consultar o histórico de uma alteração e verificar que uma tentativa anterior continua ligada à versão aplicada ou a uma correção explicitamente registrada.
- **Rastreabilidade:** RF-05, RF-06, RF-10; NEC-06.
- **A confirmar:** Retenção de histórico, acesso aos registros e tratamento de correções retroativas a definir.

**Fonte:** detalhamento proposto pela equipe a partir da visão, seção 9; validação pelos responsáveis indicados ainda pendente.

A preservação de respostas e a ausência de duplicação também são tratadas em RNF-06, seção 1.3.3.

#### 1.4.3. Não repúdio

**A levantar:** se o domínio exige evidência adicional para impedir contestação de ações. O histórico previsto no RNF-07 fornece rastreabilidade, mas não constitui, por si só, garantia de não repúdio.

#### 1.4.4. Autenticidade (autenticação)

**Referência:** RF-01 define autenticação e RNF-02 trata proteção das credenciais. Método de verificação de identidade, recuperação de acesso e gestão de sessão ainda serão definidos com STK-04.

#### 1.4.5. Resistência

**A levantar:** ameaças e controles específicos para autenticação, arquivos enviados e operações restritas. RNF-01 e RNF-02 cobrem parte da proteção; não equivalem a um conjunto completo de controles.

### 1.5. Privacidade

Categorias e condições aplicáveis registradas nas subseções abaixo.

#### 1.5.1. Licitude

**A levantar:** condições legais e institucionais aplicáveis ao tratamento, com responsável institucional a identificar. Nenhuma base legal ou hipótese de exceção foi definida neste documento; ver também seção 2.3.

#### 1.5.2. Finalidade

**RNF-10 — Minimização e retenção de dados — incompleto**

- **Requisito proposto:** O sistema deverá limitar coleta, exposição e retenção de dados pessoais às finalidades acordadas para acesso e acompanhamento pedagógico.
- **Verificação planejada:** Revisar os campos e relatórios contra a finalidade aprovada; verificar regras de acesso e executar os procedimentos de retenção e descarte quando especificados.
- **Rastreabilidade:** RF-01, RF-12, RF-13; NEC-07.
- **A confirmar:** Campos obrigatórios, períodos de retenção, procedimentos e responsáveis institucionais ainda precisam ser definidos com STK-03 e STK-04.

**Fonte:** detalhamento proposto pela equipe a partir da visão, seção 9; validação pelos responsáveis indicados ainda pendente.


#### 1.5.3. Necessidade

**Referência:** RNF-10, seção 1.5.2. Relacionar cada campo pessoal à finalidade que o exige; campos ainda não foram aprovados. Consultar STK-03 e STK-04.

#### 1.5.4. Tratamento

**Referência:** RNF-10, seção 1.5.2. Elaborar catálogo de coleta, acesso, armazenamento, eventual compartilhamento, retenção e descarte. Integrações e períodos de retenção não estão definidos.

### 1.6. Capacidade de Interação (UX, usabilidade e acessibilidade)

Categorias e condições aplicáveis registradas nas subseções abaixo.

#### 1.6.1. Reconhecimento de adequação

**A levantar:** como os usuários reconhecem a finalidade da biblioteca e dos indicadores; avaliar a compreensão em protótipo. Não há requisito independente aprovado nesta categoria.

#### 1.6.2. Facilidade de aprendizado (learnability)

**Referência:** RNF-03, seção 1.6.3. Medir compreensão das tarefas e necessidade de ajuda com estudantes; metas dependem do levantamento.

#### 1.6.3. Operabilidade

**RNF-03 — Usabilidade**

- **Requisito proposto:** As tarefas de busca de material, resposta de questão e consulta de resultado devem oferecer instruções, mensagens de erro e indicação do estado da operação em português.
- **Verificação planejada:** Percorrer os fluxos e provocar erros de preenchimento; verificar indicação clara do problema e de como corrigi-lo. Avaliar depois com estudantes taxa de conclusão e necessidade de ajuda.
- **Rastreabilidade:** RF-03, RF-04, RF-09, RF-12, RF-17; NEC-01, NEC-02, NEC-03.
- **A confirmar:** Metas de sucesso e tempo por tarefa ainda dependem de avaliação com STK-01.

**Fonte:** detalhamento proposto pela equipe a partir da visão, seção 9; validação pelos responsáveis indicados ainda pendente.


#### 1.6.4. Proteção contra erros do usuário

**Referências:** RF-10 prevê confirmação do envio e RNF-03 prevê mensagens de erro. A suficiência dessas medidas deve ser avaliada em tarefas com estudantes; demais situações a levantar.

#### 1.6.5. Inclusividade (acessibilidade)

**RNF-04 — Acessibilidade**

- **Requisito proposto:** Os fluxos principais devem permitir navegação por teclado, foco visível, rótulos associados aos campos e compreensão de resultados sem depender apenas de cores.
- **Verificação planejada:** Executar os fluxos por teclado e revisar rótulos e mensagens; gráficos devem ter valores ou alternativa textual equivalente.
- **Rastreabilidade:** RF-03, RF-09, RF-12, RF-13; necessidades de qualidade da visão.
- **A confirmar:** Necessidades dos usuários, referência normativa e demais critérios de acessibilidade a definir; não há declaração de conformidade nesta versão.

**Fonte:** detalhamento proposto pela equipe a partir da visão, seção 9; validação pelos responsáveis indicados ainda pendente.


#### 1.6.6. Assistência ao usuário (acessibilidade)

**Referências:** RNF-03 e RNF-04. Investigar necessidade de ajuda contextual e alternativas de apresentação com STK-01; nenhum canal de suporte ou tecnologia assistiva específica foi confirmado.

#### 1.6.7. Engajamento do usuário

**A levantar:** utilidade percebida e satisfação na consulta, prática e acompanhamento. Não há requisito de gamificação ou meta de engajamento assumida.

### 1.7. Manutenibilidade

Categorias e condições aplicáveis registradas nas subseções abaixo.

#### 1.7.1. Modularidade

**A levantar:** responsabilidades e dependências dos componentes na modelagem inicial. Não há limite de acoplamento ou arquitetura aprovada.

#### 1.7.2. Reusabilidade

**A levantar:** oportunidades justificadas de reutilização após a definição dos componentes; não há obrigação de adotar biblioteca ou tecnologia específica.

#### 1.7.3. Analisabilidade

**Referência parcial:** RNF-07 permite identificar alterações de conteúdo. Diagnóstico técnico de falhas e registros operacionais ainda precisam de especificação com STK-04, sem expor segredos tratados pelo RNF-02.

#### 1.7.4. Modificabilidade

**A levantar:** mudanças esperadas e procedimento para avaliar impactos nos requisitos e componentes. Nenhuma meta de tempo ou esforço de manutenção foi definida.

#### 1.7.5. Testabilidade

**A levantar:** ambiente e dados adequados para executar os critérios de aceitação dos RF e verificações deste documento. A existência dos critérios auxilia a especificação, mas não comprova testabilidade de uma implementação.

### 1.8. Compatibilidade

Categorias e condições aplicáveis registradas nas subseções abaixo.

#### 1.8.1. Interoperabilidade

**Sem integração confirmada:** investigar necessidade e condições de troca de informações com plataformas institucionais (PQ-06). Importar um PDF enviado pelo usuário não pressupõe integração direta com o INEP.

#### 1.8.2. Coexistência

**A levantar:** coexistência com outros serviços caso compartilhem hospedagem ou recursos. Depende do ambiente definido com STK-04.

### 1.9. Segurança Operacional (safety)

Categorias e condições aplicáveis registradas nas subseções abaixo.

#### 1.9.1. Restrição operacional

**Não se aplica ao escopo atual:** não há controle de equipamento ou processo físico com estado operacional perigoso identificado. Reavaliar se o contexto mudar.

#### 1.9.2. Identificação de riscos

**Não se aplica ao escopo atual:** não foi identificado cenário de risco físico a pessoas, propriedades ou ambiente. Riscos pedagógicos e de dados continuam tratados na visão e nas seções de confiabilidade, segurança e privacidade.

#### 1.9.3. Segurança contra falhas (fail-safe)

**Não se aplica ao escopo atual de safety:** não há modo seguro de equipamento ou processo físico a definir. Integridade de tentativas e recuperação continuam cobertas por RNF-06 e RNF-09.

#### 1.9.4. Aviso de perigo

**Não se aplica ao escopo atual:** não foram identificados perigos físicos que exijam alertas. Mensagens de erro e término de tempo permanecem nos requisitos pertinentes.

#### 1.9.5. Integração segura

**Não se aplica ao escopo atual de safety:** não há integração com componente de operação física perigosa. Segurança da informação de eventuais integrações deverá ser avaliada separadamente.

### 1.10. Adequação funcional

Categorias e condições aplicáveis registradas nas subseções abaixo.

#### 1.10.1. Completude funcional

**Referência:** catálogo RF-01 a RF-17. A cobertura deverá ser conferida contra necessidades e casos de uso após elicitação; sem resultados de entrevistas, não há confirmação de completude.

#### 1.10.2. Corretude funcional

**Referências:** RF-10, RF-12 e RF-13; RN-09 e RN-10 e seus desdobramentos em [regras de negócio](regras-negocio.md). Verificar cálculos com entradas e resultados esperados após validação das fórmulas; não criar outra fórmula neste documento.

#### 1.10.3. Adequação funcional

**Referências:** RNF-03 e benefícios da visão. Avaliar se busca, prática, resultados e reforço permitem cumprir tarefas reais dos usuários. Metas e cenários a validar.

## 2. Requisitos Externos

Categorias e condições aplicáveis registradas nas subseções abaixo.

### 2.1. Ético

**A levantar:** critérios de aceitação dos usuários para apresentação e uso de resultados, evitando conclusões de domínio sem critérios pedagógicos validados (RN-10.2). Consultar estudantes e professores; nenhuma política ética institucional foi fornecida.

### 2.2. Regulatório

**A levantar:** critérios aplicáveis da instituição e das entidades envolvidas no contexto ENADE. Solicitar referências oficiais aos responsáveis; não há resolução específica validada nesta versão.

### 2.3. Legislativo

**A levantar:** condições de proteção de dados pessoais, acessibilidade e uso de materiais, com orientação institucional. O documento de propostas já indica a necessidade de atenção à LGPD; este rascunho não define obrigações jurídicas específicas nem atesta conformidade. Vincular requisitos à fonte pertinente após a verificação.

## 3. Requisitos Organizacionais

Categorias e condições aplicáveis registradas nas subseções abaixo.

### 3.1. Ambientais

**A levantar:** ambiente operacional, hospedagem e restrições de recursos com STK-04. Acesso web em computador e celular é hipótese registrada no RNF-05, não decisão técnica aprovada.

### 3.2. Operacionais

**Referências:** RNF-09 e RNF-10. Definir responsáveis por operação, atualização do acervo, recuperação e retenção. A falta desses dados limita a prontidão para uso.

### 3.3. Desenvolvimento

**Restrição acadêmica informada:** documentação majoritariamente em Markdown para entrega pelo GitHub; Sprint 1 voltada à elicitação e modelagem inicial, sem exigência de implementação de código. Fonte: SRC-03 e SRC-04 da visão. Evidência de atendimento à entrega: arquivos versionados e artefatos obrigatórios disponíveis no repositório, cuja identificação ainda não foi fornecida. Linguagens, frameworks e padrões de desenvolvimento da futura plataforma permanecem a definir.

## 4. Checklist de Validação do Artefato (RNF)

Checklist reservado à revisão do grupo. Os itens permanecem abertos porque existem lacunas e não houve validação por pares ou pelas partes interessadas.

### 4.1. Estrutura e escopo

* [ ] O documento possui histórico de versões preenchido.
* [ ] O escopo da solução está claro no documento.
* [ ] Há requisitos registrados nas seções aplicáveis (produto, externos e organizacionais).
* [ ] Requisitos não aplicáveis estão explicitamente marcados como "Não se aplica", quando necessário.

### 4.2. Qualidade dos requisitos

* [ ] Cada requisito está escrito de forma objetiva e verificável.
* [ ] Cada requisito possui critério mensurável (tempo, percentual, limite, condição ou evidência).
* [ ] Não há requisito ambíguo com termos vagos (ex.: "rápido", "seguro", "fácil") sem métrica.
* [ ] Requisitos duplicados ou conflitantes foram eliminados.

### 4.3. Conformidade e rastreabilidade

* [ ] Requisitos regulatórios/legais relevantes foram registrados.
* [ ] Requisitos de privacidade e segurança foram contemplados quando aplicáveis.
* [ ] Os requisitos estão alinhados com visão da demanda, glossário e casos de uso.
* [ ] Existe rastreabilidade dos requisitos para fontes de negócio, norma ou decisão técnica.

### 4.4. Prontidão para uso

* [ ] Os requisitos podem ser usados como base para implementação e testes.
* [ ] Há insumos suficientes para criar critérios de aceitação.
* [ ] O documento foi revisado por pares.
* [ ] A versão está pronta para aprovação/publicação.
