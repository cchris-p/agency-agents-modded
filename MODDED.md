# Crown Foundry Labs Modded Fork

This is Ametrine LLC's custom fork of
[msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents), used
by **Crown Foundry Labs**.

## What Is Different

- Forked and maintained under `cchris-p/agency-agents-modded`.
- Customizations live on the `development` branch.
- Adds the **`crown-foundry/`** division:
  - `studio-producer` - portfolio and production planning.
  - `va-operations-manager` - supervises agents and reports status.
  - `game-market-scout` - research and opportunity scoring.
- `main` stays close to upstream for easier syncs.

## Why This Fork Exists

Crown Foundry Labs is an agent-first video game business owned by Ametrine LLC.
This fork adds the roles needed to run the agent + virtual-assistant operating
model across mobile, PC, Roblox, and GTA/FiveM products.

## Install Into A Project

```bash
./scripts/convert.sh --tool opencode
./scripts/install.sh --tool opencode \
  --division crown-foundry,game-development,product,project-management,research,finance \
  --path /path/to/project/.opencode/agents --no-interactive
```

## Sync Policy

```bash
git fetch upstream
git checkout development
git merge upstream/main
```

Do not force-push over fork history. This fork is public; never commit secrets,
player data, or proprietary business data.

## Upstream

Upstream project and documentation:
<https://github.com/msitarzewski/agency-agents>

This fork remains MIT-licensed. See `LICENSE`.
