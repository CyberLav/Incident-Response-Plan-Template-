# Playbook: Ransomware

Applies the core framework ([00–06](../00-framework-overview.md)) with the following
ransomware-specific additions. Everything not listed here follows the core phases as
written.

## Identification — Type-Specific Indicators

- Ransom note discovered, files renamed with unfamiliar extensions, mass file modification
  alerts, backup deletion attempts, shadow copy deletion (`vssadmin delete shadows`)
- Default severity: **SEV1** unless scope is confirmed extremely limited

## Containment — Type-Specific Options

- **Isolate, don't shut down**, where possible — powering off can destroy volatile evidence
  and encryption keys held in memory that may enable recovery without paying
- Network segmentation to stop lateral spread takes priority over individual host cleanup
- Identify and isolate the backup infrastructure immediately — ransomware operators
  frequently target backups first

## Additional Stakeholders

- Executive sponsor and legal involved from activation, not just at containment — the
  ransom-payment decision requires this
- Cyber insurance carrier notified early; many policies require notification before
  incurring response costs to remain covered
- Law enforcement notification per organizational policy/jurisdiction

## Eradication Notes

- Full rebuild from clean backups is strongly preferred over "decrypt and clean in place"
- Confirm backup integrity and that backups themselves are not compromised before restoring

## Ransom Payment Decision

- Not a technical decision — routed to Executive Sponsor + Legal per
  [Annex B](../annexes/B-raci-matrix.md)
- Log the decision and full rationale in the [decision log](../annexes/E-decision-log-template.md)
  regardless of outcome

---
[← Playbook index](../annexes/I-playbook-index.md)
