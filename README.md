# Daash Angbao rates

The rates guide for the Daash Angbao app: what people in Singapore usually give at weddings, festivals and other occasions.

The app ships with a copy of `rates.json`. Its "Refresh rates" button downloads the newest version of this file and keeps it until the next refresh. Nothing else in the app goes online.

## Changing the rates

Edit `rates.json` and bump `updated` (YYYY-MM-DD). The app only takes a file that has `version`, `updated` and `occasions`.

- `occasions[].groups[].rows`: who, with a `min` and `max` in SGD.
- Weddings use `venue` instead: each venue has a price `level`; each level has a range per time (`slots`); `relations` multiply that range for colleagues, friends, close friends and family. Results are rounded to amounts people like to give (such as 188 or 288).

Figures are rough estimates, from public guides and common practice in Singapore.
