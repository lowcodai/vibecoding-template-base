# itshaker-template-base

> Template générique pour tout nouveau projet itshaker.

[![Governance](https://img.shields.io/badge/governance-itshaker-blue)](https://github.com/itshaker/itshaker-copilot-governance)

## Description

Ce repository est un template GitHub pour tout nouveau projet itshaker. Il inclut :
- Structure de documentation standard (`docs/adr/`, `docs/architecture/`, `docs/runbooks/`)
- Configuration GitHub Copilot (instructions, hooks, workflows)
- Fichiers de gouvernance (CONTRIBUTING, SECURITY, SUPPORT)
- Templates d'issues et de pull requests

## Utilisation

### Via le bootstrap (recommandé)

```bash
git clone https://github.com/itshaker/itshaker-bootstrap
cd itshaker-bootstrap
./scripts/new-project.sh --type base --name <mon-projet>
```

### Via GitHub (template repo)

Cliquer sur **Use this template** depuis l'interface GitHub.

## Structure

```
.
├── docs/
│   ├── adr/           # Architecture Decision Records
│   ├── architecture/  # Diagrammes et documentation d'architecture
│   └── runbooks/      # Runbooks opérationnels
└── .github/
    ├── copilot-instructions.md  # Instructions GitHub Copilot
    ├── instructions/            # Instructions spécialisées
    ├── hooks/                   # Hooks Copilot
    ├── workflows/               # GitHub Actions
    ├── ISSUE_TEMPLATE/          # Templates d'issues
    └── PULL_REQUEST_TEMPLATE.md
```

## Gouvernance

Ce template est géré par [itshaker-copilot-governance](https://github.com/itshaker/itshaker-copilot-governance).

Pour synchroniser les mises à jour de gouvernance :

```bash
./scripts/sync-governance.sh --dest .
```

## Éléments Awesome Copilot inclus

| Élément | Type | Usage |
|---------|------|-------|
| `tool-guardian` | Hook | Valide l'usage des outils |
| `secrets-scanner` | Hook | Bloque les fuites de secrets |
| `governance-audit` | Hook | Vérifie la conformité aux policies |
| `adr-generator` | Agent | Génère les ADRs |
| `acquire-codebase-knowledge` | Skill | Analyse la codebase |
| `breakdown-*` | Skills | Découpage de tâches |
| `audit-integrity` | Skill | Audit d'intégrité |
| `arch` | Plugin | Diagrammes d'architecture |

## Références

- [itshaker-copilot-governance](https://github.com/itshaker/itshaker-copilot-governance)
- [github/awesome-copilot](https://github.com/github/awesome-copilot)
- [itshaker-bootstrap](https://github.com/itshaker/itshaker-bootstrap)
