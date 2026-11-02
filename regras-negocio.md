# Regras de negócio da solução (RN) - LAPIS

**Projeto:** Plataforma de Gestão do Conhecimento e Aprendizagem ENADE — Engenharia da Computação  
**Versão:** 0.2 — 01/11/2026  
**Situação:** rascunho adaptado ao template; elicitação e validação pendentes.  
**Elaboração:** grupo do projeto — nomes a preencher.

Os conteúdos são propostas derivadas da [Visão da Demanda](visao-demanda-enade-computacao.md), não resultados de entrevistas nem decisões institucionais aprovadas. SRC, NEC, F, AT, STK e PQ mantêm os significados dos documentos existentes. Consultar os [stakeholders](stakeholders.md), o [roteiro de entrevistas](roteiro-entrevistas.md) e os [requisitos funcionais](requisitos-funcionais.md). A alternativa de Google Forms continua pendente de consulta ao professor.

**Modelo utilizado:** `template-rn-regra-negocio.md`. Cada registro abaixo contém as seções e o checklist do template. O arquivo reúne as regras para facilitar a entrega em Markdown.

Os identificadores RN-01 a RN-14 foram preservados nas regras principais. Desdobramentos recebem sufixos, como RN-05.1, e integram o mesmo conjunto de política referenciado pelos documentos anteriores. As referências antigas devem ser lidas com os desdobramentos listados no índice até o detalhamento dos casos de uso. Estados de conteúdo propostos: rascunho, em revisão, publicado e retirado; fluxos de transição serão detalhados nos casos de uso.

## Histórico de Versões

| Data | Versão | Descrição | Autor |
| --- | --- | --- | --- |
| 01/11/2026 | 0.1 | Proposta inicial de 14 conjuntos de regras | Grupo — nomes a preencher |
| 01/11/2026 | 0.2 | Adequação ao template LAPIS, nomes com sujeito e verbo, desdobramento de decisões e checklists por regra | Grupo — nomes a preencher |

## Índice de rastreabilidade

| Referência anterior | Regras desta versão | RF relacionados |
| --- | --- | --- |
| RN-01 | RN-01 | RF-01, RF-02, RF-09, RF-12, RF-13, RF-14 |
| RN-02 | RN-02, RN-02.1 | RF-03, RF-06, RF-07, RF-17 |
| RN-03 | RN-03, RN-03.1 | RF-03, RF-04, RF-05, RF-06, RF-15 |
| RN-04 | RN-04 | RF-04, RF-05 |
| RN-05 | RN-05, RN-05.1 | RF-06, RF-08, RF-11, RF-15, RF-17 |
| RN-06 | RN-06, RN-06.1 | RF-07 |
| RN-07 | RN-07, RN-07.1 | RF-08, RF-09, RF-11 |
| RN-08 | RN-08, RN-08.1 | RF-09, RF-10 |
| RN-09 | RN-09, RN-09.1, RN-09.2, RN-09.3 | RF-10, RF-12, RF-13 |
| RN-10 | RN-10, RN-10.1, RN-10.2 | RF-10, RF-12, RF-13 |
| RN-11 | RN-11 | RF-14 |
| RN-12 | RN-12 | RF-15 |
| RN-13 | RN-13 | RF-16 |
| RN-14 | RN-14 | RF-17 |

Os checklists permanecem abertos para revisão do grupo; não há aprovação ou revisão por pares registrada.

## RN-01 — Perfis autorizados delimitam o acesso aos resultados

### 1. Regra de negócio

* **Identificador:** RN-01 — Perfis autorizados delimitam o acesso aos resultados.
* **Descrição:** Ao consultar resultados, o estudante acessa apenas os próprios; o professor acessa somente estudantes ou grupos autorizados; a coordenação acessa inicialmente resultados consolidados. A função de administrador técnico não concede, por si só, acesso pedagógico irrestrito.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-07; PQ-05; detalhamento proposto pela equipe.
- **Consultar:** STK-01, STK-02, STK-03, STK-04.
- **Pendente:** Matriz de permissões, vínculo com grupos e exceções de acesso individual.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-02 — Conteúdos atendem ao curso de Engenharia da Computação

