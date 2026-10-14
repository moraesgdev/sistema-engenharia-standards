# STMA | Registro Auditável de Uso de Inteligência Artificial

> **Tipo:** Governança e rastreabilidade de uso relevante de IA  
> **Norma de referência:** `TI-ENG-001-NOR` · versão de referência `0.1 Beta` · **pendente de aprovação formal**  
> **Estado deste arquivo:** TEMPLATE de registro. Não inserir dados sensíveis em repositório com acesso amplo.

## 1. Finalidade e alcance

A STMA utiliza **ChatGPT no plano Business**, com organização por setor em pastas/espaços internos, conforme informado para esta norma. **Codex e Work** devem ser utilizados com atenção aos limites e cotas apresentados no ambiente contratado. O registro cobre usos relevantes de IA em desenvolvimento, engenharia, documentação, integração e operações.

**Inventário verificado na norma beta:** ChatGPT Business, com Codex e Work conforme disponibilidade da contratação. **Outros produtos, licenças e planos precisam de validação interna antes de constarem como contratados.**

### Quando registrar obrigatoriamente

Registrar quando ocorrer **qualquer** uma destas situações:

- Alteração material de código, arquitetura, contratos ou dados, especialmente executada por agente.
- Tarefa extensa ou consumo expressivo de Codex/Work em relação à cota visível.
- Integração com API, repositório, sistema interno ou ferramenta externa.
- Produção de documento técnico com impacto em decisões relevantes ou aceites.
- Geração/avaliação de cálculos, automações, regras de engenharia ou resultado de segurança.
- Acesso a informação interna relevante, sob as permissões aprovadas.
- Decisão de engenharia de software ou infraestrutura influenciada de forma significativa por IA.

Tarefas triviais e pontuais podem ser dispensadas do registro detalhado quando não se enquadram nesses critérios e a política interna permitir. Em caso de dúvida, registrar resumidamente.

### Regras de confidencialidade

1. Informar **referências** às entradas/saídas, não reproduzir prompts com dados de clientes, segredos, tokens ou credenciais.
2. Documentar a **classificação da informação** e respeitar o acesso do repositório/pasta de cada setor.
3. Minimizar dados enviados; quando necessário, anonimizar ou sanitizar conforme política da organização.
4. Para execução autônoma, registrar permissões concedidas, ações externas e o que efetivamente foi executado.
5. Resultados de IA **não** equivalem a teste, revisão humana, validação normativa ou aprovação técnica.
6. Registrar consumo/cota **somente se visível ou mensurável**. Não inventar números ou presumir recursos de planos/licenças.

## 2. Campos de controle do registro

| Campo | Valor |
|---|---|
| Projeto | `stma-[nomedoplugin]-[plataforma]` |
| Setor / pasta de trabalho | `[PREENCHER: setor e caminho autorizado]` |
| Responsável pelo arquivo | `[nome / equipe]` |
| Classificação e controle de acesso | `[PREENCHER: política vigente]` |
| Última atualização | `[AAAA-MM-DD]` |
| Revisão do documento | `0.1.0` |

## 3. Índice resumido dos registros

| ID | Data | Ferramenta | Objetivo | Issue/PR | Estado | Validação |
|---|---|---|---|---|---|---|
| `AI-AAAA-0001` | `[AAAA-MM-DD]` | `[ChatGPT/Codex/Work]` | `[título não sensível]` | `[link]` | `Aberto / Concluído / Cancelado` | `Pendente / Aprovado / Reprovado` |

> Usar identificadores por **ano e sequência**, por exemplo `AI-2026-0001`. Verificar duplicidade no escopo definido pela equipe antes de criar um novo ID.

## 4. Ficha de execução — duplicar por uso relevante

### AI-AAAA-0001 — `[Título objetivo da atividade]`

| Campo | Preenchimento |
|---|---|
| ID | `AI-AAAA-0001` |
| Data e período | `[AAAA-MM-DD HH:mm–HH:mm TZ]` |
| Responsável humano | `[nome / equipe / setor]` |
| Projeto / repositório / branch | `[repo] / [branch]` |
| Demanda de origem | `[issue/tarefa/solicitação autorizada]` |
| Ferramenta e modalidade | `[ChatGPT Business (chat) / Codex / Work / outro aprovado]` |
| Ambiente/pasta/setor | `[pasta/equipe; sem dados restritos]` |
| Objetivo | `[qual problema se pretende resolver]` |
| Escopo permitido | `[arquivos, sistemas, operações permitidas]` |
| Restrições / proibições | `[ex.: sem deploy, sem apagar dados, sem acesso a segredos]` |
| Entradas utilizadas | `[links internos autorizados / descrição sanitizada]` |
| Classificação das entradas | `[pública/interna/restrita conforme política aplicável]` |
| Ações executadas | `[ler, editar arquivos, abrir PR, executar testes, acessar sistemas...]` |
| Saídas produzidas | `[links para commits, diffs, docs, artefatos]` |
| Proposta vs. execução real | `[o que foi apenas sugerido e o que foi efetivamente alterado]` |
| Status | `Concluído / Parcial / Falhou / Cancelado` |
| Incidentes/limitações | `[falhas, comportamento inesperado, ações revertidas]` |
| Registro de consumo | `[cota/limite indicado no produto; valor ou Não disponível]` |
| Aprovação para ação externa | `[nome/registro/N/A]` |
| Revisor humano | `[nome, cargo/disciplina]` |
| Validação executada | `[revisão de diff, segurança, testes, host real, parecer de engenharia]` |
| Evidências de validação | `[links para TEST_PLAN, relatório CI, PR, screenshots]` |
| Resultado da validação | `Aprovado / Reprovado / Pendente` |
| Decisão final | `Aceito / Ajustar / Descartado / Pendente` |
| Pendências | `[issue/ação e responsável]` |

