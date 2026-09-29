# AI-use and independent-verification log

**Tool/task:** ChatGPT was used to help structure the DS-A1 audit, propose a testable association question, draft notebook/report text, and generate reproducibility scaffolding.

**Accepted assistance:** variable-selection idea (daily Bz GSM vs daily Kp), audit checklist, provenance narrative, data-card structure, and code organization.

**Rejected/qualified advice:** any suggestion that would turn the association into a causal claim, predictive claim, or unsupported generalization was excluded. The report explicitly keeps the analysis descriptive.

**Independent verification performed:**
1. The local file was hashed with SHA-256 and the notebook asserts the same hash before analysis.
2. The 55-column schema was checked against NASA's published OMNI2 format description.
3. Sentinel values were checked against NASA's documented fill values.
4. Duplicate-row and duplicate-date checks were executed.
5. Range/anomaly checks were executed.
6. The reported group counts, means, difference, and correlation were computed directly from the frozen file by executable code.

**Important:** the AI did not create or invent observations. All numerical results in the report come from the frozen local dataset.
