# Recovery

## Restoration

- [ ] Restore from known clean backups or rebuild, avoid clean in place where feasible
- [ ] Patch and harden before returning to production
- [ ] Rotate credentials for all potentially exposed accounts, including service accounts
- [ ] Restoration order set by business criticality

## Heightened monitoring

- [ ] Enhanced monitoring applied for a defined window, 30, 60, or 90 days depending on
  severity
  - Security Onion, Kibana: build a saved search or dashboard scoped to the affected
    systems for the monitoring window
- [ ] Monitoring thresholds owned by a named person, not left ambiguous

## Sign off

- [ ] Business owner confirms functionality restored
- [ ] Exec sponsor confirms status downgraded from active
- [ ] Closure timestamp logged

→ Next: [Lessons Learned](05-lessons-learned.md)
