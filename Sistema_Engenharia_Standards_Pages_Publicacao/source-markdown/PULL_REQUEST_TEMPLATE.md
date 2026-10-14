<!--
STMA | Template oficial de Pull Request
Norma de referência: TI-ENG-001-NOR (0.1 Beta, pendente de aprovação formal)
Local recomendado: .github/PULL_REQUEST_TEMPLATE.md
Apague orientações desnecessárias antes de enviar. Não marque testes como executados sem evidência.
-->

# [tipo]: resumo objetivo da alteração

## 1. Identificação e contexto

| Campo | Informação |
|---|---|
| Projeto/repositório | `stma-[nomedoplugin]-[plataforma]` |
| Issue / demanda | `Closes #...` / `[LINK]` |
| Tipo | `feat / fix / docs / refactor / test / chore / hotfix` |
| Branch de origem | `feature/<ticket>-<descricao>` / `fix/<ticket>-<descricao>` / `hotfix/<ticket>-<descricao>` |
| Branch de destino | `main` / `[branch de integração autorizada]` |
| Versão alvo | `[ex.: 0.2.0 / sem release]` |
| Responsável | `@usuario` |
| Disciplina afetada | `[TI, Elétrica, Hidrossanitário, PPCI, Automação, ...]` |

**Problema:** `[o que estava errado/ausente e impacto]`.

**Resultado esperado:** `[comportamento verificável]`.

## 2. Alterações realizadas

- `[módulo/arquivo]` — `[o que mudou e por quê]`.
- `[módulo/arquivo]` — `[o que mudou e por quê]`.

**Fora do escopo:** `[o que esta PR deliberadamente não modifica]`.

**Mudança incompatível (breaking change)?** `Não / Sim — [contrato afetado, plano de migração]`.

**Há mudança de arquitetura?** `Não / Sim — ADR: [link]`.

**Requisitos e critérios de aceite relacionados:** `[RF-..., RNF-..., RE-..., CA-...]`.

## 3. Impacto técnico e engenharia

| Item | Resultado / evidência |
|---|---|
| Módulos/contratos afetados | `[PREENCHER]` |
| Banco/migração | `Não aplicável / [detalhe e rollback]` |
| Permissões, segredos e dados sensíveis | `[análise e controles]` |
| Performance e volume | `[benchmark ou justificativa]` |
| Versões do host / SDK | `[PREENCHER / N/A]` |
| Unidades, coordenadas, parâmetros ou transações | `[impacto / N/A]` |
| Risco de efeitos em modelos/dados existentes | `[risco, mitigação]` |
| Compatibilidade retroativa | `[mantida / alterada, evidência]` |

## 4. Validação executada — resultados reais

> Distinga testes automatizados, compilação e testes realizados dentro do host. Marcar **Não executado** quando necessário; não transformar ausência de falhas reportadas em aprovação.

| Verificação | Estado | Ambiente / comando / versão | Evidência |
|---|---|---|---|
| Build / compilação | `Aprovado / Reprovado / Não executado / N/A` | `[comando e SO]` | `[link para log/CI]` |
| Lint / formatação | `...` | `[comando]` | `[link]` |
| Testes unitários | `...` | `[comando e quantidade]` | `[link]` |
| Integração | `...` | `[serviço / SDK]` | `[link]` |
| Regressão | `...` | `[cenário]` | `[link]` |
| Execução dentro do Revit/AutoCAD/host | `...` | `[produto e versão]` | `[imagem/vídeo/log]` |
| Homologação da engenharia | `...` | `[disciplina e responsável]` | `[aceite]` |
| Segurança e segredos | `...` | `[scanner/revisão]` | `[resultado]` |

### Procedimento de reprodução

1. `[pré-requisitos reais]`.
2. `[comando/ação exata]`.
3. `[resultado observado]`.
4. `[critério de aprovação]`.

**Cenários negativos/limites:** `[entradas inválidas, erros, projeto vazio, dados incompletos, ausência de rede, undo/rollback]`.

**Evidência visual:** `[links para capturas/vídeos autorizados; sem dados sensíveis]`.

## 5. Documentação, configuração e operação

- [ ] `README.md` atualizado quando a instalação, uso ou suporte mudou.
- [ ] `DEVELOPMENT.md` atualizado se houve mudança de funcionamento, stack ou procedimento.
- [ ] `ARCHITECTURE.md`/ADR atualizado se a arquitetura mudou.
- [ ] `TEST_PLAN.md` atualizado com casos e resultados associados.
- [ ] `CHANGELOG.md` atualizado se a alteração será publicada.
- [ ] Procedimentos de deploy/rollback atualizados quando aplicáveis.
- [ ] Arquivos de configuração e variáveis de ambiente documentados **sem valores secretos**.

**Justificativas dos itens não aplicáveis:** `[PREENCHER]`.

## 6. Uso de IA durante esta alteração

**Houve atividade relevante que exige registro?** `Não / Sim / A avaliar`.

Se sim:
- **ID de auditoria:** `AI-AAAA-0001`.
- **Ferramenta:** `[ChatGPT / Codex / Work / outra aprovada]`.
- **Registro:** `[link para AI_USAGE_LOG.md ou sistema autorizado]`.
- **Partes assistidas:** `[documentação / testes / código / análise]`.
- **Validação humana:** `[revisor, evidência e resultado]`.

> Nunca compartilhar credenciais nem colar prompts que contenham informações restritas em PR visível a pessoas não autorizadas.

## 7. Riscos, rollout e reversão

**Risco residual:** `[baixo/médio/alto + justificativa]`.

**Plano de implantação:** `[etapas; janela e responsável, se aplicável]`.

**Rollback:** `[como restaurar versão/dados; condição de acionamento]`.

**Pendências conhecidas:** `[issues e limitações]`.

## 8. Checklist antes de solicitar revisão

- [ ] Branch conforme padrão (`feature/`, `fix/`, `hotfix/`) e issue vinculada.
- [ ] Commits seguindo Conventional Commits (`feat:`, `fix:`, `docs:`, `refactor:`, `test:`, `chore:`).
- [ ] Nenhum push direto na `main`.
- [ ] Código revisado pelo autor; sem alterações acidentais, segredos ou dados sensíveis.
- [ ] Requisitos e critérios de aceite identificáveis e verificados.
- [ ] CI aprovado; falhas ou impossibilidade de execução justificadas e submetidas à aprovação.
- [ ] Evidências anexadas correspondem à versão/commit desta PR.
- [ ] Testes no software hospedeiro executados quando exigidos, ou explicitamente pendentes.
- [ ] Documentação atualizada e riscos/rollback registrados quando relevantes.
- [ ] Revisor **diferente do autor** atribuído para aprovação.

## 9. Parecer do revisor (preenchido na revisão)

**Decisão:** `Aprovar / Solicitar alterações / Bloquear`  
**Revisor:** `@usuario`  
**Resultado da revisão:** `[análise técnica, riscos e requisitos conferidos]`  
**Pendências / follow-up:** `[links]`  
**Exceção emergencial:** `[se aplicada, motivo, autorização e revisão posterior]`

<!-- Política de merge de referência da TI-ENG-001-NOR: CI aprovado e pelo menos uma revisão por pessoa distinta; emergências exigem justificativa registrada. Release em SemVer com tag vMAJOR.MINOR.PATCH. -->
