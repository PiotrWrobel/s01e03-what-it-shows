# Shared date parser reads day-first dates as month-first (379 reports)

Ticket #4471 contains 379 unique reports across 11 tenants where the shared date parser reads
month first even though the tenant uses a day-first locale. Dates are consequently interpreted
as a different day.

The affected reports arrived through app, email, and booking forms. This issue is distinct from
the booking-v3 hint mismatch: classify by tenant locale, booking form, and intake channel rather
than by the intake tag, which is only a guess.

Five reports noted by the desk as one-day moves remain in this group under that rule; the export
does not support counting them as a separate cause.
