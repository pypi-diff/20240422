# Comparing `tmp/mosqito-1.2.0.tar.gz` & `tmp/mosqito-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosqito-1.2.0.tar", last modified: Thu Apr 18 19:08:35 2024, max compression
+gzip compressed data, was "mosqito-1.2.1.tar", last modified: Fri Apr 19 13:11:04 2024, max compression
```

## Comparing `mosqito-1.2.0.tar` & `mosqito-1.2.1.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.471934 mosqito-1.2.0/
--rw-rw-rw-   0        0        0    11558 2024-02-07 11:04:08.000000 mosqito-1.2.0/LICENSE
--rw-rw-rw-   0        0        0       89 2024-02-07 11:04:08.000000 mosqito-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1446 2024-04-18 19:08:35.470936 mosqito-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      840 2024-04-18 15:23:21.000000 mosqito-1.2.0/README.md
--rw-rw-rw-   0        0        0    15006 2024-02-07 11:04:08.000000 mosqito-1.2.0/logo.png
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.047148 mosqito-1.2.0/mosqito/
--rw-rw-rw-   0        0        0     3545 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.075150 mosqito-1.2.0/mosqito/sound_level_meter/
--rw-rw-rw-   0        0        0      798 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/__init__.py
--rw-rw-rw-   0        0        0     2946 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/comp_spectrum.py
--rw-rw-rw-   0        0        0     2765 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/freq_band_synthesis.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.110152 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/__init__.py
--rw-rw-rw-   0        0        0     2350 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_center_freq.py
--rw-rw-rw-   0        0        0     2153 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_filter_bandwidth.py
--rw-rw-rw-   0        0        0     1121 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_getFrequencies.py
--rw-rw-rw-   0        0        0     1308 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_n_oct_freq_filter.py
--rw-rw-rw-   0        0        0     2031 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_n_oct_time_filter.py
--rw-rw-rw-   0        0        0      813 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_nominal_frequency.py
--rw-rw-rw-   0        0        0     3119 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/noct_spectrum.py
--rw-rw-rw-   0        0        0     3660 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/noct_synthesis.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.112152 mosqito-1.2.0/mosqito/sq_metrics/
--rw-rw-rw-   0        0        0     2760 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.115156 mosqito-1.2.0/mosqito/sq_metrics/loudness/
--rw-rw-rw-   0        0        0     1252 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.145236 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/__init__.py
--rw-rw-rw-   0        0        0      837 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_auditory_filters_centre_freq.py
--rw-rw-rw-   0        0        0     5570 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_band_pass_signals.py
--rw-rw-rw-   0        0        0     1395 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_ear_filter_design.py
--rw-rw-rw-   0        0        0     2259 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_ecma_time_segmentation.py
--rw-rw-rw-   0        0        0     1977 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_gammatone.py
--rw-rw-rw-   0        0        0      838 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_loudness_ecma_data.py
--rw-rw-rw-   0        0        0     2481 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_loudness_from_bandpass.py
--rw-rw-rw-   0        0        0      996 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_nonlinearity.py
--rw-rw-rw-   0        0        0     1118 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_preprocessing.py
--rw-rw-rw-   0        0        0     4769 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/loudness_ecma.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.178238 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/__init__.py
--rw-rw-rw-   0        0        0    14615 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/_calc_slopes.py
--rw-rw-rw-   0        0        0     1270 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/_get_rns_index.py
--rw-rw-rw-   0        0        0     7678 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/_main_loudness.py
--rw-rw-rw-   0        0        0     4097 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst.py
--rw-rw-rw-   0        0        0     7209 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst_freq.py
--rw-rw-rw-   0        0        0     4309 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst_perseg.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.201239 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/__init__.py
--rw-rw-rw-   0        0        0     1657 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_lowpass_intp.py
--rw-rw-rw-   0        0        0     6284 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_nonlinear_decay.py
--rw-rw-rw-   0        0        0      925 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_square_and_smooth.py
--rw-rw-rw-   0        0        0      950 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_temporal_weighting.py
--rw-rw-rw-   0        0        0     9700 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_third_octave_levels.py
--rw-rw-rw-   0        0        0     4690 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/loudness_zwtv.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.217240 mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/__init__.py
--rw-rw-rw-   0        0        0     3505 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/equal_loudness_contours.py
--rw-rw-rw-   0        0        0      913 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/phone2spl.py
--rw-rw-rw-   0        0        0      929 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/sone2phone.py
--rw-rw-rw-   0        0        0      681 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/sone_to_phon.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.219241 mosqito-1.2.0/mosqito/sq_metrics/roughness/
--rw-rw-rw-   0        0        0      782 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.241243 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/
--rw-rw-rw-   0        0        0     4959 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/_H_weighting.py
--rw-rw-rw-   0        0        0      276 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/__init__.py
--rw-rw-rw-   0        0        0     1291 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/_ear_filter_coeff.py
--rw-rw-rw-   0        0        0      820 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/_gzi_weighting.py
--rw-rw-rw-   0        0        0     6966 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/_roughness_dw_main_calc.py
--rw-rw-rw-   0        0        0     3964 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/roughness_dw.py
--rw-rw-rw-   0        0        0     5370 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/roughness_dw_freq.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.273919 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/
--rw-rw-rw-   0        0        0      216 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/__init__.py
--rw-rw-rw-   0        0        0     2303 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_estimate_fund_mod_rate.py
--rw-rw-rw-   0        0        0     1090 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_interpolation_50.py
--rw-rw-rw-   0        0        0     1779 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_lowpass_filter.py
--rw-rw-rw-   0        0        0     1516 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_noise_reduction.py
--rw-rw-rw-   0        0        0     1588 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_non_linear_transform.py
--rw-rw-rw-   0        0        0     2454 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_peak_picking.py
--rw-rw-rw-   0        0        0     2655 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_refinement.py
--rw-rw-rw-   0        0        0      432 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_von_hann_window.py
--rw-rw-rw-   0        0        0     4009 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_weighting.py
--rw-rw-rw-   0        0        0     8364 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/roughness_ecma.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.278923 mosqito-1.2.0/mosqito/sq_metrics/sharpness/
--rw-rw-rw-   0        0        0     1112 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/sharpness/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.297920 mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/
--rw-rw-rw-   0        0        0      484 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/__init__.py
--rw-rw-rw-   0        0        0     2148 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/_weighting_fastl.py
--rw-rw-rw-   0        0        0     6708 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_freq.py
--rw-rw-rw-   0        0        0     4454 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_from_loudness.py
--rw-rw-rw-   0        0        0     3935 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_perseg.py
--rw-rw-rw-   0        0        0     3858 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_st.py
--rw-rw-rw-   0        0        0     4102 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_tv.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.299920 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/
--rw-rw-rw-   0        0        0      778 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.317923 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/__init__.py
--rw-rw-rw-   0        0        0    11748 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_band_procedure_data.py
--rw-rw-rw-   0        0        0     5730 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_main_sii.py
--rw-rw-rw-   0        0        0     9141 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_speech_data.py
--rw-rw-rw-   0        0        0     6062 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi.py
--rw-rw-rw-   0        0        0     6244 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_freq.py
--rw-rw-rw-   0        0        0     5779 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_level.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.319923 mosqito-1.2.0/mosqito/sq_metrics/tonality/
--rw-rw-rw-   0        0        0     1371 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.333923 mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/__init__.py
--rw-rw-rw-   0        0        0     8281 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/_pr_main_calc.py
--rw-rw-rw-   0        0        0     5737 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_freq.py
--rw-rw-rw-   0        0        0     5849 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_perseg.py
--rw-rw-rw-   0        0        0     5188 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_st.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.364926 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/
--rw-rw-rw-   0        0        0     1318 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_LTH.py
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/__init__.py
--rw-rw-rw-   0        0        0     1532 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_critical_band.py
--rw-rw-rw-   0        0        0     2253 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_find_highest_tone.py
--rw-rw-rw-   0        0        0     2156 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_peak_level.py
--rw-rw-rw-   0        0        0     6128 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_screening_for_tones.py
--rw-rw-rw-   0        0        0     3570 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_spectrum_smoothing.py
--rw-rw-rw-   0        0        0     9680 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_tnr_main_calc.py
--rw-rw-rw-   0        0        0     5718 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_freq.py
--rw-rw-rw-   0        0        0     5879 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_perseg.py
--rw-rw-rw-   0        0        0     5226 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_st.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.386928 mosqito-1.2.0/mosqito/utils/
--rw-rw-rw-   0        0        0     5315 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/LTQ.py
--rw-rw-rw-   0        0        0     1793 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/utils/__init__.py
--rw-rw-rw-   0        0        0     3693 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/utils/am_noise_generator.py
--rw-rw-rw-   0        0        0     4067 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/utils/am_sine_generator.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.401928 mosqito-1.2.0/mosqito/utils/conversion/
--rw-rw-rw-   0        0        0        0 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/conversion/__init__.py
--rw-rw-rw-   0        0        0      671 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/conversion/amp2db.py
--rw-rw-rw-   0        0        0     1781 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/conversion/bark2freq.py
--rw-rw-rw-   0        0        0      531 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/conversion/db2amp.py
--rw-rw-rw-   0        0        0     1789 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/conversion/freq2bark.py
--rw-rw-rw-   0        0        0     3619 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/conversion/spectrum2dBA.py
--rw-rw-rw-   0        0        0     4265 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/utils/fm_sine_generator.py
--rw-rw-rw-   0        0        0     2251 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/isoclose.py
--rw-rw-rw-   0        0        0     2901 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/load.py
--rw-rw-rw-   0        0        0     1963 2024-04-18 15:23:21.000000 mosqito-1.2.0/mosqito/utils/sine_wave_generator.py
--rw-rw-rw-   0        0        0     1735 2024-03-28 14:53:48.000000 mosqito-1.2.0/mosqito/utils/time_segmentation.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.468934 mosqito-1.2.0/mosqito.egg-info/
--rw-rw-rw-   0        0        0     1446 2024-04-18 19:08:34.000000 mosqito-1.2.0/mosqito.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7348 2024-04-18 19:08:34.000000 mosqito-1.2.0/mosqito.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 19:08:34.000000 mosqito-1.2.0/mosqito.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-18 19:08:34.000000 mosqito-1.2.0/mosqito.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-18 19:08:34.000000 mosqito-1.2.0/mosqito.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       21 2024-02-07 11:04:08.000000 mosqito-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0       86 2024-04-18 19:08:35.474944 mosqito-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1495 2024-03-28 15:18:23.000000 mosqito-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.005145 mosqito-1.2.0/tests/
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.405930 mosqito-1.2.0/tests/output/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/tests/output/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.407931 mosqito-1.2.0/tests/sq_metrics/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/tests/sq_metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.416933 mosqito-1.2.0/tests/sq_metrics/loudness/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/tests/sq_metrics/loudness/__init__.py
--rw-rw-rw-   0        0        0     1205 2024-04-18 15:23:21.000000 mosqito-1.2.0/tests/sq_metrics/loudness/test_loudness_ecma.py
--rw-rw-rw-   0        0        0     6728 2024-03-28 14:53:48.000000 mosqito-1.2.0/tests/sq_metrics/loudness/test_loudness_zwst.py
--rw-rw-rw-   0        0        0     1913 2024-03-28 14:53:48.000000 mosqito-1.2.0/tests/sq_metrics/loudness/test_loudness_zwtv.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.426930 mosqito-1.2.0/tests/sq_metrics/roughness/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/tests/sq_metrics/roughness/__init__.py
--rw-rw-rw-   0        0        0     4743 2024-04-18 15:23:21.000000 mosqito-1.2.0/tests/sq_metrics/roughness/signals_test_generation.py
--rw-rw-rw-   0        0        0     3834 2024-04-18 15:23:21.000000 mosqito-1.2.0/tests/sq_metrics/roughness/test_roughness_dw.py
--rw-rw-rw-   0        0        0     2280 2024-04-18 15:23:21.000000 mosqito-1.2.0/tests/sq_metrics/roughness/test_roughness_ecma.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.435931 mosqito-1.2.0/tests/sq_metrics/sharpness/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/tests/sq_metrics/sharpness/__init__.py
--rw-rw-rw-   0        0        0     6885 2024-03-28 14:53:48.000000 mosqito-1.2.0/tests/sq_metrics/sharpness/test_sharpness_din.py
-drwxrwxrwx   0        0        0        0 2024-04-18 19:08:35.463935 mosqito-1.2.0/tests/sq_metrics/tonality/
--rw-rw-rw-   0        0        0        0 2024-02-07 11:04:08.000000 mosqito-1.2.0/tests/sq_metrics/tonality/__init__.py
--rw-rw-rw-   0        0        0     1837 2024-03-28 14:53:48.000000 mosqito-1.2.0/tests/sq_metrics/tonality/test_pr_ecma_freq.py
--rw-rw-rw-   0        0        0     1310 2024-04-18 15:23:21.000000 mosqito-1.2.0/tests/sq_metrics/tonality/test_pr_ecma_st.py
--rw-rw-rw-   0        0        0     1399 2024-04-18 15:23:21.000000 mosqito-1.2.0/tests/sq_metrics/tonality/test_pr_ecma_tv.py
--rw-rw-rw-   0        0        0     1819 2024-03-28 14:53:48.000000 mosqito-1.2.0/tests/sq_metrics/tonality/test_tnr_ecma_freq.py
--rw-rw-rw-   0        0        0     1411 2024-03-28 14:53:48.000000 mosqito-1.2.0/tests/sq_metrics/tonality/test_tnr_ecma_st.py
--rw-rw-rw-   0        0        0     1502 2024-03-28 14:53:48.000000 mosqito-1.2.0/tests/sq_metrics/tonality/test_tnr_ecma_tv.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.226246 mosqito-1.2.1/
+-rw-rw-rw-   0        0        0    11558 2023-12-01 16:14:34.000000 mosqito-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0       89 2023-12-01 16:14:34.000000 mosqito-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1380 2024-04-19 13:11:04.226246 mosqito-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      840 2024-04-19 12:50:36.000000 mosqito-1.2.1/README.md
+-rw-rw-rw-   0        0        0    15006 2023-12-01 16:14:34.000000 mosqito-1.2.1/logo.png
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.085980 mosqito-1.2.1/mosqito/
+-rw-rw-rw-   0        0        0     3545 2024-04-19 12:51:33.000000 mosqito-1.2.1/mosqito/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.092978 mosqito-1.2.1/mosqito/sound_level_meter/
+-rw-rw-rw-   0        0        0      798 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sound_level_meter/__init__.py
+-rw-rw-rw-   0        0        0     2946 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sound_level_meter/comp_spectrum.py
+-rw-rw-rw-   0        0        0     2765 2024-03-07 08:36:47.000000 mosqito-1.2.1/mosqito/sound_level_meter/freq_band_synthesis.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.102977 mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/
+-rw-rw-rw-   0        0        0        0 2023-12-01 16:14:34.000000 mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/__init__.py
+-rw-rw-rw-   0        0        0     2350 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/_center_freq.py
+-rw-rw-rw-   0        0        0     2153 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/_filter_bandwidth.py
+-rw-rw-rw-   0        0        0     1121 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/_getFrequencies.py
+-rw-rw-rw-   0        0        0     1308 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/_n_oct_freq_filter.py
+-rw-rw-rw-   0        0        0     2031 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/_n_oct_time_filter.py
+-rw-rw-rw-   0        0        0      813 2023-12-01 16:14:34.000000 mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/_nominal_frequency.py
+-rw-rw-rw-   0        0        0     3119 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/noct_spectrum.py
+-rw-rw-rw-   0        0        0     3660 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/noct_synthesis.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.102977 mosqito-1.2.1/mosqito/sq_metrics/
+-rw-rw-rw-   0        0        0     2760 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.103978 mosqito-1.2.1/mosqito/sq_metrics/loudness/
+-rw-rw-rw-   0        0        0     1252 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.114978 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/
+-rw-rw-rw-   0        0        0        0 2023-12-05 15:52:44.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/__init__.py
+-rw-rw-rw-   0        0        0      837 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_auditory_filters_centre_freq.py
+-rw-rw-rw-   0        0        0     5570 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_band_pass_signals.py
+-rw-rw-rw-   0        0        0     1395 2024-03-07 08:36:47.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_ear_filter_design.py
+-rw-rw-rw-   0        0        0     2259 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_ecma_time_segmentation.py
+-rw-rw-rw-   0        0        0     1977 2024-03-07 08:36:47.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_gammatone.py
+-rw-rw-rw-   0        0        0      838 2024-03-07 08:36:47.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_loudness_ecma_data.py
+-rw-rw-rw-   0        0        0     2481 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_loudness_from_bandpass.py
+-rw-rw-rw-   0        0        0      996 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_nonlinearity.py
+-rw-rw-rw-   0        0        0     1118 2024-03-07 08:36:47.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_preprocessing.py
+-rw-rw-rw-   0        0        0     4769 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/loudness_ecma.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.119978 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwst/
+-rw-rw-rw-   0        0        0        0 2023-12-05 15:52:44.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwst/__init__.py
+-rw-rw-rw-   0        0        0    14615 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwst/_calc_slopes.py
+-rw-rw-rw-   0        0        0     1270 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwst/_get_rns_index.py
+-rw-rw-rw-   0        0        0     7678 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwst/_main_loudness.py
+-rw-rw-rw-   0        0        0     4097 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst.py
+-rw-rw-rw-   0        0        0     7209 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst_freq.py
+-rw-rw-rw-   0        0        0     4309 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst_perseg.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.126978 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwtv/
+-rw-rw-rw-   0        0        0        0 2023-12-05 15:52:44.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwtv/__init__.py
+-rw-rw-rw-   0        0        0     1657 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwtv/_lowpass_intp.py
+-rw-rw-rw-   0        0        0     6284 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwtv/_nonlinear_decay.py
+-rw-rw-rw-   0        0        0      925 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwtv/_square_and_smooth.py
+-rw-rw-rw-   0        0        0      950 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwtv/_temporal_weighting.py
+-rw-rw-rw-   0        0        0     9700 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwtv/_third_octave_levels.py
+-rw-rw-rw-   0        0        0     4690 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwtv/loudness_zwtv.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.133978 mosqito-1.2.1/mosqito/sq_metrics/loudness/utils/
+-rw-rw-rw-   0        0        0        0 2023-12-01 16:14:34.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/utils/__init__.py
+-rw-rw-rw-   0        0        0     3505 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/utils/equal_loudness_contours.py
+-rw-rw-rw-   0        0        0      913 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/utils/phone2spl.py
+-rw-rw-rw-   0        0        0      929 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/utils/sone2phone.py
+-rw-rw-rw-   0        0        0      681 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/loudness/utils/sone_to_phon.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.134978 mosqito-1.2.1/mosqito/sq_metrics/roughness/
+-rw-rw-rw-   0        0        0      782 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.139985 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_dw/
+-rw-rw-rw-   0        0        0     4959 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_dw/_H_weighting.py
+-rw-rw-rw-   0        0        0      276 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_dw/__init__.py
+-rw-rw-rw-   0        0        0     1291 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_dw/_ear_filter_coeff.py
+-rw-rw-rw-   0        0        0      820 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_dw/_gzi_weighting.py
+-rw-rw-rw-   0        0        0     6966 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_dw/_roughness_dw_main_calc.py
+-rw-rw-rw-   0        0        0     3964 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_dw/roughness_dw.py
+-rw-rw-rw-   0        0        0     5370 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_dw/roughness_dw_freq.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.153105 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/
+-rw-rw-rw-   0        0        0      216 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/__init__.py
+-rw-rw-rw-   0        0        0     2303 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_estimate_fund_mod_rate.py
+-rw-rw-rw-   0        0        0     1090 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_interpolation_50.py
+-rw-rw-rw-   0        0        0     1779 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_lowpass_filter.py
+-rw-rw-rw-   0        0        0     1516 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_noise_reduction.py
+-rw-rw-rw-   0        0        0     1588 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_non_linear_transform.py
+-rw-rw-rw-   0        0        0     2454 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_peak_picking.py
+-rw-rw-rw-   0        0        0     2655 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_refinement.py
+-rw-rw-rw-   0        0        0      432 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_von_hann_window.py
+-rw-rw-rw-   0        0        0     4009 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_weighting.py
+-rw-rw-rw-   0        0        0     8364 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/roughness_ecma.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.154104 mosqito-1.2.1/mosqito/sq_metrics/sharpness/
+-rw-rw-rw-   0        0        0     1112 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/sharpness/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.162105 mosqito-1.2.1/mosqito/sq_metrics/sharpness/sharpness_din/
+-rw-rw-rw-   0        0        0      484 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/sharpness/sharpness_din/__init__.py
+-rw-rw-rw-   0        0        0     2148 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/sharpness/sharpness_din/_weighting_fastl.py
+-rw-rw-rw-   0        0        0     6708 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_freq.py
+-rw-rw-rw-   0        0        0     4454 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_from_loudness.py
+-rw-rw-rw-   0        0        0     3935 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_perseg.py
+-rw-rw-rw-   0        0        0     3858 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_st.py
+-rw-rw-rw-   0        0        0     4102 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_tv.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.163107 mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/
+-rw-rw-rw-   0        0        0      778 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.172246 mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/
+-rw-rw-rw-   0        0        0        0 2024-01-03 13:45:15.000000 mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/__init__.py
+-rw-rw-rw-   0        0        0    11748 2024-03-07 08:36:47.000000 mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_band_procedure_data.py
+-rw-rw-rw-   0        0        0     5730 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_main_sii.py
+-rw-rw-rw-   0        0        0     9141 2024-03-07 08:36:47.000000 mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_speech_data.py
+-rw-rw-rw-   0        0        0     6062 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi.py
+-rw-rw-rw-   0        0        0     6244 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_freq.py
+-rw-rw-rw-   0        0        0     5779 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_level.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.173246 mosqito-1.2.1/mosqito/sq_metrics/tonality/
+-rw-rw-rw-   0        0        0     1371 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.180247 mosqito-1.2.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/
+-rw-rw-rw-   0        0        0        0 2023-12-05 15:52:44.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/__init__.py
+-rw-rw-rw-   0        0        0     8281 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/_pr_main_calc.py
+-rw-rw-rw-   0        0        0     5737 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_freq.py
+-rw-rw-rw-   0        0        0     5849 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_perseg.py
+-rw-rw-rw-   0        0        0     5188 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_st.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.191245 mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/
+-rw-rw-rw-   0        0        0     1318 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_LTH.py
+-rw-rw-rw-   0        0        0        0 2023-12-05 15:52:44.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/__init__.py
+-rw-rw-rw-   0        0        0     1532 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_critical_band.py
+-rw-rw-rw-   0        0        0     2253 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_find_highest_tone.py
+-rw-rw-rw-   0        0        0     2156 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_peak_level.py
+-rw-rw-rw-   0        0        0     6128 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_screening_for_tones.py
+-rw-rw-rw-   0        0        0     3570 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_spectrum_smoothing.py
+-rw-rw-rw-   0        0        0     9680 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_tnr_main_calc.py
+-rw-rw-rw-   0        0        0     5718 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_freq.py
+-rw-rw-rw-   0        0        0     5879 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_perseg.py
+-rw-rw-rw-   0        0        0     5226 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_st.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.200246 mosqito-1.2.1/mosqito/utils/
+-rw-rw-rw-   0        0        0     5315 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/utils/LTQ.py
+-rw-rw-rw-   0        0        0     1793 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/utils/__init__.py
+-rw-rw-rw-   0        0        0     3693 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/utils/am_noise_generator.py
+-rw-rw-rw-   0        0        0     4067 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/utils/am_sine_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.205246 mosqito-1.2.1/mosqito/utils/conversion/
+-rw-rw-rw-   0        0        0        0 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/utils/conversion/__init__.py
+-rw-rw-rw-   0        0        0      671 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/utils/conversion/amp2db.py
+-rw-rw-rw-   0        0        0     1781 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/utils/conversion/bark2freq.py
+-rw-rw-rw-   0        0        0      531 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/utils/conversion/db2amp.py
+-rw-rw-rw-   0        0        0     1789 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/utils/conversion/freq2bark.py
+-rw-rw-rw-   0        0        0     3619 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/utils/conversion/spectrum2dBA.py
+-rw-rw-rw-   0        0        0     4265 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/utils/fm_sine_generator.py
+-rw-rw-rw-   0        0        0     2251 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/utils/isoclose.py
+-rw-rw-rw-   0        0        0     2901 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/utils/load.py
+-rw-rw-rw-   0        0        0     1963 2024-04-19 12:50:37.000000 mosqito-1.2.1/mosqito/utils/sine_wave_generator.py
+-rw-rw-rw-   0        0        0     1735 2024-03-26 15:59:30.000000 mosqito-1.2.1/mosqito/utils/time_segmentation.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.090978 mosqito-1.2.1/mosqito.egg-info/
+-rw-rw-rw-   0        0        0     1380 2024-04-19 13:11:03.000000 mosqito-1.2.1/mosqito.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7348 2024-04-19 13:11:04.000000 mosqito-1.2.1/mosqito.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 13:11:03.000000 mosqito-1.2.1/mosqito.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-19 13:11:03.000000 mosqito-1.2.1/mosqito.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 13:11:03.000000 mosqito-1.2.1/mosqito.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       21 2024-02-07 11:01:22.000000 mosqito-1.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       86 2024-04-19 13:11:04.227245 mosqito-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1472 2024-04-19 12:51:16.000000 mosqito-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.075977 mosqito-1.2.1/tests/
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.206246 mosqito-1.2.1/tests/output/
+-rw-rw-rw-   0        0        0        0 2023-12-01 16:14:34.000000 mosqito-1.2.1/tests/output/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.206246 mosqito-1.2.1/tests/sq_metrics/
+-rw-rw-rw-   0        0        0        0 2023-12-01 16:14:34.000000 mosqito-1.2.1/tests/sq_metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.210246 mosqito-1.2.1/tests/sq_metrics/loudness/
+-rw-rw-rw-   0        0        0        0 2023-12-01 16:14:34.000000 mosqito-1.2.1/tests/sq_metrics/loudness/__init__.py
+-rw-rw-rw-   0        0        0     1205 2024-04-19 12:50:37.000000 mosqito-1.2.1/tests/sq_metrics/loudness/test_loudness_ecma.py
+-rw-rw-rw-   0        0        0     6728 2024-03-26 15:59:30.000000 mosqito-1.2.1/tests/sq_metrics/loudness/test_loudness_zwst.py
+-rw-rw-rw-   0        0        0     1913 2024-03-07 08:36:47.000000 mosqito-1.2.1/tests/sq_metrics/loudness/test_loudness_zwtv.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.215246 mosqito-1.2.1/tests/sq_metrics/roughness/
+-rw-rw-rw-   0        0        0        0 2023-12-01 16:14:34.000000 mosqito-1.2.1/tests/sq_metrics/roughness/__init__.py
+-rw-rw-rw-   0        0        0     4743 2024-04-19 12:50:37.000000 mosqito-1.2.1/tests/sq_metrics/roughness/signals_test_generation.py
+-rw-rw-rw-   0        0        0     3834 2024-04-19 12:50:37.000000 mosqito-1.2.1/tests/sq_metrics/roughness/test_roughness_dw.py
+-rw-rw-rw-   0        0        0     2280 2024-04-19 12:50:37.000000 mosqito-1.2.1/tests/sq_metrics/roughness/test_roughness_ecma.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.217246 mosqito-1.2.1/tests/sq_metrics/sharpness/
+-rw-rw-rw-   0        0        0        0 2023-12-01 16:14:34.000000 mosqito-1.2.1/tests/sq_metrics/sharpness/__init__.py
+-rw-rw-rw-   0        0        0     6885 2024-03-26 15:59:30.000000 mosqito-1.2.1/tests/sq_metrics/sharpness/test_sharpness_din.py
+drwxrwxrwx   0        0        0        0 2024-04-19 13:11:04.224246 mosqito-1.2.1/tests/sq_metrics/tonality/
+-rw-rw-rw-   0        0        0        0 2023-12-01 16:14:34.000000 mosqito-1.2.1/tests/sq_metrics/tonality/__init__.py
+-rw-rw-rw-   0        0        0     1837 2024-03-26 15:59:30.000000 mosqito-1.2.1/tests/sq_metrics/tonality/test_pr_ecma_freq.py
+-rw-rw-rw-   0        0        0     1310 2024-04-19 12:50:37.000000 mosqito-1.2.1/tests/sq_metrics/tonality/test_pr_ecma_st.py
+-rw-rw-rw-   0        0        0     1399 2024-04-19 12:50:37.000000 mosqito-1.2.1/tests/sq_metrics/tonality/test_pr_ecma_tv.py
+-rw-rw-rw-   0        0        0     1819 2024-03-26 15:59:30.000000 mosqito-1.2.1/tests/sq_metrics/tonality/test_tnr_ecma_freq.py
+-rw-rw-rw-   0        0        0     1411 2024-03-07 08:36:47.000000 mosqito-1.2.1/tests/sq_metrics/tonality/test_tnr_ecma_st.py
+-rw-rw-rw-   0        0        0     1502 2024-03-26 15:59:30.000000 mosqito-1.2.1/tests/sq_metrics/tonality/test_tnr_ecma_tv.py
```

### Comparing `mosqito-1.2.0/LICENSE` & `mosqito-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/PKG-INFO` & `mosqito-1.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: mosqito
-Version: 1.2.0
+Version: 1.2.1
 Summary: Modular Sound Quality Integrated Toolbox
 Home-page: https://github.com/Eomys/MoSQITo
