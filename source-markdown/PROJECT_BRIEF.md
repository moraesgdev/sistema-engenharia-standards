# STMA | Termo de Abertura e Definição do Projeto

> **Tipo:** Briefing técnico e autorização para desenvolvimento  
> **Norma de referência:** `TI-ENG-001-NOR` · versão de referência `0.1 Beta` · **pendente de aprovação formal**  
> **Estado deste arquivo:** TEMPLATE — preencher e validar antes de implementar.  
> **Regra:** hipóteses, metas e benefícios estimados não são resultados comprovados.

## Controle documental

| Campo | Valor |
|---|---|
| Projeto / nome comercial | `[PREENCHER]` |
| Repositório previsto | `stma-[nomedoplugin]-[plataforma]` |
| ID da demanda | `[PREENCHER: ticket/protocolo]` |
| Código documental deste projeto (se existente) | `[PREENCHER / Não aplicável]` |
| Revisão deste briefing | `0.1.0` |
| Data de emissão | `[AAAA-MM-DD]` |
| Solicitante / setor | `[PREENCHER]` |
| Responsável de TI | `[PREENCHER]` |
| Responsável técnico de engenharia | `[PREENCHER ou Não aplicável]` |
| Estado | `Proposto / Em análise / Aprovado / Suspenso / Encerrado` |
| Classificação da informação | `[PREENCHER: categoria da STMA]` |

## 1. Resumo executivo (para apresentação)

**Cenário atual:** `[3–5 linhas: qual atividade, fluxo ou problema existe hoje]`.

**Proposta:** `[2–4 linhas: o que será construído e para quem]`.

**Benefício esperado:** `[ganho mensurável ou qualitativo, separado entre hipótese e medição]`.

**Situação real no momento:** `[ideação / protótipo / desenvolvimento / piloto / produção; evidência disponível]`.

## 2. Problema, usuários e processo atual

| Item | Descrição |
|---|---|
| Problema operacional | `[PREENCHER]` |
| Setores/disciplina envolvidos | `[PREENCHER]` |
| Usuários afetados | `[PREENCHER]` |
| Processo atual | `[passo a passo manual / sistema atual]` |
| Frequência e volume | `[ex.: N vezes/semana; origem da estimativa]` |
| Falhas/riscos atuais | `[erros, retrabalho, prazos, segurança]` |
| Evidências do problema | `[entrevistas, registros, prints autorizados, indicadores]` |

## 3. Objetivos e indicadores

| ID | Objetivo | Indicador | Linha de base | Meta | Fonte do dado | Prazo |
|---|---|---|---|---|---|---|
| `OBJ-01` | `[resultado]` | `[KPI]` | `[medido/não medido]` | `[valor alvo]` | `[origem]` | `[data]` |

**Critério de sucesso global:** `[condição verificável que permite chamar o projeto de bem-sucedido]`.

**Método de medição:** `[amostra, período, responsável e possíveis vieses]`.

## 4. Escopo, fronteiras e entregáveis

### Incluído (in scope)

| ID | Entrega/funcionalidade | Resultado esperado | Prioridade | Dependência |
|---|---|---|---|---|
| `ESC-01` | `[funcionalidade]` | `[comportamento observável]` | `Obrigatório / Desejável` | `[ID/N/A]` |

### Excluído (out of scope)

- `[EXC-01 — O que não será implementado nesta etapa]`.
- `[EXC-02 — Pedido relacionado que exige outra demanda]`.

### Entregáveis do projeto

- [ ] Código-fonte no Git e histórico auditável.
- [ ] Artefato executável/instalador ou serviço implantado, conforme aplicável.
- [ ] `README.md` e `DEVELOPMENT.md` preenchidos.
- [ ] `ARCHITECTURE.md` e decisões técnicas relevantes.
- [ ] `TEST_PLAN.md` com resultados e evidências.
- [ ] `CHANGELOG.md`, tag SemVer e release quando publicado.
- [ ] Manual de uso ou orientação ao usuário, quando necessário.
- [ ] Registro de IA relevante, quando houver utilização que exija auditoria.

## 5. Requisitos rastreáveis

### Funcionais

| ID | Requisito | Ator/gatilho | Pré-condição | Resultado verificável | Prioridade | Aceite/teste |
|---|---|---|---|---|---|---|
| `RF-001` | `[descrição sem ambiguidade]` | `[ator]` | `[condição]` | `[saída]` | `Alta / Média / Baixa` | `[CA-001/CT-001]` |

### Não funcionais

| ID | Categoria | Requisito mensurável | Ambiente/amostra | Aceite/teste |
|---|---|---|---|---|
| `RNF-001` | `[performance, usabilidade, segurança, suporte]` | `[valor/regra]` | `[condições]` | `[CA/CT]` |

### Requisitos e validação de engenharia (quando aplicável)

| ID | Disciplina / norma / padrão técnico | Regra a respeitar | Responsável | Evidência de validação |
|---|---|---|---|---|
| `RE-001` | `[disciplina, documento/versão aplicável]` | `[regra específica]` | `[nome]` | `[link/CT]` |

> Regras normativas e cálculos de engenharia devem ser confirmados pelo responsável técnico competente. **Não presumir** que uma automação ou saída de IA possui validação normativa.

