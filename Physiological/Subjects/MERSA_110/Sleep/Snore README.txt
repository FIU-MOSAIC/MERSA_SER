Snore Details is providing the acoustic noise metrics during sleep. The acoustic noise metrics include noise level and snoring events.
The acoustic noise metrics are computed every segment (default 30 second).
The noise level is reported in A-weighting which is adjusted for loudness perceived by the human ear. The noise level is computed every 100 milliseconds.
- timestamp: the start time of this segment.
- mean_dba: average A-weighted noise level in decibels measured on the device in this segment.
- max_dba: maximum A-weighted noise level in decibels measured on the device in this segment.
- min_dba: minimum A-weighted noise level in decibels measured on the device in this segment.
- events_number: the number of sound events detected in this segment.
- snoring_events_number: the number of snoring events detected in this segment.
- snore_label: a binary label indicating whether there is enough snoring events in this segment.
- sample_duration: the duration of this segment, the default is 30 seconds.