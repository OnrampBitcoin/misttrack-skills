# Onramp vendored subset

Read-only risk-check scripts from misttrack-skills at commit
`6ecbfd250f4efdf9cd03ce551b4c838e74e15009` (metadata 1.5.1), copied unchanged
from `scripts/`. Reviewed pin for OPS-759.

| File | SHA-256 |
|---|---|
| `risk_check.py` | `79b106db9c67314c81ab7f6566e57cb660ae8c5d2c533f1540e4a8aa391391d3` |
| `batch_risk_check.py` | `6f6e09c7529df1ff08ead46498605d9f5fd9f7f1addab1a51ac42cbea0d28128` |
| `address_investigation.py` | `8acc20d62e70167f7be6cfa610e8ed6e99c651726115d51438ae6d25d674889b` |
| `multisig_analysis.py` | `0cc254a5327a498859544c299bf037dcfbc1047ff18f4f3bb2fd1b493e3267af` |
| `LICENSE` (MIT) | `4aa5ce9621e2e372c9afd6de18d66dd4cbb4d721b8a00619466ebbebbc34e2e6` |

Only this directory is in scope. The payment module (`scripts/pay.py`,
`skills/payment.md`, `docs/x402.md`), `scripts/transfer_security_check.py`,
`skills/core.md` and the upstream `SKILL.md` are not vendored and must not be used.

Install:

```
python3 -m venv .venv
.venv/bin/pip install --require-hashes -r requirements.txt
```

`requirements.txt` was generated from `requirements.in` with pip-tools 7.6.2
(Python 3.14); the command is in its header. Changes to any file here are
submitted as reviewed diffs.
