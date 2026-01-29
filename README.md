# om

Daily spiritual reading from St. Josemaría Escrivá's works.

Fetches a random point (1-1055) from:
- **Caminho** (The Way)
- **Sulco** (Furrow)
- **Forja** (The Forge)

## Setup

1. Get a free API key from [random.org](https://api.random.org/)
2. Set the environment variable:
   ```bash
   export RANDOM_ORG_API_KEY="your-api-key"
   ```
3. Make executable and run:
   ```bash
   chmod +x om
   ./om
   ```

## Dependencies

- `curl`
- `jq`
- `perl` (optional, for better HTML entity decoding)

## Example Output

```
══════════════════════════════════════════════════════════════
                        № 630
══════════════════════════════════════════════════════════════

┌─ CAMINHO ─────────────────────────────────────────────────┐
  Não o esqueças: tem mais aquele que precisa de menos. - Não
  cries necessidades.
└───────────────────────────────────────────────────────────┘

┌─ SULCO ────────────────────────────────────────────────────┐
  Esquece-te de ti mesmo… Que a tua ambição seja a de não
  viveres senão para os teus irmãos, para as almas...
└───────────────────────────────────────────────────────────┘

┌─ FORJA ────────────────────────────────────────────────────┐
  Quereria que vivêssemos a identidade de uns com outros
  e de todos com Cristo.
└───────────────────────────────────────────────────────────┘
```
