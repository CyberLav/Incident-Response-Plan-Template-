# Job Aid

## What this is

The Job Aid is a stripped down, execution focused companion to the full
[Reference Plan](../00-framework-overview.md). Where the Reference Plan explains and
justifies each phase, the Job Aid assumes you already know the plan and gives you only
what you need mid incident: checklists, decision points, and pointers to the tools and
templates that do the actual work.

One page per phase, five pages total. Preparation is intentionally excluded, since it
happens before anything is on fire and belongs to onboarding and tabletop exercises, not
to a document you reach for during a live response.

## How to use it

Print it, laminate it, or keep it open on a second screen. If a line references an annex
or a tool such as the [Order Builder](../annexes/C-smesc-order-template.md), go there for
the full template rather than expecting this document to spell it out. The Job Aid points,
it does not explain.

## Structure

| File | Phase |
|---|---|
| `00-quick-reference.md` | Severity table, roles, links to the live tools |
| `01-identification.md` | Identification |
| `02-containment.md` | Containment |
| `03-eradication.md` | Eradication |
| `04-recovery.md` | Recovery |
| `05-lessons-learned.md` | Lessons Learned |

## On the tools referenced throughout

Several checklist lines point to a specific open source tool so the step reads as
something you can actually go and do, not just a doctrine statement. Four tools come up
repeatedly:

- **Security Onion**: a free network security monitoring platform bundling Suricata,
  Zeek, and the Elastic stack. Used for initial alerting and the underlying event data.
- **Kibana**: the search and dashboard layer sitting on top of that same Elastic stack.
  Worth noting this is not a separate platform from Security Onion, it is the interface
  you use to look at what Security Onion already collected. It is called out separately
  here because specific dashboards matter more than the platform name.
- **Velociraptor**: an open source endpoint visibility and digital forensics tool. Used
  for host isolation, artifact collection, and hunting across a fleet during containment
  and eradication.
- **Wireshark**: a packet capture and analysis tool. Used where confirmation at the
  packet level is needed, beyond what a log entry can tell you.

**These four are examples, not a requirement.** They were chosen because they are free,
widely deployed, and well documented, which makes this Job Aid usable by a team of any
size, including one with no security budget at all. The actual requirement in every
checklist line is the underlying task, for example identify a persistence mechanism, or
isolate a compromised host, not the specific tool named next to it.

If your organization runs a different stack, whether that is Splunk, Microsoft Sentinel,
CrowdStrike, Corelight, or something built in house, the same steps apply. Swap the tool
name, keep the task. Where a line reads "check the Alerts dashboard in Kibana," read it
as "check wherever your alerts actually land."

## Relationship to the Reference Plan

This Job Aid does not duplicate the Reference Plan's phase descriptions, battle procedure
mapping, or annexes. It is a distillation, not a summary, meaning content only appears
here if it changes what a responder does in the moment. Anything explanatory,
justificatory, or annex level detail stays in the Reference Plan where it belongs.

here if it changes what a responder does in the moment. Anything explanatory,
justificatory, or annex level detail stays in the Reference Plan where it belongs.
