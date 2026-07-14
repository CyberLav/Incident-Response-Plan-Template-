# Quick Reference

## Severity

| SEV | Criteria | Notify | Tempo |
|---|---|---|---|
| 1 | Active exploitation, critical system down, exfiltration confirmed, regulatory clock started | Exec and Legal immediately, IC in 15 min | Verbal direction first, write the SMESC order after |
| 2 | Confirmed compromise, contained blast radius | Exec in 1 hr, IC in 30 min | Abbreviate the estimate, move to order faster |
| 3 | Suspected compromise, unconfirmed, limited scope | Team lead, IC in 2 hrs | Full tempo |
| 4 | Anomaly, no confirmed compromise | Standard queue | Investigation only |

Full detail: [Annex A](../annexes/A-severity-escalation-matrix.md)

## Roles

- Incident Commander (IC), single point of decision authority
- Technical Lead, executes containment and eradication
- Scribe, owns the decision log, do not skip even solo
- Comms Lead, owns internal and external messaging
- Exec Sponsor, authorizes anything above the IC's authority

Full detail: [Annex B](../annexes/B-raci-matrix.md)

## Live tools

- [Back Brief Builder](https://cyberlav.io/backbrief-builder.html), confirms understanding before you execute
- [Order Builder](https://cyberlav.io/order-builder.html), generates a formal SMESC order


## Tool key used throughout this Job Aid

| Phase | Tool | What it is for |
|---|---|---|
| Identification | Security Onion, Kibana | Initial alert, triage view |
| Containment | Velociraptor, Wireshark | Host isolation, scoping, packet level confirmation |
| Eradication | Velociraptor, Wireshark | Validate root cause removed |
| Recovery | Security Onion, Kibana | Heightened monitoring window |

These are examples, not a requirement. See the [Job Aid README](README.md) for why these
four and how to substitute your own stack.
