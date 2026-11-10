# Shehab

CTO at **ClearSplit**. I build fintech and payments infrastructure, the kind of system where a
wrong number is a real loss, so correctness has to be structural, not a hope.

**What that looks like in practice:**

- A double-entry trust-accounting ledger built from scratch: a single write boundary, append-only
  journals enforced at the database layer, corrections by reversal only, and a financial record
  that deliberately outlives the operational rows it refers to.
- A multi-provider payment orchestration engine that routes each charge across gateways, cascades
  on soft declines, handles 3-D Secure, and never double-charges a retried request.
- A multi-PMS reconciliation engine that unifies several source systems into one set of books at
  cent-level, multi-currency accuracy.

**Selected work:**

- [**orchestrant**](https://github.com/Shehab1106/orchestrant): a framework-agnostic payment
  orchestration engine (TypeScript). The failure model is the point: cascade, 3DS, idempotent
  replay, clean ports for providers and storage.
- [**trust-ledger**](https://github.com/Shehab1106/trust-ledger): an architecture case study of
  the trust-accounting ledger, the invariants that keep money from leaking and why each is enforced
  by structure rather than convention.

I care more about systems I understand end to end than about volume. If something here is worth a
conversation, reach me on [LinkedIn](https://www.linkedin.com/in/shehab-elsedody/).
