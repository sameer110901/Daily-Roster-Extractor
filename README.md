# Daily-Roster-Extractor
short description  Browser-only tool that reads a monthly shift roster PDF and shows who works a chosen day, with their shift codes and multi-select filters.
# Roster Extractor

Single-file HTML tool that reads a monthly Dienstplan PDF and lists everyone
working on a chosen day with their shift code (S20, F5, F5L, ...).

- Runs fully in the browser (pdf.js). No server, and no data leaves your device.
- Pick a date, or type it (e.g. "13. Okt"). Results appear on screen, sorted by shift.
- Multi-select filter chips: top codes S20, S17, S2, S8L, S20/S17 (both together), then the rest.
- Name/shift search, All reset, light and dark mode.
- Tested on the September and October rosters (every day checked against the
  PDF's table cells).

## Limits
- Needs a text-based PDF (not a scan) with the same layout: dates across the
  top, names down the left, one shift per day.
- Matches the day number only; the month comes from the uploaded file.

## Use
Open roster-parser.html in a browser, choose the PDF, choose the date.

Stack: HTML, CSS, vanilla JS, pdf.js 3.11.174 (cdnjs).