### 1. Regra de negócio

* **Identificador:** RN-02 — Conteúdos atendem ao curso de Engenharia da Computação.
* **Descrição:** Para integrar o acervo ou o banco de questões, o conteúdo deve ser pertinente à formação geral ou aos conhecimentos específicos de Engenharia da Computação.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**SRC-04; NEC-02, NEC-04; detalhamento proposto pela equipe.
- **Consultar:** STK-02, STK-03.
- **Pendente:** Referências pedagógicas para determinar pertinência.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-02.1 — A classificação distingue os componentes de formação

### 1. Regra de negócio

* **Identificador:** RN-02.1 — A classificação distingue os componentes de formação.
* **Descrição:** Ao classificar uma questão ou material, o responsável deve identificar sua relação com formação geral ou conhecimentos específicos, conforme a referência pedagógica adotada.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**SRC-04; NEC-02, NEC-04; detalhamento proposto pela equipe.
- **Consultar:** STK-02, STK-03.
- **Pendente:** Referências pedagógicas para determinar pertinência.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-03 — Responsáveis autorizados aprovam conteúdos antes da publicação

### 1. Regra de negócio

* **Identificador:** RN-03 — Responsáveis autorizados aprovam conteúdos antes da publicação.
* **Descrição:** Uma questão ou material só pode ser disponibilizado para estudo após aprovação por responsável autorizado. Rascunhos e itens em revisão não são disponibilizados como conteúdos aprovados.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-06; PQ-03; detalhamento proposto pela equipe.
- **Consultar:** STK-02, STK-05.
- **Pendente:** Quem aprova; possibilidade de autor revisar o próprio material; tratamento de revisões rejeitadas.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-03.1 — Alterações pedagógicas exigem nova aprovação

### 1. Regra de negócio

* **Identificador:** RN-03.1 — Alterações pedagógicas exigem nova aprovação.
* **Descrição:** Uma alteração no conteúdo pedagógico de um item publicado só substitui a versão disponibilizada após nova revisão e aprovação.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-06; PQ-03; detalhamento proposto pela equipe.
- **Consultar:** STK-02, STK-05.
- **Pendente:** Quem aprova; possibilidade de autor revisar o próprio material; tratamento de revisões rejeitadas.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-04 — A publicação exige comprovação da origem e das condições de uso

### 1. Regra de negócio

* **Identificador:** RN-04 — A publicação exige comprovação da origem e das condições de uso.
* **Descrição:** Um material só pode ser publicado quando sua fonte estiver identificada e a verificação das condições de uso estiver registrada. Catalogar um link externo não representa autorização para copiar ou hospedar o conteúdo.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-06; PQ-03; detalhamento proposto pela equipe.
- **Consultar:** STK-05 e responsável institucional a identificar.
- **Pendente:** Como comprovar a verificação e quem decide sobre publicação.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-05 — Questões publicáveis apresentam os elementos obrigatórios

### 1. Regra de negócio

* **Identificador:** RN-05 — Questões publicáveis apresentam os elementos obrigatórios.
* **Descrição:** Na proposta inicial, uma questão publicável deve ser objetiva de alternativa única e conter enunciado, alternativas, exatamente um gabarito, comentário revisado e referência de origem.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-02, NEC-06; detalhamento proposto pela equipe.
- **Consultar:** STK-02.
- **Pendente:** Tipos de questões aceitos e procedimento explícito para corrigir erros ou anular itens já aplicados.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-05.1 — Tentativas concluídas preservam as versões utilizadas

### 1. Regra de negócio

