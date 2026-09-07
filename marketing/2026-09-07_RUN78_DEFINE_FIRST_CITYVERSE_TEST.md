# RUN78 — CV-TXT-001: Define Your First CityVerse Test

## Customer Truth

The previous waitlist flow did not write a durable request. It changed local UI state and then told the visitor they were officially a founding member while displaying unverified benefits such as locked pricing, lifetime discounts, priority event access, and a direct product-team line. That was not a trustworthy conversion state.

CityVerse should qualify the first experience or commercial proof point a visitor wants to test, then keep membership activation, event inventory, partnership acceptance, investment activity, payment, and entitlement as separate verified states.

## Creative Strategy

**Hook:** Do not join a generic waitlist. Tell CityVerse what it would need to prove for you first.

**CTA:** Record My CityVerse Test.

The flow asks for role, one experience/proof point, decision timing, optional organization context, optional illustrative membership tier interest, and optional marketing consent.

## Production Readiness

A new durable Base44 entity `CityVerseInterest` was created. Required fields are email, role, and `experience_to_test`; it also stores organization, illustrative tier interest, decision window, marketing consent, attribution, submission timestamp, and an internal review status that does not imply acceptance.

`src/pages/Waitlist.jsx` now creates the durable request before success is shown. On success the product says **Interest recorded** and explicitly states that the record is not membership activation, event reservation, partnership acceptance, an investment offer, a purchase, or an entitlement.

- Base44 app: `6a199815362bdb480622c17d`
- Sandbox build: exit `0`
- Checkpoint: `6a9ef38b52b3b57de593bced`
- Base44 commit: `bebf8761534dbd7c4cde27704b7b639033f7aa0f`

## Distribution Queue

The WCL vault asset is approved and unpublished. CityVerse currently has 0/81 Base44 connectors connected, so no authenticated external distribution was attempted or claimed.

## Analytics / Evaluation

Fresh `CityVerseInterest` baseline after instrumentation: **0 durable requests**. This is a new empty measurement baseline, not evidence that market demand is zero.

The first meaningful conversion is a successfully persisted qualified-interest record. Future evaluation should segment Fan, Creator, Brand, and Investor intent and measure progression separately into human review, verified partner/pilot discussion, and any later commercial state.

## Winner Library

No CityVerse winner is declared from a newly instrumented zero-request baseline. A winner requires attributable production traffic and comparable samples.

## Claims Boundary

A request is not founding-member status. A selected tier is not a purchase. A partner role is not partnership acceptance. A concept event is not live inventory. A sandbox build is not production deployment.

## Source-of-Truth Exception

The `Willie2728/Cityverse-AI` README identifies this repository as the canonical source of truth for the current CityVerse Live Base44 application, but GitHub code search did not expose the matching Waitlist application source. No guessed path was written. Base44↔GitHub application-source parity remains a Build Liaison blocker.
