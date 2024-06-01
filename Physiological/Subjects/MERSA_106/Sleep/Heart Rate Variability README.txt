Heart rate variability (HRV) is the physiological phenomenon of variation in the time interval between heartbeats. It is measured by the variation in the beat-to-beat interval.

The "Heart Rate Variability Details" files include 5 minutes granularity recordings of your HRV during a sleep. The description for the values of each row is as follows:

- timestamp: the start of the 5 minutes interval for which the following values were computed
- rmssd: "root mean square of successive differences" - the square root of the mean of the squares of the successive differences between adjacent beat-to-beat intervals
- coverage: the number of data points in the interval, multiplied by the mean beat-to-beat of the interval in seconds and divided by the number of seconds in the interval (300 seconds)
- low_frequency: measures long term variations in heart rate and reflects activity from both the sympathetic and parasympathetic branches
- high_frequency: measures short term variations in heart rate and captures parasympathetic activity

The "Heart Rate Variability Histogram" files include histograms that shows the spread in the beat-to-beat intervals for your sleeps:

- timestamp: the wake time
- bucket_values: 29 bins grouping and counting the similar beat-to-beat durations during your sleep. The bins interval is 0.05s, and the bins start at 0.3s. E.g. 0.3s, 0.35s, 0.4s, etc