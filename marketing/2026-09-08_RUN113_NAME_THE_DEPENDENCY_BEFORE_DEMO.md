# RUN113 · CityVerse Live · Name the Dependency Before the Demo

## Customer Truth
An immersive-experience idea is not a runnable test merely because the buyer can describe the experience and success signal. Live feeds, venue/media rights, commerce rails, inventory, partner APIs, or a deliberately synthetic/owned demo environment can be hard external dependencies. If that dependency is hidden until after contact, qualified interest gets confused with execution readiness.

## Creative Strategy
**CV-TXT-005 — “Name the dependency before the demo.”**

Buyer-facing frame: **One Proof Point · One Signal · One Receipt · One Dependency.** Define the first experience, the observation that earns a second step, the evidence category that would make the result inspectable, and what must be true before the test is actually runnable.

## Production Readiness
The CityVerse first-test flow now requires one structured dependency before the brief is scope-ready:
- owned / synthetic demo can run without external rights;
- venue, media, or event rights must be confirmed;
- a live feed / camera source must be available;
- commerce or payment rails must be available;
- a partner integration / API must be available; or
- not sure yet — dependency review is part of the next step.

`CityVerseScopeSignal` stores the structured dependency with `brief_copy` and `review_request_click` events, but not the visitor's free-text experience or email. `CityVerseInterest` carries the same dependency only after explicit private-review intent.

## Distribution Queue
Production-ready for owned buyer/creator/brand/investor qualification. Do not claim a live demo, feed, right, partnership, payment rail, inventory source, event reservation, or public campaign without a provider or external receipt.

## Analytics / Evaluation
RUN113 baseline: **0 CityVerseScopeSignal records and 0 CityVerseInterest records**. Evaluate which dependency types appear with no-contact brief copies and later durable review requests before expanding acquisition spend.

## Winner Library
No winner promoted. There is no production conversion denominator in the reviewed CityVerse records.

## Claims Boundary
A selected dependency is a planning gate, not proof the dependency is resolved. A copied brief or review request does not establish live inventory, rights, feed access, commerce capability, partnership acceptance, payment, membership, reservation, or production availability.

## Market Context
IBM reported on August 24, 2026, from a survey of 20,589 sports fans, that fans increasingly want reliable connected experiences while 39% reported frustration managing multiple sports subscriptions. The same study reported app-based purchases for tickets, food/beverage, and merchandise among portions of respondents. That supports reducing friction and making experience dependencies explicit; it does not establish CityVerse demand or capability.

## Build Receipt
Base44 checkpoint: `6aa0b693c4b1bcea1ecd75df`
Base44 commit: `404d28b9708df62c8efde2c20165e64367f2531e`
Final build: `npm run build` from `/app` exited `0`; stale Browserslist/caniuse-lite warning only.

## Source-Parity Note
The connected `Willie2728/Cityverse-AI` repository contains README and durable marketing records but not the active Base44 React application tree. RUN113 therefore does not claim Base44↔GitHub application-source parity.