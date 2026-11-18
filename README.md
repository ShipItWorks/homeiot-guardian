# HomeIoT Guardian

Guided checks of your home Wi-Fi settings, a scan for devices that announce themselves, and a checklist to harden each one.

**Score: 66 / 100** on our own [rubric](https://shipitworks.com/how-we-score/). Stage: Beta. Scored 2026-11-12; this record was updated 2026-11-18 from the [product page](https://shipitworks.com/homeiotguardian/).

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
- No feature label rests on a run log from a phone or a real network: five are built and tested with sample data on a desktop JVM, one (PDF export) is not tested yet
- One scan on a real phone and home network is recorded in the repo (proof/real-phone-scan.txt, written by floor/r1.sh on 2026-11-11: Pixel 8 Pro, 2 devices listed, 0 mDNS services resolved); it was read, not re-run, on 2026-11-18. The PDF render and the notification prompt on a phone were not checked
- The PDF export attempt on the JVM failed (4 of 4 tests, 2026-11-07); it needs a device or an instrumented test
- README links proof/upnp-fetch-http.log and proof/port-connect-sockets.log; neither is on main at 8ebed11
- 12x14 closed test not started per repo docs; no signed .aab built here (no upload key on this machine)
- A LICENSE file is on main since PR #29 (e57bab7, 2026-11-11); README.md line 5 at e57bab7 still says no license has been chosen, and the licence is held for the owner; no user guide beyond the release docs; lintDebug exit 1 on a ByteOrderMark false positive was reported earlier and not re-run
- TalkBack, contrast and large-font checks not run; no reduced-motion setting in the app
- Network use not yet traced on a phone (no network capture of the app on a real network); the base network config turns plain HTTP off (checked at d96164b on 2026-11-18)

## What changed

- 2026-11-18: A review at commit d96164b corrected three lines here: the base network config turns plain HTTP off, one real-phone scan is recorded in the repo, and the open-port check has run on an emulator. The one-line description now says the Wi-Fi checks are guided. No feature label or score changed.
- 2026-11-11: Merged into the app: when you mark a guided check Completed you can now pick the day you really did it, and the device page shows that day (it showed the day in UTC before); a device that announced no brand or operating system is now read through its own SSH greeting and web page, and the scan shows what they name and where it was read; and the real-phone scan record gained a scan started from the Scan button on the screen. Proof scripts and automated checks for these were added. They were read by path and diff only and not run in this scorecard round, so no feature label or score changed (PRs #34, #36 and #40). Scorecard rows: "Guided device checks + tasks list + readiness score" (works true, Tested with sample data) covers the completed-day picker, and "Wi-Fi/router posture, mDNS+SSDP LAN scan, UPnP check" (works true, Tested with sample data) covers the scan; reading brand and operating system from the SSH greeting and web page is not scored (no row covers it).
- 2026-11-11: A LICENSE file was added to the repository (PR #29); the file says all rights are reserved (text in ev/homeiotguardian-contents-LICENSE-e57bab7.txt; the repository is private, so this says what the file says). This scorecard does not state its terms, and no feature label or score changed. Not scored: no scorecard row covers a licence file.
- 2026-11-11: Merged into the app: a router check, a wider open-port check and a new-device alert; unencrypted traffic is switched off in the app's network settings; and a sample exported PDF, a packet trace and a log of one scan on a real phone were added as records. No feature label or score changed (PRs #33, #28 and #27).
- 2026-11-10: Site copy only: a dated correction now sits under the demo video for the narration line at 2:20, and the privacy policy page on this site shows 'not from internet addresses' with a limit beside it. No code or score change.
- 2026-11-10: Land PR #26 merged into main as 8ebed11 (11 lane PRs included); no feature label changed this round. Tagged v0.2.0 at 8ebed11.

See [CHANGELOG](CHANGELOG.md).

## Demo

[Transcript of the demo (1:50)](https://shipitworks.com/homeiotguardian/transcript/) · video on the [product page](https://shipitworks.com/homeiotguardian/)

The demo voice is AI-generated (ElevenLabs, "Bella") and the demo shows made-up data. The video says so at the end.

## Source code

The source is private for now. This repository holds the public record for the product: this README and a CHANGELOG, and soon a LICENSE. Until the source is public, the [product page](https://shipitworks.com/homeiotguardian/) is the source of truth, and the score above is the one to trust.

## How we work

Say only what we can back. Say what is not finished before anyone asks. Name people, companies and tools to give credit. Collect as little data as possible. We use AI and say so: Claude (by Anthropic) helps write the code and wrote this README.

Full version: [github.com/ShipItWorks](https://github.com/ShipItWorks) · Contact: support@shipitworks.com

---

Drafted with Claude (Anthropic) from the product page on 2026-11-02. Owner review by Robert Sweetman: pending.
