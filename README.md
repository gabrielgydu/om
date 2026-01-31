# om

Daily spiritual reading from St. Josemaría Escrivá's works.

Fetches a random point (1-1055) from:
- **Caminho** (The Way)
- **Sulco** (Furrow)
- **Forja** (The Forge)

## Setup

```bash
chmod +x om
./om
```

Optionally, for true randomness via [random.org](https://api.random.org/):
```bash
export RANDOM_ORG_API_KEY="your-api-key"
```

Without the API key, the script falls back to bash's `$RANDOM`.

Optionally specify a point number directly:
```bash
./om 42
```

## Interactive Mode

The script runs as an interactive TUI:

| Key | Action |
|-----|--------|
| ↑/↓ | Navigate between quotes |
| Enter | Toggle notes for selected quote |
| Enter (on notes) | Open notes in `$EDITOR` |
| q | Quit |

## Notes

Personal notes can be attached to each quote. Press Enter on a quote to show its notes section, then Enter again to edit.

Notes are stored as markdown files:
- Default path: `~/.om_notes/`
- Override with: `export OM_NOTES_PATH="/your/path"`
- Filename format: `{NNNN}_{book}.md` (e.g., `0042_caminho.md`)

Each notes file contains the quote as a blockquote header, followed by your notes after a `---` separator.

## Dependencies

- `curl`
- `jq`
- `perl` (optional, for better HTML entity decoding)

## Example

```
══════════════════════════════════════════════════════════════
                        № 630
══════════════════════════════════════════════════════════════

┌─ CAMINHO ──────────────────────────────────────────────────┐
  Não o esqueças: tem mais aquele que precisa de menos. - Não
  cries necessidades.
└────────────────────────────────────────────────────────────┘

┌─ SULCO ────────────────────────────────────────────────────┐
  Esquece-te de ti mesmo… Que a tua ambição seja a de não
  viveres senão para os teus irmãos, para as almas...
└────────────────────────────────────────────────────────────┘

┌─ FORJA ────────────────────────────────────────────────────┐
  Quereria que vivêssemos a identidade de uns com outros
  e de todos com Cristo.
└────────────────────────────────────────────────────────────┘

  ↑↓ navegar  Enter selecionar/editar  q sair
```
