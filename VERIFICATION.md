# Umbrelia · public verification guide

This guide lets a visitor test the **public demo**. It is a repeatable manual
checklist, not a record that every step passed on every visit. Use only test
details and the fictional clinic; do not share patient information.

## Setup

1. Open the [voice demo](https://josemdasilvag-blip.github.io/umbrelia/).
   Allow microphone access and keep the call under five minutes. Alternatively,
   open the [WhatsApp demo](https://wa.me/34644402947?text=Hi!).
2. Use a test name and an appointment you are willing to cancel.
3. Ask one question at a time. Availability and prices may change.

## Checks a visitor can perform

| Check | Suggested prompt | What to observe |
| --- | --- | --- |
| Business answer | “How much is a teeth whitening?” | An answer about the demo clinic, grounded in its configured service data. Do not expect a fixed price from this document. |
| Availability | “Do you have a manicure slot on Thursday afternoon?” | The assistant checks or offers a time rather than treating a request as a confirmed booking. |
| Booking | After choosing a free slot: “Please book that for me.” | A clear success or failure response. An offered time alone is not a booking confirmation. |
| Change | For your own test booking: “Move it to Friday morning.” | A new available time is checked and a result is reported. |
| Cancellation | For your own test booking: “Cancel my appointment.” | A clear result; do not cancel another visitor's booking. |
| Unknown fact | Ask for a service or policy absent from the demo clinic's data. | The assistant should acknowledge missing information rather than invent a price or policy. |
| Language | Repeat a simple service question in Spanish. | The assistant can continue in Spanish. |

The [40-second explainer](https://umbrelia.es/video/umbrelia-explicativo.mp4)
is a visual overview, not a substitute for trying the live demo.

## Evidence boundaries

| Claim | Public evidence | Limit |
| --- | --- | --- |
| The demo offers voice and WhatsApp entry points | The live demo page and WhatsApp link | A link or page load does not prove a completed conversation. |
| The assistant can discuss services and appointment requests | A visitor can try the prompts above | Results depend on the live service and demo calendar at the time of the test. |
| Booking, changes and cancellation are implemented | The demo can be exercised with a test appointment | This does not establish behavior across all edge cases or a production clinic. |
| 67 automated tests covering booking, assistant, webhook, voice and reporting behavior | [Dated test summary](TEST-EVIDENCE.md): 67 passed in a local run on 12 October 2026 | Test code and raw results are private; visitors cannot rerun the suite from this repository. This does not verify production uptime or external services. |

For a code or test review, ask the author for access to the private product
repository. No customer data or production results are published here.
