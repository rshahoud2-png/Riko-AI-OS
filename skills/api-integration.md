# API Integration Skill

## Purpose
Connect external APIs safely and reliably.

## Use When
Adding third-party services, webhooks, SDKs, or internal service calls.

## Inputs
- API docs and version.
- Auth method without secret values.
- Required endpoints and data mapping.
- Rate limits and error behaviors.

## Method
1. Verify current docs.
2. Model auth, retries, timeouts, and idempotency.
3. Define request/response schema.
4. Protect secrets server-side.
5. Test happy path and failure cases.

## Output
- Integration plan.
- Data mapping.
- Error handling.
- Security notes.
- Test plan.
