# HomeIoT Guardian

Audit home Wi-Fi security, discover smart devices, harden your connected home.

**Score: 73 / 100** on the [ShipItWorks rubric](https://shipitworks.com/how-we-score/). Stage: Beta. As of 2026-11-02, from the [product page](https://shipitworks.com/apps/#HomeIoTGuardian).

Every number on the product page names the file it came from. The lists below are copied from that page, not rewritten.

**Platform.** Android. Not on Google Play yet.

## What works today

- Guided device checks + tasks list + readiness score
- JSON backup/restore, data erase
- Review reminders (WorkManager)
- Catalog seed + Room migration

## Not done yet

- Not run on a device or a real LAN this pass: the mDNS/SSDP scan, the PDF render and the notification prompt
- 12x14 closed test not started per repo docs; no signed .aab built here
- No user guide beyond the release docs; lintDebug still exits 1
- TalkBack, contrast and large-font checks never run; no reduced-motion setting in the app

## Demo

[Transcript of the demo (2:55)](https://shipitworks.com/homeiotguardian/transcript/) · video on the [product page](https://shipitworks.com/apps/#HomeIoTGuardian)

The demo voice is AI-generated (ElevenLabs, "Alice") and the demo shows made-up data. The video says so at the end.

## Source code

The source is private for now. This repository holds the public record for the product: this README, and soon a CHANGELOG and LICENSE. Until the source is public, the [product page](https://shipitworks.com/apps/#HomeIoTGuardian) is the source of truth, and the score above is the one to trust.

## How we work

Say only what we can back. Say what is not finished before anyone asks. Name people, companies and tools to give credit. Collect as little data as possible. We use AI and say so: Claude (by Anthropic) helps write the code and wrote this README.

Full version: [github.com/ShipItWorks](https://github.com/ShipItWorks) · Contact: support@shipitworks.com

---

Drafted with Claude (Anthropic) from the product page on 2026-11-02. Owner review by Robert Sweetman: pending.
