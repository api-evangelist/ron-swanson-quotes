# Ron Swanson Quotes (ron-swanson-quotes)

A community-built, open source HTTP API that returns Ron Swanson quotes from the NBC television series Parks and Recreation. Returns one or more quotes per request as a JSON array of strings, with an optional case-insensitive full-text search over the quote corpus. The service is a small Node.js / TypeScript Express app authored by James Wright and hosted on Heroku.

**URL:** [Visit APIs.json URL](https://github.com/jamesseanwright/ron-swanson-quotes)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=opensource-api-evangelist&utm_content=repo)

## Status

- **x-type:** opensource
- **x-status:** deprecated
- **Reason:** Upstream GitHub repository was archived by the author on 2026-01-19 due to personal time constraints. The Heroku-hosted API endpoint (`https://ron-swanson-quotes.herokuapp.com/v2/quotes`) remains alive and responsive as of 2026-05-30, but no further code changes will be made and the service has no formal SLA. Treat as a community-maintained educational resource: useful for tutorials, learning projects, and demos, but not appropriate for production dependencies.

## Tags

 - Entertainment, Television, Parks and Recreation, Quotes, Open Source, Public APIs, Node.js, TypeScript, Heroku, REST

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### Ron Swanson Quotes API

Read-only REST API returning random or searched Ron Swanson quotes as a JSON array of strings. No authentication is required. CORS is enabled (`Access-Control-Allow-Origin: *`) so the API can be called directly from browsers. Three endpoints are exposed at the `/v2/` base path: `GET /quotes` returns a single random quote, `GET /quotes/{count}` returns N random quotes, and `GET /quotes/search/{term}` returns every quote that contains the given term (case-insensitive).

**Human URL:** [https://github.com/jamesseanwright/ron-swanson-quotes#ron-swanson-quotes-api](https://github.com/jamesseanwright/ron-swanson-quotes#ron-swanson-quotes-api)

**Base URL:** `https://ron-swanson-quotes.herokuapp.com/v2`

#### Tags

 - Entertainment, Television, Quotes, REST

#### Properties

- [Documentation](https://github.com/jamesseanwright/ron-swanson-quotes#ron-swanson-quotes-api)
- [OpenAPI](openapi/ron-swanson-quotes-openapi.yml)
- [APIReference - Live OpenAPI 3.0 Schema Endpoint](https://ron-swanson-quotes.herokuapp.com/v2/schema)
- [JSONSchema - Quote Schema](json-schema/ron-swanson-quotes-quote-schema.json)
- [JSONSchema - QuoteList Schema](json-schema/ron-swanson-quotes-quote-list-schema.json)
- [JSONSchema - RateLimitError Schema](json-schema/ron-swanson-quotes-rate-limit-error-schema.json)
- [JSONStructure - Quote JSON Structure](json-structure/ron-swanson-quotes-quote-structure.json)
- [JSONStructure - QuoteList JSON Structure](json-structure/ron-swanson-quotes-quote-list-structure.json)
- [JSONStructure - RateLimitError JSON Structure](json-structure/ron-swanson-quotes-rate-limit-error-structure.json)
- [Example - Quote Example](examples/ron-swanson-quotes-quote-example.json)
- [Example - QuoteList Example](examples/ron-swanson-quotes-quote-list-example.json)
- [Example - RateLimitError Example](examples/ron-swanson-quotes-rate-limit-error-example.json)
- [NaftikoCapability - Quotes Capability](capabilities/ron-swanson-quotes-quotes.yaml)

## Common Properties

- [GitHubRepository](https://github.com/jamesseanwright/ron-swanson-quotes)
- [Documentation](https://github.com/jamesseanwright/ron-swanson-quotes#ron-swanson-quotes-api)
- [PublicAPIsListing](https://github.com/public-apis/public-apis)
- [ChangeLog](https://github.com/jamesseanwright/ron-swanson-quotes/blob/master/CHANGELOG.md)
- [Authentication - No Authentication Required](https://github.com/jamesseanwright/ron-swanson-quotes#ron-swanson-quotes-api)
- [RateLimits - Per-Client Rate Limit Headers](https://github.com/jamesseanwright/ron-swanson-quotes#ron-swanson-quotes-api)
- [SDK - Hubot Swanson (npm) - Chatbot Integration by Author](https://github.com/jamesseanwright/hubot-swanson)
- [CodeExamples - Browser JavaScript Demo (JSFiddle)](http://jsfiddle.net/7g2w4dhc/27/)
- [License - Apache License 2.0](https://github.com/jamesseanwright/ron-swanson-quotes/blob/master/LICENCE)
- [SpectralRules - Ron Swanson Quotes Spectral Ruleset](rules/ron-swanson-quotes-rules.yml)
- [JSONLD - Ron Swanson Quotes JSON-LD Context](json-ld/ron-swanson-quotes-context.jsonld)
- [Vocabulary - Ron Swanson Quotes Vocabulary](vocabulary/ron-swanson-quotes-vocabulary.yml)

## Features

| Name | Description |
|------|-------------|
| Random Quote | Return a single random Ron Swanson quote as a one-element JSON array. |
| Batch Random Quotes | Return N random Ron Swanson quotes in a single response via `/quotes/{count}`. |
| Full-Text Search | Search the quote corpus for a substring with case-insensitive matching via `/quotes/search/{term}`; returns every matching quote. |
| No Authentication | Public endpoint with no API key, OAuth, or signup required. |
| CORS Enabled | `Access-Control-Allow-Origin` is set to `*` so the API can be called directly from any browser-based frontend without a proxy. |
| Self-Describing OpenAPI 3.0 Schema | Live OpenAPI 3.0 specification served by the API itself at `GET /v2/schema`, contributed by Chris Gali. |
| Rate Limit Headers | Standard `X-RateLimit-Limit` / `X-RateLimit-Remaining` / `X-RateLimit-Reset` headers are returned on every response. |

## Use Cases

| Name | Description |
|------|-------------|
| API Tutorial Fixture | Widely used in beginner Node.js, JavaScript, and HTTP tutorials and bootcamp coursework as a friendly, no-auth public API to learn fetch, async/await, and JSON parsing. |
| Voice Assistant Skill | Powers Alexa skills and other voice-assistant demos that deliver a Ron Swanson quote on request. |
| Chatbot Integration | Supplies the underlying quote source for Hubot, Slack, and Discord bot examples (see `hubot-swanson` npm package by the same author). |
| Frontend Demo App | CORS-enabled endpoint makes it suitable for in-browser SPA demos (React, Vue, Svelte) without requiring a backend proxy. |
| API Client Library Test Target | Stable shape and no auth make it a practical test target for HTTP-client libraries and SDK generators. |
| Workshop and Conference Demo | Used in conference talks and workshops to illustrate REST, OpenAPI-from-code, and API mocking concepts. |

## Integrations

| Name | Description |
|------|-------------|
| Hubot | Official Hubot script (`hubot-swanson`, by the API author) that pulls quotes into Hubot-powered chatops bots. |
| Heroku | Service is deployed on the Heroku platform; the production host is `ron-swanson-quotes.herokuapp.com`. |
| Alexa Skills | Multiple community-built Amazon Alexa skills consume this API to read Ron Swanson quotes on Echo devices. |
| Slack and Discord Bots | Used as a quote source by various community chatbots. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Ron Swanson Quotes API](openapi/ron-swanson-quotes-openapi.yml)

### JSON Schema

- [Quote](json-schema/ron-swanson-quotes-quote-schema.json)
- [QuoteList](json-schema/ron-swanson-quotes-quote-list-schema.json)
- [RateLimitError](json-schema/ron-swanson-quotes-rate-limit-error-schema.json)

### JSON Structure

- [Quote](json-structure/ron-swanson-quotes-quote-structure.json)
- [QuoteList](json-structure/ron-swanson-quotes-quote-list-structure.json)
- [RateLimitError](json-structure/ron-swanson-quotes-rate-limit-error-structure.json)

### JSON-LD

- [Ron Swanson Quotes Context](json-ld/ron-swanson-quotes-context.jsonld)

### Examples

- [Quote](examples/ron-swanson-quotes-quote-example.json)
- [QuoteList](examples/ron-swanson-quotes-quote-list-example.json)
- [RateLimitError](examples/ron-swanson-quotes-rate-limit-error-example.json)

## Capabilities

Naftiko capabilities organized as self-contained, per-tag definitions exposing both REST and MCP adapters.

| Capability | API | Tools | Operations |
|------------|-----|-------|------------|
| [Quotes](capabilities/ron-swanson-quotes-quotes.yaml) | Ron Swanson Quotes API | 3 | `getRandomQuote`, `getRandomQuotes`, `searchQuotes` |

## Vocabulary

- [Ron Swanson Quotes Vocabulary](vocabulary/ron-swanson-quotes-vocabulary.yml) - Unified taxonomy mapping 1 resource, 3 actions, 1 workflow, and 3 personas across operational (OpenAPI) and capability (Naftiko) dimensions.

## Rules

- [Ron Swanson Quotes Spectral Ruleset](rules/ron-swanson-quotes-rules.yml) - 32 rules across 12 categories enforcing Ron Swanson Quotes API conventions (title prefix, kebab-case paths, camelCase operationIds, snake_case parameters, HTTPS servers, mandatory 2xx and 429 responses, Microcks extensions).

## Notes

This entry was initially bulk-registered as part of a public-apis catalog sweep on 2026-05-28 and enriched on 2026-05-30 via the API Evangelist opensource pipeline. The upstream OpenAPI 3.0 specification was authored by Chris Gali and is served live by the API itself at `GET /v2/schema`; the version stored in this repo adds operationIds, tags, named examples, rate-limit headers, the 429 error response, and Microcks extensions on top of the canonical document.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com

## Upstream Author

**FN:** James Wright

**URL:** [https://james.engineering](https://james.engineering)

**GitHub:** [https://github.com/jamesseanwright](https://github.com/jamesseanwright)
