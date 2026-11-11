# trpelka

I build small, testable Python tools for multilingual information work:
monitoring public sources, checking translation quality and keeping lead data
tidy.

I care more about a tool that can be checked than one that sounds clever.
Every project below has a README that says what it does **and what it does
not** do, plus tests where the behaviour is non-trivial.

## Selected projects

### [Tender Intelligence](https://github.com/trpelka/tender-intel)

Collects EU (TED) and Polish (BZP) tenders, scores relevance with explainable
rules and produces an HTML digest. The scoring table in the README matches the
code and is pinned by tests.

`Python` · `SQLite` · `pytest` · `CI`

### [Trend Monitor](https://github.com/trpelka/trend-monitor)

Daily RSS monitor for European tech news. Flags topics that appear in two or
more independent sources, collapses duplicate links and keeps one GitHub Issue
updated instead of opening a new one every day.

`Python` · `GitHub Actions` · `pytest` · `CI`

### [Language job search](https://github.com/trpelka/language-job-search)

Multilingual job discovery across Polish boards and international aggregators,
with SQLite deduplication and a scheduled GitHub Actions run.

`Python` · `SQLite` · `GitHub Actions`

### [OSINT Lead Pipeline](https://github.com/trpelka/osint-lead-pipeline)

A FastAPI + SQLite lead book with search, pagination, a zero-build dashboard
and a guarded homepage email scraper. It is a demo of CRUD and API hardening,
not an OSINT data provider.

`Python` · `FastAPI` · `React` · `Docker` · `CI`

### Translation QA tools

- [MT quality scorer](https://github.com/trpelka/MT-quality-scorer) — BLEU and
  chrF scoring that flags weak segments for review.
- [Terminology consistency checker](https://github.com/trpelka/Terminology-consistency-checker)
  — compares a translation against an approved glossary.
- [Multilingual document RAG](https://github.com/trpelka/multilingual-doc-rag)
  — local retrieval over PDF/DOCX/TXT with no API keys.

## How I work

- Rules compute the numbers; a model only writes prose or routes work.
- Unverified output is blocked or labelled, not quietly shipped.
- Tests, CI and a limitations section are part of the deliverable.
- No scraping claim without a source row and a timestamp.

## Contact

Open an issue on any repository.
