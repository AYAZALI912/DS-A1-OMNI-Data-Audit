# Provenance and lineage

```text
spacecraft instruments / contributing datasets
        ↓
source measurements near Earth / L1
        ↓
OMNI processing: cross-comparison, cross-normalization and time shifting where applicable
        ↓
OMNI2 hourly records
        ↓
arithmetic daily averages (omni_01_av.dat)
        ↓
frozen local file: omni_01_av.txt
        ↓
whitespace parsing into 55 documented fields
        ↓
sentinel-aware quality checks
        ↓
association estimand: daily Bz GSM threshold vs daily Kp
```

Frozen file SHA-256: `1dd1327e601713be59903b064dbed45421673040f443f4148fd11a4deb4e0c1c`.

The NASA documentation states that daily averages are calculated from hourly OMNI values, only arithmetic averaging is used, no minimum number of points is required, and the spacecraft IDs are set to zero because daily averages can combine multiple spacecraft.
