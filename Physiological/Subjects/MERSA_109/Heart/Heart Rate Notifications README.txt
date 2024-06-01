Heart Rate Notifications Data Export

The Heart Rate Notifications (HRNs) category of your export includes all the data related to your HRNs, including your profile settings and alert history. Some Fitbit devices such as Fitbit Charge 5, Fitbit Sense, and Fitbit Versa 3 notify you when we detect that your heart rate is outside your high or low thresholds while you appear to be inactive for at least 10 minutes.

Files Included:
----------

Heart Rate Notifications Profile.csv

This is the data related to a user's Heart Rate Notifications settings.

threshold_high_custom               - Custom upper threshold for HRN set by user
threshold_low_custom                - Custom lower threshold for HRN set by user
use_custom_threshold_high           - Use the custom high threshold
use_custom_threshold_low            - Use the custom low threshold
alert_high_on                       - Are alerts on for heart rate exceeding high threshold
alert_low_on                        - Are alerts on for heart rate subceeding the lower threshold

----------

Heart Rate Notifications Alerts.csv

This is the data that was collected for each Heart Rate Notification alert.

id                                  - Unique numeric id for the alert
start_timestamp                     - Timestamp for the start of the HRN
end_timestamp                       - Timestamp for the end of the HRN
type                                - HIGH or LOW indicating whether HRN was triggered by crossing the high or low threshold
threshold                           - Threshold value crossed
value                               - Heart rate that triggered the notification