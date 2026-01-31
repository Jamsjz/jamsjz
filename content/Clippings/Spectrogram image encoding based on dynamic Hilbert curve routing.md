---
publish: true
title: Spectrogram image encoding based on dynamic Hilbert curve routing
description: In this paper we propose an image-based biological classification system that can identify different creatures via their sounds. The overall system involves the
created: "[[2026-01-30]]"
modified: 2026-01-30T22:33:09.246+05:45
tags:
  - clippings
cssclasses: ""
---

Spectrogram image encoding based on dynamic Hilbert curve routing | IEEE Conference Publication | IEEE Xplore 

## Abstract:

In this paper we propose an image-based biological classification system that can identify different creatures via their sounds. The overall system involves the relative...

---

### I. Introduction

One of the first decisions in any audio identification system is to choose appropriate features. The criteria may count on how exactly the classifying signals are represented, and how easily the following classification can be performed \[1\]. In this paper, we not only use a sophisticated representation to reduce the dependence on the database, but also provide a simplified encoding to process the matching in the classification. The proposed method is composed of three stages. In the first step, Relative Spectral Transform-Perceptual Linear Prediction (RASTA-PLP), an extension of Linear Predictive Coding (LPC), is used to represent the spectral envelope of a digital signal by using the information of a psychoacoustics-based linear predictive method. Second, to preserve a perceived naturalness in the timbral transitions, it is also necessary to detect the endpoints of input features along the time axis. Conventional approach to audio classification uses feature vectors based on spectral amplitude and harmonic location for this purpose. However, for such an application as spectrogram analysis that requires accurate locations along the time axis, we use the cosine similarity measure (CSM) as an alternative to separate and establish the spectrogram database. Finally, dynamic Hilbert curve, an intermittent fractal space-filling curve, is introduced to preserve and encode the locality behavior of spectrogram image. The result is represented as a size-reduced sequence to facilitate the comparison with the pre-transformed sequences in the database by the Gaussian mixture model (GMM). Unlike the full reference model that makes comparisons among a series of audio samples and the classifying audio, the reference-reduced approach uses only a handful of database, which makes this algorithm more suitable for being implemented on a handheld device. The flowchart outlining such a spectrogram image encoding for bio-classification system is illustrated in Fig. 1, where each step will be explained in detail in the following sections.Flowchart of spectrogram image encoding for biological classification system.