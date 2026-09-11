# Neural Circuit → Homoeopathic Remedy Finder

A clinician tool that phenotypes a patient across the **six Williams-taxonomy neural
circuits** and returns a **shortlist of homoeopathic remedies** — drawn from Rajan
Sankaran's *The Soul of Remedies* — whose core feeling is organised around the same
axis.

Prepared for **Dr. Archit Mehta, MD (Hom.) Psychiatry** — Dr. Archit's Clinic, Surat.

## What's here

| File | Purpose |
| --- | --- |
| [`remedy-finder.html`](remedy-finder.html) | **The tool.** Open in any browser. Score the six-circuit interview → get the circuit-matched remedy shortlist + a searchable materia medica reference. |
| [`data/remedies.json`](data/remedies.json) | The structured dataset: all **96 remedies** grouped under their dominant circuit, each with its *core feeling* and *why-it-matches* rationale. |
| [`index.html`](index.html) | The original reference tool this design was cloned from (allopathic Rx/Tx by biotype). |

## How it works

1. **Phenotype first.** The left column is a bedside interview across the six circuits,
   three items each (scored 0–3), identical to the reference assessment:

   | # | Circuit | Biotype | Remedies |
   | --- | --- | --- | --- |
   | I | Default Mode | "Rumination" | 10 |
   | II | Salience | "Anxious Avoidance" | 20 |
   | III | Negative Affect | "Threat" | 35 |
   | IV | Positive Affect | "Reward" | 5 |
   | V | Attention | "Inattention" | 7 |
   | VI | Cognitive Control | "Cognitive Dyscontrol" | 19 |

2. **Read the dominant circuit.** A live radar profile shows relative circuit
   dysfunction; the panel names the dominant circuit, its bedside cue and clinical
   hallmark.

3. **Get the remedy shortlist.** The tool lists every remedy mapped to that circuit,
   each expandable to its core feeling and the rationale for the mapping. When a
   second circuit is co-elevated, it is flagged (constitutional remedies straddle
   circuits).

4. **Send a case note.** Emails a structured triage note (default:
   `architmehta98@gmail.com`).

## Method & caveat

The mapping reads each of the 96 remedies described in *The Soul of Remedies* against
the neural-circuit rule book (*Brain Circuits: Clinical Identification for
Psychiatrists*) and places each under the single circuit whose clinical hallmark most
closely matches the remedy's core feeling.

This is a **clinical thinking tool — a shortlist to differentiate, not a repertory or
an automatic prescription.** Constitutional remedies are multidimensional; the mapping
captures the dominant, best-matching axis only. Prescribing should still proceed from
full case-taking, rubric selection and differentiation as Sankaran describes.

**Sources.** Rule book: *Precision Psychiatry and the Neural Circuit Taxonomy* (Brain
Circuits: Clinical Identification for Psychiatrists). Materia medica: Rajan Sankaran,
*The Soul of Remedies*.
