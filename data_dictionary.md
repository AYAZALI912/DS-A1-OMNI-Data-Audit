# Data Dictionary

The 55 columns follow the official OMNI2 format. Fill values are documented by NASA/SPDF; selected fields below show their sentinel values.

| # | Field | Meaning | Unit | Fill |
|---:|---|---|---|---|
| 1 | `year` | calendar year | year |  |
| 2 | `doy` | day of year | day |  |
| 3 | `hour` | hour marking first hour of daily average | hour |  |
| 4 | `bartels` | Bartels rotation number | index |  |
| 5 | `imf_sc` | IMF spacecraft identifier | code |  |
| 6 | `plasma_sc` | solar-wind plasma spacecraft identifier | code |  |
| 7 | `n_imf` | hourly points contributing to IMF daily average | count |  |
| 8 | `n_plasma` | hourly points contributing to plasma daily average | count |  |
| 9 | `B_mag` | daily mean |B| | nT | 999.9 |
| 10 | `B_vec_mag` | magnitude of average field vector | nT |  |
| 11 | `B_lat` | latitude of average field vector, GSE | deg |  |
| 12 | `B_lon` | longitude of average field vector, GSE | deg |  |
| 13 | `Bx_GSE` | IMF Bx, GSE/GSM | nT |  |
| 14 | `By_GSE` | IMF By, GSE | nT |  |
| 15 | `Bz_GSE` | IMF Bz, GSE | nT |  |
| 16 | `By_GSM` | IMF By, GSM | nT |  |
| 17 | `Bz_GSM` | IMF Bz, GSM | nT | 999.9 |
| 18 | `sigma_Bmag` | OMNI2 documented field; see source dictionary | documented unit |  |
| 19 | `sigma_B` | OMNI2 documented field; see source dictionary | documented unit |  |
| 20 | `sigma_Bx` | OMNI2 documented field; see source dictionary | documented unit |  |
| 21 | `sigma_By` | OMNI2 documented field; see source dictionary | documented unit |  |
| 22 | `sigma_Bz` | OMNI2 documented field; see source dictionary | documented unit |  |
| 23 | `proton_temp` | proton temperature | K |  |
| 24 | `proton_density` | proton density | cm^-3 | 999.9 |
| 25 | `flow_speed` | plasma flow speed | km/s | 9999 |
| 26 | `flow_lon` | OMNI2 documented field; see source dictionary | documented unit |  |
| 27 | `flow_lat` | OMNI2 documented field; see source dictionary | documented unit |  |
| 28 | `Na_Np` | OMNI2 documented field; see source dictionary | documented unit |  |
| 29 | `flow_pressure` | plasma flow pressure | nPa |  |
| 30 | `sigma_T` | OMNI2 documented field; see source dictionary | documented unit |  |
| 31 | `sigma_N` | OMNI2 documented field; see source dictionary | documented unit |  |
| 32 | `sigma_V` | OMNI2 documented field; see source dictionary | documented unit |  |
| 33 | `sigma_phi_V` | OMNI2 documented field; see source dictionary | documented unit |  |
| 34 | `sigma_theta_V` | OMNI2 documented field; see source dictionary | documented unit |  |
| 35 | `sigma_Na_Np` | OMNI2 documented field; see source dictionary | documented unit |  |
| 36 | `electric_field` | OMNI2 documented field; see source dictionary | documented unit |  |
| 37 | `plasma_beta` | OMNI2 documented field; see source dictionary | documented unit |  |
| 38 | `alfven_mach` | OMNI2 documented field; see source dictionary | documented unit |  |
| 39 | `Kp` | daily Kp code; e.g. 33=3+, 57=6- | encoded index | 99 |
| 40 | `sunspot_R` | new-version sunspot number | count | 999 |
| 41 | `Dst` | Dst index | nT | 99999 |
| 42 | `AE` | AE index | nT |  |
| 43 | `proton_gt1` | OMNI2 documented field; see source dictionary | documented unit |  |
| 44 | `proton_gt2` | OMNI2 documented field; see source dictionary | documented unit |  |
| 45 | `proton_gt4` | OMNI2 documented field; see source dictionary | documented unit |  |
| 46 | `proton_gt10` | proton flux >10 MeV | cm^-2 s^-1 sr^-1 |  |
| 47 | `proton_gt30` | OMNI2 documented field; see source dictionary | documented unit |  |
| 48 | `proton_gt60` | OMNI2 documented field; see source dictionary | documented unit |  |
| 49 | `proton_flag` | proton-flux contamination flag | code |  |
| 50 | `ap` | ap index | nT | 999 |
| 51 | `F10_7` | 10.7 cm solar radio flux | sfu | 999.9 |
| 52 | `PCN` | PC(N) index | index |  |
| 53 | `AL` | AL index | nT |  |
| 54 | `AU` | AU index | nT |  |
| 55 | `magnetosonic_mach` | magnetosonic Mach number | ratio |  |
