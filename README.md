# WISE-Light-Curves
WISE light curves of ultra cool dwarfs analyzed with Lomb-Scargle periodogram.

Source lists:   https://zenodo.org/records/4169085  

This work has benefited from The UltracoolSheet at http://bit.ly/UltracoolSheet, maintained by Will Best, Trent Dupuy, Michael Liu, Rob Siverd, and Zhoujian Zhang:


| Column Name   | d_type   | unit   | Description                                                                                         |
|---------------|----------|--------|-----------------------------------------------------------------------------------------------------|
| name          | object   | -      | Common identifier from source file. Can be used as join key.                                       |
| designation   | object   | -      | WISE designation calculated from mean coordinates.                                                  |
| ra            | float64  | deg    | Mean ra coordinates calculated from filtered data.                                                  |
| ra_err        | float64  | arcsec | Mean ra uncertainty calculated from filtered data.                                                  |
| dec           | float64  | deg    | Mean dec coordinates calculated from filtered data.                                                  |
| dec_err       | float64  | arcsec | Mean dec uncertainty calculated from filtered data.                                                  |
| w1_mean       | float64  | mag    | Mean w1mpro calculated from filtered data.                                                          |
| w1_mean_err   | float64  | mag    | Mean w1sigmpro calculated from filtered data.                                                       |
| w1_median     | float64  | mag    | Median w1mpro calculated from filtered data.                                                        |
| w1_median_err | float64  | mag    | Median w1sigmpro calculated from filtered data.                                                     |
| w1_min        | float64  | mag    | Minimum w1mpro calculated from filtered data.                                                       |
| w1_min_err    | float64  | mag    | Uncertainty for w1_min.                                                                            |
| w1_max        | float64  | mag    | Maximum w1mpro calculated from filtered data.                                                       |
| w1_max_err    | float64  | mag    | Uncertainty for w1_max.                                                                            |
| w1_snr        | float64  | number | Mean S/N ratio for W1.                                                                              |
| w1_snr_min    | float64  | number | Minimum S/N ratio for W1_mpro.                                                                       |
| w1_snr_max    | float64  | number | Maximum S/N ratio for W1_mpro.                                                                       |
| w1_num_pts    | int64    | number | Number of datapoints used in W1 after filtering.                                                    |
| w1_amplitude  | float64  | mag    | Total variability in W1 from filtered data (w1_max-w1_min).                                          |
| w1_mean_median| float64  | mag    | w1_mean - w1_median from filtered data                                          |
| w1_M_value    | float64  | mag    | M test value to test variabilty in W1 (Kinemuchi et al. 2006).                                          |
| w1_fap        | float64  | number | Lomb-Scargle False Alarm Probability (EXPERIMENTAL STAGE).                                           |
| w1_sde        | float64  | number | Signal Detection Efficiency (Alcock et al. 2000, Kovacs et al. 2002).                                |
| w1_power      | float64  | number | Highest relative power from signals detected in W1.                                                  |
| w1_period     | float64  | days   | Period matching highest detected signal from W1.                                                      |
| w2_mean       | float64  | mag    | Mean w2mpro calculated from filtered data.                                                          |
| w2_mean_err   | float64  | mag    | Mean w2sigmpro calculated from filtered data.                                                        |
| w2_median     | float64  | mag    | Median w2mpro calculated from filtered data.                                                         |
| w2_median_err | float64  | mag    | Median w2sigmpro calculated from filtered data.                                                       |
| w2_min        | float64  | mag    | Minimum w2mpro calculated from filtered data.                                                        |
| w2_min_err    | float64  | mag    | Uncertainty for w2_min.                                                                             |
| w2_max        | float64  | mag    | Maximum w2mpro calculated from filtered data.                                                        |
| w2_max_err    | float64  | mag    | Uncertainty for w2_max.                                                                             |
| w2_snr        | float64  | number | Mean S/N ratio for W2.                                                                              |
| w2_snr_min    | float64  | number | Minimum S/N ratio for W2_mpro.                                                                       |
| w2_snr_max    | float64  | number | Maximum S/N ratio for W2_mpro.                                                                       |
| w2_num_pts    | int64    | number | Amount of datapoints after filtering.                                                                |
| w2_amplitude  | float64  | mag    | Total variability in W2 from filtered data (w2_max-w2_min).                                          |
| w2_mean_median| float64  | mag    | w2_mean - w2_median from filtered data                                          |
| w2_M_value    | float64  | mag    | M test value to test variabilty in W2 (Kinemuchi et al. 2006).                                          |
| w2_fap        | float64  | number | Lomb-Scargle False Alarm Probability (EXPERIMENTAL STAGE).                                           |
| w2_sde        | float64  | number | Signal Detection Efficiency (Alcock et al. 2000, Kovacs et al. 2002).                                |
| w2_power      | float64  | number | Highest relative power from signals detected in W2.                                                   |
| w2_period     | float64  | days   | Period matching highest detected signal from W2.                                                       |
| w3_mean       | object   | mag    | Mean w3mpro magnitude from l1b tables.                                                               |
| w3_mean_err   | object   | mag    | Mean w3sigmpro from l1b tables.                                                                     |
| w3_snr        | object   | number | Mean w3snr from l1b tables.                                                                         |
| w4_mean       | object   | mag    | Mean W4mpro magnitude from l1b tables.                                                               |
| w4_mean_err   | object   | mag    | Mean w4sigmpro from l1b tables.                                                                     |
| w4_snr        | object   | number | Mean w3snr from l1b tables.                                                                         |
| w1_w2         | float64  | mag    | W1_mpro - W2_mpro from filtered data.                                                                |
| delta_time    | float64  | days   | Time between first and last data points.                                                             |
| filter_flags  | object   | -      | Filtering flags for W1 and W2. A= Data filtered succesfully- Quality of data can be considered as good. B= Default filters returned less than 50 data points and filtering criteria was lowered to obtain more data. Quality of data should be considered unreliable. S= Filtering was skipped by user.|
| wiseview        | object   | link | Link to WISEView (Caselden et al. 2018).                                                                     |



