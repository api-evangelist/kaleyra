---
name: Place a click-to-call bridged call
description: Bridge two phone numbers with a Kaleyra click-to-call voice call.
api: openapi/kaleyra-openapi.yml
operations: [clickToCall]
generated: '2026-07-17'
method: generated
---

# Place a click-to-call bridged call (Kaleyra)

Authenticate with the `api-key` header; account SID in the path.

## Steps
1. **Bridge** — `POST /v1/{sid}/voice/click-to-call` (`clickToCall`) with form
   body `from` (first leg, called first), `to` (second leg, bridged after the
   first answers), optional `caller_id`, and `callback_url` for call-status
   events. Kaleyra dials `from`, then `to`, and bridges the legs.
2. **Track** — read `id`/`status` from the `VoiceResponse`; subscribe to call
   status via `callback_url` or a Callback Profile.

## Rules
- This places real outbound calls and consumes credits — confirm intent before
  calling; it is an outbound-communication action (audit it).
- `caller_id` must be a permitted/verified number for the account.
- `401` = missing/invalid `api-key`; `400` = malformed body.
