# Kaleyra (kaleyra)

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
