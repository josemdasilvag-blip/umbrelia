# Umbrelia · customer journeys

These are **demo scenarios**, not accounts of real clients or measured outcomes.
The fictional Madrid clinic and its demo calendar are used throughout. Exact
prices and available times can change with the demo configuration and calendar.

## 1. From a price question to an appointment

**Situation:** A prospective customer asks about teeth whitening while the
clinic team is busy.

**Journey**

1. The customer asks in English or Spanish for the price.
2. The receptionist answers from the demo clinic's own service information.
3. The customer asks for a Thursday afternoon appointment.
4. The receptionist checks availability, offers a free slot and asks for the
   details needed to book.
5. It confirms the booking only if the calendar accepts it.

**What this demonstrates:** one conversation can connect a factual service
answer with an appointment request. The exact price and slot are deliberately
not hard-coded in this example.

## 2. Moving or cancelling a booking

**Situation:** The customer cannot attend the booked time.

**Journey**

1. The customer asks to move the appointment to Friday morning, or to cancel.
2. The receptionist identifies the relevant demo booking and checks the
   calendar before making the change.
3. It confirms the new state only after the calendar records it.

**What this demonstrates:** booking is a continuing workflow, rather than a
one-time lead capture. Use a test appointment that you created yourself;
do not try to change another visitor's booking.

## 3. When the answer is outside the clinic's data

**Situation:** Someone asks for a service or policy the clinic has not provided.

**Journey**

1. The customer asks a specific question outside the published demo data.
2. The receptionist should say that it does not have a reliable answer and
   offer a human follow-up when appropriate.

**What this demonstrates:** the intended boundary is to avoid inventing a
business fact. The exact hand-off path depends on the demo configuration;
the public demo does not prove how a real clinic would respond.

## Try these journeys

Start with the [browser voice demo](https://josemdasilvag-blip.github.io/umbrelia/)
or [WhatsApp demo](https://wa.me/34644402947?text=Hi!). The
[verification guide](VERIFICATION.md) gives prompts, expected observations and
limits for each check.
