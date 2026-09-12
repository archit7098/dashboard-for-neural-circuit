# Neural Circuit Assessment Dashboard

A lightweight, single-page clinician-facing tool for organizing observations
during a psychiatric interview around six brain-circuit "biotypes." It renders a
live radar profile of circuit severity and surfaces illustrative treatment
considerations as the clinician scores each item.

The entire app is contained in [`index.html`](index.html) — open it in any modern
browser, no build step or server required.

## ⚠️ Disclaimer

This tool is a **screening/education aid, not a diagnostic tool or medical
device.** It does not diagnose any condition, does not replace clinical judgment,
and its output must not be used as the basis for any treatment decision. Any
medication (Rx) or therapy (Tx) suggestions shown are **illustrative examples
only — not prescriptive recommendations.**

This project is **not affiliated with or endorsed by Stanford University** or any
of its faculty. It draws on publicly described concepts but is an independent,
unvalidated adaptation.

## Taxonomy

The circuit framework is **inspired by the Williams Neural Circuit Taxonomy
(independent, unvalidated adaptation).** It has not been clinically validated in
this form and should be treated as an organizational aid only.

## Known limitations

- **Single-winner logic.** The current interpretation picks the single
  highest-scoring circuit as the "dominant biotype." It does **not** yet handle
  mixed or comorbid presentations, where two or more circuits are elevated
  together — a common real-world pattern.
- **Illustrative treatment content.** The Rx/Tx and caution notes are generic
  teaching examples, not individualized clinical advice.
- **No data storage.** Scores live only in the browser session and are not saved.

## Usage

1. Open `index.html` in a browser.
2. Score each item (0–3) during or after the interview.
3. Review the live circuit profile and the identified biotype panel.
4. Use **Send Clinical Note** to draft an email summary in your own mail client;
   fill in the recipient yourself.
