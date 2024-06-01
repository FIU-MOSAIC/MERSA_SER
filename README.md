# MERSA: Multimodal Emotion Recognition and Sentiment Analysis Dataset (version 1.0)

## Overview

The **MERSA** dataset comprises multimodal data collected from 150 participants between October 2022 and September 2023. It is designed to facilitate research in emotion recognition and sentiment analysis across various modalities.

Here, 10% of the dataset is available. To request the full dataset, please complete and submit the form provided at (https://forms.gle/vXTq1p64wnKLoNTJ6).

## Data Collection
Participants were required to participate in the study for at least 14 days. During this period, they completed various surveys, including the daily Emotional State Survey (ESS), and wore a wrist-worn Fitbit Charge 5 tracker to collect physiological data.

### Audios: from ESS

  - **Survey Composition**: 30 questions including:
  - 9 spoken response questions. The first response is considered spontaneous or 'natural,' where participants are prompted to report any incidents, observations, or general events from their day. The following eight responses are 'scripted,' consisting of participants reading sentences that depict specific scenarios. The details of these questions can be found in '/Audios/ESS_questions.txt.'

  - 20 adjectives for self-reported emotional intensity.

  - 1 question about the timing of reported emotions.

  - **Unlabeled**: In the initial stages of data collection, participants were offered the option to submit a shortened version of the ESS if they were too busy with schoolwork or other personal commitments to complete the full daily assessment. This abbreviated version consists only of the 9 audio questions. The unlabeled audio data, found under 'Audios/Unlabeled,' was not utilized in this study but is intended for use in future research in conjunction with the physiological data collected simultaneously.

### Labels

  - **PANAS**: Emotional assessments were conducted using the Positive Affect and Negative Affect Schedule (PANAS), which includes 20 items evenly divided between positive and negative affects. A Likert scale ranging from 1 to 5 was used.
  - **Dimensional Labels**: Valence, arousal, and dominance scores, which range from 20 (lowest) to 100 (highest), are provided alongside sentiment labels (negative, neutral, positive) for each ESS submission. These were calculated using the method outlined in the paper. Each label is aligned with the name of the corresponding natural speech file. Researchers may also choose to apply these labels to the entire submission, not just the natural response. For example, the labels for 'MERSA_101_01_001' could also be used for the audio files 'MERSA_101_01_002' through 'MERSA_101_01_009', as they are all from the same submission.
  - **Alternative Labeling**: Original PANAS responses for each ESS submission are included, providing researchers with alternative labeling options for future studies based on the ground truth.

### Transcripts
  Transcriptions are available for all 'natural' audio responses, stored under the 'Transcripts' directory with filenames corresponding to the audio files.

### Physiological Data

Collected using the Fitbit Tracker 5, the physiological data includes:
- **Electrocardiogram (ECG)**: Daily reports, each lasting 30 seconds.
- **Heart Data**: Atrial fibrillation (Afib) ECG readings.
- **Oxygen Variation**: Estimated oxygen level changes.
- **Personal Profile**: Demographic characteristics of the subject.
- **Physical Activity**: Step count, continuous heart rate, and calories burned. Active zone minutes categorized into very active, moderately active, light active, and sedentary. In addition, different physical exercises recorded.
- **Sleep Data**: SpO2 monitoring, sleep efficiency, sleep score. Duration of various sleep stages (deep, wake, light, REM).

## Audio File Naming

Structure: 'MERSA_ParticipantId_SubmissionNumber_QuestionNumber'

- **Example for natural audio**: /MERSA_SER/Audios/Natural/MERSA_101_01_001 indicates participant 101's response to the first question ('001') within the first submission ('01').
- **Example for scripted audio**: /MERSA_SER/Audios/Scripted/MERSA_101_01_002 to MERSA_101_01_009 represents the eight scripted responses from the same submission ('01') by participant 101.
