# Priority Targets for Independent SETI Analysis

**Date:** February 5, 2026  
**Purpose:** Identify underserved targets in BL archive for original analysis

---

## Selection Criteria

Targets were prioritized based on:
1. ✅ **Raw data publicly available** — Downloadable from BL Open Data Archive
2. ✅ **Little or no published analysis** — Not covered in existing BL papers
3. ✅ **Scientific interest** — Compelling reasons for ETI search
4. ✅ **Feasible data size** — Manageable for independent analysis

---

## Top 5 Priority Targets

### 1. 🥇 GALACTIC CENTER BACKGROUND FIELDS (Highest Priority)

**Why Underserved:**
- 400+ hours of Parkes observations released in BLDR 2.0 (Feb 2020)
- Explicitly described as "so-far unanalyzed" by BL team
- Gajjar et al. (2021) analyzed only ~18 hours of this dataset
- Remaining ~382 hours have no published technosignature search

**Scientific Interest:**
- Line-of-sight contains **60 million stars** (greatest stellar density in sky)
- If ETI exists in the Milky Way, the galactic center offers the highest probability per pointing
- EIRP constraints achieved: ≥4×10^18 W (L-band), ≥5×10^17 W (C-band)

**Data Available:**
- Telescope: Parkes (L/S-band), GBT (C-band)
- Format: Filterbank/HDF5
- Size: ~100s of GB total
- Location: Search "BLGCSURVEY" or galactic coordinates on archive

**Analysis Status:**
| Component | Status |
|-----------|--------|
| Gajjar et al. 2021 paper | 18 hours analyzed (narrowband + magnetar search) |
| Remaining ~382 hours | **UNANALYZED** |
| Extended drift rates | Not searched |
| Background sources in FOV | **NOT SEARCHED** |

**Recommended Action:** Standard turboSETI analysis on full dataset, followed by background source extraction.

---

### 2. 🥈 BACKGROUND EXTRAGALACTIC SOURCES (143,024 Objects)

**Why Underserved:**
- Garrett et al. (2022) identified 143,024 extragalactic objects in 469 BL target fields
- These objects exist *in existing data* — no new observations needed
- Paper only placed statistical upper limits; **no individual source analysis performed**
- Almost none have dedicated SETI searches

**Scientific Interest:**
- Includes radio-loud AGN, quasars, and galaxies
- Type II/III Kardashev civilizations could produce detectable signals
- Multi-galaxy statistics constrain prevalence of advanced civilizations

**Data Available:**
- Telescope: GBT L-band observations
- Format: Filterbank/HDF5 (same files as primary targets)
- Size: Already downloaded with primary target data
- Source catalog: Cross-match BL pointings with NVSS/FIRST/VLASS

**Analysis Status:**
| Component | Status |
|-----------|--------|
| Primary nearby stars | Analyzed in multiple papers |
| Background FOV sources | **UNANALYZED** (only statistical limits) |
| Individual source searches | **NOT PERFORMED** |

**Recommended Action:** 
1. Extract background source positions from Garrett catalog
2. Check for narrowband signals at each position
3. Constrain individual EIRP limits

---

### 3. 🥉 BL EXOTICA CATALOG (700+ Exotic Objects)

**Why Underserved:**
- Catalog published June 2020 (Lacki et al., arXiv:2006.11304)
- Contains "one of everything" — anomalies, superlatives, prototypes
- Only preliminary Parkes data released for ~9 targets (2020)
- Vast majority have **observations but no published analysis**

**Scientific Interest:**
- Includes unexplained phenomena (Anomaly sample)
- Extreme objects (fastest star, coldest pulsar, brightest transient)
- Deliberately selected for "things we don't understand"

**Available Exotica Data (from public archive):**
| Target | Type | Data Available | Analysis Status |
|--------|------|----------------|-----------------|
| S5-HVS1 | Hypervelocity star (4M mph) | Parkes 1.3-1.5 GHz | **No SETI paper** |
| ASASSN-15lh | Hypernova/TDE | Parkes L-band | **No SETI paper** |
| ASASSN-V J213939 | Mysterious dimming star | Parkes L-band | **No SETI paper** |
| PSR J2144-3933 | Coldest/faintest pulsar | Parkes L-band | **No SETI paper** |
| Phoenix Cluster | Massive galaxy cluster | Parkes L-band | **No SETI paper** |
| A2744z8OD | z~8 overdensity | Parkes L-band | **No SETI paper** |
| NGC 4214 (ID11) | Dwarf starburst | Parkes L-band | **No SETI paper** |
| HIP 114176 | Erroneous Hipparcos star | Parkes L-band | **No SETI paper** |
| Epsilon Indi | Nearby star system | Parkes L-band | Minimal |

