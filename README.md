# Josh Talks AI — Product Task Submission (July 2026)

This folder contains the full submission for both questions in the assignment brief. Start with **`Main Document/Main_Document.pdf`** for the complete write-up, or **`One page report/One_Page_Report.pdf`** for a quick summary.

**Note:** the compulsory video walkthrough is being shared separately and is not included in this folder.

## Deliverables checklist (Question 1)

| Required deliverable | Where it is |
|---|---|
| 1. Main document (eval choice, category/use case, why it matters for India, how it works, judging method, results, scaling plan) | `Main Document/Main_Document.pdf` |
| 2. One-page report | `One page report/One_Page_Report.pdf` |
| 3. Supporting material — prompts | `Supporting materials/prompts/JoshTalks_Prompts_Used.pdf` |
| 3. Supporting material — generated images (3 required models) | `Images/Gemini 2.5 Flash Image/`, `Images/Gemini 3.1 Flash Image Preview/`, `Images/GPT Image/` |
| 3. Supporting material — participant ratings | `Supporting materials/josh_talks_image_eval_ratings.csv` |
| 3. Supporting material — screenshots / proof of generation | `Supporting materials/screenshots/` (one subfolder per model) |
| 3. Supporting material — consent proof | `Supporting materials/josh_talks_image_eval_consent_records.csv` |
| 4. UI / dashboard / leaderboard design | `UI Dashboard Design/UI_Dashboard_Leaderboard-Design.pptx` |
| 5. Video walkthrough (≤2 min) | **Shared separately — not in this folder** |
| Final reflection (5 questions) | Final Reflection/Final_Reflection.pdf` |

The live rating tool participants used to generate `josh_talks_image_eval_ratings.csv` and the consent CSV is `index.html`.

## Deliverables checklist (Question 2)

| Required deliverable | Where it is |
|---|---|
| Part I — at least 2 warning signs (what it tells us / how to measure / thresholds / false alarms) | `Question 2/Part 1 & 2/Part1&2_..._recommendation_system.pdf` (Part I section) |
| Part II — practical detection system / blocking logic for engineering | Same file, Part II section |
| Underlying data | `Question 2/Part 1 & 2/Data Check.xlsx` |
| Reproducible analysis | `Question 2/Part 1 & 2/Analysis.ipynb` (runs end-to-end against the xlsx in the same folder) |

## Full folder structure

```
assignment/
    Product_Task_July2026.pdf              The original assignment brief

Main Document/
    Main_Document.pdf                      Full Q1 write-up + final reflection

One page report/
    One_Page_Report.pdf                    1-page summary of Q1: eval, setup, findings, takeaway

Question 2/Part 1 & 2/
    Data Check.xlsx                        Raw task-level transcription data
    Analysis.ipynb                          Runnable notebook reproducing every metric/finding
    Part1&2_..._recommendation_system.pdf   Full Part I (warning signs) + Part II (blocking logic)

Images/                                    Generated images, 7 per model, 3 required models
    Gemini 2.5 Flash Image/
    Gemini 3.1 Flash Image Preview/
    GPT Image/

Supporting materials/
    josh_talks_image_eval_consent_records.csv   Consent proof for all participants
    josh_talks_image_eval_ratings.csv           Raw per-participant ratings, all models/prompts
    prompts/JoshTalks_Prompts_Used.pdf           The prompts used, verbatim
    screenshots/                                 Proof of generation, one subfolder per model

UI Dashboard Design/
    UI_Dashboard_Leaderboard-Design.pptx    Mockup of the rating UI / results dashboard / leaderboard

index.html                                  The rating tool used to run the eval with participants
```

## Notes for the reviewer

- `Analysis.ipynb` expects `Data Check.xlsx` in the same folder — no path changes needed.
- Each model's `Images/` subfolder has a matching `screenshots/` subfolder under `Supporting materials/`, using the same model name, so a model's outputs and its generation-session proof can be cross-referenced directly.
- `index.html` is the actual tool used to collect participant consent and ratings; the two CSVs in `Supporting materials/` are its output.
