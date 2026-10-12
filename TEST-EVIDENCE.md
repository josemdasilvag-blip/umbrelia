# Umbrelia · automated test summary

- **Run date:** 12 October 2026
- **Result:** 67 passed, 0 failed
- **Environment:** Python 3.12 on Windows, local test run
- **Source:** private Umbrelia product repository; no source code, credentials,
  customer data or raw logs are published here.

The suite was run with `python -m pytest -q` and a workspace-local temporary
directory. The run finished successfully in 7.73 seconds. This is a dated
result for that checkout, not a continuously updated CI badge.

## What the suite covers

- Appointment availability, duration and opening rules; booking, moving,
  cancelling, conflicting slots and concurrent requests.
- Calendar behavior with simulated Google Calendar responses, including
  unavailable calendars and failed writes.
- Assistant conversation flow: use of business information, tool errors,
  hand-off and avoiding unsupported answers.
- Webhook signature checks, message routing, retry handling and persistence
  using a local test server.
- Voice request parsing, authorization and response format.
- Owner reports and learning from business-provided answers.

## What this result does not prove

These are automated tests with simulated dependencies and a localhost server.
They do not measure uptime, latency, production concurrency, customer outcomes
or live Meta, Google Calendar, Claude and ElevenLabs availability. Visitors can
try the [public demo](https://josemdasilvag-blip.github.io/umbrelia/) and follow
the [manual verification guide](VERIFICATION.md), but cannot inspect or rerun
the private suite from this repository. Code review can be arranged on request.
