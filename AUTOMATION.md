# Content automation, with verification at each step

Miami This Week combines human-readable editorial decisions with repeatable checks. It does not present a found event, a generated image, a passing build, and a successful public deployment as the same kind of evidence.

## Schedule and roles

| Stage | What happens | What the result proves |
| --- | --- | --- |
| Daily local Codex heartbeat, 08:00 ET | The remaining current week is checked for additions, changes, cancellations, and ended events. | A completed research handoff can be reviewed; the schedule alone proves nothing about publication. |
| Sunday local Codex heartbeat, 11:00 ET | The following Monday–Sunday is researched more deeply. | This heartbeat was active as of 28 September 2026; its first real scheduled run was still pending. |
| Researcher · GPT-6 Astra, xhigh | Official organizer, venue, municipality, and ticket sources are checked; each dated event has an evidence record. | Source-backed facts and explicit uncertainty for the candidate agenda. |
| Visual · GPT-6 Sol, xhigh + integrated ImageGen | One original editorial illustration is generated and inspected for each current event. | An image asset and recorded visual review. The exact ImageGen model version is not exposed. |
| Developer · GPT-6 Sol, xhigh | Current and candidate listings are reconciled; data, evidence, image integrity, and static build gates run. | A release candidate ready for browser review and publication. |
| Publication | The static build is sent over SSH, with a backup of the previous site version and a rollback path. | Public checks confirm that the expected agenda, pages, calendars, and images are served. |

These heartbeats depend on the local Mac and Codex being available. If a run fails or a handoff is incomplete, the previous public site remains in place until the release checks pass.

## Editorial and technical gates

1. **Research:** Confirm the event's date, time, venue, address, and price or free-entry conditions against a concrete source. Track cancellations, sold-out sessions, and uncertainty. A currently running event remains listed only when a documented end proves it is still underway.
2. **Reconciliation:** Keep stable event IDs and existing images for unchanged listings. Mark verified new listings and time or venue corrections. Remove ended or invalid items from the next published data.
3. **Images:** Require one inspected original WebP per current event ID, with a manifest and matching SHA-256 hash. These are editorial illustrations, not documentary photos of future events or reused organizer artwork.
4. **Location:** Pin only verified exact addresses. An event without reliable coordinates remains findable in the agenda without a guessed map point.
5. **Release:** Validate the agenda against its evidence, build all static routes and calendar files, review representative pages in a browser, then publish with a backup. Check the public JSON and representative pages, images, calendars, and map again after the switch.

A successful data check is about structure and provenance; it does not establish visual quality. A successful build is local; it does not establish what the public server serves. Public HTTP responses and a JavaScript-enabled browser provide separate deployment evidence.

## What has been observed

On **28 September 2026**, the first daily heartbeat completed, added four verified events, and passed the integration and public checks. The published week then contained 34 dated events and 16 evergreen places. The Sunday heartbeat had not yet completed a scheduled run. The previously used site-curation timers were disabled after the Codex schedule became active; the separate newsletter process was not changed.

The site is updated from changing public sources. No snapshot guarantees that a future ticket will remain available or a price will remain unchanged. [Return to the showcase](README.md).
