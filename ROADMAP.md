# NoMore — Roadmap / Feuille de route

**Status: planning.** This document describes intended work, not delivered functionality or a guaranteed schedule.

**Statut : préparation.** Ce document présente les travaux envisagés, et non des fonctionnalités livrées ou un calendrier garanti.

## Current documented decisions / Décisions documentées

- Focus: self-monitoring, motivation and orientation; no diagnostic or treatment service.
- Initial sequence: alcohol, tobacco, gambling.
- Initial language targets: French, English, Spanish.
- Proposed foundation: PHP, MySQL/MariaDB, HTML/CSS/JavaScript.
- Intended free-access service; published project material under AGPL-3.0-only, with third-party notices preserved. Application implementation and release preparation remain pending.

## Milestone 1 — Publish a trustworthy foundation

- [ ] Verify that LICENSE contains the complete GNU AGPL v3 text and that project notices consistently specify AGPL-3.0-only.
- [ ] Document the actual rights holders and review the origin and licence compatibility of every component before adding application code.
- [ ] Define release scope, repository structure and contribution process.
- [ ] Define data categories, access boundaries, retention and deletion requirements.
- [ ] Review safety wording and support-resource selection with appropriate expertise.
- [ ] Define hosting, operational responsibility, incident handling and legal requirements before collecting real personal data.

## Milestone 2 — Build and verify the shared application

- [ ] Implement accounts, authentication, account recovery and administrative roles.
- [ ] Verify cross-account isolation and least-privilege access.
- [ ] Implement the multilingual interface and separate language/country settings.
- [ ] Build the responsive design system, daily journal and accessible chart components.
- [ ] Implement transparent consent records, user exports and deletion workflows.
- [ ] Add automated tests, dependency checks and a documented deployment procedure.

## Milestone 3 — Alcohol module first

- [ ] Specify quantities, units and personal baseline handling.
- [ ] Distinguish missing records from explicit zero-consumption entries.
- [ ] Implement descriptive trends and clearly labelled financial estimates.
- [ ] Review all safety wording and country-specific orientation resources.
- [ ] Test the module without any automated withdrawal or medication recommendation.

## Milestone 4 — Tobacco module

- [ ] Specify self-reported quantities and configurable costs.
- [ ] Implement baseline comparisons and non-judgmental progress summaries.
- [ ] Separate general, sourced information from individual measurements.
- [ ] Verify accessibility, translations and calculation edge cases.

## Milestone 5 — Gambling module

- [ ] Specify spending, deposits, withdrawals and losses without conflating them.
- [ ] Implement optional time, urge and goal tracking.
- [ ] Avoid speculative claims about savings or recovered losses.
- [ ] Exclude wagering advice, variable rewards and gambling-style animations.
- [ ] Review country-appropriate help and voluntary exclusion resources.

## Milestone 6 — Prepare a limited public release

- [ ] Complete security and privacy review appropriate to the actual implementation.
- [ ] Check language quality, accessibility and visual behaviour on mobile and desktop.
- [ ] Test backup restoration, access recovery, exports, deletion and incident procedures.
- [ ] Publish installation instructions, release notes and known limitations.
- [ ] Define a limited deployment scope before wider international availability.

No milestone is declared completed solely because it appears in this document. Progress must be evidenced by the corresponding code, tests, reviews or published documents.
