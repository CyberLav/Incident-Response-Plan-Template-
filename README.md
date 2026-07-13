# Incident Response Plan Template
### SANS PICERL + 16-Step Battle Procedure

A scalable, operational incident response plan that pairs the SANS PICERL framework
(Preparation, Identification, Containment, Eradication, Recovery, Lessons Learned) with
the NATO/Commonwealth 16-Step Battle Procedure for moving a team
from notification to synchronized action under time pressure.

PICERL tells you *what* phase you're in. Battle procedure tells you *how fast and how
formally* to move through it. Most IR plans are strong on the first and vague on the
second; this one is built to close that gap.

**Live version:** [cyberlav.io/incident-response.html](https://cyberlav.io)  also
includes a companion one-page job aid and an interactive SMESC order builder.

## Structure

```
├── 00-framework-overview.md      Framework logic, definitions, phase map
├── 01-preparation.md
├── 02-identification.md
├── 03-containment.md
├── 04-eradication.md
├── 05-recovery.md
├── 06-lessons-learned.md
├── annexes/
│   ├── A-severity-escalation-matrix.md
│   ├── B-raci-matrix.md
│   ├── C-smesc-order-template.md
│   ├── D-communications-sitrep-template.md
│   ├── E-decision-log-template.md
│   ├── F-evidence-chain-of-custody.md
│   ├── G-aar-template.md
│   ├── H-tier-scaling-guide.md
│   └── I-playbook-index.md
├── playbooks/
│   ├── ransomware.md
│   ├── bec.md
│   ├── insider-threat.md
│   ├── ddos.md
│   └── cloud-compromise.md
└── templates/                    Fillable copies of the annex templates
```

## Who This Is For

Built to scale across three tiers — see
[Annex H](annexes/H-tier-scaling-guide.md):

- **Small org** (1–2 person security function)
- **Mid-size** (dedicated security team, no full SOC)
- **Enterprise** (SOC/CSIRT with formal hierarchy)

## Getting Started

1. Read [00-framework-overview.md](00-framework-overview.md) first it explains how the
   PICERL phases and battle procedure steps map to each other.
2. Pick your tier in [Annex H](annexes/H-tier-scaling-guide.md) and adjust formality/roles
   accordingly.
3. Fill in the organization-specific placeholders, severity thresholds
   ([Annex A](annexes/A-severity-escalation-matrix.md)), RACI
   ([Annex B](annexes/B-raci-matrix.md)), and regulatory notification requirements.
4. Run a tabletop exercise against the plan before you need it for real. The tempo
   discipline (SMESC orders, time-boxed triage) is a skill and it has to be rehearsed to
   work under pressure.

## Status

This is a living document. Playbooks beyond ransomware are currently placeholders,
contributions welcome.

## License

Released under the [MIT License](LICENSE) use, adapt, and redistribute freely, including
for commercial engagements. Attribution appreciated but not required.

## Author

Maintained by [Alexander Lavrinenko](https://cyberlav.io) IT Audit & Cybersecurity,
Cyber Operator with the Canadian Armed Forces.
