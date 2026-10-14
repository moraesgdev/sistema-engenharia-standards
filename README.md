# Sistema Engenharia — Biblioteca de Padrões Técnicos

> Norma de referência: `TI-ENG-001-NOR` · Pacote `0.1 Beta` · Modelo documental ainda sujeito a aprovação interna.

Biblioteca HTML de apresentação dos padrões de engenharia, automação e desenvolvimento de software da STMA/Sistema Engenharia, com as fontes Markdown versionáveis.

**Repositório:** https://github.com/moraesgdev/sistema-engenharia-standards  
**Endereço previsto do GitHub Pages:** https://moraesgdev.github.io/sistema-engenharia-standards/

## Estrutura

- `site/index.html` — página inicial da biblioteca.
- `site/*.html` — sete documentos técnicos HTML e página 404.
- `source-markdown/*.md` — documentos originais para edição, não publicados pelo workflow.
- `.github/workflows/deploy-pages.yml` — implantação estática automática pelo GitHub Actions.

## Implantação

1. Publique **todo o conteúdo desta pasta na raiz da branch `main`** do repositório, preservando arquivos ocultos como `.github/` e `site/.nojekyll`.
2. Em **Settings → Pages → Build and deployment**, selecione **Source: GitHub Actions**.
3. Em **Actions**, habilite os workflows se solicitado e abra `Publicar documentação STMA no GitHub Pages`.
4. Execute `Run workflow` se não houver execução automática. O workflow é disparado ao atualizar `site/**` ou o próprio workflow na `main`.
5. Verifique o resultado em **Actions**, depois abra **Settings → Pages → Visit site**.

### Envio por Git (para quem tem permissão de escrita)

Clone o repositório e copie os arquivos do pacote **para dentro da pasta clonada**, sem apagar documentos existentes. Em seguida:

```bash
git add README.md .gitignore site source-markdown .github/workflows/deploy-pages.yml
git commit -m "docs: publica biblioteca tecnica Sistema Engenharia"
git push origin main
```

No primeiro envio, confira se o `README.md` existente pode ser substituído ou preservado. Não publique credenciais ou documentação confidencial. O GitHub Pages será um site público.

## Atualizações e controle de alterações

Edite o arquivo correspondente em `source-markdown/`, regenere o HTML em `site/` e revise a apresentação antes do commit. A publicação usa arquivos estáticos: alterar somente o Markdown não altera o site. Prefira branches e pull requests para mudanças posteriores.

O identificador documental `TI-ENG-001-NOR` é estável, enquanto versão e estado de aprovação permanecem registrados separadamente. Conteúdo marcado `[PREENCHER]` é um template, não documentação homologada de projeto.
