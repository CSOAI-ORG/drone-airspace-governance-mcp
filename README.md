# Drone Airspace Governance

> By [MEOK AI Labs](https://meok.ai) — MEOK AI Labs — Drone AI Governance. FAA Remote ID, EASA U-Space, BVLOS risk assessment. First physical AI governance MCP.

Drone Airspace Governance MCP — MEOK AI Labs. FAA Remote ID, EASA U-Space, autonomous flight compliance.

## Installation

```bash
pip install drone-airspace-governance-mcp
```

## Usage

```bash
# Run standalone
python server.py

# Or via MCP
mcp install drone-airspace-governance-mcp
```

## Tools

### `classify_operation`
Classify drone operation category per EASA/FAA regulations.

**Parameters:**
- `weight_kg` (float)
- `altitude_m` (float)
- `bvlos` (bool)
- `over_people` (bool)
- `autonomous` (bool)

### `bvlos_risk_assessment`
SORA 2.5 risk assessment for Beyond Visual Line of Sight operations.

**Parameters:**
- `distance_km` (float)
- `environment` (str)
- `weather` (str)
- `population` (str)

### `remote_id_compliance`
Check FAA Remote ID compliance for drone operations.

**Parameters:**
- `has_remote_id` (bool)
- `broadcast_type` (str)

### `autonomous_decision_governance`
Governance check for autonomous drone AI decisions (EU AI Act + aviation safety).

**Parameters:**
- `decision_type` (str)
- `reversible` (bool)
- `human_override` (bool)


## Authentication

Free tier: 15 calls/day. Upgrade at [meok.ai/pricing](https://meok.ai/pricing) for unlimited access.

## Links

- **Website**: [meok.ai](https://meok.ai)
- **GitHub**: [CSOAI-ORG/drone-airspace-governance-mcp](https://github.com/CSOAI-ORG/drone-airspace-governance-mcp)
- **PyPI**: [pypi.org/project/drone-airspace-governance-mcp](https://pypi.org/project/drone-airspace-governance-mcp/)

## License

MIT — MEOK AI Labs
