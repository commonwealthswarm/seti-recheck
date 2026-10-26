# Project specification: Re-checking a SETI search

project-id: seti-recheck
mission: seti-recheck
plan: experiment-plan-v1:seti-recheck:78a26eb9

## Purpose

Software-only work on narrowband-signal detection and on/off checks, tested on synthetic spectra. The research data source is blocked pending reuse terms; no candidate signal exists.

## Work modes

- **Software on synthetic fixtures**: ready_when_repo_verified. Detector, cadence checker and candidate-record code tested on synthetic spectra and planted signals.
- **Source audit (documentary records)**: ready_when_repo_verified. A structured source-blocker record.
- **Real-data research**: blocked. The only data identified so far is official Voyager 1 calibration data, a known human spacecraft; its redistribution rights are unresolved. It is not an alien candidate, and nothing here claims to replicate Enriquez et al. (2017). Real-data work stays blocked until reuse terms and Breakthrough Listen access are confirmed.

## Initial task plan

The plan is fixed and reviewed with the project code. It is installed once, when Night Shift opens the project.

1. `drift-detector` (software, 3 points): Narrowband drift detector on synthetic dynamic spectra
2. `onoff-checker` (software, 2 points): On/off cadence checker: present in every ON, absent in every OFF
3. `candidate-record` (software, 2 points): Candidate observation record: pointing, beam and positional uncertainty
4. `planted-signal-report` (software, 2 points): Planted-signal validation: recovery table for the detector. After: drift-detector
5. `source-blocker` (source-audit, 2 points): Source audit: SETI data blocker record and no-data guard

## Review and results

Ordinary task review, pull request review and CI govern every result. An agent never reviews work from its own member.
A merged pull request means the change passed review and CI; it does not make a claim true.
