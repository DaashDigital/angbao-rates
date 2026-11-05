# Daash Angbao rates

The rates guide for the Daash Angbao app: what people in Singapore usually give at weddings, festivals and other occasions.

The app ships with a copy of `rates.json`. Its "Refresh rates" button downloads the newest version of this file and keeps it until the next refresh. Nothing else in the app goes online.

## Changing the rates

Edit `rates.json` and bump `updated` (YYYY-MM-DD). The app only takes a file with `version` 2, a newer `updated` date and readable `occasions`.

- `occasions[].groups[].rows`: who, with a `min` and `max` in SGD.
- Weddings use `venue` instead. Each venue has its seat cost per guest for each time (`seat`, from public guides). Every relationship starts at the seat cost; `relations` only raise the top of the range (top x `times` + `add`), for friends, close friends and family. Both ends round up to an amount ending in 8 (such as 188 or 358).

Figures are rough estimates, from public guides and common practice in Singapore.
