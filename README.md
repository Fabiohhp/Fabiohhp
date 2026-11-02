# Fábio Henrique Peixe

Data scientist and economist. I work on football data end to end, from the pipeline to the
recruitment decision, and I report what did not work alongside what did.

[LinkedIn](https://www.linkedin.com/in/f%C3%A1bio-henrique-peixe/)

## Football

### [football-scouting](https://github.com/Fabiohhp/football-scouting)

Using only what was known on 30 June 2016, which players would a data-driven system have
recommended, and how did their careers go? Shortlists under a €5M budget scored **72.9** three
years later on a growth score where 50 is a typical career for a player's age, against **48.3** for
every player within the budget. Includes a worked case, replacing Matt Ritchie at Bournemouth, with
one-page scouting reports.

`Python` `DuckDB` `StatsBomb event data` `expected threat` `expected pass completion`

### A football data platform in three parts

- **[football-data-engineering](https://github.com/Fabiohhp/football-data-engineering):** a daily
  pipeline from two public sources to a PostgreSQL star schema, with idempotent re-runs and a
  quality gate tested by fault injection.
  `Airflow` `PySpark` `MinIO` `PostgreSQL` `Docker`
- **[football-data-analytics](https://github.com/Fabiohhp/football-data-analytics):** two questions
  about expected goals. Points above xPTS do not last (r = +0.13 across 192 club-seasons), and
  finishing barely repeats (r ≈ 0.10, against r ≈ 0.90 for shot volume).
  `dbt` `DuckDB` `SQL` `static dashboard`
- **[football-data-science](https://github.com/Fabiohhp/football-data-science):** match and shot
  models scored on a season they never saw. Nothing beat an Elo rating measurably on match results,
  and the leakage tests plant leaks on purpose to prove they fire.
  `scikit-learn` `statsmodels` `Dixon-Coles` `dbt`

## Credit risk and economics

Written in Portuguese.

- **[time-to-default](https://github.com/Fabiohhp/time-to-default):** when a loan breaks, across 2.1
  million personal loans. On 36-month contracts, risk rises sixfold in the first year and stays at
  its peak from month 12 to month 30.
  `Kaplan-Meier` `competing risks` `Cox`
- **[score-credito](https://github.com/Fabiohhp/score-credito):** credit scoring with the cutoff
  chosen by profit. Moving it from 0.50 to 0.24 cuts default losses by 34% and gives up 3.7% of the
  margin.
  `LightGBM` `scorecard` `explainability`
- **[inflacao-clima](https://github.com/Fabiohhp/inflacao-clima):** how weather shocks move food
  prices in Brazil, over 287 months of public data. Excess rain, not drought, raises vegetable and
  tuber prices, and a severe drought in corn areas is followed by higher meat prices for more than a
  year. Extends an MBA capstone (USP/Esalq).
  `local projections` `panel regressions` `VECM`
