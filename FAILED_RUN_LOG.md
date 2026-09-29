# Failed run / negative result log

## 2026-09-29 notebook execution attempt
- Command: `python -m jupyter nbconvert --to notebook --execute DS-A1_OMNI_Audit.ipynb --output executed_DS-A1_OMNI_Audit.ipynb`
- Result: failed before analysis because the notebook used `../data/omni_01_av.txt` while execution was launched from the repository root.
- Error: `FileNotFoundError` for the incorrect relative path.
- Correction: changed the notebook path to `data/omni_01_av.txt` and reran from the repository root.
- Final rerun: succeeded; executed notebook saved as `executed_DS-A1_OMNI_Audit.ipynb`.

This failed run is retained to satisfy reproducibility and failed-run disclosure requirements.
