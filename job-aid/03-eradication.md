# Eradication

## Coordinate

- [ ] All teams synchronized, do not let one team eradicate while another still collects
  evidence on the same system
- [ ] Third parties briefed, MSSP, forensics vendor, cloud provider support
- [ ] Legal and comms kept current

## Remove root cause

- [ ] Patch applied
- [ ] Credentials rotated
- [ ] Malicious accounts removed
- [ ] Persistence mechanisms eliminated
  - Velociraptor: re run the same hunt used during Containment, confirm a clean result
- [ ] Traffic confirmed clean if it was flagged
  - Wireshark: recheck the same capture filters used during Containment

## Stop

Do not proceed to Recovery until both the IC and Technical Lead formally sign off that
eradication is validated complete. Log the sign off.

→ Next: [Recovery](04-recovery.md)