* **Identificador:** RN-05.1 — Tentativas concluídas preservam as versões utilizadas.
* **Descrição:** Uma tentativa concluída permanece vinculada à versão da questão e do gabarito usados em sua aplicação. Uma correção posterior não deve reescrever silenciosamente o resultado histórico.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-02, NEC-06; detalhamento proposto pela equipe.
- **Consultar:** STK-02.
- **Pendente:** Tipos de questões aceitos e procedimento explícito para corrigir erros ou anular itens já aplicados.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-06 — Associações curriculares utilizam referências aprovadas

### 1. Regra de negócio

* **Identificador:** RN-06 — Associações curriculares utilizam referências aprovadas.
* **Descrição:** Ao associar conteúdo a disciplinas e competências, o responsável deve utilizar referências pedagógicas aprovadas e identificar a grade curricular adotada.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-04; PQ-02; detalhamento proposto pela equipe.
- **Consultar:** STK-02, STK-03.
- **Pendente:** Vocabulário, versão da grade e responsáveis por atualizar associações.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-06.1 — Conteúdos podem receber vários temas pertinentes

### 1. Regra de negócio

* **Identificador:** RN-06.1 — Conteúdos podem receber vários temas pertinentes.
* **Descrição:** Uma questão ou material pode ser associado a mais de um tema quando essas associações forem pedagogicamente justificadas.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-04; PQ-02; detalhamento proposto pela equipe.
- **Consultar:** STK-02, STK-03.
- **Pendente:** Vocabulário, versão da grade e responsáveis por atualizar associações.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-07 — Simulados publicados apresentam configuração completa

### 1. Regra de negócio

* **Identificador:** RN-07 — Simulados publicados apresentam configuração completa.
* **Descrição:** Um simulado só pode ser publicado com questões revisadas, público autorizado, duração e políticas de tentativas e de liberação do gabarito definidas.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-02; F-06, F-07; detalhamento proposto pela equipe.
- **Consultar:** STK-02.
- **Pendente:** Valores e escolhas de configuração, adaptações de tempo e possibilidade de novas tentativas.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-07.1 — Tentativas iniciadas preservam a configuração aplicada

### 1. Regra de negócio

* **Identificador:** RN-07.1 — Tentativas iniciadas preservam a configuração aplicada.
* **Descrição:** A configuração que rege uma tentativa iniciada deve permanecer preservada, mesmo que a configuração de aplicações futuras seja alterada.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-02; F-06, F-07; detalhamento proposto pela equipe.
- **Consultar:** STK-02.
- **Pendente:** Valores e escolhas de configuração, adaptações de tempo e possibilidade de novas tentativas.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-08 — O envio ou o término do tempo encerra a tentativa

### 1. Regra de negócio

* **Identificador:** RN-08 — O envio ou o término do tempo encerra a tentativa.
* **Descrição:** Uma tentativa encerra-se por envio confirmado do estudante ou por término do tempo. No término do tempo, são consideradas as respostas já confirmadas como salvas.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-02; F-07; detalhamento proposto pela equipe.
- **Consultar:** STK-01, STK-02.
- **Pendente:** Pausa, retomada, perda de conexão e tratamento de falhas durante o envio.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-08.1 — Tentativas encerradas impedem alterações de respostas

### 1. Regra de negócio

* **Identificador:** RN-08.1 — Tentativas encerradas impedem alterações de respostas.
* **Descrição:** Após o encerramento de uma tentativa, o estudante não pode alterar suas respostas.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-02; F-07; detalhamento proposto pela equipe.
- **Consultar:** STK-01, STK-02.
- **Pendente:** Pausa, retomada, perda de conexão e tratamento de falhas durante o envio.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-09 — O desempenho individual expressa a proporção de acertos válidos

### 1. Regra de negócio

