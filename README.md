# Ron Swanson Quotes (ron-swanson-quotes)

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
