# Voice Activity Detection

<p align="center">
    <img src="https://www.unidformazione.com/wp-content/uploads/2018/04/unipd-universita-di-padova.png" width="250" alt="University of Padua"/>
</p>

## Assignment

Consider a mono digital audio signal, in PCM format, which is assumed to be generated in real time. The transmitter executes a packetization of the signal, with packets of 160 audio samples (corresponding to an audio interval of 20 ms).

You want to design a Voice Activity Detection (VAD) algorithm that determines which packets they have vocal content and, therefore, must be transmitted, and which, on the other hand, can be suppressed as they have no vocal content significant. Note that packets without speech content may still contain background noise.

For each package audio, the VAD algorithm will have to output the value 1 if the packet is to be transmitted, and 0 otherwise. The decision of the VAD algorithm in relation to the n-th packet can be based on the signal samples of all the previous packets k ≤ n and, potentially, even of subsequent samples, as long as the overall encoding delay remains below 50 ms.

The goal is to transmit the lowest possible number of packets that allows the reconstruction of the voice signal without artifacts (clipping).

## Overview

Script with the aim of eliminating the noise present in an audio in moments of silence, recognizing when a person speaks and when there is only noise.

The realization of the algorithm comes from a careful analysis of the input files through the Audacity software. For all the details relating to the implemented algorithm refer to the file Final project report for VAD algorithm.pdf

<p align="center">
 <a href="https://github.com/pietrovalente/Voice-Activity-Detection-multimedia/blob/main/images/Sample1.png"><https://github.com/pietrovalente/Voice-Activity-Detection-multimedia/blob/main/images/Sample1.png" alt="" width="600px"></a>
</p>

<p align="center">
 <a href="https://github.com/pietrovalente/Voice-Activity-Detection-multimedia/blob/main/images/Sample2.png"><img src="https://github.com/pietrovalente/Voice-Activity-Detection-multimedia/blob/main/images/Sample2.png" alt="" width="600px"></a>
</p>
