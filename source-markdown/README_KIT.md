# STMA | Kit Oficial de Templates de Desenvolvimento (Beta)

**Norma associada:** `TI-ENG-001-NOR` — referência `0.1 Beta`, ainda pendente de aprovação pela liderança.  
**Kit:** `0.1.0` · **Emissão:** `2026-10-14`  
**Aplicação proposta:** projetos de software full-stack, plugins e automações para engenharia da STMA.

## Conteúdo do ZIP

| Arquivo | Propósito | Destino recomendado no repositório |
|---|---|---|
| `PROJECT_BRIEF.md` | Escopo, requisitos, aceite e stakeholders | `docs/PROJECT_BRIEF.md` |
| `ARCHITECTURE.md` | Desenho técnico, componentes, dados e integrações | `docs/ARCHITECTURE.md` |
| `TEST_PLAN.md` | Estratégia, casos, execuções e homologação | `docs/TEST_PLAN.md` |
| `AI_USAGE_LOG.md` | Auditoria de usos relevantes de IA | `docs/AI_USAGE_LOG.md` ou local interno restrito |
| `PULL_REQUEST_TEMPLATE.md` | Checklist padrão do GitHub | `.github/PULL_REQUEST_TEMPLATE.md` |

## Implementação inicial (em um projeto existente)

1. Confirmar o nome do repositório: `stma-nomedoplugin-plataforma` (minúsculas ASCII, números e hífens).
2. Copiar os arquivos para seus destinos recomendados. A pasta `.github` é necessária para o template de PR ser reconhecido automaticamente pelo GitHub.
3. Substituir todos os campos `[PREENCHER]` e exemplos por informação factual; registrar `Não aplicável` com justificativa quando pertinente.
4. Vincular `PROJECT_BRIEF.md` aos requisitos e decisões do projeto; sincronizar os demais arquivos nos PRs relevantes.
5. Aplicar a política de branch: `main` estável; `feature/<ticket>-<descricao>`, `fix/<ticket>-<descricao>`, `hotfix/<ticket>-<descricao>`; commits Conventional Commits; CI e ao menos uma revisão independente; release SemVer com tag `vMAJOR.MINOR.PATCH`.
6. Para integrações de engenharia, exigir validação no software hospedeiro e pela disciplina quando aplicável. **Build não equivale a homologação funcional.**
7. Registrar usos extensos ou relevantes de ChatGPT Business, Codex e Work, com revisão humana e dados protegidos.

## Governança documental

- O código `TI-ENG-001-NOR` identifica a **norma corporativa**, não deve ser copiado como um novo ID documental de cada projeto.
- Cada template possui revisão documental própria; o versionamento do produto ocorre separadamente com SemVer.
- O repositório e seus PRs são a trilha principal de mudança; decisões arquiteturais significativas podem ser registradas em `docs/adr/`.
- O kit é uma implementação **proposta**, fundamentada na norma beta, e não comprova aprovação formal de toda a equipe.
- Não publicar segredos, dados de clientes, artefatos privados ou conteúdos restritos em documentação acessível a terceiros.

## Controle de qualidade

Antes de considerar os templates preenchidos, conferir se: objetivo, arquitetura e testes usam IDs consistentes; stack/versões estão especificadas; links apontam para evidências da versão correta; limitações e pendências estão explícitas; revisão humana foi registrada.
