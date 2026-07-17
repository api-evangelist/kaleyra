---
name: Verify a user with an OTP
description: Generate a one-time password over Kaleyra Verify and validate the user's code.
api: openapi/kaleyra-openapi.yml
operations: [generateOtp, validateOtp]
generated: '2026-07-17'
method: generated
---

# Verify a user with an OTP (Kaleyra)

Authenticate with the `api-key` header; account SID in the path.

## Steps
1. **Generate** — `POST /v1/{sid}/verify` (`generateOtp`) with `to` (recipient
   MSISDN) and optionally `flow_id` (the configured Verify flow/template) and
   `sender`. Kaleyra delivers the code over the configured channel (SMS,
   WhatsApp, or Voice) and returns a `verify_id`.
2. **Collect** the code the end user enters.
3. **Validate** — `GET /v1/{sid}/verify/validate?verify_id=...&otp=...`
   (`validateOtp`). Check `valid: true` in the `VerifyResponse`.

## Rules
- Treat `verify_id` as short-lived; do not reuse across attempts.
- A failed validation returns `valid: false` — cap retries to prevent abuse.
- `generateOtp` sends a real message and consumes credits; do not loop it.
- `401` = missing/invalid `api-key`.