## 6. Critérios de aceite (orientados a teste)

| ID | Relacionado a | Cenário / Given–When–Then | Evidência exigida | Aprovador |
|---|---|---|---|---|
| `CA-001` | `RF-001` | `Dado [contexto], quando [ação], então [resultado mensurável].` | `[teste, vídeo, modelo, log]` | `[nome/setor]` |

**Condições impeditivas de aceite:** `[ex.: perda de dados; regressões críticas; incompatibilidade com host homologado; evidência inexistente]`.

## 7. Usuários, stakeholders e responsabilidades

| Papel | Nome/setor | Responsabilidade | Participa de qual aprovação |
|---|---|---|---|
| Solicitante | `[PREENCHER]` | `[definir problema, validar resultado]` | `[escopo/aceite]` |
| Responsável pelo desenvolvimento | `[PREENCHER]` | `[arquitetura, implementação, manutenção]` | `[técnica]` |
| Engenharia | `[PREENCHER ou N/A]` | `[requisitos técnicos, homologação]` | `[validação de disciplina]` |
| Revisor de código | `[PREENCHER]` | `[revisão independente]` | `[PR]` |
| TI/segurança/infra | `[PREENCHER ou N/A]` | `[acessos, infraestrutura, riscos]` | `[produção]` |

## 8. Plataformas, integrações e restrições

| Componente | Versão/ambiente | Integração necessária | Dono/acesso | Risco de compatibilidade |
|---|---|---|---|---|
| `[Revit / AutoCAD / web / sistema interno]` | `[versão]` | `[SDK/API/arquivo]` | `[setor]` | `[descrição]` |

- **Dependências externas:** `[fornecedores, API, infraestrutura, licenças, contratos]`.
- **Informações processadas:** `[dados de clientes, arquivos, modelos, segredos; classificação]`.
- **Ambientes previstos:** `[desenvolvimento / homologação / produção; justificativa se algum não existir]`.
- **Premissas de infraestrutura:** `[sistema operacional, rede, permissões, hosts]`.

## 9. Estratégia de entrega e marcos

| Marco | Critério de conclusão | Responsável | Previsão | Estado | Evidência |
|---|---|---|---|---|---|
| `M-01` | Briefing e escopo aprovados | `[nome]` | `[data]` | `Pendente` | `[link]` |
| `M-02` | Arquitetura definida | `[nome]` | `[data]` | `Pendente` | `[link]` |
| `M-03` | MVP executável e testado | `[nome]` | `[data]` | `Pendente` | `[link]` |
| `M-04` | Homologação de engenharia | `[nome/N/A]` | `[data]` | `Pendente` | `[link]` |
| `M-05` | Release, documentação e operação | `[nome]` | `[data]` | `Pendente` | `[link]` |

**Estratégia de implementação:** `[incremental / piloto / rollout gradual]`.

**Decisão de construção vs. aquisição:** `[se aplicável; alternativas avaliadas, custo e riscos]`.

## 10. Riscos, mudanças e pendências

| ID | Descrição | Probabilidade | Impacto | Responsável | Resposta | Issue |
|---|---|---|---|---|---|---|
| `R-01` | `[risco]` | `[baixo/médio/alto]` | `[baixo/médio/alto]` | `[nome]` | `[mitigar/aceitar/evitar]` | `[link]` |

**Controle de mudança:** novos requisitos após aceite do escopo devem ser registrados em issue e aprovados pelo solicitante e responsável técnico antes de alterar prazo/impacto. Mudanças de arquitetura relevantes devem possuir ADR; alterações de código passam por PR.

## 11. Aprovação de início e rastreabilidade

### Gate de início — checklist

- [ ] Problema, público e responsáveis identificados.
- [ ] Requisitos com IDs, prioridade e critérios de aceite.
- [ ] Escopo e exclusões explícitos.
- [ ] Restrições técnicas e de engenharia conhecidas ou marcadas como pendências.
- [ ] Riscos relevantes conhecidos e com plano de resposta.
- [ ] Repositório planejado conforme `stma-nomedoplugin-plataforma`.
- [ ] Aprovação formal do escopo registrada em sistema autorizado.

| Aprovador | Papel | Decisão | Data | Evidência / link |
|---|---|---|---|---|
| `[NOME]` | Solicitante | `Aprova / Solicita ajustes` | `[AAAA-MM-DD]` | `[link]` |
| `[NOME]` | TI | `Aprova / Solicita ajustes` | `[AAAA-MM-DD]` | `[link]` |
| `[NOME/N/A]` | Engenharia | `Aprova / Solicita ajustes / N/A` | `[AAAA-MM-DD]` | `[link]` |

> Não inserir assinatura fictícia. Na ausência de aprovação, manter **Em análise**.

## Referências cruzadas

- `ARCHITECTURE.md` — solução arquitetural para o escopo aprovado.
- `DEVELOPMENT.md` — descrição do funcionamento e ambiente de desenvolvimento.
- `TEST_PLAN.md` — cobertura dos requisitos e evidências.
- `.github/PULL_REQUEST_TEMPLATE.md` — revisão de incrementos.
- `AI_USAGE_LOG.md` — atividades relevantes com IA.
