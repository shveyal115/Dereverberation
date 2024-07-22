# Magnitude or Phase? a Two Stage Algorithm for  Single-Microphone Dereverberation

Ayal Schwartz, Sharom Gannot and Shlomo E. Chazan 

Int.Workshop on Acoustic Signal Enhancement (IWAENC), 2024

![flow](/flow5.png)

In this work, we present a new single-microphone speech dereverberation algorithm. Initially, we provide empirical evidence highlighting the importance of separate processing for magnitude and phase in dereverberation tasks. Additionally, we illustrate that in our task, unlike noise reduction, certain objective metrics strongly correlate with the magnitude while others with the phase. Consequently, we propose a new architecture that consists of two modules, each of which is responsible for a different task. The first module estimates the clean magnitude, while the second is focused on estimating the phase using the noisy input phase with the estimated magnitude. Subjective tests indicate that enhancing either only the magnitude or only the phase components is insufficient for this task. In our experimental evaluation, the proposed method demonstrates a consistent improvement in the magnitude and phase compared to prior approaches that primarily address one of these aspects.


## Table of Examples

| Noisy | RI2RI (SI-SDR) | MM+Noisy phase | MM+PM (Our) |
|-------|-------|-------|-------|
| ![Noisy 1](noisy/0.png) <br> [Noisy 1 WAV](noisy/0.wav) | ![RI2RI 1](RI2RI/0.png) <br> [RI2RI 1 WAV](RI2RI/0.wav) | ![MM+NP 1](MM_NP/0.png) <br> [MM+NP 1 WAV](MM_NP/0.wav) | ![MM+PM 1](proposed/0.png) <br> [MM+PM 1 WAV](proposed/0.wav) |
| ![Noisy 2](noisy/1.png) <br> [Noisy 2 WAV](noisy/1.wav) | ![RI2RI 2](RI2RI/1.png) <br> [RI2RI 2 WAV](RI2RI/1.wav) | ![MM+NP 2](MM_NP/1.png) <br> [MM+NP 2 WAV](MM_NP/1.wav) | ![MM+PM 2](proposed/1.png) <br> [MM+PM 2 WAV](proposed/1.wav) |
| ![Noisy 3](noisy/3.png) <br> [Noisy 3 WAV](noisy/3.wav) | ![RI2RI 3](RI2RI/3.png) <br> [RI2RI 3 WAV](RI2RI/3.wav) | ![MM+NP 3](MM_NP/3.png) <br> [MM+NP 3 WAV](MM_NP/3.wav) | ![MM+PM 3](proposed/3.png) <br> [MM+PM 3 WAV](proposed/3.wav) |
| ![Noisy 4](noisy/6.png) <br> [Noisy 4 WAV](noisy/6.wav) | ![RI2RI 4](RI2RI/6.png) <br> [RI2RI 4 WAV](RI2RI/6.wav) | ![MM+NP 4](MM_NP/6.png) <br> [MM+NP 4 WAV](MM_NP/6.wav) | ![MM+PM 4](proposed/6.png) <br> [MM+PM 4 WAV](proposed/6.wav) |
| ![Noisy 5](noisy/9.png) <br> [Noisy 5 WAV](noisy/9.wav) | ![RI2RI 5](RI2RI/9.png) <br> [RI2RI 5 WAV](RI2RI/9.wav) | ![MM+NP 5](MM_NP/9.png) <br> [MM+NP 5 WAV](MM_NP/9.wav) | ![MM+PM 5](proposed/9.png) <br> [MM+PM 5 WAV](proposed/9.wav) |
| ![Noisy 6](noisy/10.png) <br> [Noisy 6 WAV](noisy/10.wav) | ![RI2RI 6](RI2RI/10.png) <br> [RI2RI 6 WAV](RI2RI/10.wav) | ![MM+NP 6](MM_NP/10.png) <br> [MM+NP 6 WAV](MM_NP/10.wav) | ![MM+PM 6](proposed/10.png) <br> [MM+PM 6 WAV](proposed/10.wav) |
| ![Noisy 7](noisy/12.png) <br> [Noisy 7 WAV](noisy/12.wav) | ![RI2RI 7](RI2RI/12.png) <br> [RI2RI 7 WAV](RI2RI/12.wav) | ![MM+NP 7](MM_NP/12.png) <br> [MM+NP 7 WAV](MM_NP/12.wav) | ![MM+PM 7](proposed/12.png) <br> [MM+PM 7 WAV](proposed/12.wav) |
| ![Noisy 8](noisy/14.png) <br> [Noisy 8 WAV](noisy/14.wav) | ![RI2RI 8](RI2RI/14.png) <br> [RI2RI 8 WAV](RI2RI/14.wav) | ![MM+NP 8](MM_NP/14.png) <br> [MM+NP 8 WAV](MM_NP/14.wav) | ![MM+PM 8](proposed/14.png) <br> [MM+PM 8 WAV](proposed/14.wav) |
| ![Noisy 9](noisy/15.png) <br> [Noisy 9 WAV](noisy/15.wav) | ![RI2RI 9](RI2RI/15.png) <br> [RI2RI 9 WAV](RI2RI/15.wav) | ![MM+NP 9](MM_NP/15.png) <br> [MM+NP 9 WAV](MM_NP/15.wav) | ![MM+PM 9](proposed/15.png) <br> [MM+PM 9 WAV](proposed/15.wav) |
| ![Noisy 10](noisy/21.png) <br> [Noisy 10 WAV](noisy/21.wav) | ![RI2RI 10](RI2RI/21.png) <br> [RI2RI 10 WAV](RI2RI/21.wav) | ![MM+NP 10](MM_NP/21.png) <br> [MM+NP 10 WAV](MM_NP/21.wav) | ![MM+PM 10](proposed/21.png) <br> [MM+PM 10 WAV](proposed/21.wav) |