-Download-URL: https://github.com/Eomys/MoSQITo/archive/v1.2.0.tar.gz
+Download-URL: https://github.com/Eomys/MoSQITo/archive/v1.2.1.tar.gz
 Author: MoSQITo Developers
 Author-email: martin.glesser@eomys.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >= 3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: pyuff
 
 <div align="center">
     <img src="https://raw.githubusercontent.com/Eomys/MoSQITo/master/logo.png">
 </div>
 
 ## What is MOSQITO ?
```

### Comparing `mosqito-1.2.0/README.md` & `mosqito-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/logo.png` & `mosqito-1.2.1/logo.png`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/__init__.py` & `mosqito-1.2.1/mosqito/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from mosqito.utils.conversion.amp2db import amp2db
 from mosqito.utils.conversion.db2amp import db2amp
 from mosqito.utils.conversion.freq2bark import freq2bark
 from mosqito.utils.conversion.bark2freq import bark2freq
 from mosqito.utils.conversion.spectrum2dBA import spectrum2dBA
 
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 # Colors and linestyles
 COLORS = [
     "#69c3c5",
     "#ffd788",
     "#ff8b88",
     "#7894cf",
```

### Comparing `mosqito-1.2.0/mosqito/sound_level_meter/__init__.py` & `mosqito-1.2.1/mosqito/sound_level_meter/__init__.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sound_level_meter/comp_spectrum.py` & `mosqito-1.2.1/mosqito/sound_level_meter/comp_spectrum.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sound_level_meter/freq_band_synthesis.py` & `mosqito-1.2.1/mosqito/sound_level_meter/freq_band_synthesis.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_center_freq.py` & `mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/_center_freq.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_filter_bandwidth.py` & `mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/_filter_bandwidth.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_getFrequencies.py` & `mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/_getFrequencies.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_n_oct_freq_filter.py` & `mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/_n_oct_freq_filter.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_n_oct_time_filter.py` & `mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/_n_oct_time_filter.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/_nominal_frequency.py` & `mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/_nominal_frequency.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/noct_spectrum.py` & `mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/noct_spectrum.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sound_level_meter/noct_spectrum/noct_synthesis.py` & `mosqito-1.2.1/mosqito/sound_level_meter/noct_spectrum/noct_synthesis.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/__init__.py` & `mosqito-1.2.1/mosqito/sq_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/__init__.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/__init__.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_auditory_filters_centre_freq.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_auditory_filters_centre_freq.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_band_pass_signals.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_band_pass_signals.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_ear_filter_design.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_ear_filter_design.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_ecma_time_segmentation.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_ecma_time_segmentation.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_gammatone.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_gammatone.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_loudness_ecma_data.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_loudness_ecma_data.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_loudness_from_bandpass.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_loudness_from_bandpass.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_nonlinearity.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_nonlinearity.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/_preprocessing.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_ecma/loudness_ecma.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_ecma/loudness_ecma.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/_calc_slopes.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwst/_calc_slopes.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/_get_rns_index.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwst/_get_rns_index.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/_main_loudness.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwst/_main_loudness.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst_freq.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst_freq.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst_perseg.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwst/loudness_zwst_perseg.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_lowpass_intp.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwtv/_lowpass_intp.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_nonlinear_decay.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwtv/_nonlinear_decay.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_square_and_smooth.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwtv/_square_and_smooth.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_temporal_weighting.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwtv/_temporal_weighting.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/_third_octave_levels.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwtv/_third_octave_levels.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/loudness_zwtv/loudness_zwtv.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/loudness_zwtv/loudness_zwtv.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/equal_loudness_contours.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/utils/equal_loudness_contours.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/phone2spl.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/utils/phone2spl.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/sone2phone.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/utils/sone2phone.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/loudness/utils/sone_to_phon.py` & `mosqito-1.2.1/mosqito/sq_metrics/loudness/utils/sone_to_phon.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/roughness/__init__.py` & `mosqito-1.2.1/mosqito/sq_metrics/roughness/__init__.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/_H_weighting.py` & `mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_dw/_H_weighting.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/_ear_filter_coeff.py` & `mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_dw/_ear_filter_coeff.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/_gzi_weighting.py` & `mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_dw/_gzi_weighting.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/_roughness_dw_main_calc.py` & `mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_dw/_roughness_dw_main_calc.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/roughness_dw.py` & `mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_dw/roughness_dw.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_dw/roughness_dw_freq.py` & `mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_dw/roughness_dw_freq.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_estimate_fund_mod_rate.py` & `mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_estimate_fund_mod_rate.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_interpolation_50.py` & `mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_interpolation_50.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_lowpass_filter.py` & `mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_lowpass_filter.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_noise_reduction.py` & `mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_noise_reduction.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_non_linear_transform.py` & `mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_non_linear_transform.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_peak_picking.py` & `mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_peak_picking.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_refinement.py` & `mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_refinement.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/_weighting.py` & `mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/_weighting.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/roughness/roughness_ecma/roughness_ecma.py` & `mosqito-1.2.1/mosqito/sq_metrics/roughness/roughness_ecma/roughness_ecma.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/sharpness/__init__.py` & `mosqito-1.2.1/mosqito/sq_metrics/sharpness/__init__.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/_weighting_fastl.py` & `mosqito-1.2.1/mosqito/sq_metrics/sharpness/sharpness_din/_weighting_fastl.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_freq.py` & `mosqito-1.2.1/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_freq.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_from_loudness.py` & `mosqito-1.2.1/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_from_loudness.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_perseg.py` & `mosqito-1.2.1/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_perseg.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_st.py` & `mosqito-1.2.1/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_st.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_tv.py` & `mosqito-1.2.1/mosqito/sq_metrics/sharpness/sharpness_din/sharpness_din_tv.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/__init__.py` & `mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/__init__.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_band_procedure_data.py` & `mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_band_procedure_data.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_main_sii.py` & `mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_main_sii.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_speech_data.py` & `mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/_speech_data.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi.py` & `mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_freq.py` & `mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_freq.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_level.py` & `mosqito-1.2.1/mosqito/sq_metrics/speech_intelligibility/sii_ansi/sii_ansi_level.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/tonality/__init__.py` & `mosqito-1.2.1/mosqito/sq_metrics/tonality/__init__.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/_pr_main_calc.py` & `mosqito-1.2.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/_pr_main_calc.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_freq.py` & `mosqito-1.2.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_freq.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_perseg.py` & `mosqito-1.2.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_perseg.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_st.py` & `mosqito-1.2.1/mosqito/sq_metrics/tonality/prominence_ratio_ecma/pr_ecma_st.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_LTH.py` & `mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_LTH.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_critical_band.py` & `mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_critical_band.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_find_highest_tone.py` & `mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_find_highest_tone.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_peak_level.py` & `mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_peak_level.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_screening_for_tones.py` & `mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_screening_for_tones.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_spectrum_smoothing.py` & `mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_spectrum_smoothing.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_tnr_main_calc.py` & `mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/_tnr_main_calc.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_freq.py` & `mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_freq.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_perseg.py` & `mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_perseg.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_st.py` & `mosqito-1.2.1/mosqito/sq_metrics/tonality/tone_to_noise_ecma/tnr_ecma_st.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/utils/LTQ.py` & `mosqito-1.2.1/mosqito/utils/LTQ.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/utils/__init__.py` & `mosqito-1.2.1/mosqito/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/utils/am_noise_generator.py` & `mosqito-1.2.1/mosqito/utils/am_noise_generator.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/utils/am_sine_generator.py` & `mosqito-1.2.1/mosqito/utils/am_sine_generator.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/utils/conversion/amp2db.py` & `mosqito-1.2.1/mosqito/utils/conversion/amp2db.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/utils/conversion/bark2freq.py` & `mosqito-1.2.1/mosqito/utils/conversion/bark2freq.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/utils/conversion/db2amp.py` & `mosqito-1.2.1/mosqito/utils/conversion/db2amp.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/utils/conversion/freq2bark.py` & `mosqito-1.2.1/mosqito/utils/conversion/freq2bark.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/utils/conversion/spectrum2dBA.py` & `mosqito-1.2.1/mosqito/utils/conversion/spectrum2dBA.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/utils/fm_sine_generator.py` & `mosqito-1.2.1/mosqito/utils/fm_sine_generator.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/utils/isoclose.py` & `mosqito-1.2.1/mosqito/utils/isoclose.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/utils/load.py` & `mosqito-1.2.1/mosqito/utils/load.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/utils/sine_wave_generator.py` & `mosqito-1.2.1/mosqito/utils/sine_wave_generator.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito/utils/time_segmentation.py` & `mosqito-1.2.1/mosqito/utils/time_segmentation.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/mosqito.egg-info/PKG-INFO` & `mosqito-1.2.1/mosqito.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: mosqito
-Version: 1.2.0
+Version: 1.2.1
 Summary: Modular Sound Quality Integrated Toolbox
 Home-page: https://github.com/Eomys/MoSQITo