**Data Location:** http://blpd1.ssl.berkeley.edu/pks_exotica/

**Recommended Action:** Systematic turboSETI search of all Exotica data, prioritizing Anomaly sample.

---

### 4. 🏅 TESS EXOPLANET HOSTS (27+ Systems)

**Why Underserved:**
- Barrett et al. (2025) searched 27 eclipsing TESS exoplanets
- Innovative eclipse-based methodology (signal should disappear during transit)
- But: Only searched for eclipse-correlated signals, not continuous emission
- Many more TESS hosts observed but not in that paper

**Scientific Interest:**
- Known exoplanets = confirmed habitable zone candidates
- Eclipse methodology is novel angle
- TESS has discovered 7,000+ planet candidates since 2018

**Data Available:**
- Telescope: Parkes (UWL receiver, 0.7-4.0 GHz)
- Format: HDF5
- Size: ~3.8 GB per observation
- Targets: TOI systems (searchable in archive)

**Analysis Status:**
| Component | Status |
|-----------|--------|
| Eclipse-correlated search | Barrett 2025 (27 targets) |
| Continuous narrowband search | **NOT PERFORMED** |
| Extended drift rates | **NOT PERFORMED** |
| Additional TESS hosts | Many observed, not analyzed |

**Recommended Action:** Standard narrowband search of all TESS host observations, independent of eclipse timing.

---

### 5. 🎖️ ANDROMEDA SYSTEM DWARF GALAXIES

**Why Underserved:**
- Archive contains observations of AND_I through AND_XXIX (Andromeda satellite galaxies)
- No published SETI analysis of these specific targets found
- Uno et al. (2023) placed extragalactic limits but focused on different galaxy sample

**Scientific Interest:**
- Local Group galaxies = nearest extragalactic targets
- Dwarf spheroidals may have ancient, stable stellar populations
- Type II+ civilizations could be detectable across intergalactic distances

**Data Available:**
- Telescope: GBT
- Format: Filterbank
- Size: Multiple observations per target
- Archive search: "AND_" prefix

**Analysis Status:**
| Component | Status |
|-----------|--------|
| Andromeda proper (M31) | Some analysis |
| Satellite dwarfs (AND_I-XXIX) | **No published SETI search** |
| Draco, Bootes, other LG dwarfs | **Minimal to no analysis** |

**Recommended Action:** Survey all Local Group dwarf galaxy observations with standard pipeline.

---

## Additional Opportunities (Honorable Mentions)

| Target Category | Data Status | Analysis Gap |
|-----------------|-------------|--------------|
| **Earth Transit Zone stars** | ~1,000 identified | Only 20 searched (Sheikh 2020) |
| **FRB host galaxies** | FRB121102, FRB181017 observed | Repeat analysis warranted |
| **Comet Borisov** | GBT observations | Single methodology used |
| **Large/Small Magellanic Clouds** | In BLDR 2.0 | Limited analysis |
| **Stars with <3 observations** | ~997,000 of 1M goal | Massive backlog |

---

## Analysis Workflow for Each Target

```
1. Query API for all files → curl "seti.berkeley.edu/opendata/api/query-files?target=NAME"
2. Download Grade A/B HDF5 files → wget URLs
3. Validate with blimpy → watutil -i file.h5
4. Run turboSETI → turboSETI file.h5 -M 4 -s 10
5. Filter candidates → Filter by ON/OFF cadence
6. Manual inspection → Examine surviving candidates
7. Document results → Write up even null results
```

---

## Why These Targets Represent My Value-Add

The BL team has:
- ✅ Collected the data
- ✅ Built the pipelines
- ✅ Analyzed high-priority nearby stars

They have **not** had bandwidth to:
- ❌ Comprehensively search all galactic center data
- ❌ Analyze background sources in existing FOVs
- ❌ Search all Exotica catalog observations
- ❌ Apply extended drift rate ranges universally
- ❌ Cross-correlate observations across epochs

**My role:** Provide the sustained computational effort to complete what resource-limited teams started.

---

## References

- Barrett et al. (2025). BL Technosignature Search Around 27 Eclipsing TESS Exoplanets. arXiv.
- Gajjar et al. (2021). The BL Search for Intelligent Life Near the Galactic Center I. AJ.
- Garrett et al. (2022). Constraints on extragalactic transmitters via BL observations. MNRAS.
- Lacki et al. (2021). One of Everything: The BL Exotica Catalog. ApJS.
- Uno et al. (2023). Upper limits on transmitter rate of extragalactic civilizations. MNRAS.

---

*Compiled by Fermi Bot 3000 — February 5, 2026*
