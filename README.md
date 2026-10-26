# Ron Swanson Quotes (ron-swanson-quotes)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

A community-built, open source HTTP API that returns Ron Swanson quotes from the NBC television series Parks and Recreation. Returns one or more quotes per request as a JSON array of strings, with an optional case-insensitive full-text search over the quote corpus. The service is a small Node.js / TypeScript Express app authored by James Wright and hosted on Heroku.

**APIs.json:** [https://github.com/jamesseanwright/ron-swanson-quotes](https://github.com/jamesseanwright/ron-swanson-quotes)

## Tags

- Entertainment
- Television
- Parks and Recreation
- Quotes
- Open Source
- Public APIs
- Node.js
- TypeScript
- Heroku
- REST

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### Ron Swanson Quotes API

Read-only REST API returning random or searched Ron Swanson quotes as a JSON array of strings. No authentication is required. CORS is enabled (Access-Control-Allow-Origin is set to *) so the API can be called directly from browsers. Three endpoints are exposed at the /v2/ base path: GET /quotes returns a single random quote, GET /quotes/{count} returns N random quotes, and GET /quotes/search/{term} returns every quote that contains the given term (case-insensitive).

- **Human URL:** [https://github.com/jamesseanwright/ron-swanson-quotes#ron-swanson-quotes-api](https://github.com/jamesseanwright/ron-swanson-quotes#ron-swanson-quotes-api)
- **Base URL:** `https://ron-swanson-quotes.herokuapp.com/v2`

#### Tags

- Entertainment
- Television
- Quotes
- REST

#### Properties

- [Documentation](https://github.com/jamesseanwright/ron-swanson-quotes#ron-swanson-quotes-api)
- [OpenAPI](openapi/ron-swanson-quotes-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ron-swanson-quotes.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ron-swanson-quotes.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [API Reference](https://ron-swanson-quotes.herokuapp.com/v2/schema)
- [JSON Schema](json-schema/ron-swanson-quotes-quote-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/ron-swanson-quotes-quote-list-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/ron-swanson-quotes-rate-limit-error-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/ron-swanson-quotes-quote-structure.json)
- [JSON Structure](json-structure/ron-swanson-quotes-quote-list-structure.json)
- [JSON Structure](json-structure/ron-swanson-quotes-rate-limit-error-structure.json)
- [Example](examples/ron-swanson-quotes-quote-example.json)
- [Example](examples/ron-swanson-quotes-quote-list-example.json)
- [Example](examples/ron-swanson-quotes-rate-limit-error-example.json)

## Common Properties

- [GitHub Repository](https://github.com/jamesseanwright/ron-swanson-quotes)
- [Documentation](https://github.com/jamesseanwright/ron-swanson-quotes#ron-swanson-quotes-api)
- [Public APIs Listing](https://github.com/public-apis/public-apis)
- [Changelog](https://github.com/jamesseanwright/ron-swanson-quotes/blob/master/CHANGELOG.md)
- [Authentication](https://github.com/jamesseanwright/ron-swanson-quotes#ron-swanson-quotes-api)
- [Rate Limits](https://github.com/jamesseanwright/ron-swanson-quotes#ron-swanson-quotes-api)
- [SDK](https://github.com/jamesseanwright/hubot-swanson)
- [Code Examples](http://jsfiddle.net/7g2w4dhc/27/)
- [License](https://github.com/jamesseanwright/ron-swanson-quotes/blob/master/LICENCE)
- [Spectral Rules](rules/ron-swanson-quotes-rules.yml)
- [JSON-LD](json-ld/ron-swanson-quotes-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](vocabulary/ron-swanson-quotes-vocabulary.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
