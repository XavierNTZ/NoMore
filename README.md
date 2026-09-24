# NoMore

**Make progress visible. Move forward without judgment.**

[Présentation en français](README.fr.md) · [Roadmap](ROADMAP.md) · [Architecture proposal](ARCHITECTURE.md) · [Contributing](CONTRIBUTING.md)

NoMore is an early-stage project for a free-access, multilingual platform focused on **self-monitoring, motivation and finding appropriate support** for people concerned about addictive behaviours.

The initial development order is **alcohol, then tobacco, then gambling**.

## Current status

This repository currently documents the project vision and proposed development requirements. It does **not** yet provide an installable NoMore application, an operational support service or a clinically validated intervention.

All application features described below are **planned**, not implemented or verified by this documentation. The project does not claim an established user community, adoption metrics, a security certification or medical effectiveness.

An open-source release is intended. The licence remains to be selected and added; see [Licensing status](LICENSING.md).

## Why this project

The aim is to help people see changes in their own habits over time, rather than reduce their experience to a single success-or-failure counter.

A private daily journal, understandable charts and transparent spending comparisons could make those changes easier to recognise. The design should support returning after a difficult day without shame, competitive rankings or an erased history.

NoMore is intended to complement access to professional support, not replace it.

## Planned first modules

| Order | Module | Intended scope |
| --- | --- | --- |
| 1 | Alcohol | Self-reported consumption, personal trends, spending estimates, optional notes and country-appropriate support resources. No automated withdrawal plan. |
| 2 | Tobacco | Self-reported use, comparisons with a personal baseline, transparent cost estimates and supportive progress summaries. |
| 3 | Gambling | Self-reported spending, time spent, urges and personal goals, with links to appropriate support. No betting tips, gambling promotion or claims about recovering losses. |

Shared planned features include a personal account, a short daily journal, an accessible dashboard, user-selected goals, data export and deletion, and an administration interface for approved content, translations and resources.

Missing entries must remain distinguishable from days with no consumption or gambling. Financial estimates must explain their assumptions and must not be described as money actually saved without the necessary evidence.

## International access

French, English and Spanish are the first planned interface languages. Additional languages are an extension goal, not currently available versions.

Language and country will be separate settings. Currencies, dates, time zones, measurement units and support resources need appropriate localisation. Safety-related content requires review, not only automatic translation.

The ambition is international access; availability in every country is not yet promised.

## Privacy and safety requirements

The intended design is to minimise collection, allow a pseudonym where appropriate, restrict administrative access, and give users control over their records.

Real personal records, credentials, database dumps and private configuration must never be published in this repository. Development examples and tests must use clearly labelled synthetic data.

NoMore is not intended to diagnose, prescribe, calculate personalised life expectancy or recommend unsupervised withdrawal. Health-related wording and referral resources require qualified review before a public launch.

No advertising trackers, session recording or behavioural marketing integrations are planned inside personal tracking areas.

These are development requirements, not claims of completed implementation, legal compliance or security certification.

## Proposed technical direction

The proposed foundation is a structured PHP application, MySQL/MariaDB, semantic HTML, modern CSS and lightweight JavaScript.

The objectives are a responsive and accessible interface, modest deployment requirements, documented installation, and maintainable code. Application security should use maintained, reviewed mechanisms rather than invented cryptography.

See [ARCHITECTURE.md](ARCHITECTURE.md) for the proposal and the decisions still to be resolved.

## Open development

Useful early contributions include feedback on requirements, accessibility, localisation, documentation and privacy or safety design. Future implementation work should follow published scope, tests and review criteria.

Please read [CONTRIBUTING.md](CONTRIBUTING.md) before contributing and [SECURITY.md](SECURITY.md) before sharing security-related information.

## Project stewardship

Project initiated by **Xavier**, using the GitHub account **XavierNTZ**.

Public repository discussions must not contain personal health histories or requests for urgent assistance. This repository is a software-development space, not a care or emergency service.