* **Identificador:** RN-09 — O desempenho individual expressa a proporção de acertos válidos.
* **Descrição:** Na proposta inicial, o percentual individual é 100 × acertos / questões válidas consideradas, com peso igual por questão. Sem questões válidas, apresentar sem dados, em vez de um percentual.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-03; PQ-04; detalhamento proposto pela equipe.
- **Consultar:** STK-02, STK-03.
- **Pendente:** Confirmar pesos, anulações, tentativas consideradas e adequação dessa agregação; não apresentar o resultado como nota oficial do ENADE.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-09.1 — Respostas em branco contam como não acertadas

### 1. Regra de negócio

* **Identificador:** RN-09.1 — Respostas em branco contam como não acertadas.
* **Descrição:** Quando uma questão válida não tiver resposta registrada no encerramento, ela permanece no denominador e não acrescenta acerto.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-03; PQ-04; detalhamento proposto pela equipe.
- **Consultar:** STK-02, STK-03.
- **Pendente:** Confirmar pesos, anulações, tentativas consideradas e adequação dessa agregação; não apresentar o resultado como nota oficial do ENADE.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-09.2 — Questões anuladas deixam de compor o desempenho

### 1. Regra de negócio

* **Identificador:** RN-09.2 — Questões anuladas deixam de compor o desempenho.
* **Descrição:** Uma questão anulada deve ser excluída do numerador e do denominador do indicador ao qual a anulação se aplica. O procedimento de anulação após aplicação ainda precisa ser definido.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-03; PQ-04; detalhamento proposto pela equipe.
- **Consultar:** STK-02, STK-03.
- **Pendente:** Confirmar pesos, anulações, tentativas consideradas e adequação dessa agregação; não apresentar o resultado como nota oficial do ENADE.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-09.3 — O consolidado utiliza a proporção de acertos sobre oportunidades válidas

### 1. Regra de negócio

* **Identificador:** RN-09.3 — O consolidado utiliza a proporção de acertos sobre oportunidades válidas.
* **Descrição:** Para o conjunto de participantes e tentativas selecionado, somar acertos e oportunidades válidas de resposta antes de calcular o percentual consolidado. Sem oportunidades válidas, apresentar sem dados.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-03; PQ-04; detalhamento proposto pela equipe.
- **Consultar:** STK-02, STK-03.
- **Pendente:** Confirmar pesos, anulações, tentativas consideradas e adequação dessa agregação; não apresentar o resultado como nota oficial do ENADE.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-10 — Questões multitemáticas contribuem uma vez para cada tema

### 1. Regra de negócio

* **Identificador:** RN-10 — Questões multitemáticas contribuem uma vez para cada tema.
* **Descrição:** Uma questão pode contribuir uma vez para cada tema ao qual está associada, mas apenas uma vez para o total geral da tentativa.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-03, NEC-04; PQ-04; detalhamento proposto pela equipe.
- **Consultar:** STK-02, STK-03.
- **Pendente:** Cobertura mínima, limites de interpretação e comparação entre simulados.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-10.1 — Indicadores apresentam a quantidade de itens considerada

### 1. Regra de negócio

* **Identificador:** RN-10.1 — Indicadores apresentam a quantidade de itens considerada.
* **Descrição:** Todo indicador de desempenho por tema deve informar a quantidade de questões ou oportunidades válidas de resposta usada no cálculo, conforme seu tipo.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-03, NEC-04; PQ-04; detalhamento proposto pela equipe.
- **Consultar:** STK-02, STK-03.
- **Pendente:** Cobertura mínima, limites de interpretação e comparação entre simulados.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-10.2 — Diagnósticos dependem de critérios pedagógicos aprovados

### 1. Regra de negócio

* **Identificador:** RN-10.2 — Diagnósticos dependem de critérios pedagógicos aprovados.
* **Descrição:** Classificações como dificuldade ou domínio só podem ser apresentadas após aprovação dos critérios pedagógicos de interpretação. Até lá, os resultados devem ser descritivos.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-03, NEC-04; PQ-04; detalhamento proposto pela equipe.
- **Consultar:** STK-02, STK-03.
- **Pendente:** Cobertura mínima, limites de interpretação e comparação entre simulados.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-11 — Professores autorizados indicam ações de reforço

