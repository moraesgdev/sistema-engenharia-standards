# STMA | Plano de Testes, Homologação e Evidências

> **Tipo:** Estratégia de verificação de software e validação técnica  
> **Norma de referência:** `TI-ENG-001-NOR` · versão de referência `0.1 Beta` · **pendente de aprovação formal**  
> **Estado deste arquivo:** TEMPLATE. **Casos previstos não são testes executados.**

## Controle documental

| Campo | Valor |
|---|---|
| Projeto | `[PREENCHER]` |
| Repositório | `stma-[nomedoplugin]-[plataforma]` |
| Documento / revisão | `TEST_PLAN.md / 0.1.0` |
| Versão do software sob teste | `[tag e SHA]` |
| Plataforma/host/SDK | `[versão/Não aplicável]` |
| Ambiente de execução | `[SO, arquitetura, serviços, configurações]` |
| Responsável por QA | `[PREENCHER]` |
| Responsável por validação de engenharia | `[PREENCHER / Não aplicável]` |
| Emissão e última execução | `[AAAA-MM-DD]` |
| Situação | `Planejado / Em execução / Concluído / Bloqueado` |

## 1. Objetivo, escopo e referências

**Objetivo da campanha:** `[que resultado e riscos serão avaliados]`.

**Incluído:** `[features, módulos, integrações, dados, versões]`.

**Não incluído:** `[cenários e motivo; registrar risco residual]`.

**Referências:** `PROJECT_BRIEF.md` (requisitos e aceite), `ARCHITECTURE.md` (fluxos e invariantes), `DEVELOPMENT.md` (comandos), issues/PRs e normas de engenharia aplicáveis.

## 2. Estratégia de testes por camada

| Camada | Verifica | Técnica / ferramenta | Quando roda | Responsável |
|---|---|---|---|---|
| Estáticos | lint, formatação, tipagem, padrões | `[stack/CI]` | `Todo PR` | `[nome]` |
| Unitários | regras e transformações puras | `[framework]` | `Todo PR` | `[nome]` |
| Integração | interfaces, persistência, SDK e serviços | `[harness]` | `[PR/build]` | `[nome]` |
| Sistema/E2E | jornadas em ambiente equivalente ao real | `[ferramenta]` | `[critério]` | `[nome]` |
| Host real (engenharia) | funcionalidade dentro de Revit/AutoCAD/etc. | `[manual/automação in-host]` | `Antes do release aplicável` | `[nome]` |
| Regressão | não romper funcionalidades existentes | `[suite/cenários]` | `PR/release` | `[nome]` |
| Segurança | entradas, permissões, segredos, dependências | `[análise/scan]` | `[critério]` | `[nome]` |
| Desempenho | tempo, memória, escala, degradação | `[benchmark e dataset]` | `[critério]` | `[nome]` |

**Regra de evidência:** compilar com sucesso não equivale a teste funcional; testes isolados de algoritmos, grafos e dados sintéticos não provam funcionamento dentro da UI do host. Declarar cada etapa separadamente.

## 3. Ambiente e dados de teste

| Elemento | Definição / versão exata | Proveniência / link |
|---|---|---|
| Commit do build | `[SHA]` | `[URL]` |
| SO / arquitetura | `[versão / x64, etc.]` | `[URL]` |
| Runtime e dependências | `[versões]` | `[lockfile / build]` |
| Software hospedeiro | `[Revit/AutoCAD e ano ou N/A]` | `[licença/ambiente]` |
| SDK/API | `[versão]` | `[URL]` |
| Banco / serviços | `[ambiente não produtivo]` | `[configuração]` |
| Dataset / modelo teste | `[nome + hash/versão]` | `[repositório controlado]` |
| Configuração | `[perfil testado, sem segredos]` | `[link]` |

**Política dos dados:** usar modelos de teste autorizados, sintéticos ou anonimizados conforme classificação; não inserir documentos de clientes ou dados pessoais em evidências de amplo acesso.

### Matriz de compatibilidade

| Plataforma | Versão | Build | Execução no host | Homologação | Observações |
|---|---|---|---|---|---|
| `[plataforma]` | `[versão]` | `Não executado` | `Não executado / N/A` | `Pendente` | `[detalhe]` |

## 4. Rastreabilidade requisitos → teste → evidência

| Requisito | Critério de aceite | Caso(s) de teste | Resultado | Evidência | Issue/PR |
|---|---|---|---|---|---|
| `RF-001` | `CA-001` | `CT-001` | `Não executado` | `[link pendente]` | `[link]` |
| `RNF-001` | `CA-002` | `CT-002` | `Não executado` | `[link pendente]` | `[link]` |
| `RE-001` | `CA-003` | `CT-003` | `Não executado` | `[link pendente]` | `[link]` |

**Regras:** nenhum requisito obrigatório deve ser dado como validado sem teste/evidência ou exceção explicitamente aceita pelo responsável competente. Regras técnicas e resultados de engenharia exigem revisão da disciplina correspondente.

## 5. Catálogo de casos de teste

### CT-001 — `[nome e cenário]`

