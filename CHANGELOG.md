# Changelog

Public record of changes to HomeIoTGuardian, written from the product page on shipitworks.com. The source is private. Format: [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). Release tags exist on the private repository's default branch.

## 2026-11-08 (release v0.1.3)

- 2026-11-08: Rescored under the per-feature rule: no core feature has a run log on main, so five count as built and tested with sample data (half share each) and the PDF export counts as not tested yet. 66/100 on our own rubric (was 73). Release tag v0.1.3.
- 2026-11-08: The UPnP description fetch now has tests of its HTTP behaviour over local sockets (PR #24, tag v0.1.3); the log it points to is not on main. CI now runs on the self-hosted runner (PR #23).

Score 66 / 100 on our own rubric, scored 2026-11-08. Product page: https://shipitworks.com/apps/#HomeIoTGuardian

## 2026-11-07 (release v0.1.2)

- The public contact is now support@shipitworks.com in the privacy policy, the Play listing draft and the project site pages, and the README has an AI use section. Release v0.1.2.
- A recorded attempt to run the PDF export in a JVM test failed (4 of 4 tests, in three graphics modes). The PDF export is still not proven; it needs a device or an instrumented test.

Score 73 / 100 on our own rubric, scored 2026-11-01; no score or proof label changed in this update. Product page: https://shipitworks.com/homeiotguardian/
