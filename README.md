# ITCS 6190/8190 – Cloud Computing for Data Analysis

## Course Project: Data Analysis with Apache Spark

> **Teams: replace everything in this block before the Week 4 milestone.**
>
> **Team name:**
>
> | Name | Student ID | Email | GitHub handle |
> | ---- | ---------- | ----- | ------------- |
> |      |            |       |               |
>
> **Project description (one paragraph):**
>
> **Dataset:**

---

## Repository structure

| Path | What goes here |
| ---- | -------------- |
| `src/` | The pipeline: ingestion, transformations, streaming, ML. Run in this order by `run.sh`. |
| `notebooks/` | Exploratory work. Notebooks support the analysis; `src/` is the deliverable. |
| `tests/` | Tests validating your queries and transformations. |
| `data/` | Small samples only, under `data/sample/`. Large data stays external (S3, public URL). |
| `docs/` | Dataset overview, methodology, results, limitations, reproduction guide. |
| `docs/slides/` | Final presentation, or a link to it from the release. |

## Running the pipeline

```bash
pip install -r requirements.txt
make run          # or: bash run.sh
```

This must execute the whole pipeline end to end, from ingestion to final output, in local
mode with a single command. Keep it working as you go — it is part of the grade.

```bash
pytest            # run the tests
```

## Milestones

| Week | Milestone | What we look for |
| ---- | --------- | ---------------- |
| 4 | Team Setup | Repository created, collaborators added, this README filled in |
| 6 | Proposal | Project Proposal issue opened, presented at the check-in |
| 9 | Data Ingestion + EDA | Pull request with ingestion code and updated README |
| 11 | Complex Queries + Streaming | Pull request with Spark SQL queries, tests, and streaming job |
| 13 | ML Component + Pipeline | Pull request with feature pipeline, model, metrics; end-to-end run |
| 15 | Final Release | Tag `v1.0.0`, GitHub Release, presentation in class |

Check-ins happen in Weeks 6, 9, 11 and 13. Each team gets 10 minutes. Open a **Project
Check-in** issue before class using the issue template.

## Working conventions

- Do the work on branches and merge through pull requests. Do not commit directly to `main`.
- Link pull requests to issues (`Closes #12`) so the history explains itself.
- Add the instructor and TAs as collaborators at Week 4 and keep that access until grades
  are posted.

Full requirements, milestones and grading are in the project description on Canvas.
