# [HeartWise](https://ishushan02.github.io/Heart-Rate-Vizualizer/)

A biomedical informatics project that turns raw heart rate numbers into real-time 3D cardiac visualization  making the heartbeat legible for patients and clinicians alike.

## Predictions
HeartWise shows an educational 10-minute acute MI cue based on the entered BPM and selected symptom state. It displays warnings only when the current reading suggests a relevant concern, such as bradycardia, tachycardia, extreme tachycardia, or chest-pain/severe-symptom concern.

This is not a validated heart attack prediction model. A real Myocardial Infarction (MI) or arrhythmia classifier requires measured ECG data, previous clinical context, and often lab findings; the demo uses BPM plus a synthetic ECG visualization. PTB-XL and MIT-BIH are included as reference datasets for real ECG-based classification, while AHA/CDC guidance is used for heart-rate ranges and symptom warnings.

PTB-XL/PhysioNet: https://physionet.org/content/ptb-xl/1.0.2/

American Heart Association symptoms: https://www.heart.org/en/about-us/heart-attack-and-stroke-symptoms

CDC heart attack guidance: https://www.cdc.gov/heart-disease/about/heart-attack.html

MIT-BIH Arrhythmia Database for ECG rhythm-analysis context: https://physionet.org/physiobank/database/html/mitdbdir/intro.htm

AHA heart-rate ranges, bradycardia/tachycardia definitions: https://www.heart.org/en/health-topics/high-blood-pressure/the-facts-about-high-blood-pressure/all-about-heart-rate-pulse

AHA arrhythmia definitions: https://www.heart.org/en/health-topics/arrhythmia/about-arrhythmia

## Structure

- `/`  Landing page (HeartWise marketing site)
- `/Heartwise/`  Live demo (3D anatomical heart with EKG)
- `/storyBoard/`  Project storyboard and design rationale

## Running locally

Open `index.html` directly in a browser, or serve with any static file server:

```
npx serve .
```

The demo at `/Heartwise/` requires a server (not `file://`) due to ES module imports.

## Tech

- Three.js (v0.165.0) via ES module import map
- Vanilla JS, HTML, CSS  no build step
- Hosted on GitHub Pages

## Team

Ishan Kumar Anand
Abhiraj Yogesh Srivastava
Rammya Sakpal
Built by the Design Innovations Group, 2026.
