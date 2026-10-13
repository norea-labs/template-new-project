# template-new-project

Il repo modello di Norea Labs: ogni nuovo progetto parte da qui e nasce già a norma.

## Cosa contiene

- `CLAUDE.md` in due parti: la parte fissa uguale in ogni repo, da non toccare, e la sezione "Questo progetto" da compilare.
- `.claude/settings.json`: attiva il plugin `norea` con le regole per l'AI.
- `.github/workflows/norea.yml`: su ogni PR lancia i controlli centrali di `norea-labs/ci`.
- `.github/pull_request_template.md`: il modello di descrizione delle PR.
- `.gitignore`: esclude i file di sistema e i file `.env`, perché i segreti stanno in 1Password.

## Creare un nuovo progetto

1. Su GitHub: "Use this template", "Create a new repository", proprietario `norea-labs`.
2. Nel nuovo repo: scrivi nome e descrizione in cima al `CLAUDE.md` e compila "Questo progetto".
3. Sostituisci questo README con quello del progetto.
4. Apri la prima PR: i controlli devono passare.

## Modificare il modello

Si cambia con una PR, come ogni altro repo. La parte fissa del `CLAUDE.md` invece si cambia solo in `norea-labs/ci` (`modello/claude-parte-fissa.md`) e poi si copia qui e negli altri repo.
