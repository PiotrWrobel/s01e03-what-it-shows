# booking-v3 date hint conflicts with day-first tenant locales (33 reports)

Ticket #4471 contains 33 unique reports from booking-v3 forms in day-first locales. The form
instructs people to enter `MM/DD/YYYY`, while the tenant's locale interprets dates day first.
This hint mismatch is a separate cause from the shared parser bug.

The reports span Alder Physio (12), Copper Studio (11), and Pale Harbour (10). The intake tag
is not authoritative: 15 of these reports were tagged `parser`.
