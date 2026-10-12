# Umbrelia · project brief

**In one sentence:** Umbrelia is an AI receptionist for appointment-based service
businesses that handles customer questions and appointment requests through
WhatsApp and phone.

## The problem

A small team can miss enquiries while serving customers. A booking request also
depends on the business's actual prices, hours, staff availability and rules;
a plausible-sounding answer is not enough if the calendar does not confirm it.

## Who it is for

The product is designed for businesses such as beauty salons and dental clinics.
The public demonstration uses a **fictional beauty and dental clinic in Madrid**.
It is not a customer deployment or evidence of business results.

## What the assistant is designed to do

1. Answer questions using the business's own services, prices, opening hours and
   policies. If the information is missing, say so.
2. Look for an available slot and book, move or cancel an appointment in the
   connected calendar. Confirm a change only after the calendar saves it.
3. Hand a conversation to a person when the request needs human attention.
4. Summarise conversations, bookings and hand-offs for the owner.

The same product logic serves WhatsApp and phone. Each business has its own
configuration for services, durations, team and rules.

## What you can inspect today

- [Voice demo in a browser](https://josemdasilvag-blip.github.io/umbrelia/) —
  needs microphone permission; calls are limited to five minutes.
- [WhatsApp demo](https://wa.me/34644402947?text=Hi!) — opens a conversation
  with the demo number.
- [40-second explainer video](https://umbrelia.es/video/umbrelia-explicativo.mp4).
- [Use cases](USE-CASES.md) and [public verification guide](VERIFICATION.md).

These demos use a demo business and calendar. The backend and automated test
suite are private. The public materials show the intended customer experience,
not production performance, security, uptime or measured business impact.

## Implementation at a glance

Python server · Claude API tool use · Meta WhatsApp Cloud API · ElevenLabs
voice agent · Google Calendar · Cloudflare · Linux/systemd.

**Built by:** José Manuel Da Silva · [umbrelia.es](https://umbrelia.es)