-Download-URL: https://github.com/Eomys/MoSQITo/archive/v1.2.0.tar.gz
+Download-URL: https://github.com/Eomys/MoSQITo/archive/v1.2.1.tar.gz
 Author: MoSQITo Developers
 Author-email: martin.glesser@eomys.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >= 3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: pyuff
 
 <div align="center">
     <img src="https://raw.githubusercontent.com/Eomys/MoSQITo/master/logo.png">
 </div>
 
 ## What is MOSQITO ?
```

### Comparing `mosqito-1.2.0/mosqito.egg-info/SOURCES.txt` & `mosqito-1.2.1/mosqito.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/setup.py` & `mosqito-1.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import setuptools
 
 # /!\ update before a release
-from mosqito import __version__
-version = __version__
+version = __version__ = "1.2.1"
 
 # MoSQITo description
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 python_requires = ">= 3.5"
```

### Comparing `mosqito-1.2.0/tests/sq_metrics/loudness/test_loudness_ecma.py` & `mosqito-1.2.1/tests/sq_metrics/loudness/test_loudness_ecma.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/tests/sq_metrics/loudness/test_loudness_zwst.py` & `mosqito-1.2.1/tests/sq_metrics/loudness/test_loudness_zwst.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/tests/sq_metrics/loudness/test_loudness_zwtv.py` & `mosqito-1.2.1/tests/sq_metrics/loudness/test_loudness_zwtv.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/tests/sq_metrics/roughness/signals_test_generation.py` & `mosqito-1.2.1/tests/sq_metrics/roughness/signals_test_generation.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/tests/sq_metrics/roughness/test_roughness_dw.py` & `mosqito-1.2.1/tests/sq_metrics/roughness/test_roughness_dw.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/tests/sq_metrics/roughness/test_roughness_ecma.py` & `mosqito-1.2.1/tests/sq_metrics/roughness/test_roughness_ecma.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/tests/sq_metrics/sharpness/test_sharpness_din.py` & `mosqito-1.2.1/tests/sq_metrics/sharpness/test_sharpness_din.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/tests/sq_metrics/tonality/test_pr_ecma_freq.py` & `mosqito-1.2.1/tests/sq_metrics/tonality/test_pr_ecma_freq.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/tests/sq_metrics/tonality/test_pr_ecma_st.py` & `mosqito-1.2.1/tests/sq_metrics/tonality/test_pr_ecma_st.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/tests/sq_metrics/tonality/test_pr_ecma_tv.py` & `mosqito-1.2.1/tests/sq_metrics/tonality/test_pr_ecma_tv.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/tests/sq_metrics/tonality/test_tnr_ecma_freq.py` & `mosqito-1.2.1/tests/sq_metrics/tonality/test_tnr_ecma_freq.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/tests/sq_metrics/tonality/test_tnr_ecma_st.py` & `mosqito-1.2.1/tests/sq_metrics/tonality/test_tnr_ecma_st.py`

 * *Files identical despite different names*

### Comparing `mosqito-1.2.0/tests/sq_metrics/tonality/test_tnr_ecma_tv.py` & `mosqito-1.2.1/tests/sq_metrics/tonality/test_tnr_ecma_tv.py`

 * *Files identical despite different names*

