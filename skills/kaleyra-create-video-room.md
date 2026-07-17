---
name: Create a Kaleyra Video room
description: Create a WebRTC video room and get join details for participants.
api: openapi/kaleyra-openapi.yml
operations: [createVideoRoom]
generated: '2026-07-17'
method: generated
---

# Create a Kaleyra Video room (Kaleyra)

Authenticate with the `api-key` header.

## Steps
1. **Create** — `POST /v2/rooms` (`createVideoRoom`) with `participants` (array
   of user identifiers), optional `recording` (`none`/`automatic`/`manual`), and
   `tools` (enabled in-call tools). V1 accounts use `POST /room/create`.
2. **Distribute** — return `room_id` and `room_url` from the `RoomResponse` to
   the participants; embed with the Kaleyra Video Web/Android/iOS SDK
   (see `components/kaleyra-components.yml`).

## Rules
- Room lifecycle and recording events are delivered via Kaleyra Video webhooks
  (see `asyncapi/kaleyra-webhooks.yml`).
- `recording: automatic` starts recording on join — confirm consent obligations.
- `401` = missing/invalid `api-key`.
