# DS-A1 — OMNI Data Provenance and Measurement Audit

## Question
Is a more southward daily mean IMF Bz (GSM Bz ≤ −5 nT) associated with higher daily Kp than days with Bz > −5 nT?

## Frozen source
NASA/GSFC SPDF OMNI 2 daily averages, `omni_01_av.dat`. Local file SHA-256: `1dd1327e601713be59903b064dbed45421673040f443f4148fd11a4deb4e0c1c`.

Official documentation: https://omniweb.gsfc.nasa.gov/html/ow_data.html and https://cdaweb.gsfc.nasa.gov/pub/data/omni/low_res_omni/omni2.text

## Reproduce
```bash
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux: source .venv/bin/activate
pip install -r requirements.txt
jupyter nbconvert --to notebook --execute DS-A1_OMNI_Audit.ipynb --output executed_DS-A1_OMNI_Audit.ipynb
```

The notebook checks the frozen SHA-256 before reading the data.

## Results
The audit found 23,376 daily rows and 55 fields, no duplicate dates, and no invalid calendar dates. Missingness is encoded with sentinel values. For the analysis subset, n=20,300; Bz ≤ −5 nT: 266. Mean standard Kp difference (southward minus other): 2.595; Pearson r: -0.328.

These are descriptive associations only. They do not establish causality or predictive validity.
