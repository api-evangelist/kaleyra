# Kaleyra (kaleyra)

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

Kaleyra is a global omnichannel CPaaS provider (a Tata Communications company since October 2023) offering SMS, WhatsApp, RCS, Voice, Email, Verify (OTP), and Video communication APIs. Its REST APIs authenticate with an api-key header, address accounts by SID in the path, and are served from region-specific hosts for India, APAC, and EU data residency.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/apis.yml)

## Tags

- CPaaS
- Messaging
- SMS
- WhatsApp
- Voice
- OTP
- India

## Timestamps

- **Created:** 2026-07-17
- **Modified:** 2026-07-17

## APIs

### Kaleyra SMS API

Send single and bulk SMS (MKT/TXN/OTP) via POST /v2/{sid}/messages, manage sender IDs and templates, and pull delivery status and logs. India DLT entity/template fields are supported.

- **Human URL:** [https://developers.kaleyra.io/docs/sms-api](https://developers.kaleyra.io/docs/sms-api)
- **Base URL:** `https://api.kaleyra.io`

#### Tags

- SMS
- Messaging
- OTP

#### Properties

- [Documentation](https://developers.kaleyra.io/docs/sms-api)
- [API Reference](https://developers.kaleyra.io/reference/single-sms-api)
- [OpenAPI](openapi/kaleyra-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kaleyra.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Kaleyra WhatsApp API

Send WhatsApp Business messages (text, media, interactive, template) over the WhatsApp API V2, with number registration, template management, group management, and WhatsApp Payment support.

- **Human URL:** [https://developers.kaleyra.io/docs/whatsapp-api-v2-overview](https://developers.kaleyra.io/docs/whatsapp-api-v2-overview)
- **Base URL:** `https://api.kaleyra.io`

#### Tags

- WhatsApp
- Messaging
- Templates

#### Properties

- [Documentation](https://developers.kaleyra.io/docs/whatsapp-api-v2-overview)
- [API Reference](https://developers.kaleyra.io/reference/whatsapp-messages-api-v2-overview)
- [OpenAPI](openapi/kaleyra-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kaleyra.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Kaleyra RCS API

Send Rich Communication Services (RCS) messages, manage brands and agents, handle templates, and perform device capability lookups.

- **Human URL:** [https://developers.kaleyra.io/docs/rcs-overview](https://developers.kaleyra.io/docs/rcs-overview)
- **Base URL:** `https://api.kaleyra.io`

#### Tags

- RCS
- Messaging
- Rich Messaging

#### Properties

- [Documentation](https://developers.kaleyra.io/docs/rcs-overview)
- [OpenAPI](openapi/kaleyra-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kaleyra.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Kaleyra Voice API

Click-to-call bridging via POST /v1/{sid}/voice/click-to-call, outbound calling campaigns, call log pull, and call recording extraction.

- **Human URL:** [https://developers.kaleyra.io/docs/voice-api](https://developers.kaleyra.io/docs/voice-api)
- **Base URL:** `https://api.kaleyra.io`

#### Tags

- Voice
- Click to Call
- IVR

#### Properties

- [Documentation](https://developers.kaleyra.io/docs/voice-api)
- [API Reference](https://developers.kaleyra.io/docs/click-to-call-api)
- [OpenAPI](openapi/kaleyra-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kaleyra.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Kaleyra Verify (OTP) API

Generate and validate one-time passwords via POST /v1/{sid}/verify, with configurable multichannel verification flows (SMS, WhatsApp, Voice) and Verify templates.

- **Human URL:** [https://developers.kaleyra.io/docs/generating-otp](https://developers.kaleyra.io/docs/generating-otp)
- **Base URL:** `https://api.kaleyra.io`

#### Tags

- OTP
- Verify
- Two Factor

#### Properties

- [Documentation](https://developers.kaleyra.io/docs/generating-otp)
- [OpenAPI](openapi/kaleyra-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kaleyra.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Kaleyra Email API

Send single and batch transactional email (Email API v2) with domain management, templates, webhooks, and delivery statistics.

- **Human URL:** [https://developers.kaleyra.io/reference/email-api-v2-overview](https://developers.kaleyra.io/reference/email-api-v2-overview)
- **Base URL:** `https://api.kaleyra.io`

#### Tags

- Email
- Transactional Email

#### Properties

- [Documentation](https://developers.kaleyra.io/reference/email-api-v2-overview)
- [API Reference](https://developers.kaleyra.io/reference/email-api-v2-send-a-single-email)

### Kaleyra Video API

Create and orchestrate WebRTC video rooms via the Kaleyra Video REST API (POST /v2/rooms), plus recording, transcription, e-signature, and Web/Android/iOS SDK integration.

- **Human URL:** [https://developers.kaleyra.io/reference/video-make-a-video-call-with-rest-api](https://developers.kaleyra.io/reference/video-make-a-video-call-with-rest-api)
- **Base URL:** `https://api.kaleyra.io`

#### Tags

- Video
- WebRTC
- Conferencing

#### Properties

- [Documentation](https://developers.kaleyra.io/reference/video-make-a-video-call-with-rest-api)
- [API Reference](https://developers.kaleyra.io/reference/video-v2-roomcall-postl)
- [OpenAPI](openapi/kaleyra-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/kaleyra.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Kaleyra Platform API

Account-level platform operations - subaccount management, billing, numbers provisioning, callback profiles, consent, and blocklist management.

- **Human URL:** [https://developers.kaleyra.io/reference/api-reference-overview](https://developers.kaleyra.io/reference/api-reference-overview)
- **Base URL:** `https://api.kaleyra.io`

#### Tags

- Platform
- Subaccounts
- Billing

#### Properties

- [Documentation](https://developers.kaleyra.io/reference/api-reference-overview)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/kaleyra)
- [Website](https://www.kaleyra.com/)
- [Documentation](https://developers.kaleyra.io/)
- [Plans](plans/kaleyra-plans-pricing.yml)
- [Rate Limits](rate-limits/kaleyra-rate-limits.yml)
- [Fin Ops](finops/kaleyra-finops.yml)

## Acquisition

Kaleyra, Inc. was acquired by **Tata Communications** in an all-cash transaction (~US$100M) that completed on **October 5, 2023**. Kaleyra now operates as a Tata Communications company; the kaleyra.io developer platform and APIs remain in operation.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
