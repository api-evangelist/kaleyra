---
name: Send an SMS and track delivery
description: Send a single or bulk SMS via Kaleyra and pull its delivery status.
api: openapi/kaleyra-openapi.yml
operations: [sendMessage, getMessageStatus, listMessages]
generated: '2026-07-17'
method: generated
---

# Send an SMS and track delivery (Kaleyra)

Authenticate every request with the `api-key` header (key from the kaleyra.io
console) and put your account SID in the path.

## Steps
1. **Send** — `POST /v2/{sid}/messages` (`sendMessage`) with form or JSON body:
   `to` (comma-separate for bulk), `sender` (registered sender ID), `body`,
   `channel: sms`, and `type` (`MKT`/`TXN`/`OTP` — India DLT-aware). Supply
   `template_id` where the region/DLT requires an approved template.
2. **Read the response** — capture `id` and `status` from the `MessageResponse`.
3. **Poll status** — `GET /v2/{sid}/messages/{message_id}` (`getMessageStatus`),
   or pull logs with `GET /v2/{sid}/messages` (`listMessages`) filtered by
   `type`, `from_date`, `to_date`.

## Rules
- No idempotency key exists — retry only after confirming the prior send failed,
  or you will double-charge and double-send.
- Delivery outcomes come back as status/trace codes (e.g. `DELIVRD`, `NO-CREDITS`,
  `CON-DND`, `OPT-OUT`) — see `errors/kaleyra-error-codes.yml`.
- `401` means a missing/invalid `api-key`; `400` means malformed body.
- Prefer DLR callbacks (Callback Profiles) over polling for scale.
