# Identification

## Entry criteria

Alert, user report, third party notification, threat intel match, anomaly during routine
monitoring.

## Triage, target 15 minutes

- [ ] What alerted, and on what asset or system
  - Security Onion: check the Alerts dashboard in Kibana, cross reference the Suricata or
    Zeek event
- [ ] Is this plausibly a true positive
- [ ] Apparent blast radius: single host or multiple, standard user or privileged, internal
  only or internet facing
- [ ] Initial severity estimate, see [Quick Reference](00-quick-reference.md)

## Decision point

**False positive** → close, log for tuning, done.

**True positive or uncertain** → formal activation, continue below.

## Formal activation

- [ ] Incident declared, unique ID assigned
- [ ] IC designated by role, confirm authority, do not default to whoever is online
- [ ] Severity confirmed
- [ ] Decision log opened, [Annex E](../annexes/E-decision-log-template.md)

## Mission analysis, one paragraph

State plainly: what are we actually being asked to do, what constraints apply
(regulatory clock, contractual SLA, litigation hold), what don't we know yet. If you
cannot say it in one paragraph, this step is not done.

→ Next: [Containment](02-containment.md)
