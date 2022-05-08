# AirGuitar

The repository contains the Python code I wrote for the [paper](https://www.duo.uio.no/bitstream/handle/10852/79392/1/SMC_2020_cameraReady.pdf):

> Erdem, C., Lan, Q., Fuhrer, J., Martin, C. P., Tørresen, J., & Jensenius, A. R. (2020). Towards Playing in the'Air': Modeling Motion-Sound Energy Relationships in Electric Guitar Performance Using Deep Neural Networks. In Proceedings of the SMC Conferences (pp. 177-184). Axea sas/SMC Network.

## Contribution statement

The code in this repository is all written by Qichao Lan including:
- the code for recording the Myo data from both arms (https://github.com/chaosprint/dual-myo-recorder)
- the code for processing the data such as interpolating some missing Myo samples: [interpolation_emg.ipynb](https://github.com/chaosprint/AirGuitar/blob/main/interpolation_emg.ipynb)
- the code for training the model which can predict RMS from the Myo data: [emg_rms_training.ipynb](https://github.com/chaosprint/AirGuitar/blob/main/emg_rms_training.ipynb)
- the code for predicting RMS from the Myo data (both arms, 16 channels): [EMG_to_RMS_both_hands_person_load.ipynb](https://github.com/chaosprint/AirGuitar/blob/main/EMG_to_RMS_both_hands_person_load.ipynb)

Cagri Erdem has contributed the Max/MSP patch for the visual hint during recording. Based on the code in this repo, he also further tweaked the model and worked on the statistical analysis. See the non-overlapped part in this repo:
https://github.com/cerdemo/air_model
