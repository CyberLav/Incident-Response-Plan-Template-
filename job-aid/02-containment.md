# Containment

## Warning order

- [ ] Response team notified, out of band channel
- [ ] Exec sponsor notified per severity threshold
- [ ] Legal notified if data exposure or litigation risk is plausible
- [ ] Holding statement drafted if customer facing impact is possible

## Scoping

- [ ] Full timeline reconstructed, earliest indicator to present
  - Velociraptor: hunt across the fleet for the same indicators
- [ ] All affected systems, accounts, and data identified, not only what alerted
- [ ] Persistence mechanisms identified
  - Velociraptor: check scheduled tasks, startup items, new accounts
- [ ] Data exposure scope assessed

## Reconnaissance

- [ ] Collection priorities set, volatile evidence first
- [ ] Chain of custody log opened, [Annex F](../annexes/F-evidence-chain-of-custody.md)
- [ ] Collection executed without altering evidence where avoidable
  - Wireshark: capture and confirm suspicious traffic at the packet level before it is
    gone

## Course of action

- [ ] 2 to 3 candidate courses of action weighed: what it stops, what it does not,
  operational cost, evidence impact
- [ ] IC selects a course of action, logs the decision and rationale

## Order

Issue a formal containment order using the SMESC format.

→ [Order Builder](https://cyberlav.io/order-builder.html) or [Annex C](../annexes/C-smesc-order-template.md)

- [ ] Short term containment executed, isolate, block, disable
  - Velociraptor: isolate the host at the endpoint level
- [ ] Long term containment planned if short term is a stopgap, log the gap

→ Next: [Eradication](03-eradication.md)