### 1. Regra de negócio

* **Identificador:** RN-11 — Professores autorizados indicam ações de reforço.
* **Descrição:** A indicação de reforço cabe ao professor autorizado a acompanhar o destinatário e deve identificar o tema e a orientação. Essa indicação não representa garantia de melhora da aprendizagem.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-05; F-09; detalhamento proposto pela equipe.
- **Consultar:** STK-01, STK-02.
- **Pendente:** Tipos de atividade, destinatários e necessidade de acompanhar conclusão.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-12 — Questões extraídas aguardam conferência com a fonte

### 1. Regra de negócio

* **Identificador:** RN-12 — Questões extraídas aguardam conferência com a fonte.
* **Descrição:** Questões importadas de PDF permanecem em rascunho até conferência com a prova de origem, incluindo enunciados, imagens, fórmulas, alternativas e gabaritos quando presentes. Conteúdo incompleto não pode ser publicado como revisado.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-06; PQ-08; detalhamento proposto pela equipe.
- **Consultar:** STK-02, STK-05.
- **Pendente:** Critérios de aceite da extração e identificação de duplicatas.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-13 — Análises históricas identificam o conjunto e o método utilizados

### 1. Regra de negócio

* **Identificador:** RN-13 — Análises históricas identificam o conjunto e o método utilizados.
* **Descrição:** Uma análise histórica só deve apresentar ranking ou percentuais após definição do conjunto de provas e do método de contagem. A apresentação deve identificar provas, anos, unidade de contagem e tratamento de múltiplos temas, sem afirmar previsão de provas futuras.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-08; PQ-09; detalhamento proposto pela equipe.
- **Consultar:** STK-02, STK-03.
- **Pendente:** Conjunto de provas, denominador, itens anulados e método de contagem.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## RN-14 — Indicadores distinguem prática individual e simulado

### 1. Regra de negócio

* **Identificador:** RN-14 — Indicadores distinguem prática individual e simulado.
* **Descrição:** Respostas de prática individual devem ser diferenciadas das respostas de simulados. Sua combinação, inclusive de repetições, em um mesmo indicador exige regra explícita e validada.
* **Situação:** proposta, pendente de validação.

- **Origem e rastreabilidade:**NEC-02, NEC-03; F-07, F-08; detalhamento proposto pela equipe.
- **Consultar:** STK-01, STK-02.
- **Pendente:** Se a prática compõe o histórico e como repetições são apresentadas.

### 2. Checklist de Validação da Regra de Negócio


#### 2.1 Estrutura mínima

* [ ] Identificador único e padronizado (ex.: RN1, RN1.1, RN2).
* [ ] Nome da regra no formato sujeito + verbo + objeto.
* [ ] Descrição clara, direta e sem ambiguidades.

#### 2.2 Qualidade da regra

* [ ] A regra descreve apenas uma decisão/comportamento principal.
* [ ] Condições de aplicação (gatilho/contexto) estão explícitas.
* [ ] Resultado esperado da regra está explícito.
* [ ] A regra é verificável e testável.

#### 2.3 Consistência e rastreabilidade

* [ ] Não há conflito com outras regras já existentes.
* [ ] A regra referencia origem (negócio, norma, lei ou decisão do cliente), quando aplicável.
* [ ] A regra está alinhada com CDU, RNF e demais artefatos relacionados.

#### 2.4 Prontidão

* [ ] Conteúdo revisado por pares.
* [ ] Regra pronta para uso em análise, desenvolvimento e testes.

## Registro de decisões

Nenhuma regra desta versão foi validada por entrevistados. Ao revisar, registrar ID, decisão, justificativa, fonte, responsável, data e artefatos afetados. Os responsáveis nominais serão definidos pelo grupo.