#### Objetivo e contexto (sem reproduzir informação restrita)

`[PREENCHER: contexto mínimo necessário para auditoria. Quais critérios definiam sucesso?]`

#### Resumo do trabalho efetivamente realizado

1. `[ação ou análise 1; fonte e destino, quando autorizados]`.
2. `[ação ou análise 2]`.
3. `[diferença entre intenção, proposta e execução real]`.

#### Artefatos e mudanças rastreáveis

| Artefato | Tipo | Referência exata | Verificado por |
|---|---|---|---|
| `[arquivo/commit]` | `Código / Documento / Análise / Teste` | `[URL, SHA ou ID]` | `[nome]` |

#### Consumo de recursos e limites

| Indicador | Antes | Depois | Fonte da medida | Observação |
|---|---|---|---|---|
| Cota de Codex/Work (quando visível) | `[valor/Não disponível]` | `[valor/Não disponível]` | `[interface/registro]` | `[sem estimativa inventada]` |
| Duração da execução | `[início]` | `[fim]` | `[registro de execução]` | `[fuso]` |
| Custo adicional identificado | `[valor/Não informado]` | `[valor/Não informado]` | `[faturamento autorizado]` | `[não confundir consumo com cobrança]` |

#### Conferência humana e evidências

- [ ] Escopo e permissões respeitados.
- [ ] Alterações verificadas contra o código-fonte/artefatos finais.
- [ ] Segurança e vazamento de segredos revisados.
- [ ] Requisitos e decisões confirmados pelo responsável.
- [ ] Testes planejados foram executados ou estão explicitamente pendentes.
- [ ] Execução real no software hospedeiro registrada, se exigida.
- [ ] Resultado de engenharia revisado por profissional responsável, se aplicável.
- [ ] Registro de consumo apoiado em evidência real, se disponível.
- [ ] Registro vinculado à issue/PR/release conforme necessidade.

**Parecer humano:** `[o que foi aprovado, quais limitações permanecem e por quê]`.

**Responsável pela revisão / data / referência:** `[nome / AAAA-MM-DD / link]`.

---

## 5. Indicadores agregados (preencher por período)

> Esta tabela pode apoiar gestão de capacidade, sem exigir contagens indisponíveis. Não deve ser usada como medição de produtividade individual sem critérios explícitos e aprovação interna.

| Período | Setor | Registros relevantes | Concluídos | Pendentes/reprovados | Ocorrências de limite | Fonte |
|---|---|---|---|---|---|---|
| `[AAAA-MM]` | `[setor]` | `[N]` | `[N]` | `[N]` | `[N ou Não disponível]` | `[IDs]` |

## 6. Responsabilidades e retenção

- **Operador:** define escopo, protege informações e registra a execução relevante.
- **Revisor técnico:** verifica código, testes e efeitos da alteração; não delega aceite a IA.
- **Responsável de engenharia:** valida aplicação na disciplina quando necessário.
- **Gestor de TI/governança:** define acesso, local oficial, retenção e periodicidade de auditoria, conforme política interna aprovada.

**Local oficial do histórico:** `[PREENCHER: repositório privado ou sistema interno aprovado]`.

**Prazo de retenção:** `[PREENCHER: política validada pela STMA; não presumir prazo]`.

**Plano/licenças adicionais:** `[PREENCHER somente após confirmação do inventário corporativo]`.

## 7. Auditoria de qualidade do log

- [ ] IDs únicos, sequência temporal e links funcionais.
- [ ] Entradas/saídas referenciadas sem expor dados restritos.
- [ ] Alterações efetivas separadas de recomendações não executadas.
- [ ] Registro de validação humana e riscos residuais.
- [ ] Indicação honesta quando limites, custos ou métricas não estiverem disponíveis.
- [ ] Não atribuir à IA decisões aprovadas exclusivamente por humanos.
- [ ] Setor e classificação de acesso coerentes com a localização do arquivo.

## Referências cruzadas

- `PROJECT_BRIEF.md` — objetivo e escopo autorizado.
- `ARCHITECTURE.md` — decisões arquiteturais sob análise.
- `TEST_PLAN.md` — testes que validaram as alterações.
- `.github/PULL_REQUEST_TEMPLATE.md` — revisão do código assistido.
- `DEVELOPMENT.md` — convenções gerais de desenvolvimento.
