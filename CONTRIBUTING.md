# Contributing to Vehicle Monitoring System

Thank you for your interest in contributing! Here's how to get started.

## Development Setup

```bash
git clone https://github.com/your-username/vehicle-monitoring-system.git
cd vehicle-monitoring-system
npm install
npm run dev
```

## Branching Strategy

| Branch | Purpose |
|--------|---------|
| `main` | Production-ready code |
| `develop` | Integration branch |
| `feature/*` | New features |
| `fix/*` | Bug fixes |
| `chore/*` | Maintenance tasks |

## Commit Convention

Follow [Conventional Commits](https://www.conventionalcommits.org/):

```
feat: add real-time WebSocket support
fix: correct fuel level calculation
docs: update API integration guide
chore: upgrade Recharts to v3
```

## Pull Request Checklist

- [ ] Code follows existing patterns
- [ ] Tests added or updated
- [ ] No console errors
- [ ] Responsive on mobile (375px+)
- [ ] Lint passes (`npm run lint`)
- [ ] Build succeeds (`npm run build`)

## Code Style

- Functional React components with hooks
- CSS custom properties for theming
- Descriptive variable names
- JSDoc comments on hooks and utilities

## Reporting Bugs

Use GitHub Issues with:
- Steps to reproduce
- Expected vs actual behavior
- Browser/OS info
- Screenshots if visual
