[← Back to portfolio](README.md)

# Aureon
## Translating a business proposition into a digital experience

**Focus:** Business positioning · Requirements · Customer journey · Product review  
**Status:** Institutional website implemented; access remains private. SaaS initiatives have separate development cycles.

## The business problem

Aureon combines consulting, workflow improvement, and digital products. Presenting it only as an AI provider would obscure the broader business proposition. Visitors also need a clear distinction between services they can discuss and products still being developed.

## My contribution

I defined the intended positioning, requested revisions to the visitor experience, specified the business assessment fields, and reviewed the product presentation. Development used AI-assisted tools; this case does not claim independently hand-coded implementation.

## Decisions and their rationale

| Decision | Business rationale | Implementation evidence |
|---|---|---|
| Use “Business Transformation, AI Workflows & Vertical SaaS” | Explain the relationship between consulting and technology | Shared navigation, service descriptions, and page metadata |
| Move About us to a separate page | Keep the Home focused while retaining institutional context | Dedicated `/about` route, without founder biography |
| Make products selectable | Let visitors explore relevant initiatives without an overly long catalogue | Five product tabs with audience, focus, and development status |
| Add a structured assessment | Gather context for a focused first conversation | `/contact` form with industry, needs, and challenge fields |
| Make motion controllable | Support engagement without forcing movement | Motion toggle, reduced-motion rules, and keyboard-accessible tabs |

## A concrete visitor journey

A cleaning-business owner can explore the industry example, review the direction of Track&Go, and open the assessment form. The form accepts business details, selected needs, and a description of the current challenge.

The implementation sends a JSON request to `POST /api/assessment`, applies basic server validation, and inserts the record into a Cloudflare D1 table. It has success and error states. It does not yet notify a sales team or create a product account.

## Evidence inventory

| Artifact | What it shows |
|---|---|
| `app/motion-experience.tsx` | Strategy, Workflows, and Software exploration; sequential service presentation |
| `app/experience.tsx` | Product, method, industry, and business-education interactions |
| `app/contact/page.tsx` | Structured business intake and response states |
| `app/api/assessment/route.ts` | Basic validation and persistence |
| `db/schema.ts` | Assessment lead data model |

These references describe the inspected website source. They are not links to publicly released source files. Snapshot: `50949e50077f6ce5ff759666d26557fdec87d534`.

## What is established

The website build completed, and version 10 was successfully published on September 13, 2026. That establishes delivery of the website, not customer adoption or financial impact.

## What remains to evaluate

- End-to-end intake behavior with a confirmed test record.
- Mobile, keyboard, and visual review of the published experience.
- Lead management and notification requirements.
- Completion rate and quality of submitted assessments once appropriate measurement is implemented.

**No conversion uplift, revenue impact, or customer results are claimed.**

## What this work demonstrates

The ability to connect positioning, user needs, implementation requirements, and review decisions in one business initiative.

[← Back to portfolio](README.md)
