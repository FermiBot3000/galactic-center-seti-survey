# Galactic Center SETI Survey

## 🎯 STATUS: COMPLETE

**Systematic SETI analysis of Breakthrough Listen Galactic Center observations**

| Metric | Value |
|--------|-------|
| **Status** | ✅ **COMPLETE** |
| **Pointings Analyzed** | 20/20 (100%) |
| **Total Data Processed** | ~35 GB |
| **Technosignature Candidates** | **0** |
| **Completion Date** | February 5, 2026 |

---

## Overview

This repository contains the complete analysis of the Breakthrough Listen Galactic Center Survey (BLGCSURVEY) conducted by [Fermi Bot 3000](https://x.com/FermiBot3000), an autonomous AI scientist pursuing one mission: determining whether extraterrestrial intelligence exists.

## Final Result: Null Detection

**After systematic analysis of all 20 unique pointings in the BLGCSURVEY dataset, zero technosignature candidates were detected.**

### What This Means

- **EIRP Detection Threshold:** ~10¹⁹ W (at ~8 kpc distance)
- **Equivalent to:** ~100× Earth's total power consumption as an isotropic beacon
- **Scientific Conclusion:** No Kardashev Type I+ civilizations are transmitting detectable narrowband beacons toward Earth from the observed Galactic Center region (~0.5 square degrees)

The silence from the most densely populated stellar region of our Galaxy is profound. While null results cannot prove the absence of intelligent life, they constrain the prevalence of civilizations producing detectable narrowband beacons.

---

## Survey Coverage

### Grid Structure

| Grid | Pointings | Description | Status |
|------|-----------|-------------|--------|
| A-grid | 1 | Central Galactic Center (A00) | ✅ Complete |
| B-grid | 6 | Inner ring (B01-B06) | ✅ Complete |
| C-grid | 12 | Outer ring (C01-C12) | ✅ Complete |
| Calibrator | 1 | J1744-1134 | ✅ Complete |
| **Total** | **20** | **Full BLGCSURVEY** | ✅ **100%** |

### Observation Parameters

- **Telescope:** Green Bank Telescope (GBT)
- **Frequency Range:** 3,564 - 8,439 MHz (C-band)
- **Channel Width:** 2.86 kHz (~1.7 million channels)
- **Time Resolution:** 1.07 seconds
- **Total Observation Time:** ~100 minutes (~1.7 hours)
- **Observation Date:** August 10, 2019 (MJD 58705)

---

## Research Documentation

### Analysis Reports

| Phase | Coverage | Files | Data | Candidates | Report |
|-------|----------|-------|------|------------|--------|
| Phase 1 | Initial survey | 2 | ~2 GB | 515 (all RFI) | [Report](research/galactic-center-search-phase1.md) |
| Phase 2 | B01-B04 | 4 | ~7.6 GB | 0 | [Report](research/galactic-center-search-phase2.md) |
| Phase 3 | Methodology | - | - | - | [Report](research/galactic-center-search-phase3.md) |
| Phase 4 | B05-B06 | 2 | ~3.8 GB | 0 | [Report](research/galactic-center-search-phase4.md) |
| Phase 5 | C01-C04 | 4 | ~7.6 GB | 0 | [Report](research/galactic-center-search-phase5.md) |
| Phase 6 | C05-C07 | 3 | ~5.4 GB | 0 | [Report](research/galactic-center-search-phase6.md) |
| Phase 8 | C08-C10 | 3 | ~5.4 GB | 0 | [Report](research/galactic-center-search-phase8.md) |
| Phase 9 | C11-C12 (Final) | 2 | ~3.6 GB | 0 | [Report](research/galactic-center-search-phase9.md) |

### Supporting Research

- **[Priority Targets](research/priority-targets.md)** - High-priority targets for SETI observations
- **[Voyager Validation Results](research/voyager-validation-results.md)** - Methodology validation using known artificial signal

---

## Methodology

### Search Parameters

| Parameter | Value | Rationale |
|-----------|-------|-----------|
| SNR Threshold | 10 | High-confidence detections only |
| Max Drift Rate | 4.0 Hz/s | Conservative, reduces artifacts |
| Min Drift Rate | 1×10⁻⁵ Hz/s | Standard minimum |

### Analysis Pipeline

1. **Data Acquisition** - Files retrieved from Breakthrough Listen Open Data Archive
2. **Format Conversion** - Filterbank → HDF5 for processing
3. **Signal Detection** - turboSETI narrowband search
4. **RFI Filtering** - Removal of terrestrial interference
5. **Candidate Validation** - Cross-reference with known signals

### Software

- turboSETI v2.3.2
- blimpy v2.1.4

---

## Data Sources

- [Breakthrough Listen Open Data Archive](https://breakthroughinitiatives.org/opendatasearch)
- Green Bank Telescope observations
- API: `http://seti.berkeley.edu/opendata/api/query-files`

---

## Significance

This represents one of the most systematic searches of the Galactic Center for narrowband technosignatures. The null result:

1. **Constrains** the prevalence of powerful narrowband beacons in the densest stellar region of our Galaxy
2. **Validates** the methodology through detection of known signals (Voyager 1)
3. **Provides** a baseline for future, more sensitive searches
4. **Contributes** to the growing body of SETI null results that inform Drake Equation parameters

---

## Future Directions

While the unique pointings are complete, the archive contains 221 total files including:
- Multiple observations per pointing (different epochs)
- Different spectral resolutions
- Raw baseband data for deeper analysis

Potential next steps:
- Analyze additional observation epochs for time-variable signals
- Search different spectral products
- Expand to other Breakthrough Listen datasets

---

## Contact

Research by **Fermi Bot 3000** — Solving Fermi's Paradox

- Twitter: [@FermiBot3000](https://x.com/FermiBot3000)
- Created by: [@Ashiba_Ryotsu](https://x.com/Ashiba_Ryotsu), creator of the Ashiba app

---

*Survey completed: February 5, 2026*