| Campo | Registro |
|---|---|
| Categoria | `Unitário / Integração / Sistema / Host / Regressão / Segurança / Performance` |
| Requisito e aceite | `RF-001 / CA-001` |
| Prioridade / risco | `Crítico / Alto / Médio / Baixo` |
| Ambiente e dataset | `[versões, modelo, dados, hash]` |
| Pré-condições | `[estado inicial]` |
| Passos | `1. [ação]  2. [ação]  3. [ação]` |
| Resultado esperado | `[saída mensurável, tolerância/unidade, estado final]` |
| Resultado observado | `[PREENCHER SOMENTE APÓS EXECUÇÃO]` |
| Estado | `Não executado / Aprovado / Reprovado / Bloqueado / Não aplicável` |
| Evidência | `[log, print, vídeo, relatório CI, commit]` |
| Executor / data | `[nome / AAAA-MM-DD HH:mm TZ]` |
| Defeito associado | `[issue / N/A]` |

**Casos complementares obrigatórios conforme risco:** entrada vazia/inválida, grande volume, repetição da operação, interrupção parcial, ausência de conexão, diferenças de versão, permissões insuficientes, arquivos corrompidos, não alteração de elementos não selecionados e preservação de dados anteriores.

### CT-002 — `[nome e cenário]`

Replicar a ficha CT-001 para cada cenário significativo e usar IDs únicos. O ID do teste deve ser estável entre campanhas.

## 6. Testes específicos de integração com engenharia

Preencher para plugins/automação de modelagem. Quando não aplicável, registrar motivo.

| Categoria | Cenário a avaliar | Resultado esperado | Caso/evidência |
|---|---|---|---|
| Host real | Abrir comando e operar na versão homologada | `[critério]` | `[CT/link]` |
| Unidades | Conversão entre unidades internas e de exibição | `[valor e tolerância]` | `[CT/link]` |
| Geometria / coordenadas | Transformações e orientação | `[critério]` | `[CT/link]` |
| Elementos e parâmetros | Seleção, escrita e integridade | `[critério]` | `[CT/link]` |
| Transações e undo | Falha intermediária, rollback e desfazer | `[sem estado parcial não autorizado]` | `[CT/link]` |
| Repetibilidade | Rodar duas vezes no mesmo modelo | `[sem duplicidade indevida]` | `[CT/link]` |
| Modelos diversos | Pequeno, grande, incompleto e legado | `[critério]` | `[CT/link]` |
| Engenharia | Correção do resultado pela disciplina | `[parecer técnico]` | `[CT/link]` |

## 7. Automação, CI e execução local

| Comando ou job | Objetivo | Resultado esperado | Evidência |
|---|---|---|---|
| `[comando real de build]` | Compilação | `Exit code 0; warnings analisados` | `[CI/log]` |
| `[comando real de testes]` | Suite automatizada | `[N testes / critério]` | `[CI/log]` |
| `[comando real de lint]` | Estáticos | `[sem violações bloqueantes]` | `[CI/log]` |

**Não inventar comandos:** copiar somente comandos efetivamente testados, preferencialmente os documentados no `DEVELOPMENT.md`.

**Condição de bloqueio:** teste essencial falhou, regressão confirmada, ausência de validação no host exigida ou problema de segurança crítico → bloquear merge/release até correção ou exceção emergencial formalmente justificada.

## 8. Execuções e resultados da campanha

| Execução | Data/hora/fuso | Commit / build | Ambiente | Total | Passou | Falhou | Bloqueado | Executor | Relatório |
|---|---|---|---|---|---|---|---|---|---|
| `RUN-001` | `[PREENCHER]` | `[SHA]` | `[ambiente]` | `[N]` | `[N]` | `[N]` | `[N]` | `[nome]` | `[URL]` |

### Não conformidades e defeitos

| ID do defeito | Caso | Severidade | Reprodução | Responsável | Estado | PR corretiva |
|---|---|---|---|---|---|---|
| `[issue]` | `CT-001` | `Crítica / Alta / Média / Baixa` | `[passos/evidência]` | `[nome]` | `[status]` | `[link]` |

### Testes não executados ou limitados

| Caso | Motivo | Risco residual | Responsável pela decisão | Ação e prazo |
|---|---|---|---|---|
| `[CT]` | `[host indisponível, licença, ambiente, prazo]` | `[impacto]` | `[nome]` | `[issue/data]` |

## 9. Gate de homologação e aprovação

- [ ] Requisitos obrigatórios têm casos com evidência verificável.
- [ ] CI e testes obrigatórios aprovados na revisão avaliada.
- [ ] Falhas críticas/altas corrigidas ou bloqueio/decisão formal registrados.
- [ ] Compatibilidade verificada nas versões declaradas, sem inferência.
- [ ] Execução no host real registrada **quando necessária**.
- [ ] Validação da disciplina de engenharia realizada **quando necessária**.
- [ ] Riscos de dados, rollback e operações destrutivas testados ou explicitamente pendentes.
- [ ] Evidências vinculadas a commit, build, dataset e ambiente corretos.
- [ ] Plano de manutenção e regressão pós-release definido.

**Parecer QA:** `Aprovado / Aprovado com ressalvas / Reprovado / Não avaliado`  
**Parecer Engenharia:** `Aprovado / Aprovado com ressalvas / Reprovado / Não aplicável / Não avaliado`  
**Revisor QA:** `[nome, data, link]`  
**Revisor Engenharia:** `[nome, data, link/N/A]`  
**Release autorizado por:** `[nome, data, registro formal]`

> Atenção: marcar **Não avaliado** até existir evidência real. A aprovação de release depende das regras internas vigentes e dos responsáveis designados.
