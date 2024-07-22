# Magnitude or Phase? a Two Stage Algorithm for  Single-Microphone Dereverberation

Ayal Schwartz, Sharom Gannot and Shlomo E. Chazan 

Int.Workshop on Acoustic Signal Enhancement (IWAENC), 2024

![flow](/flow5.png)

In this work, we present a new single-microphone speech dereverberation algorithm. Initially, we provide empirical evidence highlighting the importance of separate processing for magnitude and phase in dereverberation tasks. Additionally, we illustrate that in our task, unlike noise reduction, certain objective metrics strongly correlate with the magnitude while others with the phase. Consequently, we propose a new architecture that consists of two modules, each of which is responsible for a different task. The first module estimates the clean magnitude, while the second is focused on estimating the phase using the noisy input phase with the estimated magnitude. Subjective tests indicate that enhancing either only the magnitude or only the phase components is insufficient for this task. In our experimental evaluation, the proposed method demonstrates a consistent improvement in the magnitude and phase compared to prior approaches that primarily address one of these aspects.


## Table of Examples

| Noisy | RI2RI (SI-SDR) | MM+Noisy phase | MM+PM (Ours) |
|-------|-------|-------|-------|
| <img src="noisy/0.png" alt="Noisy 1" width="200"> <br> [Noisy 1 WAV](noisy/0.wav) | <img src="RI2RI/0.png" alt="RI2RI 1" width="200"> <br> [RI2RI 1 WAV](RI2RI/0.wav) | <img src="MM_NP/0.png" alt="MM+NP 1" width="200"> <br> [MM+NP 1 WAV](MM_NP/0.wav) | <img src="proposed/0.png" alt="MM+PM 1" width="200"> <br> [MM+PM 1 WAV](proposed/0.wav) |
| <img src="noisy/1.png" alt="Noisy 2" width="200"> <br> [Noisy 2 WAV](noisy/1.wav) | <img src="RI2RI/1.png" alt="RI2RI 2" width="200"> <br> [RI2RI 2 WAV](RI2RI/1.wav) | <img src="MM_NP/1.png" alt="MM+NP 2" width="200"> <br> [MM+NP 2 WAV](MM_NP/1.wav) | <img src="proposed/1.png" alt="MM+PM 2" width="200"> <br> [MM+PM 2 WAV](proposed/1.wav) |
| <img src="noisy/3.png" alt="Noisy 3" width="200"> <br> [Noisy 3 WAV](noisy/3.wav) | <img src="RI2RI/3.png" alt="RI2RI 3" width="200"> <br> [RI2RI 3 WAV](RI2RI/3.wav) | <img src="MM_NP/3.png" alt="MM+NP 3" width="200"> <br> [MM+NP 3 WAV](MM_NP/3.wav) | <img src="proposed/3.png" alt="MM+PM 3" width="200"> <br> [MM+PM 3 WAV](proposed/3.wav) |
| <img src="noisy/6.png" alt="Noisy 4" width="200"> <br> [Noisy 4 WAV](noisy/6.wav) | <img src="RI2RI/6.png" alt="RI2RI 4" width="200"> <br> [RI2RI 4 WAV](RI2RI/6.wav) | <img src="MM_NP/6.png" alt="MM+NP 4" width="200"> <br> [MM+NP 4 WAV](MM_NP/6.wav) | <img src="proposed/6.png" alt="MM+PM 4" width="200"> <br> [MM+PM 4 WAV](proposed/6.wav) |
| <img src="noisy/9.png" alt="Noisy 5" width="200"> <br> [Noisy 5 WAV](noisy/9.wav) | <img src="RI2RI/9.png" alt="RI2RI 5" width="200"> <br> [RI2RI 5 WAV](RI2RI/9.wav) | <img src="MM_NP/9.png" alt="MM+NP 5" width="200"> <br> [MM+NP 5 WAV](MM_NP/9.wav) | <img src="proposed/9.png" alt="MM+PM 5" width="200"> <br> [MM+PM 5 WAV](proposed/9.wav) |
| <img src="noisy/10.png" alt="Noisy 6" width="200"> <br> [Noisy 6 WAV](noisy/10.wav) | <img src="RI2RI/10.png" alt="RI2RI 6" width="200"> <br> [RI2RI 6 WAV](RI2RI/10.wav) | <img src="MM_NP/10.png" alt="MM+NP 6" width="200"> <br> [MM+NP 6 WAV](MM_NP/10.wav) | <img src="proposed/10.png" alt="MM+PM 6" width="200"> <br> [MM+PM 6 WAV](proposed/10.wav) |
| <img src="noisy/12.png" alt="Noisy 7" width="200"> <br> [Noisy 7 WAV](noisy/12.wav) | <img src="RI2RI/12.png" alt="RI2RI 7" width="200"> <br> [RI2RI 7 WAV](RI2RI/12.wav) | <img src="MM_NP/12.png" alt="MM+NP 7" width="200"> <br> [MM+NP 7 WAV](MM_NP/12.wav) | <img src="proposed/12.png" alt="MM+PM 7" width="200"> <br> [MM+PM 7 WAV](proposed/12.wav) |
| <img src="noisy/14.png" alt="Noisy 8" width="200"> <br> [Noisy 8 WAV](noisy/14.wav) | <img src="RI2RI/14.png" alt="RI2RI 8" width="200"> <br> [RI2RI 8 WAV](RI2RI/14.wav) | <img src="MM_NP/14.png" alt="MM+NP 8" width="200"> <br> [MM+NP 8 WAV](MM_NP/14.wav) | <img src="proposed/14.png" alt="MM+PM 8" width="200"> <br> [MM+PM 8 WAV](proposed/14.wav) |
| <img src="noisy/15.png" alt="Noisy 9" width="200"> <br> [Noisy 9 WAV](noisy/15.wav) | <img src="RI2RI/15.png" alt="RI2RI 9" width="200"> <br> [RI2RI 9 WAV](RI2RI/15.wav) | <img src="MM_NP/15.png" alt="MM+NP 9" width="200"> <br> [MM+NP 9 WAV](MM_NP/15.wav) | <img src="proposed/15.png" alt="MM+PM 9" width="200"> <br> [MM+PM 9 WAV](proposed/15.wav) |
| <img src="noisy/21.png" alt="Noisy 10" width="200"> <br> [Noisy 10 WAV](noisy/21.wav) | <img src="RI2RI/21.png" alt="RI2RI 10" width="200"> <br> [RI2RI 10 WAV](RI2RI/21.wav) | <img src="MM_NP/21.png" alt="MM+NP 10" width="200"> <br> [MM+NP 10 WAV](MM_NP/21.wav) | <img src="proposed/21.png" alt="MM+PM 10" width="200"> <br> [MM+PM 10 WAV](proposed/21.wav) |
