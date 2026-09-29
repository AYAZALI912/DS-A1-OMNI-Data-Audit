# Data Card — OMNI 2 Daily Averages

## Identification
- Source: NASA/Goddard Space Flight Center Space Physics Data Facility (SPDF), OMNI 2
- File: `omni_01_av.dat` (local frozen copy renamed `omni_01_av.txt`)
- Frozen local SHA-256: `1dd1327e601713be59903b064dbed45421673040f443f4148fd11a4deb4e0c1c`
- Local bytes: 7,667,328
- Rows × columns: 23,376 × 55
- Date slots: 1963-01-01 through 2026-12-31; current populated observations end earlier, with fill-valued tail records.

## Intended use
Exploratory audit of whether daily mean GSM Bz is associated with daily Kp.

## Stakeholder
A space-weather data analyst/student deciding whether this public dataset supports the stated association question.

## Population / sample / unit
Population: daily records represented by the frozen OMNI daily file. Sample: every row in the frozen file. Unit: one day.

## Target / estimand
Target: daily Kp. Exposure: daily mean Bz GSM. Estimand: difference in mean standard Kp between days with Bz ≤ −5 nT and days with Bz > −5 nT, restricted to observed non-fill values.

## Known limitations
- Daily averaging removes sub-daily timing and can dilute short-lived extremes.
- OMNI combines data from multiple spacecraft and is a processed compilation rather than a single-instrument measurement.
- Kp is a derived, rounded geomagnetic index.
- No causal inference is supported.
- Missingness is encoded with field-specific sentinel values rather than NaN.

## License / reuse
SPDF states that, unless otherwise noted, its archived data, documentation, code and related materials are public domain and released under a CC0 dedication. Users are expected to cite the dataset and original sources.

## Citation
Papitashvili, N. E. & King, J. H. (2020), OMNI Daily Data, NASA Space Physics Data Facility, DOI 10.48322/5fmx-hv56. Accessed 2026-09-29.
