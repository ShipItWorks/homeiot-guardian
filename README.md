# HomeIoT Guardian

Audit home Wi-Fi security, discover smart devices, harden your connected home.

**Score: 66 / 100** on our own [rubric](https://shipitworks.com/how-we-score/). Stage: Beta. Scored 2026-11-08; this record was updated 2026-11-08 from the [product page](https://shipitworks.com/apps/#HomeIoTGuardian).

Every number on the product page names the file it came from. The lists below are copied from that page, not rewritten.

**Platform.** Android. Not on Google Play yet.

## What works today

- Wi-Fi/router posture, mDNS+SSDP LAN scan, UPnP check (Tested with sample data)
- Guided device checks + tasks list + readiness score (Tested with sample data)
- JSON backup/restore, data erase (Tested with sample data)
- Review reminders (WorkManager) (Tested with sample data)
- Catalog seed + Room migration (Tested with sample data)

## Not done yet

- Readiness report / PDF export (Not tested yet)
- No feature has a proof log on main: five are built and tested with sample data on a desktop JVM, one (PDF export) is not tested yet
- Not run on a phone or a real home network: the mDNS/SSDP scan, the router port check, the PDF render and the notification prompt
- The PDF export attempt on the JVM failed (4 of 4 tests, 2026-11-07); it needs a device or an instrumented test
- README links proof/unit-tests.log, proof/catalog-counts.log and proof/upnp-fetch-http.log; none of the three is on main
- 12x14 closed test not started per repo docs; no signed .aab built here (no upload key on this machine)
- No CHANGELOG and no LICENSE file on main; no user guide beyond the release docs; lintDebug exit 1 on a ByteOrderMark false positive was reported earlier and not re-run
- TalkBack, contrast and large-font checks not run; no reduced-motion setting in the app
- Network use not yet traced (no network capture); cleartext traffic is permitted in the base network config

## What changed

- 2026-11-08: Rescored under the per-feature rule: no core feature has a run log on main, so five count as built and tested with sample data (half share each) and the PDF export counts as not tested yet. 66/100 on our own rubric (was 73). Release tag v0.1.3.
- 2026-11-08: The UPnP description fetch now has tests of its HTTP behaviour over local sockets (PR #24, tag v0.1.3); the log it points to is not on main. CI now runs on the self-hosted runner (PR #23).
- 2026-11-07: The public contact is now support@shipitworks.com in the privacy policy, the Play listing draft and the project site pages, and the README has an AI use section. Release v0.1.2.
- 2026-11-07: A recorded attempt to run the PDF export in a JVM test failed (4 of 4 tests, in three graphics modes). The PDF export is still not proven; it needs a device or an instrumented test.

See [CHANGELOG](CHANGELOG.md).

## Demo

[Transcript of the demo (2:55)](https://shipitworks.com/homeiotguardian/transcript/) · video on the [product page](https://shipitworks.com/apps/#HomeIoTGuardian)

The demo voice is AI-generated (ElevenLabs, "Alice") and the demo shows made-up data. The video says so at the end.

## Source code

The source is private for now. This repository holds the public record for the product: this README and a CHANGELOG, and soon a LICENSE. Until the source is public, the [product page](https://shipitworks.com/apps/#HomeIoTGuardian) is the source of truth, and the score above is the one to trust.

## How we work

Say only what we can back. Say what is not finished before anyone asks. Name people, companies and tools to give credit. Collect as little data as possible. We use AI and say so: Claude (by Anthropic) helps write the code and wrote this README.

Full version: [github.com/ShipItWorks](https://github.com/ShipItWorks) · Contact: support@shipitworks.com

---

Drafted with Claude (Anthropic) from the product page on 2026-11-02. Owner review by Robert Sweetman: pending.
